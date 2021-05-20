---
title: الجديد أو المتغير في إصدار التحديث 25، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 25، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 3aa10e1d4b23fbe6c2743d71497bdef840776008
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948855"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a>الجديد أو المتغير في إصدار التحديث 25، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو المتغير ة في إصدار التحديث 25، الإصدار 3 من Project Service Automation. يتضمن هذا الإصدار رقم البنية V 3.10.43.76 وهو يتوفر بشكل عام عبر تحديث ذاتي في أكتوبر 2020.

## <a name="update-release-25"></a>إصدار التحديث 25

### <a name="bug-fixes"></a>إصلاحات الأخطاء

**الوقت والمصروفات**

تم إصلاح المشاكل التالية:

- مخطط إدخال الوقت يعرض بيانات إضافية استنادًا إلى فاصل زمني بحجم كبير جدًا تم استرداده.

**إدارة الموارد**

تم إصلاح المشاكل التالية:

- تمت إضافة كود Package Deployer لتخطي استيراد تصحيح Universal Resource Scheduling في حال وجود تصحيح من إصدار أعلى.

**إدارة المشروع**

تم إصلاح المشكلات التالية:

- تصحيح اختلافات التقريب وسعر الصرف التي تؤدي إلى تكلفة مخططة غير صحيحة في شبكة تعقب المشروع.
- دعم القدرة على عرض شبكتين أو أكثر من شبكات التفاعل على نموذج **المشروع**.
- توفير التحقق من الصحة لمعالجة القدرة على تعيين مهمة قبل تاريخ انتهاء التقويم، مما يؤدي إلى تعيين مورد فاشل.
- معالجة محسنة للأخطاء لمعالجة استثناء القيمة الفارغة الذي ينشأ مما يلي:

    - المكون الإضافي **PreValidateProjectTeamMemberCreate‎**
    - **PreValidateProjectTaskCreate** عند إنشاء مهمة مشروع بدون مشروع مقترن
    - المكون الإضافي **PreProjectTeamMemberCreate‎**
    - المكون الإضافي **PostProjectTeamMemberDelete‎**
    - المكون الإضافي **PreValidateProjectTaskDelete**

**المبيعات**

تم إصلاح المشكلات التالية:

- معالجة محسنة للأخطاء لمعالجة استثناء القيمة الفارغة الذي ينشأ من **Copy Project: Estimates HelperResource Management**.
- الخيار **غير جاهز للفوترة** على **تراكم فوترة الوقت والمواد‬** لا يمسح حالة الفوترة.
- أزرار **الأسعار** ذات التسمية المصححة على علامة تبويب **دور السعر** و **أصناف الكتالوج**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]