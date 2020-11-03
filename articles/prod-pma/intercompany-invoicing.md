---
title: الفوترة بين الشركات الشقيقة
description: توفر هذه المقالة معلومات وأمثله حول الفوترة بين الشركات الشقيقة للمشاريع.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerInterCompany
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 94153
ms.assetid: 33e98da7-01c1-4369-923d-aa1c8326cb80
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 4604708dbd7c835c8df1cf48f67e645952f49774
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070670"
---
# <a name="intercompany-invoicing"></a>الفوترة بين الشركات الشقيقة

[!include [banner](../includes/banner.md)]

توفر هذه المقالة معلومات وأمثله حول الفوترة بين الشركات الشقيقة للمشاريع.

قد يكون لدي مؤسستك أقسام وشركات متعددة وكيانات قانونيه أخرى تقوم بنقل المنتجات والخدمات إلى بعضها البعض للمشاريع. ويطلق علي الكيان القانوني الذي يوفر الخدمة أو المنتج *الكيان القانوني المقرض* ، ويطلق علي الكيان القانوني الذي يتلقى الخدمة أو المنتج *الكيان القانوني المقترض*. 

يوضح الرسم التوضيحي التالي سيناريو نموذجي حيث يتشارك كيانان قانونيان ، SI FR (الكيان القانوني المقترض) و SI USA (الكيان القانوني المُقرض) في الموارد لتسليم مشروع للعميل أ. بالنسبة لهذا السيناريو ، تم التعاقد مع SI FR لتسليم العمل للعميل أ. 

[![مثال على الفوترة بين الشركات الشقيقة](./media/interco.invoicing-01.jpg)](./media/interco.invoicing-01.jpg) 

الهدف هو جعل التحكم في التكلفة ، والاعتراف بالإيرادات ، والضرائب ، وسعر التحويل لمعاملات المشروع بين الشركات الشقيقة أكثر مرونة وقوة. بالإضافة إلى ذلك ، يتم توفير الإمكانات التالية:

-   قم بإنشاء فواتير العملاء مقابل مشروع في كيان قانوني مقترض باستخدام الجداول الزمنية بين الشركات الشقيقة والمصروفات وفواتير المورد في كيان قانوني مُقرض.
-   حسابات ضريبة الدعم والتكاليف غير المباشرة.
-   تاجيل التعرف علي الإيرادات في الكيان القانوني الإقراض والوقت الذي ينبغي ان تتعرف فيه الكيان القانوني البورووينج علي التكلفة.
-   استحقاق إيرادات الأعمال قيد التنفيذ (WIP) في الكيان القانوني المُقرض.
-   قم بتعيين أسعار التحويل التي يمكن ان تستند إلى نماذج تسعير متعددة. وإليك بعض الأمثلة:
    -   **الكمية** - المبلغ الذي تقوم بإدخاله في حقل **التسعير** هو التكلفة الفعلية لكل كميه أو وحده.
    -   **مبلغ الرسوم** – السعر/التكلفة لكل حركه بالاضافه إلى مبلغ المصاريف الذي تقوم بإدخاله في حقل **التسعير**.
    -   **النسبة المئوية للمصايف** – يكون سعر التحويل هو السعر/التكلفة لكل حركه مضروبه في النسبة المئوية للمصاريف التي تقوم بإدخالها في حقل **التسعير**.
    -   **النسبة المئوية لسعر المبيعات** – النسبة المئوية لسعر المبيعات التي يتم تحويلها إلى الكيان القانوني الإقراض.
    -   **المبلغ اقل من سعر المبيعات** – المبلغ الذي يحتفظ به الكيان القانوني المقترض من أسعار المبيعات قبل التحويل إلى الكيان القانوني المُقرض.
    -   **نسبة المساهمة** - الرقم الذي تقوم بإدخاله في حقل **التسعير** هو هامش المساهمة، والذي يتم التعبير عنه كنسبه مئوية من سعر المبيعات.

