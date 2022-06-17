---
title: الجديد أو المتغير في الإصدار 3.x من Project Service Automation، الموجة 1 لعام 2020
description: يقدم هذا المقال معلومات حول الجديد والمتغير في الموجة 1 لعام 2020 للإصدار 3 من Project Service Automation.
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
ms.reviewer: johnmichalak
ms.openlocfilehash: c762f2e7931046d32464cfa8486ef8405aa7d836
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928600"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a>الجديد أو المتغير في الإصدار 3 من Project Service Automation، الموجة 1 لعام 2020

[!include [banner](../includes/psa-now-project-operations.md)]

يسلط هذا المقال الضوء على اعتبارات الترقية الأساسية عند الانتقال إلى الإصدار الأخير من الموجة 1 لعام 2020 للإصدار 3.x من Project Service Automation (PSA).

## <a name="time-entry"></a>إدخال الوقت
تم توسيع تجربة إدخال الوقت لتوفير إمكانيات لتوسيع إدخال الوقت في المزيد من سيناريوهات العملاء. وهذا يشمل إمكانية إضافة أنواع إدخالات، التي تعزز الآن سلوكيات معنية بالاستناد إلى اسم مخطط الحقل **إعدادات إدخال الوقت** الذي يظهر على أنه **مصدر الوقت**. تمت إضافة حل جديد مسمى الوقت والمصروفات والحالات والموافقات (TESA) لدعم هذه الوظيفة.

### <a name="upgrade-consideration"></a>اعتبارات الترقية
لدعم هذه الوظيفة، تم تحديث الأدوار الموجودة في PSA لتشمل امتيازات جديدة. تمنح هذه الامتيازات حق الوصول للقراءة للكيان الجديد، **إعدادات إدخال الوقت**.

ينبغي منح المستخدمين الذين يحتاجون إلى تسجيل الوقت دور المستخدم **مستخدم إدخال الوقت** بالإضافة إلى الأدوار الموجودة. يتضمن هذا الدور الوظائف الجديدة ويضمن استمرارية عمل إدخال الوقت.

علاوةً على ذلك، إذا كانت لديك وحدات تطبيقات مخصصة تتضمن جميع نماذج كيان إدخالات الوقت، فستتم مطالبتك بإزالة **نموذج الإنشاء السريع لإدخال الوقت TESA‬‬** من الوحدة.

### <a name="currently-extended-time-entry-changes"></a>تغييرات إدخال الوقت الممدد حاليًا
لتقليل التأثير على مستخدمي إدخال الوقت الحاليين، يعتبر تغيير الدور هذا الشرط الأساسي الوحيد المطلوب لمتابعة استخدام إدخال الوقت. إذا كنت قد قمت بإنشاء طرق عرض مخصصة أو تجارب إدخال وقت منفصلة، فيجب تعيين حقول **إعداد إدخال الوقت** إلى قيمه PSA الصحيحة.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
