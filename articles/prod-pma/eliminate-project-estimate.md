---
title: إزالة تقدير مشروع
description: يقدم هذا الموضوع معلومات حول إزالة تقدير المشروع بعد اكتماله.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 8bda8a7357e883b948449b2a19bea476996dde3c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070697"
---
# <a name="eliminate-a-project-estimate"></a>إزالة تقدير مشروع

[!include [banner](../includes/banner.md)]

توفر تقديرات المشروع طريقة عرض الشؤون المالية للعمل المقدر والمجدول لمشروع. للعمل مع التقديرات الخاصة بمشروع، يجب إرفاق المشروع بمشروع تقديري. يستند المشروع التقديري دائمًا إلى مشروع موجود، ومع ذلك بإمكان مشاريع متعددة أن تشير إلى مشروع تقديري واحد. يمكن إرفاق مشروعات الأسعار الثابتة والاستثمارية فقط بالمشروعات التقديرية، ويجب أن تنتمي هذه المشاريع إلى مجموعة المشاريع نفسها التي ينتمي إليها المشروع التقديري.

لإزالة مشروع تقديري، يجب أن يكون مكتملاً. توضح الخطوات التالية كيفية إزالة تقدير.

1. انتقل إلى **إدارة المشاريع والمحاسبة** > **جميع المشاريع** وافتح المشروع. 
2. على علامة التبويب **إدارة** ، حدد **التقديرات** ، وفي الصفحة **تقدير** ، حدد **إزالة**.
3. في الصفحة **إزالة التقدير** على علامة التبويب **عام** ، قم بتعيين الخيارات التالية:

   - **كود الفترة** : حدد كود الفترة لاختيار المشروعات التقديرية المناسبة. 
   - **تاريخ التقدير** : حدد تاريخ التقدير المناسب للإزالة.
   - **إزالة مع تحذيرات العمل قيد التنفيذ** : قم بتمكين هذا الخيار لتقديم إعلام عندما ستتم إزالة تقدير يرتبط بعمل قيد التنفيذ (WIP). عند عدم تمكين هذا الخيار، لا يمكن متابعة الإزالة في حال وجود حركات غير تقديرية. 
   > [!NOTE]
   > لا يتوفر هذا الخيار الا عندما يتم تطبيق الإزالة على مشروع تقديري. ولا يكون متوفرًا إذا كنت تستخدم عمليات الترحيل الدورية. يعمل هذا الإعداد مع الإعدادات الموجودة على علامة التبويب **تقدير** في صفحة **معلمات المشروع** في مجموعة حقول **السماح بالإزالة عند وجود حركات غير مقدرة**.
   - **تعيين المرحلة إلى منتهية** : يمكنك تمكين هذا الخيار لتعيين مرحلة المشروع التقديري إلى **منتهية** بعد تشغيل الإزالة.
   - **طباعة قائمة التقديرات** : حدد المعلومات التي سيتم تضمينها عند طباعة قائمة التقديرات‏‎.
   - **إظهار سجل المعلومات** : يمكنك تمكين هذا الخيار لعرض سجل المعلومات.
   - **تاريخ الترحيل** : اختر تاريخ ترحيل دفتر الأستاذ للتقدير.

4.  حدد **موافق**.
5. بعد اكتمال عملية الإزالة، يظهر المشروع التقدير المُزال مع قيمة سالبة. 

إذا لم تكن تهدف إلى إزالة تقدير، فيمكنك تحديد التقدير المُزال وتحديد **عكس عملية الإزالة**.   