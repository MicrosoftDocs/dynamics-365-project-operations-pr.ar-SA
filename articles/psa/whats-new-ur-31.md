---
title: الجديد أو المتغير في إصدار التحديث 31، للإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 31، الإصدار 3 من Project Service Automation‬.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: a595c0a129ac35d3416984e57908e73e1eaef2fd
ms.sourcegitcommit: 6e1498502461e86cff722ccaf8795ff11c7c47ad
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5945519"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a>الجديد أو المتغير في إصدار التحديث 31، للإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في في إصدار التحديث 31، الإصدار 3 من Project Service Automation‬. لدى هذا الإصدار رقم البنية V3.10.52.77 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر مايو 2021.

## <a name="update-release-31"></a>إصدار التحديث 31

### <a name="bug-fixes"></a>إصلاحات الأخطاء

**الوقت والمصروفات**

تم إصلاح المشكلات التالية:

- كانت أزرار أوامر التحكم في إدخال الوقت في صفحة **الموارد القابلة للحجز** محيرة.
- تم إنشاء استثناء مرجعي فارغ في **Project.SetTrackingFields** عند الموافقة على إدخال وقت.

**إدارة الموارد**

تم إصلاح المشكلات التالية:

- لا يعرض  **إنشاء عضو الفريق**  بشكل صحيح إعداد بيانات تعريف إعداد الحجز لـ **حالة الحجز الملتزم بها في السجل الافتراضي‬**.
- عند الترقية من PSA 1.X إلى 3.X، تفشل عملية الترقية في **UpgradeResourceRequirements**.


**‏المبيعات**

تم إصلاح المشكلات التالية:

- يحول الإيراد الفعلي المبالغ إلى عملة المشروع في شبكة التعقب.
- يكون افتراضي العملة غير واضح عند إنشاء خطوط سطور دفتر اليومية وسطور عرض الأسعار وشروط التعاقد في السيناريوهات التي تختلف فيها العملة الأساسية للمنظمة عن عملة المشروع.
- لا يتم تصفية استعلام **التحقق من صحة دفتر يومية التصحيحات المعلقة** حسب المشروع.
- يتم حساب المبيعات المتبقية بشكل غير صحيح على المشروع.
- تفشل عروض الأسعار المستندة إلى جهة اتصال عند إنشائها دون قائمة أسعار.
- لا يظهر مؤشر تقدم المعالجة الدائري عند تحديد **تأكيد الفاتورة**.
- لا يظهر مؤشر تقدم المعالجة الدائري عند تحديد **إنشاء الفاتورة**.
- لا يلغي إغلاق عرض الأسعار الحجوزات.






