---
title: نقل موازنات المشروع في نهاية السنة المالية
description: توفر هذه المقالة معلومات حول كيفية نقل مبالغ الموازنة المتبقية إلى سنوات مستقبليه وإنشاء تفاصيل سجل الموازنة.
author: Yowelle
manager: AnnBe
ms.date: 03/23/2020
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
ms.openlocfilehash: 26e013ab99e9a0aeafe25916715ce0ee024df3f7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070777"
---
# <a name="transfer-project-budgets-at-fiscal-year-end"></a>نقل موازنات المشروع في نهاية السنة المالية

[!include [banner](../includes/banner.md)]

عند العمل على مشروع متعدد السنوات، قد يكون لديك موازنة متبقية في نهاية السنة المالية. يمكنك نقل مبالغ الموازنة المتبقية إلى سنة مستقبلية، وإنشاء تفاصيل سجل الموازنة للمبالغ الموجودة في الحسابات المقترنة في دفتر الأستاذ العام. قبل تحويل المبالغ المتبقية، يمكنك مراجعة وتحليل مبالغ الموازنة المتبقية.

## <a name="review-and-analyze-remaining-budget-amounts"></a>مراجعة وتحليل مبالغ الموازنة المتبقية

أكمل الخطوات التالية لمراجعة مبالغ موازنة نهاية السنه للمشاريع، ولكن دون تحويل المبالغ.

1. انتقل إلى **إدارة المشاريع والمحاسبة‬** > **دوري** > **الموازنات** > **تحويل الموازنات**. 
2. في الصفحة **معالجة تحويل موازنة المشروع** ، على علامة التبويب **خيارات نهاية السنة** ، تأكد من عدم تمكين الخيار **تحويل مبالغ موازنة المشروع المتبقية**.
3. من علامة التبويب **المعلمات** ، في حقل **سنه موازنة المشروع** ، حدد السنة المالية التي ترغب في عرض مبلغ الموازنة المتبقية لها. 
4. في حقل **السنة المالية الافتتاحية** ، حدد السنة المالية التي ترغب في عرض مبلغ الموازنة المتبقية لها. 
5. في الحقل **من نموذج التنبؤ** ، حدد **الموازنة المتبقية**. 
6. لتضمين المشاريع التي تتوافق مع معاييرك المحددة والتي ليس لديها موازنة متبقية، حدد **إظهار القيمة الصفرية المتبقية**.  
7. في علامة التبويب **موازنات محددة** ، حدد **استرداد جميع الموازنات** لتحميل جميع الموازنات التي تتطابق مع معاييرك المحددة، ثم حدد **معالجة**. 
8. لتصميم استعلام قاعدة بيانات يقوم بتحميل مجموعة محددة من الموازنات في الجزء، حدد **استرداد موازنات محددة**.

لمزيد من المعلومات حول بند معين في الجزء، حدد البند، ثم حدد **عرض تفاصيل الموازنة** أو **عرض الحسابات**.

## <a name="carry-forward-remaining-budget-amounts"></a>تحويل مبالغ الموازنة المتبقية 

