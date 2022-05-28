---
title: الجديد أو المتغير في إصدار التحديث 29، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 29، الإصدار V3 من Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 56cf47d207c7ee518d5d4b53866c3d6ddf1d1fb3
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8587202"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a>الجديد أو المتغير في إصدار التحديث 29، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار V3 من Project Service Automation، إصدار التحديث 29. يحتوي هذا الإصدار على رقم إصدار V3.10.47.7 وهو متاح بشكل عام من خلال التحديث الذاتي في فبراير 2021.

## <a name="update-release-29"></a>إصدار التحديث 29

### <a name="bug-fixes"></a>إصلاحات الأخطاء

**الوقت والمصروفات**

تم إصلاح المشكلات التالية:

- يتعذر على للمستخدمين رؤية ساعات العمل المسجلة في أيام خارج أيام العمل في شبكة إدخال الوقت.
- يمكن تحرير إدخالات المصروفات الموافق عليها على الشبكة.

**إدارة المشروع**

تم إصلاح المشكلات التالية:

- منطق التحقق من الصحة مفقود للتأكد من أن ساعات مجهود تعيين الموارد لا يمكن أن تكون سالبة.
- يقوم الإجراء المخصص، **AssignResourcesForTask** بتحديث جميع الحقول بدلاً من الحقول المتغيرة فقط.
- عند نسخ مشروع في بيئة بها مكونات إضافية أو عمليات سير عمل مسجلة في الحدث **CreateProject**، لا يتم تحديث السمة **msdyn_bulkgenerationstatus** عند فشل **CopyWBSToProject**.
- عند توسيع تقويم المشروع، لا يتم فرز أيام العمل بالترتيب التصاعدي مما يتسبب في فشل بعض تحديثات مهام المشروع.
- يؤدي تغيير مدير المشروع في مشروع موجود إلى تشغيل المنطق الافتراضية للوحدة المؤسسية.

**‏المبيعات**

تم إصلاح المشكلات التالية:

- تفشل علامة التبويب **أداء العقد** في صفحة **العقد‏‎** بشكل صامت أثناء التهيئة عند عدم وجود شروط تعاقد.
