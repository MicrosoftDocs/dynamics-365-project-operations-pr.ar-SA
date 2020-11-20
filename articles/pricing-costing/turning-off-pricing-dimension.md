---
title: إيقاف تشغيل بُعد تسعير
description: يقدم هذا الموضوع معلومات حول كيفية إيقاف تشغيل أبعاد التسعير.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: ffeff2ab465f37b8a4e40f4e64b118e3bb412cb8
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4119267"
---
# <a name="turning-off-a-pricing-dimension"></a><span data-ttu-id="7ac6d-103">إيقاف تشغيل بُعد تسعير</span><span class="sxs-lookup"><span data-stu-id="7ac6d-103">Turning off a pricing dimension</span></span>

<span data-ttu-id="7ac6d-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="7ac6d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7ac6d-105">قد تحتاج إلى مراجعه استراتيجية التسعير وتحديثها كل بضع سنوات.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-105">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="7ac6d-106">قد تتطلب أي تحديثات تقوم بإجرائها أن تقوم بإيقاف تشغيل بُعد تسعير موجود وإنشاء واحد جديد.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-106">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="7ac6d-107">على سبيل المثال، ربما قمت مسبقًا بالتسعير حسب **الدور**، ولكنك قررت الآن التسعير حسب **تجربة العمل**.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-107">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="7ac6d-108">قد يتطلب هذا منك إيقاف تشغيل **الدور** كبُعد تسعير وإنشاء **تجربة عمل** كبعد تسعير جديد.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-108">This may require you to turn off **Role** as a pricing dimension and create **Work Experience** as a new pricing dimension.</span></span> 

<span data-ttu-id="7ac6d-109">ويمكن إيقاف تشغيل بعد التسعير، سواء كان جاهزًا أو مخصصًا، عن طريق تعيين حقلي **قابل للتطبيق على التكلفة** و **قابل للتطبيق على المبيعات** الخاصين ببعد التسعير إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-109">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="7ac6d-110">ومع ذلك، عند القيام بذلك قد تظهر رسالة الخطأ، **لا يمكن تحديث بعد التسعير أو حذفه في حالة وجود سجلات أسعار مرتبطة.**</span><span class="sxs-lookup"><span data-stu-id="7ac6d-110">However, when you do this, you might receive the error message, **Pricing dimension cannot be updated or deleted if there are associated price records.**</span></span>

<span data-ttu-id="7ac6d-111">تشير رسالة الخطأ هذه إلى أن هناك سجلات أسعار تم إعدادها مسبقًا للبعد الذي تم إيقاف تشغيله.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="7ac6d-112">يجب حذف كل سجلات **سعر الدور** و **رفع سعر الدور** التي تشير إلى بُعد قبل التمكن من تعيين إمكانية تطبيق البُعد إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="7ac6d-113">يتم تطبيق هذه القاعدة على كل من أبعاد التسعير الجاهزة وأبعاد التسعير المخصصة التي ربما قمت بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="7ac6d-114">ويرجع سبب هذا التحقق من الصحة إلى أن كل **سعر دور** يجب أن يحتوي على مجموعة فريدة من الأبعاد.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-114">The reason for this validation is because each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="7ac6d-115">على سبيل المثال، في قائمة الأسعار المسماة **أسعار التكلفة بالولايات المتحدة لعام 2018**، يكون لديك صفوف **سعر الدور** التالية.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="7ac6d-116">العنوان القياسي</span><span class="sxs-lookup"><span data-stu-id="7ac6d-116">Standard Title</span></span>         | <span data-ttu-id="7ac6d-117">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="7ac6d-117">Org Unit</span></span>    |<span data-ttu-id="7ac6d-118">الوحدة</span><span class="sxs-lookup"><span data-stu-id="7ac6d-118">Unit</span></span>   |<span data-ttu-id="7ac6d-119">السعر</span><span class="sxs-lookup"><span data-stu-id="7ac6d-119">Price</span></span>  |<span data-ttu-id="7ac6d-120">العملات</span><span class="sxs-lookup"><span data-stu-id="7ac6d-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="7ac6d-121">مهندس الأنظمة</span><span class="sxs-lookup"><span data-stu-id="7ac6d-121">Systems Engineer</span></span>|<span data-ttu-id="7ac6d-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="7ac6d-122">Contoso US</span></span>|<span data-ttu-id="7ac6d-123">Hour‬</span><span class="sxs-lookup"><span data-stu-id="7ac6d-123">Hour</span></span>| <span data-ttu-id="7ac6d-124">100</span><span class="sxs-lookup"><span data-stu-id="7ac6d-124">100</span></span>|<span data-ttu-id="7ac6d-125">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="7ac6d-125">USD</span></span>|
| <span data-ttu-id="7ac6d-126">مهندس أنظمة أول</span><span class="sxs-lookup"><span data-stu-id="7ac6d-126">Senior Systems Engineer</span></span>|<span data-ttu-id="7ac6d-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="7ac6d-127">Contoso US</span></span>|<span data-ttu-id="7ac6d-128">Hour‬</span><span class="sxs-lookup"><span data-stu-id="7ac6d-128">Hour</span></span>| <span data-ttu-id="7ac6d-129">150</span><span class="sxs-lookup"><span data-stu-id="7ac6d-129">150</span></span>| <span data-ttu-id="7ac6d-130">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="7ac6d-130">USD</span></span>|


<span data-ttu-id="7ac6d-131">عندما تقوم بإيقاف تشغيل **العنوان القياسي** باعتباره بُعد التسعير، ويقوم محرك التسعير بالبحث عن سعر، فسيبحث فقط عن قيمة **الوحدة التنظيمية** من سياق الإدخال.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-131">When you turn off **Standard Title** as the pricing dimension, and the pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="7ac6d-132">إذا كانت **الوحدة التنظيمية** الخاصة بسياق الإدخال هي "مؤسسة حسني بالولايات المتحدة"، فستكون النتيجة غير محددة لأن كلا الصفين سيتطابقان.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="7ac6d-133">لتجنب هذا السيناريو، عند إنشاء سجلات **سعر الدور** يقوم النظام بالتحقق من أن مجموعة الأبعاد فريدة من نوعها.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-133">To avoid this scenario, when you create **Role Price** records, the system validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="7ac6d-134">إذا تم إيقاف تشغيل البُعد بعد إنشاء سجلات **سعر الدور**، فيمكن مخالفة هذا القيد.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="7ac6d-135">وبالتالي، من المطلوب أن تقوم قبل إيقاف تشغيل أحد الأبعاد بحذف جميع صفوف **سعر الدور** و **رفع سعر الدور** التي تمت تعبئتها بقيمة البُعد.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>
