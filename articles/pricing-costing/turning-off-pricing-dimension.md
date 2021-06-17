---
title: إيقاف تشغيل بُعد تسعير
description: يقدم هذا الموضوع معلومات حول كيفية إيقاف تشغيل أبعاد التسعير.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 7b7c1d1b3363c0d158fcf6fda532822354b852a3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004515"
---
# <a name="turning-off-a-pricing-dimension"></a><span data-ttu-id="e95c2-103">إيقاف تشغيل بُعد تسعير</span><span class="sxs-lookup"><span data-stu-id="e95c2-103">Turning off a pricing dimension</span></span>

<span data-ttu-id="e95c2-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="e95c2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e95c2-105">قد تحتاج إلى مراجعه استراتيجية التسعير وتحديثها كل بضع سنوات.</span><span class="sxs-lookup"><span data-stu-id="e95c2-105">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="e95c2-106">قد تتطلب أي تحديثات تقوم بإجرائها أن تقوم بإيقاف تشغيل بُعد تسعير موجود وإنشاء واحد جديد.</span><span class="sxs-lookup"><span data-stu-id="e95c2-106">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="e95c2-107">على سبيل المثال، ربما قمت مسبقًا بالتسعير حسب **الدور**، ولكنك قررت الآن التسعير حسب **تجربة العمل**.</span><span class="sxs-lookup"><span data-stu-id="e95c2-107">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="e95c2-108">قد يتطلب هذا منك إيقاف تشغيل **الدور** كبُعد تسعير وإنشاء **تجربة عمل** كبعد تسعير جديد.</span><span class="sxs-lookup"><span data-stu-id="e95c2-108">This may require you to turn off **Role** as a pricing dimension and create **Work Experience** as a new pricing dimension.</span></span> 

<span data-ttu-id="e95c2-109">ويمكن إيقاف تشغيل بعد التسعير، سواء كان جاهزًا أو مخصصًا، عن طريق تعيين حقلي **قابل للتطبيق على التكلفة** و **قابل للتطبيق على المبيعات** الخاصين ببعد التسعير إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="e95c2-109">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="e95c2-110">ومع ذلك، عند القيام بذلك قد تظهر رسالة الخطأ، **لا يمكن تحديث بعد التسعير أو حذفه في حالة وجود سجلات أسعار مرتبطة.**</span><span class="sxs-lookup"><span data-stu-id="e95c2-110">However, when you do this, you might receive the error message, **Pricing dimension cannot be updated or deleted if there are associated price records.**</span></span>

![احتمال حدوث خطأ في عمليه الأعمال عند عدم القيام بإيقاف تشغيل بعد تسعير](media/Business-Process-Error.png)

<span data-ttu-id="e95c2-112">تشير رسالة الخطأ هذه إلى أن هناك سجلات أسعار تم إعدادها مسبقًا للبعد الذي تم إيقاف تشغيله.</span><span class="sxs-lookup"><span data-stu-id="e95c2-112">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="e95c2-113">يجب حذف كل سجلات **سعر الدور** و **رفع سعر الدور** التي تشير إلى بُعد قبل التمكن من تعيين إمكانية تطبيق البُعد إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="e95c2-113">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="e95c2-114">يتم تطبيق هذه القاعدة على كل من أبعاد التسعير الجاهزة وأبعاد التسعير المخصصة التي ربما قمت بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="e95c2-114">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="e95c2-115">ويرجع سبب هذا التحقق من الصحة إلى أن كل **سعر دور** يجب أن يحتوي على مجموعة فريدة من الأبعاد.</span><span class="sxs-lookup"><span data-stu-id="e95c2-115">The reason for this validation is because each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="e95c2-116">على سبيل المثال، في قائمة الأسعار المسماة **أسعار التكلفة بالولايات المتحدة لعام 2018**، يكون لديك صفوف **سعر الدور** التالية.</span><span class="sxs-lookup"><span data-stu-id="e95c2-116">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="e95c2-117">العنوان القياسي</span><span class="sxs-lookup"><span data-stu-id="e95c2-117">Standard Title</span></span>         | <span data-ttu-id="e95c2-118">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="e95c2-118">Org Unit</span></span>    |<span data-ttu-id="e95c2-119">الوحدة</span><span class="sxs-lookup"><span data-stu-id="e95c2-119">Unit</span></span>   |<span data-ttu-id="e95c2-120">السعر</span><span class="sxs-lookup"><span data-stu-id="e95c2-120">Price</span></span>  |<span data-ttu-id="e95c2-121">عملة</span><span class="sxs-lookup"><span data-stu-id="e95c2-121">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="e95c2-122">مهندس الأنظمة</span><span class="sxs-lookup"><span data-stu-id="e95c2-122">Systems Engineer</span></span>|<span data-ttu-id="e95c2-123">Contoso US</span><span class="sxs-lookup"><span data-stu-id="e95c2-123">Contoso US</span></span>|<span data-ttu-id="e95c2-124">ساعة</span><span class="sxs-lookup"><span data-stu-id="e95c2-124">Hour</span></span>| <span data-ttu-id="e95c2-125">100</span><span class="sxs-lookup"><span data-stu-id="e95c2-125">100</span></span>|<span data-ttu-id="e95c2-126">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="e95c2-126">USD</span></span>|
| <span data-ttu-id="e95c2-127">مهندس أنظمة أول</span><span class="sxs-lookup"><span data-stu-id="e95c2-127">Senior Systems Engineer</span></span>|<span data-ttu-id="e95c2-128">Contoso US</span><span class="sxs-lookup"><span data-stu-id="e95c2-128">Contoso US</span></span>|<span data-ttu-id="e95c2-129">ساعة</span><span class="sxs-lookup"><span data-stu-id="e95c2-129">Hour</span></span>| <span data-ttu-id="e95c2-130">150</span><span class="sxs-lookup"><span data-stu-id="e95c2-130">150</span></span>| <span data-ttu-id="e95c2-131">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="e95c2-131">USD</span></span>|


<span data-ttu-id="e95c2-132">عندما تقوم بإيقاف تشغيل **العنوان القياسي** باعتباره بُعد التسعير، ويقوم محرك التسعير بالبحث عن سعر، فسيبحث فقط عن قيمة **الوحدة التنظيمية** من سياق الإدخال.</span><span class="sxs-lookup"><span data-stu-id="e95c2-132">When you turn off **Standard Title** as the pricing dimension, and the pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="e95c2-133">إذا كانت **الوحدة التنظيمية** الخاصة بسياق الإدخال هي شركة "Contoso الولايات المتحدة الأمريكية"، فستكون النتيجة غير محددة لأن كلا الصفين سيتطابقان.</span><span class="sxs-lookup"><span data-stu-id="e95c2-133">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="e95c2-134">لتجنب هذا السيناريو، عند إنشاء سجلات **سعر الدور** يقوم النظام بالتحقق من أن مجموعة الأبعاد فريدة من نوعها.</span><span class="sxs-lookup"><span data-stu-id="e95c2-134">To avoid this scenario, when you create **Role Price** records, the system validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="e95c2-135">إذا تم إيقاف تشغيل البُعد بعد إنشاء سجلات **سعر الدور**، فيمكن مخالفة هذا القيد.</span><span class="sxs-lookup"><span data-stu-id="e95c2-135">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="e95c2-136">وبالتالي، من المطلوب أن تقوم قبل إيقاف تشغيل أحد الأبعاد بحذف جميع صفوف **سعر الدور** و **رفع سعر الدور** التي تمت تعبئتها بقيمة البُعد.</span><span class="sxs-lookup"><span data-stu-id="e95c2-136">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]