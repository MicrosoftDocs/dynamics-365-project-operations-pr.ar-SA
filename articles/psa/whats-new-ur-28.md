---
title: الجديد أو المتغير في إصدار التحديث 28، الإصدار V3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 28، الإصدار V3 من Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: b06a5ee6d0e2da76801a36701f38f1885d6c7562
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010500"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a>الجديد أو المتغير في إصدار التحديث 28، الإصدار V3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو المتغير ة في إصدار التحديث 28، الإصدار V3 من Project Service Automation. يتضمن هذا الإصدار رقم البنية V3.10.46.32 وهو يتوفر بشكل عام عبر تحديث ذاتي في يناير 2021.

## <a name="update-release-28"></a>إصدار التحديث 28

### <a name="bug-fixes"></a>إصلاحات الأخطاء

**الوقت والمصروفات**

تم إصلاح المشكلات التالية:

- يمكن للمستخدمين عمل **تحرير مجمع** لتحديث إدخالات الوقت التي تم قبولها وتم إرسالها.

**إدارة المشروع**

تم إصلاح المشكلات التالية:

- في الحالات التي يتم فيها تفسير المعرف الفريد العمومي للمهمة كرقم، لا يمكن فتح المهام للتحرير باستخدام **تحرير المهمة** في الشريط في صفحة **هيكل تنظيم العمل**.

**المبيعات**

تم إصلاح المشكلات التالية:

- يتم إنشاء استثناء مرجع فارغ عند استدعاء المكون الإضافي **GetEstimatesForProject**.
- **وضع علامة جاهزة للفاتورة** على شبكة الأحداث الرئيسي جزئيًا فقط يؤدي إلى تحديث السمات، باستثناء السمة **InvoiceStatus** الذي يتم تحديثه.



[!INCLUDE[footer-include](../includes/footer-banner.md)]