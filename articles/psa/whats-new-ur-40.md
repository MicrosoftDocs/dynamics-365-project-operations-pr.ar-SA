---
title: الجديد أو المتغير في إصدار التحديث 40، الإصدار 3 من Project Service Automation
description: يسرد هذا المقال الميزات والإصلاحات المتوفرة في إصدار التحديث 40، الإصدار 3 من Microsoft Dynamics 365 Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/31/2022
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
ms.openlocfilehash: dca7f340b8d544b183aa0390ac3c11a38f536ed0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912776"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-40-v3"></a>الجديد أو المتغير في إصدار التحديث 40، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. وهو متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا المقال الميزات والإصلاحات الجديدة أو المتغيرة في إصدار التحديث 40، الإصدار 3 من Project Service Automation. يحتوي هذا الإصدار على رقم إصدار V3.10.61.61 وهو متاح بشكل عام من خلال التحديث الذاتي في فبراير 2022.

## <a name="update-release-40"></a>إصدار التحديث 40

### <a name="features"></a>الميزات
سيتم إصدار المرحلة الأولى من الترقية من Project Service Automation إلى Project Operations - الخفيف في فبراير 2022 لجميع العملاء. للتحقق من التأهيل، راجع [الترقية من Project Service Automation إلى Project Operations](upgrade-project-operations-non-stocked.md). إذا لم يظهر التطبيق في المثيل الخاص بك في مركز إدارة Power Platform، اتصل بالدعم واطلب تمكين الرحلة لبيئاتك. يجب أن يتضمن طلبك قائمة بمعرفات البيئة حيث تحتاج الرحلة إلى التمكين.

### <a name="bug-fixes"></a>إصلاحات الأخطاء

تم إصلاح المشكلات التالية.

**الوقت والمصروفات**
- يكون إدخال الملاحظة مفقودًا عند رفض إدخال الوقت أو إلغاؤه. 

**‏المبيعات**

- عند تحديث تقديرات التكلفة أو المبيعات باستخدام المكونات الإضافية الجاهزة، تم السماح لك بشكل غير صحيح بإرسال حمولات JSON غير الصالحة خارج واجهة المستخدم.
- عند تحديث سطور عرض الأسعار باستخدام العرض السريع، يُسمح لك بتنشيط عروض الأسعار.