## <a name="example-1-set-up-parameters-for-intercompany-invoicing"></a>المثال رقم 1: اعداد المحددات للفوترة بين الشركات الشقيقة
في هذا المثال ، تعتبر USSI كيانًا قانونيًا للإقراض ، وتبلغ مواردها الوقت مقابل الكيان القانوني المقترض ، FRSI ، الذي يمتلك العقد مع العميل النهائي. يمكن تضمين الساعات والمصروفات التي يبلغ عنها موظفو USSI في فاتورة المشروع التي تصدرها FRSI. بالإضافة إلى ذلك ، هناك مصدر ثالث للمعاملات التي يمكن أن تنشأ من الكيان القانوني للإقراض (USSI في هذا المثال) عندما يقدم خدمات الموردين المشتركة للشركات التابعة (مثل FRSI) ثم ينقل تلك التكاليف إلى المشاريع داخل تلك الشركات التابعة. يتم إكمال جميع مستندات الفاتورة المطابقة وحسابات الضرائب بواسطة Finance. 

في هذا المثال ، يجب أن تكون FRSI عميلاً في الكيان القانوني USSI ، ويجب أن تكون USSI مورِّدًا في الكيان القانوني FRSI. يمكنك بعد ذلك إعداد علاقة بين الشركات الشقيقة بين الكيانين القانونيين. يوضح الإجراء التالي كيفية إعداد المعلمات بحيث يمكن للكيانين القانونيين المشاركة في الفواتير بين الشركات الشقيقة.

1. قم بإعداد FRSI كعميل في الكيان القانوني USSI ، وقم بإعداد USSI كبائع في الكيان القانوني FRSI. هناك ثلاث نقاط دخول للخطوات المطلوبة لهذه المهمة.

   | الخطوة |                                                       نقطة الإدخال                                                        |                                                                                                                                                                                               ‏‏الوصف                                                                                                                                                                                               |
   |------|--------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
   |  ش   | في USSI، انقر فوق <strong>الحسابات المدينة</strong>&gt;<strong>العملاء</strong>&gt;<strong>جميع العملاء</strong>. |                                                                                                                                                                  قم بإنشاء سجل عميل جديد لـ FRSI ، وحدد مجموعة العملاء.                                                                                                                                                                  |
   |  B   |    في FRSI، انقر فوق <strong>الحسابات الدائنة</strong>&gt;<strong>الموردين</strong>&gt;<strong>كافة الموردين</strong>.     |                                                                                                                                                                    قم بإنشاء سجل بائع جديد لـ USSI ، وحدد مجموعة البائعين.                                                                                                                                                                    |
   |  C   |                                  في FRSI ، افتح سجل البائع الذي أنشأته للتو.                                  | في جزء الإجراءات، ضمن علامة التبويب <strong>عام</strong>، في مجموعة <strong>الإعداد</strong>، انقر فوق <strong>بين الشركات الشقيقة</strong>. في صفحة <strong>بين الشركات الشقيقة</strong>، في علامة التبويب <strong>علاقة التداول</strong>، قم بتعيين شريط التمرير <strong>النشط</strong> إلى <strong>نعم</strong>. في حقل <strong>شركة العميل</strong>، حدد سجل العميل الذي قمت بإنشائه في الخطوة أ. |


