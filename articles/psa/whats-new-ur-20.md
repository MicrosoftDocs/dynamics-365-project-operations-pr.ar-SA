---
title: الجديد أو المتغير في الإصدار 3 من Project Service Automation، إصدار التحديث 20
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 20.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: 12edae76dbc6de63d3e2d36058c4092f80ede77d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070593"
---
# <a name="project-service-automation-update-release-20-v3"></a>الإصدار 3 من Project Service Automation، إصدار التحديث 20

يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 20. لدى هذا الإصدار رقم البنية V 3.10.31.37 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر يونيو 2020.

## <a name="update-release-20"></a>إصدار التحديث 20

### <a name="bug-fixes"></a>إصلاحات الأخطاء

**إدارة المشروع**

تم إصلاح المشكلات التالية:

- يؤدي استيراد أعضاء فريق المشروع الذين لديهم طريقة تخصيص تحتاج إلى ساعات ساعات إلى ظهور رسالة خطأ غير واضحة عندما تكون قيمة الساعات المحددة صفرية.
- يتلقى المستخدمون رسالة خطأ غير صحيحة عند إدخال الحد الأقصى لعدد الأحرف في حقل **الوصف** لمهمة مشروع.
- تقوم صفحة **تنزيل الوظيفة الإضافية Microsoft Dynamics 365 Project Service Automation** بإعادة التوجيه إلى صفحة التنزيل باللغة الإنجليزية عند تعيين إعدادات لغة المستخدم إلى اليابانية.
- عند حدوث خطأ في الخادم، تبقى في بعض الأحيان تسمية المزامنة على علامة تبويب **الجدول** في نموذج **المشاريع**.
- يتم إرسال تحديثات المهمة المتكررة إلى الخادم عند تعديل مهمة.

**المبيعات**

تم إصلاح المشكلات التالية:

- في نموذج **العقد** ، يؤدي النقر المزدوج فوق **إنشاء فاتورة** إلى إنشاء فاتورتين لسجل القيمة الفعلية الفردية.
- في Internet Explorer 11، يتعذر على المستخدمين إنشاء إدخالات مصروفات.
- عكس التكلفة وعكس قيم المبيعات الفعلية غير المفوترة غير مرتبطين.
- لا يؤدي الضغط على الزر **تحديث القيم الفعلية** على نموذج **المشروع** إلى تحديث **الساعات الفعلية‬ للمهمة**.
- بإمكان المكون الإضافي **PreValidateProjectTeamMemberCreate** إنشاء موارد عامة قابلة للحجز عند تعيين السمة **msdyn_isgenericresourceprojectscoped** إلى **خطأ**.
- يقوم الخيار **إعادة الحساب** بمسح التكاليف الخاضعة للرسوم لتفاصيل بنود عرض أسعار يستند إلى منتج وتفاصيل شروط التعاقد.
- في سيناريوهات معينة، يعرض المكون الإضافي **PostEstimateLineUpdate** خطأ استثناء مرجعيُا.
- لا تتطابق مدة المرحلة الزمنية على **مخطط تحليل الربحية** مع مدة التكاليف في تفاصيل بنود عرض الأسعار الثابتة السعر في عرض الأسعار.
- لا يتم تحديد قيم الوحدة ومجموعات الوحدات بشكل افتراضي صحيح لفئات المصروفات في النموذجين **تفاصيل شروط التعاقد** و **تفاصيل بنود عرض الأسعار**.
- تسمح قوائم **سعر تكلفة الوحدة التنظيمية** بحالات تداخل في سريان التاريخ.‬
- لا يُسمح للمستخدمين بتغيير **OrgUnit** عندما لا يكون نوع الأمر قائمًا على العمل لأنه سيؤدي إلى خطأ استثناء مرجعي فارغ.
- عند محاولة الانتقال من نموذج **تفاصيل بنود عرض الأسعار** ، والعودة إلى علامة تبويب **عرض الأسعار** ، يتم تحديث النموذج ويعرض علامة تبويب **الملخص**.