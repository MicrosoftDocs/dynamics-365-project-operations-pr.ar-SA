---
title: تطوير قوالب المشروع مع نسخ المشروع‬
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء قوالب مشروع باستخدام إجراء "نسخ المشروع" المخصص.
author: stsporen
ms.date: 01/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 7a1f602e789e07014fd6c742940f52341ce6c672
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005640"
---
# <a name="develop-project-templates-with-copy-project"></a>تطوير قوالب المشروع مع نسخ المشروع‬

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

يدعم Dynamics 365 Project Operations القدرة علي نسخ مشروع وإرجاع أي تعيينات إلى الموارد العامة التي تمثل الدور. يمكن للعملاء استخدام هذه الوظيفة لبناء قوالب المشروع الأساسية.

عند تحديد **نسخ المشروع**، يتم تحديث حالة المشروع الهدف. استخدم **سبب الحالة** لتحديد وقت اكتمال إجراء النسخ. يؤدي أيضًا تحديد **نسخ المشروع** إلى تحديث تاريخ بدء المشروع إلى تاريخ البدء الحالي في حال عدم اكتشاف تاريخ مستهدف في كيان المشروع الهدف.

## <a name="copy-project-custom-action"></a>الإجراء المخصص "نسخ المشروع" 

### <a name="name"></a>اسم 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>معلمات الإدخال
توجد ثلاث معلمات إدخال:

| المعلمة‬          | النوع   | القيم                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** أو **{"clearTeamsAndAssignments":true}** |
| SourceProject      | مرجع الكيان | Source Project |
| هدف             | مرجع الكيان | المشروع الهدف |


- **{"clearTeamsAndAssignments":true}**: السلوك الافتراضي لمشروع الويب، وستتم إزالة جميع التعيينات وأعضاء الفريق.
- **{"removeNamedResources":true}** السلوك الافتراضي لـ Project Operations، وستُعاد التعيينات إلى الموارد العامة.

لمزيد من الإعدادات الافتراضية حول الإجراءات، راجع [استخدام إجراءات API الويب](/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>تحديد الحقول المراد نسخها 
عند استدعاء الإجراء، يبحث **نسخ المشروع** في طريقة عرض المشروع **نسخ أعمدة المشروع** لتحديد الحقول التي يجب نسخها عند نسخ المشروع.


### <a name="example"></a>مثال
يوضح المثال التالي كيفية استدعاء الإجراء المخصص **CopyProject** مع مجموعة المعلمات **RemoveNamedResources**.
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

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
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]