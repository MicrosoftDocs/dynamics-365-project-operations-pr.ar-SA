---
title: معلمات تكامل Project Service Automation
description: توضح هذه الموضوع كيفيه تكوين كيفيه إدخال البيانات الافتراضية عند تكامل Microsoft Dynamics 365 for Project Service Automationمع Microsoft Dynamics 365 Finance.
author: ruhercul
manager: AnnBe
ms.date: 03/03/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 1a0cee090e0ecb306aa3bda62c79a57dfade93c0
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070784"
---
# <a name="project-service-automation-integration-parameters"></a>معلمات تكامل Project Service Automation

[!include[banner](../includes/banner.md)]

في الصفحة **معلمات تكامل Project Service Automation** ، يمكنك تكوين كيفيه إدخال البيانات عند دمج Dynamics 365 Project Service Automation مع Dynamics 365 Finance. لكي تتم مزامنة المشاريع بنجاح من Project Service Automation إلى Finance ، يجب عليك إعداد الحقول التالية.

لفتح الصفحة **معلمات تكامل Project Service Automation** ، انتقل إلى **إدارة المشاريع والمحاسبة**\>**إعداد**\>**معلمات تكامل Dynamics 365 for Project Service Automation**. 

> [!NOTE]
> - يتوفر تكامل مهام المشروع ، وفئات حركات المصروفات ، وتقديرات الساعة ، وتقديرات المصروفات ، وتأمين الوظائف في الإصدار 8.0.
> - القيم الفعلية المتكاملة متوفرة في الإصدار 8.0.1 أو أحدث.


| علامة التبويب                    | الحقل                | ‏‏الوصف |
|------------------------|----------------------|-------------|
| شائع                | نوع المشروع الافتراضي | حدد نوع المشروع الافتراضي. عندما تتم مزامنة المشاريع من Project Service Automation ، يتم استخدام هذه القيمة إذا لم تقدم قيمة افتراضية في قالب التكامل. أثناء المزامنة، يتم تعيين حقل **نوع المشروع** للمشروعات الجديدة على هذه القيمة. ومع ذلك ، قد يتم تحديث القيمة عند مزامنة بنود عقد المشروع من Project Service Automation. |
|                        | فئة الوقت        | حدد فئة الوقت الافتراضية. يتم استخدام هذه القيمة عند مزامنة تقديرات الساعات من Project Service Automation. عندما تتم مزامنة تقديرات الساعات والقيم الفعلية للساعات من Project Service Automation ، فإن حقل **الفئة** تم تعيين توقعات ساعات المشروع الجديدة في Finance على هذه القيمة. |
|                        | فئة الرسوم         | حدد فئة الرسوم الافتراضية. يتم استخدام هذه القيمة عند مزامنة القيم الفعلية للرسوم من Project Service Automation. عندما تتم مزامنة القيم الفعلية للرسوم من Project Service Automation، فإن حقل **Category** لحركات الرسوم الجديدة في Finance على هذه القيمة. |
| افتراضيات مجموعة المشروعات | نوع المشروع         | انقر فوق **جديد** لإضافة صف حيث يمكنك تحديد نوع المشروع المراد تعيين مجموعه المشروع الافتراضية له. يمكن تحديد نوع مشروع معين مرة واحدة فقط في التكوين. |
|                        | مجموعة المشاريع        | حدد مجموعه المشاريع الافتراضية لنوع المشروع المحدد. عند مزامنة المشاريع الجديدة من Project Service Automation، يتم تعيين حقل **مجموعة المشاريع** إلى القيمة الافتراضية لنوع المشروع في حالة عدم توفر قيمه افتراضيه في قالب التكامل. |
| افتراضيات نوع الفوترة  | نوع الفوترة         | انقر فوق **جديد** لإضافة صف حيث يمكنك تحديد نوع الفوترة لتعيين خاصية الخط الافتراضية له. يمكن تحديد نوع فوترة معين مرة واحدة فقط في التكوين. |
|                        | خاصية السطر        | حدد خاصية السطر الافتراضية لنوع الفوترة المحدد. عندما تتم مزامنة تقديرات الساعات الجديدة أو تقديرات المصروفات الجديدة أو القيم الفعلية الجديدة من Project Service Automation، فإنه يتم تعيين حقل **خاصية السطر** إلى القيمة الافتراضية لنوع الفوترة. |
| تأمين الوظائف  | غير قابل للتطبيق       | حدد الوظيفة المطلوب تعطيلها في Finance للمشاريع والعقود التي نشأت من Project Service Automation. على سبيل المثال ، يمكنك إيقاف تشغيل القدرة على تحرير العقود والمشاريع ، وإنشاء هياكل تقسيم العمل ، وإدخال الجداول الزمنية في Finance. سيستمر تمكين الحقول المتعلقة بالمحاسبة ، حتى إذا لم يتم توفيرها بواسطة إعداد المعلمة. بشكل افتراضي ، يتم تمكين جميع الوظائف. |
