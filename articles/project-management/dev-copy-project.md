---
title: تطوير قوالب المشروع مع نسخ المشروع‬
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء قوالب مشروع باستخدام إجراء "نسخ المشروع" المخصص.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb49109e8c199bc4569702ae844a19985534294d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070584"
---
# <a name="develop-project-templates-with-copy-project"></a>تطوير قوالب المشروع مع نسخ المشروع‬

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

يدعم Dynamics 365 Project Operations القدرة على نسخ مشروع وإرجاع أي تعيينات إلى الموارد العامة التي تمثل الدور. يمكن للعملاء استخدام هذه الوظيفة لبناء قوالب المشروع الأساسية.

عند تحديد **نسخ المشروع** ، يتم تحديث حالة المشروع الهدف. استخدم **سبب الحالة** لتحديد وقت اكتمال إجراء النسخ. يؤدي أيضًا تحديد **نسخ المشروع** إلى تحديث تاريخ بدء المشروع إلى تاريخ البدء الحالي في حال عدم اكتشاف تاريخ مستهدف في كيان المشروع الهدف.

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


- **{"clearTeamsAndAssignments":true}** : السلوك الافتراضي لمشروع الويب، وستتم إزالة جميع التعيينات وأعضاء الفريق.
- **{"removeNamedResources":true}** السلوك الافتراضي لـ Project Operations، وستُعاد التعيينات إلى الموارد العامة.

لمزيد من الإعدادات الافتراضية حول الإجراءات، راجع [استخدام إجراءات API الويب](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>تحديد الحقول المراد نسخها 
عند استدعاء الإجراء، يبحث **نسخ المشروع** في طريقة عرض المشروع **نسخ أعمدة المشروع** لتحديد الحقول التي يجب نسخها عند نسخ المشروع.