2. انقر فوق **إدارة المشاريع والمحاسبة** &gt; **الإعداد** &gt; **معلمات محاسبة إدارة المشاريع** ، ثم انقر فوق علامة التبويب **بين الشركات الشقيقة**. تعتمد طريقة إعداد المعلمات على ما إذا كنت أنت الكيان القانوني المستعير أو الكيان القانوني المُقرض.
   -   إذا كنت الكيان القانوني المستعير ، فحدد فئة التدبير التي يجب استخدامها لمطابقة فواتير المورّد ، والتي يتم إنشاؤها تلقائيًا.
   -   إذا كنت الكيان القانوني المُقرض ، فلكل كيان مقترض ، حدد فئة مشروع افتراضية لكل نوع حركة. تُستخدم فئات المشروع لتكوين الضرائب عندما تكون الفئة التي تم إصدار فاتورة بها في المعاملات بين الشركات الشقيقة موجودة فقط في الكيان القانوني المقترض. يمكنك اختيار استحقاق إيراد الحركات بين الشركات الشقيقة. يتم إجراء هذا الاستحقاق عند ترحيل الحركات ، ثم يتم عكسه عند ترحيل الفاتورة بين الشركات الشقيقة.

3. انقر فوق **إدارة المشاريع والمحاسبة** &gt; **الإعداد** &gt; **الأسعار** &gt; **سعر التحويل**.
4. حدد العملة ونوع الحركة ونموذج السعر الذي يمكن تحويله. العملة المستخدمة في الفاتورة هي العملة التي تم تكوينها في سجل العميل للكيان القانوني المقترض في الكيان القانوني المُقرض. تُستخدم العملة لمطابقة الإدخالات في جدول سعر التحويل.
5. انقر فوق **دفتر الأستاذ العام** &gt; **إعداد الترحيل** &gt; **المحاسبة بين الشركات الشقيقة** ، وقم بإنشاء علاقة بين USSI وFRSI.

## <a name="example-2-create-and-post-an-intercompany-timesheet"></a>مثال 2: إنشاء ونشر جدول زمني بين الشركات الشقيقة
يجب أن تقوم USSI ، الكيان القانوني المُقرض ، بإنشاء ونشر الجدول الزمني لمشروع من FRSI ، الكيان القانوني المُقترض. هناك نقطتا دخول للخطوات المطلوبة لهذه المهمة.

| الخطوة | نقطة الإدخال                                                                       | ‏‏الوصف                                                                                                                                                                                       |
|------|-----------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ش    | **إدارة المشاريع والمحاسبة** &gt; **الجداول الزمنية** &gt; **جميع الجداول الزمنية** | أنشئ جدول زمني جديد. في سطر الجدول الزمني، في حقل **الكيان القانوني** ، حدد **FRSI**. في حقل **معرف المشروع** ، حدد المشروع في FRSI. أدخل الساعات لكل يوم من أيام الأسبوع. |
| B    | صفحة **الجدول الزمني**                                                                | بعد تشغيل سير العمل ، انشر الجدول الزمني ، وقم بتدوين رقم الإيصال.                                                                                                               |

## <a name="example-3-create-and-post-an-intercompany-vendor-invoice"></a>مثال 3: إنشاء فاتورة مورّد بين الشركات الشقيقة وترحيلها
يجب أن تنشئ USSI ، الكيان القانوني المُقرض ، فاتورة المورد بين الشركات الشقيقة لمشروع من FRSI ، الكيان القانوني المُقترض. تمثل فاتورة البائع هذه العمالة والمصروفات الخارجية التي تم إجراؤها بواسطة البائعين والتي تم دفعها بواسطة USSI. هناك نقطتا دخول للخطوات المطلوبة لهذه المهمة.

| الخطوة | نقطة الإدخال                                                                                      | ‏‏الوصف                                                                                                                                                                                                                                                                          |
|------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ش    | **الحسابات الدائنة** &gt; **الفواتير** &gt; **فتح فواتير الموردين** &gt; **فاتورة المورد الجديدة** | قم بإنشاء فاتورة بائع جديدة ، وأدخل الخدمات التي تم الحصول عليها نيابة عن مشروع FRSI.                                                                                                                                                                                  |
| B    | صفحة **فاتورة المورد**                                                                      | أدخل سطورًا تمثل خدمات الاستعانة بمصادر خارجية نيابة عن FRSI. في علامة التبويب السريعة **تفاصيل السطر** ، في علامة التبويب **المشروع** لسطر الفاتورة، في حقل **شركة المشروع** ، أدخل **FRSI**. أدخل المشروع والمعلومات المقابلة. ثم قم بترحيل فاتورة المورد. |

