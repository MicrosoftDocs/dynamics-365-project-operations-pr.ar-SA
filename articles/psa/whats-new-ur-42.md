---
title: الجديد أو المتغير في إصدار التحديث 42، الإصدار 3 من Project Service Automation
description: يسرد هذا المقال الميزات والإصلاحات المتوفرة في إصدار التحديث 42، الإصدار 3 من Microsoft Dynamics 365 Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/05/2022
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
ms.openlocfilehash: e9911531e4acbd78db416f554c8d85c4f1fee1cf
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912699"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>الجديد أو المتغير في إصدار التحديث 42، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. وهو متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا المقال الميزات والإصلاحات الجديدة أو المتغيرة في إصدار التحديث 42، الإصدار 3 من Project Service Automation. لدى هذا الإصدار رقم البنية V3.10.73.61 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر أبريل 2022.

## <a name="update-release-42"></a>إصدار التحديث 42

### <a name="bug-fixes"></a>إصلاحات الأخطاء

تم إصلاح المشكلات التالية.

**الوقت والمصروفات**

- عندما يتم رفض صحيفة زمنية، يتم تحديد المستخدم الذي رفضها بشكل غير صحيح على أنه **النظام**.
- عند استيراد إدخالات الوقت، تكون قيمة **فئة المورد** مفقودة.
- يمكن للموافقين على المشروع الموافقة على المشاريع المقدمة عندما لا يتم تعيين أذوناتهم على وجه التحديد على **يمكن الموافقة**.

**‏المبيعات**

- عندما يتم تسجيل القيم الفعلية في مهام ليست على مستوى الجذر، يتم تجميع التكاليف الفعلية بشكل غير صحيح.
