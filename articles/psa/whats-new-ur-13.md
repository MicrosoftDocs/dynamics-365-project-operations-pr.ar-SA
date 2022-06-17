---
title: الجديد أو المتغير في إصدار التحديث 13، الإصدار 3 من Project Service Automation
description: يقدم هذا المقال معلومات حول الجديد والمتغير في إصدار التحديث 13، الإصدار 3 ‬من Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: f4898391922f5ecbc99d78e49358ea749fe27b3f
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930670"
---
# <a name="project-service-automation-update-release-13-v3"></a>الإصدار 3 من Project Service Automation، إصدار التحديث 13

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا الإعلان عن آخر تحديث لتطبيق Dynamics 365 Project Service Automation (PSA). يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا المقال الميزات والإصلاحات الجديدة أو المتغيرة في إصدار التحديث 13، الإصدار 3 من Project Service Automation. يتضمن هذا الإصدار رقم البنية V3.10.3.18 وهو متوفر وفق الجدول التالي:

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

     - إصلاح: استثناء مرجع فارغ عند تعيين عضو الفريق عندما يفتقد **TransactionType** معلومات الإعداد لكل من **الوحدة** و **DefaultGroup**.

- ‏‏Sales

     - إصلاح: سجلات نوع الحركة المكررة ترجع خطأ عند إنشاء سجلات أسعار الأدوار.
     - ‏‫تم الإصلاح: الأزرار الإضافية **فرصة جديدة** و **عرض الأسعار** و **بند الأمر** و **إضافة منتج** مرئية في الأوامر في الشبكة الفرعية الفرص وعروض الأسعار ومنتجات الأوامر والبنود القائمة على المشروع.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
