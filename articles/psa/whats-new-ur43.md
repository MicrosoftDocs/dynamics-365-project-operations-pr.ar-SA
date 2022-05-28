---
title: الجديد أو المتغير في إصدار التحديث 43، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في تحديث Microsoft Dynamics 365 Project Service Automation الإصدار 43، V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 05/04/2022
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
ms.openlocfilehash: fcf18a24b3bc354a16a415368063133743e79696
ms.sourcegitcommit: 7e419a5f73f80fa887084e3b212c90586fc397dd
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/05/2022
ms.locfileid: "8709952"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-43-v3"></a>الجديد أو المتغير في إصدار التحديث 43، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. إنه متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو المتغيرة لتحديث Project Service Automation الإصدار 43، V3. لدى هذا الإصدار رقم البنية V3.10.74.200 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر مايو 2022.

## <a name="update-release-43"></a>إصدار التحديث 43

### <a name="bug-fixes"></a>إصلاحات الأخطاء

تم إصلاح المشكلات التالية.


**الوقت والمصروفات**

- عند استيراد إدخالات الوقت من الحجوزات أو تعيينات الموارد، لا يتم الاحتفاظ بالإشارة إلى المورد القابل للحجز ذي الصلة.
- عندما يتم توسيع شبكة إدخال الوقت إلى وضع ملء الشاشة، لا يعمل التنقل في الشبكة باستخدام مفتاح علامة التبويب.
- عند إرسال إدخال وقت تم إنشاؤه بواسطة مستخدم آخر، يتم ملء حقل **الإرسال بواسطة** المستخدم الذي أنشأ جدول الوقت بشكل غير صحيح.
