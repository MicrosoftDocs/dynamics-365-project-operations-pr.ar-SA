---
title: الجديد أو المتغير في تحديث Project Service Automation الإصدار 34, V3
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في تحديث Project Service Automation، الإصدار 34, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 08/05/2021
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
ms.openlocfilehash: 528d4f8d108720cb9c912cea1c0d5f37e3716eec
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323265"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-34-v3"></a>الجديد أو المتغير في تحديث Project Service Automation الإصدار 34, V3

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. وهو متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في Project Service Automation V3، تحديث الإصدار 34. يحتوي هذا الإصدار على رقم إصدار V3.10.55.38 وهو متاح بشكل عام من خلال التحديث الذاتي في يوليو 2021.

## <a name="update-release-34"></a>إصدار التحديث 34

### <a name="bug-fixes"></a>إصلاحات الأخطاء
تم إصلاح المشكلات التالية.

**عام**

- لا تقوم التحديثات التي يقودها الناشر بتنشيط سير العمل الجديد للموافقة عليه.
- تفتقد السمتين **الحالة الهدف** و **"نوع الإجراء** في الصفحة الرئيسية **مجموعة الموافقة**.

**الوقت والمصروفات**

- تعذر الموافقة على طلب تقديمه باستخدام تدفق الموافقة الحديث.
- لا تعمل إدخالات نسخ أسبوع من الوقت عند نسخ الإدخالات غير المرتبطة بمستخدم التسجيل.

**تخطيط المشروع**

- تالفة في حالة استيرادها من الخاصية الإضافية سطح مكتب Microsoft Project.

**إدارة الموارد**

- عند نشر مشروع من الوظائف الإضافية في عميل سطح مكتب Microsoft Project، يتم تغيير تاريخ انتهاء المتطلبات الحالية.
- تتجاوز الدقة العشرية المكانين العشريين في مربع حوار تأكيد حجوزات تمديد الحجوزات.

**‏المبيعات**

- عند إضافة سطر مستند إلى المنتج بمنتج موجود إلى عقد مشروع، يتم عرض **مفتاح غير موجود في استثناء القاموس**.
- لا يمكن تأهيل العملاء المتوقعين عند تعيين نوع أمر من أحد العملاء المتوقعين إلى فرصة.
