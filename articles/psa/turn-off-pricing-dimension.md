---
title: إيقاف تشغيل بُعد تسعير
description: يوضح هذا الموضوع كيفية إعداد أبعاد التسعير في حل Project Service.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 1ae95430c368370145c7081a5d94d6161a7700b4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070729"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="4b901-103">إيقاف تشغيل بُعد تسعير</span><span class="sxs-lookup"><span data-stu-id="4b901-103">Turn off a pricing dimension</span></span>

<span data-ttu-id="4b901-104">قد تحتاج إلى مراجعه استراتيجية التسعير وتحديثها كل بضع سنوات.</span><span class="sxs-lookup"><span data-stu-id="4b901-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="4b901-105">قد تتطلب أي تحديثات تقوم بإجرائها أن تقوم بإيقاف تشغيل بُعد تسعير موجود وإنشاء واحد جديد.</span><span class="sxs-lookup"><span data-stu-id="4b901-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="4b901-106">على سبيل المثال، ربما قمت مسبقًا بالتسعير حسب **الدور** ، ولكنك قررت الآن التسعير حسب **تجربة العمل**.</span><span class="sxs-lookup"><span data-stu-id="4b901-106">For example, you may have previously priced by **Role** , but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="4b901-107">قد يتطلب هذا منك إيقاف تشغيل **الدور** كبُعد تسعير وإنشاء **تجربة عمل** كبعد تسعير جديد.</span><span class="sxs-lookup"><span data-stu-id="4b901-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="4b901-108">ويمكن إيقاف تشغيل بعد التسعير، سواء كان جاهزًا أو مخصصًا، عن طريق تعيين حقلي **قابل للتطبيق على التكلفة** و **قابل للتطبيق على المبيعات** الخاصين ببعد التسعير إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="4b901-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="4b901-109">ومع ذلك، عند القيام بذلك، قد تتلقى رسالة الخطأ التالية.</span><span class="sxs-lookup"><span data-stu-id="4b901-109">However, when you do this, you might receive the following error message.</span></span>

![احتمال حدوث خطأ في عمليه الأعمال عند عدم القيام بإيقاف تشغيل بعد تسعير](media/Business-Process-Error.png)


<span data-ttu-id="4b901-111">تشير رسالة الخطأ هذه إلى أن هناك سجلات أسعار تم إعدادها مسبقًا للبعد الذي تم إيقاف تشغيله.</span><span class="sxs-lookup"><span data-stu-id="4b901-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="4b901-112">يجب حذف كل سجلات **سعر الدور** و **رفع سعر الدور** التي تشير إلى بُعد قبل التمكن من تعيين إمكانية تطبيق البُعد إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="4b901-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="4b901-113">يتم تطبيق هذه القاعدة على كل من أبعاد التسعير الجاهزة وأبعاد التسعير المخصصة التي ربما قمت بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="4b901-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="4b901-114">ويرجع سبب هذا التحقق من الصحة إلى أن Project Service تحتوي على قيد بأن سجل كل **سعر دور** يجب أن يحتوي على مجموعة فريدة من الأبعاد.</span><span class="sxs-lookup"><span data-stu-id="4b901-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="4b901-115">على سبيل المثال، في قائمة الأسعار المسماة **أسعار التكلفة بالولايات المتحدة لعام 2018** ، يكون لديك صفوف **سعر الدور** التالية.</span><span class="sxs-lookup"><span data-stu-id="4b901-115">For example, on a price list called **US Cost Rates 2018** , you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="4b901-116">العنوان القياسي</span><span class="sxs-lookup"><span data-stu-id="4b901-116">Standard Title</span></span>         | <span data-ttu-id="4b901-117">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="4b901-117">Org Unit</span></span>    |<span data-ttu-id="4b901-118">الوحدة</span><span class="sxs-lookup"><span data-stu-id="4b901-118">Unit</span></span>   |<span data-ttu-id="4b901-119">السعر</span><span class="sxs-lookup"><span data-stu-id="4b901-119">Price</span></span>  |<span data-ttu-id="4b901-120">العملات</span><span class="sxs-lookup"><span data-stu-id="4b901-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="4b901-121">مهندس الأنظمة</span><span class="sxs-lookup"><span data-stu-id="4b901-121">Systems Engineer</span></span>|<span data-ttu-id="4b901-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="4b901-122">Contoso US</span></span>|<span data-ttu-id="4b901-123">Hour‬</span><span class="sxs-lookup"><span data-stu-id="4b901-123">Hour</span></span>| <span data-ttu-id="4b901-124">100</span><span class="sxs-lookup"><span data-stu-id="4b901-124">100</span></span>|<span data-ttu-id="4b901-125">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="4b901-125">USD</span></span>|
| <span data-ttu-id="4b901-126">مهندس أنظمة أول</span><span class="sxs-lookup"><span data-stu-id="4b901-126">Senior Systems Engineer</span></span>|<span data-ttu-id="4b901-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="4b901-127">Contoso US</span></span>|<span data-ttu-id="4b901-128">Hour‬</span><span class="sxs-lookup"><span data-stu-id="4b901-128">Hour</span></span>| <span data-ttu-id="4b901-129">150</span><span class="sxs-lookup"><span data-stu-id="4b901-129">150</span></span>| <span data-ttu-id="4b901-130">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="4b901-130">USD</span></span>|


<span data-ttu-id="4b901-131">عندما تقوم بإيقاف تشغيل **العنوان القياسي** باعتباره بُعد التسعير، ويقوم محرك تسعير Project Service بالبحث عن سعر، فسيبحث فقط عن قيمة **الوحدة التنظيمية** من سياق الإدخال.</span><span class="sxs-lookup"><span data-stu-id="4b901-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="4b901-132">إذا كانت **الوحدة التنظيمية** الخاصة بسياق الإدخال هي "مؤسسة حسني بالولايات المتحدة"، فستكون النتيجة غير محددة لأن كلا الصفين سيتطابقان.</span><span class="sxs-lookup"><span data-stu-id="4b901-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="4b901-133">لتجنب هذا السيناريو، عند إنشاء سجلات **سعر الدور** ، تقوم Project Service بالتحقق من أن مجموعة الأبعاد فريدة من نوعها.</span><span class="sxs-lookup"><span data-stu-id="4b901-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="4b901-134">إذا تم إيقاف تشغيل البُعد بعد إنشاء سجلات **سعر الدور** ، فيمكن مخالفة هذا القيد.</span><span class="sxs-lookup"><span data-stu-id="4b901-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="4b901-135">وبالتالي، من المطلوب أن تقوم قبل إيقاف تشغيل أحد الأبعاد بحذف جميع صفوف **سعر الدور** و **رفع سعر الدور** التي تمت تعبئتها بقيمة البُعد.</span><span class="sxs-lookup"><span data-stu-id="4b901-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>

