---
title: الجديد أو المتغير في الإصدار 3.x من Project Service Automation، الموجة 1 لعام 2020
description: يقدم هذا الموضوع معلومات حول الجديد والمتغير في الإصدار رقم 3 من Project Service Automation، الموجة 1 لعام 2020.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/15/2020
ms.topic: article
author: stsporen
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 5110679038ae7ed1e21a3e7dc80a4657e0752b49
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150922"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a>الجديد أو المتغير في الإصدار 3 من Project Service Automation، الموجة 1 لعام 2020

[!include [banner](../includes/psa-now-project-operations.md)]

هذا الموضوع يلقي الضوء على اعتبارات الترقية عند الانتقال إلى الإصدار الأخير 3.x من Project Service Automation (PSA)، الموجة 1 لعام 2020.

## <a name="time-entry"></a>إدخال الوقت
تم توسيع تجربة إدخال الوقت لتوفير إمكانيات لتوسيع إدخال الوقت في المزيد من سيناريوهات العملاء. وهذا يشمل إمكانية إضافة أنواع إدخالات، التي تعزز الآن سلوكيات معنية بالاستناد إلى اسم مخطط الحقل **إعدادات إدخال الوقت** الذي يظهر على أنه **مصدر الوقت**. تمت إضافة حل جديد مسمى الوقت والمصروفات والحالات والموافقات (TESA) لدعم هذه الوظيفة.

### <a name="upgrade-consideration"></a>اعتبارات الترقية
لدعم هذه الوظيفة، تم تحديث الأدوار الموجودة في PSA لتشمل امتيازات جديدة. تمنح هذه الامتيازات حق الوصول للقراءة للكيان الجديد، **إعدادات إدخال الوقت**.

ينبغي منح المستخدمين الذين يحتاجون إلى تسجيل الوقت دور المستخدم **مستخدم إدخال الوقت** بالإضافة إلى الأدوار الموجودة. يتضمن هذا الدور الوظائف الجديدة ويضمن استمرارية عمل إدخال الوقت.

علاوةً على ذلك، إذا كانت لديك وحدات تطبيقات مخصصة تتضمن جميع نماذج كيان إدخالات الوقت، فستتم مطالبتك بإزالة **نموذج الإنشاء السريع لإدخال الوقت TESA‬‬** من الوحدة.

### <a name="currently-extended-time-entry-changes"></a>تغييرات إدخال الوقت الممدد حاليًا
لتقليل التأثير على مستخدمي إدخال الوقت الحاليين، يعتبر تغيير الدور هذا الشرط الأساسي الوحيد المطلوب لمتابعة استخدام إدخال الوقت. إذا كنت قد قمت بإنشاء طرق عرض مخصصة أو تجارب إدخال وقت منفصلة، فيجب تعيين حقول **إعداد إدخال الوقت** إلى قيمه PSA الصحيحة.


[!INCLUDE[footer-include](../includes/footer-banner.md)]