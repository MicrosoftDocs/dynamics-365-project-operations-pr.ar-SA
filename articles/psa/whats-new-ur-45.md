---
title: الجديد أو المتغير في إصدار التحديث 45، الإصدار 3 من Project Service Automation
description: يسرد هذا المقال الميزات والإصلاحات المتوفرة في إصدار التحديث 45، الإصدار 3 من Microsoft Dynamics 365 Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 07/14/2022
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
ms.openlocfilehash: 98f7c973917d7d6334e6e0aeb15214c538b33143
ms.sourcegitcommit: 36fda4f45ddeb0f81d30bd1e22852727df644754
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2022
ms.locfileid: "9169146"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-45-v3"></a>الجديد أو المتغير في إصدار التحديث 45، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. وهو متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا المقال الميزات والإصلاحات الجديدة أو المتغيرة في إصدار التحديث 45، الإصدار 3 من Project Service Automation. يحتوي هذا الإصدار على رقم إصدار V3.10.76.168 وهو متاح بشكل عام من خلال التحديث الذاتي في يوليو 2022.

## <a name="update-release-45"></a>إصدار التحديث 45

### <a name="bug-fixes"></a>إصلاحات الأخطاء

تم إصلاح المشكلات التالية.

**‏المبيعات**

- لا يمكن للمستخدمين إنشاء الفواتير بنجاح بعد محاولتهم إنشاء فاتورة دون أية مبيعات غير مفوترة إذا يقومون بعرض نفس مثيل الصفحة ولا يقومون بتحديثها.

**الوقت والمصروفات**

- عند تمكين الموافقات الحديثة والموافقة على المشروع الذي تم قبوله، يتم تحديث مرحلة السجل بشكل غير صحيح إلى **‏‫تمت الموافقة على طلب الاستدعاء‬**.
- عند تمكين الموافقات الحديثة وحين تكون تدفقات السحابة غير نشطة، تكون عملية الاعتماد غير ناجحة، ولا يتم إعلام المستخدمين بإرسال أو موافقة.
