---
title: الجديد أو المتغير في إصدار التحديث 14، الإصدار 3 من Project Service Automation
description: يقدم هذا الموضوع معلومات حول الجديد في إصدار التحديث 14، الإصدار 3 من Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
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
ms.openlocfilehash: 71971b96ea6955b95fa519884356a310b2885d0667d60ca07856a444de77dc64
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "6987015"
---
# <a name="project-service-automation-update-release-14-v3"></a>الإصدار 3 من Project Service Automation، إصدار التحديث 14

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا الإعلان عن آخر تحديث لتطبيق Dynamics 365 Project Service Automation (PSA). يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في PSA V3، إصدار التحديث 14. يتضمن هذا الإصدار رقم البنية V3.10.4.21 وهو متوفر وفق الجدول التالي:

- **التوافر العام (ذاتي التحديث):** يناير 2020
- **تحديث تلقائي:** فبراير 2020

## <a name="update-release-14"></a>إصدار التحديث 14

### <a name="enhancements"></a>التحسينات

- ‏‏Sales

     - يتم نسخ قيم الحقول المخصصة من **تفاصيل بند عرض الأسعار‬‬** إلى **تفاصيل بنود عقد المشروع‬** عند تحديث عرض أسعار إلى **إغلاق كمكتسب**.
     - المشاريع المؤكدة يمكن **إغلاقها كخاسرة**.

- إدارة الموارد

     - عند تمديد الحجوزات، ستتم مطالبة المستخدمين بواسطة مربع حوار تأكيد لتلخيص نتائج الحجز وتوفير ارتباط إلى "المحافظة على الحجوزات‬".


### <a name="bug-fixes"></a>إصلاحات الأخطاء

- الوقت والمصروفات

     - إصلاح: تم تحسين تجربة المستخدم عندما لم يحدد المستخدم أي إدخالات لتصحيحها.

- إدارة الموارد

     - إصلاح: يؤدي حجز مورد عدة مرات إلى تجاوز اسم المورد القابل للحجز.

- ‏‏Sales

     - إصلاح: لا يتم حساب إجمالي سعر المبيعات حتى يقوم المستخدم أيضًا بإدخال سعر التكلفة لتقديرات المصروفات في المشروع.
     - ثابت: يفشل إغلاق عرض أسعار على أنه **فائز** إذا لم يكن عقد المشروع المقترن به في حالة **المسودة**.



[!INCLUDE[footer-include](../includes/footer-banner.md)]