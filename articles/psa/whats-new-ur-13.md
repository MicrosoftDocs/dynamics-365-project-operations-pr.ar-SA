---
title: الجديد أو المتغير في إصدار التحديث 13، الإصدار 3 من Project Service Automation
description: يقدم هذا الموضوع معلومات حول الجديد في إصدار التحديث 13، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 435b70255dd0053a496362c9ced9e742cfcca843
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070604"
---
# <a name="project-service-automation-update-release-13-v3"></a>الإصدار 3 من Project Service Automation، إصدار التحديث 13
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

     - إصلاح: استثناء مرجع فارغ عند تعيين عضو الفريق عندما يفتقد **TransactionType** معلومات الإعداد لكل من **الوحدة** و **DefaultGroup**.

- ‏‏Sales

     - إصلاح: سجلات نوع الحركة المكررة ترجع خطأ عند إنشاء سجلات أسعار الأدوار.
     - إصلاح: تظهر أزرار إضافية لكل من **فرصة جديدة** و **عرض أسعار** و **بند الأمر‬** و **إضافة منتج** في الأوامر الخاصة بالفرص وعروض الاسعار ومنتجات الأوامر والشبكة الفرعية للبنود المستندة إلى المشروع.

