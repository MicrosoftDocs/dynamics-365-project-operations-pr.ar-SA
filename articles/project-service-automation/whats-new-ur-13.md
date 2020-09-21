---
title: ما الجديد في إصدار التحديث 13، الإصدار 3 من Project Service Automation
description: يقدم هذا الموضوع معلومات حول الجديد في إصدار التحديث 13، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: c6f6a5b6-b5bb-467c-b7c7-7fb962504c6d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5f1b6b3879c94a77ab62082aad1e470a3ba66552
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748654"
---
# <a name="project-service-automation-v3-update-release-13"></a>الإصدار 3 من Project Service Automation، إصدار التحديث 13
يسرنا الإعلان عن آخر تحديث لتطبيق Dynamics 365 Project Service Automation (PSA). يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 13. يتضمن هذا الإصدار رقم البنية V3.10.3.18 وهو متوفر وفق الجدول التالي:

- **التوافر العام (ذاتي التحديث):** نوفمبر 2019
- **تحديث تلقائي:** ديسمبر 2019


## <a name="update-release-13"></a>إصدار التحديث 13 

### <a name="bug-fixes"></a>إصلاحات الأخطاء

- الوقت والمصروفات

     - إصلاح: لا تعمل وظيفة البحث في صفحة **الموافقة على المصروفات** عند البحث حسب غرض المصروفات.

- إدارة الموارد

     - إصلاح: تم تحديث الأرقام الموجودة في التسوية ليتم ضبطها إلى اليمين.
     - إصلاح: لا يمكن تعيين الموارد المسامة إلى المهام من خلال علامة تبويب **الجدول**.

- إدارة المشروع

     - إصلاح: استثناء مرجع فارغ عند تعيين عضو الفريق عندما يفتقد **TransactionType** معلومات الإعداد لكل من **الوحدة** و**DefaultGroup**.

- ‏‏Sales

     - إصلاح: سجلات نوع الحركة المكررة ترجع خطأ عند إنشاء سجلات أسعار الأدوار.
     - إصلاح: تظهر أزرار إضافية لكل من **فرصة جديدة** و**عرض أسعار** و**بند الأمر‬** و**إضافة منتج** في الأوامر الخاصة بالفرص وعروض الاسعار ومنتجات الأوامر والشبكة الفرعية للبنود المستندة إلى المشروع.