## <a name="example-4-create-and-post-the-intercompany-invoice"></a>مثال 4: إنشاء الفاتورة بين الشركات الشقيقة وترحيلها
يجب أن تقوم USSI ، الكيان القانوني المُقرض ، بإنشاء فاتورة بين الشركات الشقيقة وترحيلها. هناك نقطتا دخول للخطوات المطلوبة لهذه المهمة.

| الخطوة | نقطة الإدخال                                                                                             | ‏‏الوصف                                                                                                                                      |
|------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| ش    | **إدارة المشاريع والمحاسبة** &gt; **فواتير المشاريع** &gt; **فاتورة العميل بين الشركات الشقيقة**  | انقر فوق **جديد** لفتح صفحة **إنشاء الفاتورة بين الشركات الشقيقة**.                                                                                  |
| B    | **إدارة المشاريع والمحاسبة** &gt; **فواتير المشاريع** &gt; **فواتير العملاء بين الشركات الشقيقة** | في صفحة **إنشاء فاتورة بين الشركات الشقيقة** ، أدخل الكيان القانوني، وحدد الحركة التي ينبغي تضمينها، ثم انقر فوق **بحث**. |
| C    | **إدارة المشاريع والمحاسبة** &gt; **فواتير المشاريع** &gt; **فواتير العملاء بين الشركات الشقيقة** | حدد الحركات المراد فوترتها، أو انقر فوق **تحديد الكل** لفوترة كافة الحركات الموجودة في القائمة، ثم انقر فوق **موافق**.                  |
| D    | صفحة **الفاتورة بين الشركات الشقيقة**                                                                       | يتم عرض مقترح فاتورة العميل بين الشركات الشقيقة.                                                                                             |
| E    | صفحة **الفاتورة بين الشركات الشقيقة**                                                                       | انقر فوق **نشر**.                                                                                                                                  |

## <a name="example-5-post-the-vendor-invoice-and-invoice-the-customer"></a>مثال 5: ترحيل فاتورة المورد وفوترة العميل
عندما يقوم الكيان القانوني المُقرض ، USSI ، بترحيل فاتورة العميل بين الشركات الشقيقة ، يتم إنشاء فاتورة بائع معلقة مطابقة في الكيان القانوني المُقترض ، FRSI. بعد ترحيل فاتورة البائع هذه ، ترسل FRSI أيضًا فواتير لعميل المشروع بالساعات التي أدخلتها USSI. هناك ثلاث نقاط دخول للخطوات المطلوبة لهذه المهمة.

| الخطوة | نقطة الإدخال                                                                                        | ‏‏الوصف                                                                                                             |
|------|----------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| ش    | **الحسابات الدائنة** &gt; **الفواتير** &gt; **فواتير الموردين المعلقة**                            | راجع الفاتورة للتحقق من تضمين قيم الجدول الزمني ، ثم قم بترحيل فاتورة المورد.                  |
| B    | **إدارة المشاريع والمحاسبة** &gt; **فواتير المشاريع** &gt; **مقترحات فواتير المشاريع** | قم بإنشاء فاتورة مشروع جديدة للمشروع ، وتحقق من ظهور حركات الساعة التي تم ترحيلها.            |
| C    | صفحة **فاتورة المشروع**                                                                       | حدد فاتورة المشروع، ثم انقر فوق **عرض التفاصيل** لمراجعه مبلغ التكلفة والمبيعات. ثم قم بترحيل الفاتورة. |


لمزيد من المعلومات، راجع [تكوين فوترة المشروع بين الشركات الشقيقة](tasks/configure-intercompany-project-invoicing.md).

