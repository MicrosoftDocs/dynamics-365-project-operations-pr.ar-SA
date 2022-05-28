---
title: تطوير قوالب المشروع مع نسخ المشروع‬
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء قوالب مشروع باستخدام إجراء "نسخ المشروع" المخصص.
author: stsporen
ms.date: 03/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 72aa2db7c717eeab85ada448c673bf702087baeb
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8590882"
---
# <a name="develop-project-templates-with-copy-project"></a>تطوير قوالب المشروع مع نسخ المشروع‬

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

يدعم Dynamics 365 Project Operations القدرة علي نسخ مشروع وإرجاع أي تعيينات إلى الموارد العامة التي تمثل الدور. يمكن للعملاء استخدام هذه الوظيفة لبناء قوالب المشروع الأساسية.

عند تحديد **نسخ المشروع**، يتم تحديث حالة المشروع الهدف. استخدم **سبب الحالة** لتحديد وقت اكتمال إجراء النسخ. يؤدي أيضًا تحديد **نسخ المشروع** إلى تحديث تاريخ بدء المشروع إلى تاريخ البدء الحالي في حال عدم اكتشاف تاريخ مستهدف في كيان المشروع الهدف.

## <a name="copy-project-custom-action"></a>الإجراء المخصص "نسخ المشروع"

### <a name="name"></a>Name 

msdyn\_CopyProjectV3

### <a name="input-parameters"></a>معلمات الإدخال

توجد ثلاث معلمات إدخال:

- **ReplaceNamedResources** أو **ClearTeamsAndAssignments** – قم بتعيين خيار واحد على الأقل. لا تحدد كليهما.

    - **\{"ReplaceNamedResources":true\}** - السلوك الافتراضي لـ Project Operations. يتم استبدال أي موارد مسماة بموارد عامة.
    - **\{"ClearTeamsAndAssignments":true\}** – السلوك الافتراضي لـ Project for the Web. تتم إزالة جميع التعيينات وأعضاء الفريق.

- **SourceProject** – مرجع الكيان لمشروع المصدر المراد النسخ منه. لا يمكن أن تكون هذه المعلمة خالية.
- **Target** – مرجع الكيان للمشروع المستهدف المراد النسخ إليه. لا يمكن أن تكون هذه المعلمة خالية.

يوفر الجدول التالي ملخصًا للمعلمات الثلاثة.

| المعلمة                | نوع             | القيمة‬                 |
|--------------------------|------------------|-----------------------|
| ReplaceNamedResources    | Boolean          | **صواب** أو **خطأ** |
| ClearTeamsAndAssignments | Boolean          | **صواب** أو **خطأ** |
| SourceProject            | مرجع الكيان | مشروع المصدر    |
| استهداف                   | مرجع الكيان | المشروع الهدف    |

لمزيد من الإعدادات الافتراضية حول الإجراءات، راجع [استخدام إجراءات API الويب](/powerapps/developer/common-data-service/webapi/use-web-api-actions).

### <a name="validations"></a>عمليات التحقق من الصحة

تم إجراء عمليات التحقق من الصحة التالية.

1. يقوم Null بفحص واسترداد المصدر والمشاريع المستهدفة لتأكيد وجود كلا المشروعين في المؤسسة.
2. يقوم النظام بالتحقق من صلاحية المشروع المستهدف للنسخ عن طريق التحقق من الشروط التالية:

    - لا يوجد نشاط سابق على المشروع (بما في ذلك علامة التبويب **المهام**)، وقد تم إنشاء المشروع حديثًا.
    - لا توجد نسخة سابقة، ولم يتم طلب استيراد في هذا المشروع، وليس للمشروع حالة **فشل**.

3. لا يتم استدعاء العملية باستخدام HTTP.

## <a name="specify-fields-to-copy"></a>تحديد الحقول المراد نسخها

عند استدعاء الإجراء، يبحث **نسخ المشروع** في طريقة عرض المشروع **نسخ أعمدة المشروع** لتحديد الحقول التي يجب نسخها عند نسخ المشروع.

### <a name="example"></a>مثال

يوضح المثال التالي كيفية استدعاء إجراء **CopyProjectV3** المخصص مع مجموعة المعلمة **removeNamedResources**.

```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project - Copy";
            targetProject.Id = organizationService.Create(targetProject);

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption, true, false);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, bool replaceNamedResources = true, bool clearTeamsAndAssignments = false)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;

            if (replaceNamedResources)
            {
                req["ReplaceNamedResources"] = true;
            }
            else
            {
                req["ClearTeamsAndAssignments"] = true;
            }

            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```

[!INCLUDE[footer-include](../includes/footer-banner.md)]
