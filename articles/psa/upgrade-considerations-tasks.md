---
title: اعتبارات ترقية هيكل تنظيم العمل
description: يقدم هذا الموضوع معلومات حول ترقية هيكل تنظيم العمل من الإصدار 2.x حتى الإصدار 3.x من Project Service Automation.
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: 5258813410c3cea015775898cc72ba1574549edd8ee0c8b7aad8c94943eb5a60
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "6992325"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a>اعتبارات ترقية هيكل تنظيم العمل

[!include [banner](../includes/psa-now-project-operations.md)]

يقدم هذا الموضوع معلومات حول ترقية هيكل تنظيم العمل من الإصدار 2.x حتى الإصدار 3.x من Project Service Automation. يحدد هذا الموضوع الحالة السليمة لمشروع في Project Service Automation (PSA) المطلوب للترقية الناجحة. كما توجد أيضا معلومات حول حالات الحظر الشائعة التي ستؤدي إلى فشل الترقية. للحصول على مزيد من المعلومات حول تعريف مهام المشروع ووظائفها في جدول مشروع، راجع[جداول المشروع](project-creating.md).

## <a name="key-entities"></a>الكيانات الرئيسية
بالنسبة لهيكل تنظيم عمل دقيق تم تحميله بالفعل بالموارد، تكون الكيانات التالية مطلوبة:

- [المشروع](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [فريق المشروع](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [مهمة المشروع](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [تعيينات الموارد](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [تبعية مهمة المشروع](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [الموارد القابلة للحجز](/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

لتحديد هيكل تنظيم عمل تم تحميله لمورد، يجب إكمال الخطوات التالية:

1. إنشاء مشروع جديد. لمزيد من المعلومات حول كيفية إنشاء مشروع جديد، راجع [msdyn_project](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).
2. إنشاء مهمة واحده أو أكثر. لمزيد من المعلومات حول كيفية إنشاء مهمة، راجع [msdyn_projecttask](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).
3. تحديد تبعيات المهام. لمزيد من المعلومات، راجع [تبعية مهمة المشروع](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).
4. تعيين أعضاء فريق المشروع للمشروع. لمزيد من المعلومات، راجع [msdyn_projectteam](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).
5. تعيين أعضاء فريق المشروع للمهام. لمزيد من المعلومات، راجع [msdyn_resourceassignment](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).

## <a name="project-team-relationships"></a>علاقات فريق المشروع

لضمان إجراء ترقية ناجحة، يجب الاحتفاظ بالعلاقات التالية بشكل صحيح:
- يجب أن يكون كافة أعضاء فريق المشروع مقترنين بمورد قابل للحجز.
- يجب أن يكون كافة أعضاء فريق المشروع مقترنين بنفس المشروع. 

## <a name="project-task-relationships"></a>علاقات مهام المشروع
لضمان إجراء ترقية ناجحة، يجب الاحتفاظ بالعلاقات التالية بشكل صحيح:

- يجب أن تكون أي مهام مرتبطة مقترنة بنفس المشروع.
- يجب أن يكون لكل مهمة بند مهمة أصل.
- يجب أن يكون لكل مهمة مشروع أصل.

### <a name="valid-conditions"></a>الشروط الصالحة

- يجب أن تكون كافة مدد المهام أكبر من أو تساوي (> =) ساعة واحدة وأقل من 1,800,000 دقيقة (1,250 يوم).*
- يجب أن يكون لكافة المهام تاريخ بدء قبل 2000/01/01.*
- يجب أن تحتوي كافة المهام على تاريخ بدء ليس بعد 17 سنة من اليوم الحالي.*
- يجب أن يكون لكافة المهام تاريخ بدء قبل أو يساوي تاريخ الانتهاء.
- يجب أن تحتوي كافة أنواع الحركات الموجودة في التصنيفات (المصروفات، والمواد، والضريبة، والوقت) على قيم لـ **الوحدة الافتراضية** و **مجموعة الوحدات**.
- ينبغي تجنب تنسيقات التاريخ مع الأحرف.

### <a name="potential-mitigation-steps"></a>خطوات تخفيف المخاطر المحتملة
- استخدم البحث المتقدم لتحديد مهام المشروع التي لا تتضمن معرف مشروع.
- استخدم البحث المتقدم لتحديد مهام المشروع حيث المدة المجدولة أكبر من > 1,800,000.
- قبل إجراء أي تغييرات على البيانات، يجب عليك التحقق من أي تخصيصات مرتبطة بالكيان والتي من المحتمل أن تكون قد أدت إلى وجود البيانات في حالة سيئة. يجب معالجة هذه التخصيصات قبل متابعة أي تحديثات ذات صلة بالبيانات.
- بالنسبة إلى المحددة التي تم عزلها، ضع في اعتبارك حذف هذه المهام إذا لم تكن مطلوبة أو إذا كان يجب ربطها بالمشروع الأصلي الصحيح.
- بالنسبة إلى مهام تتجاوز مدتها 1,250، عليك أن تأخذ في الاعتبار إضافة مهام متعددة لتمثيل المدة الإجمالية، إذا كان ذلك ممكنًا.

> [!NOTE]
> العناصر المميزة بعلامة نجمية (\*) لها حدود لأن إدارة علاقات العملاء (CRM) تدعم 7,320 عملية فقط من عمليات توسيع التكرار. يجب أن تبقى دون هذا الحد.

## <a name="resource-assignment-relationships"></a>علاقات تعيينات الموارد
لضمان إجراء ترقية ناجحة، يجب الاحتفاظ بالعلاقات التالية بشكل صحيح:

- يجب أن تكون كافة تعيينات الموارد الموجودة في هيكل تنظيم العمل مرتبطة بنفس المشروع.
- يجب أن تكون كافة تعيينات الموارد الموجودة في هيكل تنظيم العمل مرتبطة بأعضاء فريق المشروع في نفس المشروع.

### <a name="potential-mitigation-steps"></a>خطوات تخفيف المخاطر المحتملة
- حدد كافة المهام التي تقع خارج الشروط الموضحة أعلاه.  
- ينبغي حذف تعيينات الموارد التي لم تعد صالحة.

## <a name="project-task-dependency-relationships"></a>علاقات تبعيات مهام المشاريع
لضمان إجراء ترقية ناجحة، يجب الاحتفاظ بالعلاقات التالية بشكل صحيح:

- يجب أن تكون كافة تبعيات مهام المشروع مرتبطة بنفس المشروع.
- لا يمكن أن يكون لمهمة نفس التبعية مشار إليها أكثر من مرة.


[!INCLUDE[footer-include](../includes/footer-banner.md)]