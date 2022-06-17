---
title: الجديد أو المتغير في تحديث Project Service Automation الإصدار 34, V3
description: يسرد هذا المقال الميزات والإصلاحات المتوفرة في إصدار التحديث 34، الإصدار 3 من Project Service Automation.
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
ms.reviewer: johnmichalak
ms.openlocfilehash: e47a5442f285952c165a2d30e337a362a6b065dd
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928646"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-34-v3"></a>الجديد أو المتغير في تحديث Project Service Automation الإصدار 34, V3

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. وهو متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا المقال الميزات والإصلاحات الجديدة أو المتغيرة في إصدار التحديث 34، الإصدار 3 من Project Service Automation. يحتوي هذا الإصدار على رقم إصدار V3.10.55.38 وهو متاح بشكل عام من خلال التحديث الذاتي في يوليو 2021.

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
