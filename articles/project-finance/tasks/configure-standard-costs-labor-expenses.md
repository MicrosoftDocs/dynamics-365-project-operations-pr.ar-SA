---
title: تكوين التكاليف القياسية للعمالة والمصروفات
description: يشرح هذا الموضوع كيفية إعداد التكاليف القياسية للعمالة والمصاريف لمشروع.
author: KimANelson
manager: AnnBe
ms.date: 08/02/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjCostPriceHour, ProjSalesPriceHour, ProjCostPriceExpense, ProjSalesPriceCost
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.assetid: fa7c024f-4b18-4d29-9fd4-9c430cd83fad
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: f3e796cc03aeaa28938c56ce37d5075755248dfa
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748746"
---
# <a name="configure-standard-costs-for-labor-and-expenses"></a><span data-ttu-id="9ceb4-103">تكوين التكاليف القياسية للعمالة والمصروفات</span><span class="sxs-lookup"><span data-stu-id="9ceb4-103">Configure standard costs for labor and expenses</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="9ceb4-104">يشرح هذا الموضوع كيفية إعداد التكاليف القياسية للعمالة والمصاريف لمشروع.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-104">This topic explains how to set up standard costs for labor and expenses for a project.</span></span> <span data-ttu-id="9ceb4-105">تستخدم هذه المهمة مجموعة بيانات USSI.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="9ceb4-106">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > إعداد > الأسعار > سعر النقل (بالساعة)**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-106">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (hour)**.</span></span>
2. <span data-ttu-id="9ceb4-107">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-107">Select **New**.</span></span>
3. <span data-ttu-id="9ceb4-108">في حقل **تاريخ السريان**، وأدخل تاريخًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-108">In the **Effective date** field, enter a date.</span></span>
4. <span data-ttu-id="9ceb4-109">في الحقل **سعر التكلفة**، أدخل رقمًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-109">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="9ceb4-110">يمكنك إعداد سعر تكلفة قياسي لفئة المشروع ، أو يمكنك إعداد سعر التكلفة حسب رقم العامل أو رقم المشروع أو الفئة أو التاريخ أو أي مجموعة من هذه الأسعار.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-110">You can set up a standard cost price for the project category, or you can set up a cost price by worker number, project number, category, date, or any combination of these.</span></span> <span data-ttu-id="9ceb4-111">سعر التكلفة المطبق هو سعر التكلفة بأعلى مستوى من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-111">The cost price that is applied is the cost price with the highest level of detail.</span></span>  
5. <span data-ttu-id="9ceb4-112">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-112">Select **Save**.</span></span>
6. <span data-ttu-id="9ceb4-113">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > إعداد > الأسعار > سعر المبيعات (بالساعة)**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-113">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (hour)**.</span></span>
7. <span data-ttu-id="9ceb4-114">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-114">Select **New**.</span></span>
8. <span data-ttu-id="9ceb4-115">في حقل **تاريخ السريان**، وأدخل تاريخًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-115">In the **Effective date** field, enter a date.</span></span>
9. <span data-ttu-id="9ceb4-116">في الحقل **صالح لـ**، حدد خيارًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-116">In the **Valid for** field, select an option.</span></span>
10. <span data-ttu-id="9ceb4-117">في حقل **الأسعار**، حدد رقمًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-117">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="9ceb4-118">يمكنك إعداد سعر مبيعات قياسي لحركات الساعة أو لفئة مشروع.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-118">You can set up a standard sales price for hour transactions or for a project category.</span></span> <span data-ttu-id="9ceb4-119">يمكنك أيضًا إعداد أسعار المبيعات حسب رقم العامل أو رقم المشروع أو الفئة أو تاريخ المعاملة أو أي مجموعة من هذه الأسعار.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-119">You can also set up sales prices by worker number, project number, category, transaction date, or any combination of these.</span></span> <span data-ttu-id="9ceb4-120">سعر البيع الفعلي ، الذي يتم تطبيقه عندما يدخل عامل معاملة في دفتر يومية الساعة ، هو سعر المبيعات بأعلى مستوى من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-120">The actual sales price, which is applied when a worker enters a transaction in the Hour journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="9ceb4-121">على سبيل المثال ، إذا تم إعداد كل من سعر المبيعات العام وسعر المبيعات الخاص بالعمال ، فسيتم استخدام سعر المبيعات الخاص بالعامل.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-121">For example, if both a general sales price and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
11. <span data-ttu-id="9ceb4-122">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-122">Select **Save**.</span></span>
12. <span data-ttu-id="9ceb4-123">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-123">Close the page.</span></span>
13. <span data-ttu-id="9ceb4-124">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > إعداد > الأسعار > سعر النقل (المصروفات)**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-124">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (expense)**.</span></span>
14. <span data-ttu-id="9ceb4-125">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-125">Select **New**.</span></span>
15. <span data-ttu-id="9ceb4-126">في حقل **تاريخ السريان**، وأدخل تاريخًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-126">In the **Effective date** field, enter a date.</span></span>
16. <span data-ttu-id="9ceb4-127">في الحقل **سعر التكلفة**، أدخل رقمًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-127">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="9ceb4-128">يمكن ملء عدة حقول ، ولكن هذا هو الحد الأدنى المطلوب لحفظ السجل.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-128">Multiple fields can be filled in, but this is the minimum needed to save the record.</span></span>  
17. <span data-ttu-id="9ceb4-129">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-129">Select **Save**.</span></span>
18. <span data-ttu-id="9ceb4-130">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > إعداد > الأسعار > سعر المبيعات (المصروفات)**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-130">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (expense)**.</span></span>
19. <span data-ttu-id="9ceb4-131">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-131">Select **New**.</span></span>
20. <span data-ttu-id="9ceb4-132">في حقل **تاريخ السريان**، وأدخل تاريخًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-132">In the **Effective date** field, enter a date.</span></span>
21. <span data-ttu-id="9ceb4-133">في الحقل **صالح لـ**، حدد خيارًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-133">In the **Valid for** field, select an option.</span></span>
22. <span data-ttu-id="9ceb4-134">في حقل **الأسعار**، حدد رقمًا.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-134">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="9ceb4-135">سعر المبيعات الفعلي ، الذي يتم تطبيقه عندما يدخل العامل المعاملات في دفتر يومية النفقات ، هو سعر المبيعات بأعلى مستوى من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-135">The actual sales price, which is applied when a worker enters transactions in an expense journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="9ceb4-136">على سبيل المثال ، إذا تم إعداد كلٍّ من سعر المبيعات العام والخاص بالعاملين ، فسيتم استخدام سعر المبيعات الخاص بالعامل.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-136">For example, if both a general and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
23. <span data-ttu-id="9ceb4-137">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9ceb4-137">Select **Save**.</span></span>

