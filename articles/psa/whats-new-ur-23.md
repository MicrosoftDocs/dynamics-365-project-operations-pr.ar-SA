---
title: الجديد أو المتغير في إصدار التحديث 23، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 23.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: eaae9cc62c449695cb2e999be48c57075aadbb21
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070591"
---
# <a name="project-service-automation-update-release-23-v3"></a>الإصدار 3 من Project Service Automation، إصدار التحديث 23

يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 23. يتضمن هذا الإصدار رقم البنية V 3.10.34.30 وهو متوفر بشكل عام من خلال تحديث ذاتي في أغسطس 2020.

## <a name="update-release-23"></a>إصدار التحديث 23

### <a name="bug-fixes"></a>إصلاحات الأخطاء

**الوقت والمصروفات**

تم إصلاح المشكلات التالية:
- معالجة الحالة الطرفية في **حذف عضو فريق المشروع** لتوفير استثناء ذي معنىً.
- ينتج عن استيراد التعيين شاشة إزالة فارغة.

**إدارة الموارد**

تم إصلاح المشكلات التالية:

- تعرض **بطاقة مورد شبكة استخدام المورد** بيانات غير صحيحة عندما يزيد مقياس الوقت عن خمسة أيام.
- عندما يقوم العملاء بإنشاء مورد قابل للحجز، يفشل المكون الإضافي بشكل متقطع في إضافة المورد إلى مجموعة Microsoft Office 365 بشكل تلقائي.
- تُظهر طريقة عرض **التسوية** الحدود اليدوية بشكل غير صحيح في طريق عرض **الأسبوع** أو **الشهر**.

**إدارة المشروع**

تم إصلاح المشكلات التالية:

- يتسبب عدد كبير من كيانات **RetrieveMultiple لإعدادات المستخدم** في حدوث في تراجع أداء عمليات الموافقة على المشروع والعمليات الأخرى.
- يقتصر البحث عن مورد شبكة **تخطيط المهمة** على عرض خمسة أعضاء فقط من فريق المشروع. 
- لا يقوم البحث عن مورد شبكة **تخطيط المهمة** بتصفية الموارد غير النشطة.
- الوضع اليدوي لا يعمل كما هو متوقع في هيكل تنظيم عمل تخطيط المشروع.
- شبكة **تخطيط المهمة** تعرض **فئات الحركة غير النشطة**.
- يتم تقريب شبكة **تعيينات الموارد** بشكل غير صحيح عندما تحتوي مهمة على تعيينات متعددة.
- تختلف قيم التقريب ما بين التكلفة المخططة والتكلفة الفعلية لمهمة واحدة.

**المبيعات**

تم إصلاح المشكلات التالية:

- يؤدي النقر المزدوج فوق **إحضار جميع فئات الحركات** إلى إنشاء أسطر متعددة.