عند معالجة مبالغ الموازنة المتبقية، يمكنك إنشاء حركات في دفتر الأستاذ العام للمبالغ التي تقوم بتحويلها. لإنشاء حركات دفتر أستاذ عام، استكمل الخطوات في القسم [تحويل مبالغ الموازنة وإنشاء حركات دفتر الأستاذ العام](#carry-forward). 

> [!NOTE]
> يتم نقل مبالغ الموازنة التي يتم تحويلها إلى نموذج التنبؤ المحدد في صفحة **نماذج التنبؤ** كنموذج تنبؤ التحويل.  

## <a name="carry-forward-budget-amounts-and-create-general-ledger-transactions"></a><a name="carry-forward"></a>تحويل مبالغ الموازنة وإنشاء حركات دفتر الأستاذ العام

1.  حدد **إدارة المشاريع والمحاسبة‬** > **دوري** > **الموازنات** > **تحويل الموازنات**. 
2. في الصفحة **معالجة تحويل موازنة المشروع** ، حدد **نهاية السنة** ، ثم قم بتمكين الخيارين **تحويل مبالغ موازنة المشروع المتبقية‬‏‫** و **إنشاء إدخالات سجل الموازنة في دفتر الأستاذ العام**. 
3. في علامة تبويب **المعلمات** ، في مجموعة حقول **معلمات المشروع** ، حدد الخيارات التالية:

   - **سنة موازنة المشروع** : حدد بداية السنة المالية التي ترغب في عرض مبالغ الموازنة المتبقية لها. 
   - **الأرباح والخسائر** : أنشئ حركات الأرباح والخسائر في دفتر الأستاذ العام. 
   -  **الاعمال قيد التنفيذ** : أنشئ حركات الاعمال قيد التنفيذ في دفتر الأستاذ العام.
   -  **كشف الرواتب** : أنشئ حركات توزيع كشوف الرواتب في دفتر الأستاذ العام. 

5. في مجموعة حقول **دفتر الأستاذ العام** ، أدخل المعلومات التالية: 

   - في حقل **السنة المالية الافتتاحية** ، حدد السنة المالية التي تريد أن تنقل إليها مبالغ الموازنة المتبقية للمشاريع. القيمة الافتراضية هي عام واحد بعد القيمة في الحقل **سنة موازنة المشروع**.
   -  في الحقل **فترة التحويل** ، حدد الفترة التي تريد إنشاء تفاصيل سجل الموازنة لها في دفتر الأستاذ العام. هذه هي عادةً الفترة الأولى في السنة المالية الافتتاحية‬‏‫.

6. في مجموعة حقول **نسخ من/إلى** ، أدخل المعلومات التالية:

   - في الحقل **من نموذج التنبؤ** ، حدد نموذج التنبؤ بموازنة المشروع المقترن بمبالغ الموازنة المتبقية التي ترغب في نقلها إلى المشاريع. 
   - في الحقل **إلى نموذج موازنة دفتر الأستاذ** ، حدد نموذج موازنة دفتر الأستاذ المقترن بمبالغ الموازنة المتبقية التي ترغب في نقلها إلى دفتر الأستاذ العام. 
   -  حدد **نقل عملة المبيعات** لاستخدام عملة المبيعات الخاصة بالمشروع في حركات دفتر الأستاذ العام التي يتم إنشاؤها عند نقل مبالغ الموازنة للمشاريع. وعندما لا يكون الخيار محددًا، تستخدم الحركات عملة المحاسبة. 
   -  حدد **إظهار القيمة الصفرية المتبقية** لتضمين المشاريع التي ليس لديها مبالغ متبقية في الموازنة، ولكنها تستوفي المعايير الأخرى التي تحددها في المشاريع المعروضة في الجزء السفلي.

7. في علامة التبويب **موازنات محددة** ، حدد **استرداد جميع الموازنات** لتحميل جميع الموازنات التي تتطابق مع معاييرك المحددة. إذا كنت تفضل تصميم استعلام قاعدة بيانات يقوم بتحميل مجموعة محددة من موازنات المشروع إلى الجزء، فحدد **استرداد موازنات محددة**.
8. بالنسبة لكل مشروع تريد معالجته، حدد الخيار الموجود في بداية السطر للمشروع.

    > [!TIP]
    > لتحديد كافة المشروعات أو معظمها، حدد خانة الاختيار الموجودة في الزاوية العلوية اليسرى. لاستثناء معالجة أي مشروع، قم بإلغاء تحديد خانة الاختيار الخاصة بذلك المشروع.

9. لنقل مبالغ الموازنة المتبقية للمشاريع المحددة إلى السنة المالية المحددة وإنشاء تفاصيل سجل الموازنة في دفتر الأستاذ العام، حدد **معالجة**.

## <a name="carry-forward-budget-amounts-without-creating-general-ledger-transactions"></a>تحويل مبالغ الموازنة من دون إنشاء حركات دفتر الأستاذ العام

1. انتقل إلى **إدارة المشاريع والمحاسبة‬** > **دوري** > **الموازنات** > **تحويل الموازنات**.
2. في الصفحة **معالجة تحويل موازنة المشروع** ، في حقل **خيارات نهاية السنة** ، حدد **تحويل مبالغ موازنة المشروع المتبقية**.
3. من مجموعة **المعلمات** ، في حقل **سنه موازنة المشروع** ، حدد السنة المالية التي ترغب في عرض مبالغ الموازنة المتبقية لها.
4. في المجموعة **نسخ من/إلى** ، أدخل المعلومات التالية:

   - في الحقل **من نموذج التنبؤ** ، حدد نموذج التنبؤ بموازنة المشروع المقترن بمبالغ الموازنة المتبقية التي ترغب في نقلها إلى المشاريع. 
   - حدد **إظهار القيمة الصفرية المتبقية** لتضمين المشاريع التي ليس لديها موازنة متبقية، ولكنها تتوافق مع المعايير الأخرى التي حددتها.
   - في المجموعة **موازنات محددة** ، حدد **استرداد جميع الموازنات** لتحميل جميع الموازنات التي تتطابق مع معاييرك المحددة. لتصميم استعلام قاعدة بيانات يقوم بتحميل مجموعة محددة من موازنات المشروع في الجزء، حدد **استرداد موازنات محددة**.

5. بالنسبة لكل مشروع تريد معالجته، حدد الخيار الموجود في بداية السطر للمشروع. 
6. حدد **معالجة** لنقل مبالغ الموازنة المتبقية للمشاريع المحددة إلى السنة المالية المحددة.
