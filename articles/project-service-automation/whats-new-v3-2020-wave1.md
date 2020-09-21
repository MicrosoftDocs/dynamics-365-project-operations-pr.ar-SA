---
title: الجديد أو المتغير في الإصدار 3.x من Project Service Automation، الموجة 1 لعام 2020
description: يقدم هذا الموضوع معلومات حول الجديد والمتغير في الإصدار رقم 3 من Project Service Automation، الموجة 1 لعام 2020.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 01/24/2020
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x wave 1 2020
author: stsporen
ms.assetid: 48b408c1-11e7-4005-abac-8fd7c0b064b1
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 478080c0570b71188c9f1e12b18b5aadc13903e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748650"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a>الجديد أو المتغير في الإصدار 3 من Project Service Automation، الموجة 1 لعام 2020
هذا الموضوع يلقي الضوء على اعتبارات الترقية عند الانتقال إلى الإصدار الأخير 3.x من Project Service Automation (PSA)، الموجة 1 لعام 2020.

## <a name="time-entry"></a>إدخال الوقت
تم توسيع تجربة إدخال الوقت لتوفير إمكانيات لتوسيع إدخال الوقت في المزيد من سيناريوهات العملاء. وهذا يشمل إمكانية إضافة أنواع إدخالات، التي تعزز الآن سلوكيات معنية بالاستناد إلى اسم مخطط الحقل **إعدادات إدخال الوقت** الذي يظهر على أنه **مصدر الوقت**.

### <a name="upgrade-consideration"></a>اعتبارات الترقية
لدعم هذه الوظيفة، تم تحديث الأدوار الموجودة في PSA لتشمل امتيازات جديدة. تمنح هذه الامتيازات حق الوصول للقراءة للكيان الجديد، **إعدادات إدخال الوقت**.

ينبغي منح المستخدمين الذين يحتاجون إلى تسجيل الوقت دور المستخدم **مستخدم إدخال الوقت** بالإضافة إلى الأدوار الموجودة. يتضمن هذا الدور الوظائف الجديدة ويضمن استمرارية عمل إدخال الوقت.

### <a name="currently-extended-time-entry-changes"></a>تغييرات إدخال الوقت الممدد حاليًا
لتقليل التأثير على مستخدمي إدخال الوقت الحاليين، يعتبر تغيير الدور هذا الشرط الأساسي الوحيد المطلوب لمتابعة استخدام إدخال الوقت. إذا كنت قد قمت بإنشاء طرق عرض مخصصة أو تجارب إدخال وقت منفصلة، فيجب تعيين حقول **إعداد إدخال الوقت** إلى قيمه PSA الصحيحة.
