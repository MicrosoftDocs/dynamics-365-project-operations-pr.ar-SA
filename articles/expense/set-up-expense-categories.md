---
title: إعداد فئات المصروفات
description: يقدم هذا الموضوع معلومات حول كيفية إعداد فئات المصروفات والفئات المشتركة لتقارير المصروفات.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: f051d70f3dfe3b241dc0a206c0cdfda000f87c76
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896670"
---
# <a name="set-up-expense-categories"></a><span data-ttu-id="f1d3a-103">إعداد فئات المصروفات</span><span class="sxs-lookup"><span data-stu-id="f1d3a-103">Set up expense categories</span></span>

<span data-ttu-id="f1d3a-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="f1d3a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f1d3a-105">عندما يقوم الموظفون بإنشاء تقارير مصروفات، يجب أن يكون كل بند صروفات يتم تسجيله مقترنًا بفئة مصروفات.</span><span class="sxs-lookup"><span data-stu-id="f1d3a-105">When employees create expense reports, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="f1d3a-106">يتم اشتقاق فئات المصروفات من الفئات المشتركة التي يمكن مشاركتها عبر الكيانات القانونية في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="f1d3a-106">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="f1d3a-107">واستنادا إلى الطريقة التي يتم بها تعريف مؤسستك، فإن فئات المصروفات هذه يمكن مشاركتها أيضا في مناطق أخرى.</span><span class="sxs-lookup"><span data-stu-id="f1d3a-107">Depending on how your organization is defined, these expense categories can also be shared in other areas.</span></span> <span data-ttu-id="f1d3a-108">وتبعًا لتعريف مؤسستك والإرشاد من فريق التنفيذ، يجب عليك تحديد ما إذا كان سيتم استخدام الفئات في إدارة المصروفات فقط في إدارة المصروفات أم يجب مشاركتها في مناطق أخرى.</span><span class="sxs-lookup"><span data-stu-id="f1d3a-108">Based on the definition of your organization and guidance from the implementation team, you must determine whether the categories that are used in Expense management will be used only in Expense management or should be shared in other areas.</span></span>

> [!NOTE]
> <span data-ttu-id="f1d3a-109">يمكن مشاركة هذه الفئات بين إدارة المشروع والحسابات وإدارة المصروفات، أو بين إدارة المشروع والحسابات والإنتاج.</span><span class="sxs-lookup"><span data-stu-id="f1d3a-109">These categories can be shared between Project management and accounting and Expense management, or between Project management and accounting and Production.</span></span> <span data-ttu-id="f1d3a-110">مع ذلك، لا يمكن مشاركتها بين إدارة المصروفات والإنتاج.</span><span class="sxs-lookup"><span data-stu-id="f1d3a-110">However, they can't be shared between Expense management and Production.</span></span>

<span data-ttu-id="f1d3a-111">قبل أن تتمكن من بدء عملية الإعداد، يجب اتخاذ القرارات التالية لكل فئة من فئات المصروفات:</span><span class="sxs-lookup"><span data-stu-id="f1d3a-111">Before you can begin the setup process, the following decisions must be made for each expense category:</span></span>

- <span data-ttu-id="f1d3a-112">ما هي فئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-112">What is the expense category?</span></span> <span data-ttu-id="f1d3a-113">وتتضمن الأمثلة فئات رحلات الطيران أو الفنادق أو الأميال.</span><span class="sxs-lookup"><span data-stu-id="f1d3a-113">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="f1d3a-114">هل يمكن أيضا استخدام فئة المصروفات في إدارة المشروع والمحاسبة؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-114">Can the expense category also be used in Project management and accounting?</span></span> <span data-ttu-id="f1d3a-115">إذا كان يمكن استخدامها، فيجب أيضًا أن تحسم أمرك بشأن القرارات التالية:</span><span class="sxs-lookup"><span data-stu-id="f1d3a-115">If it can, you must also make the following decisions:</span></span>

    - <span data-ttu-id="f1d3a-116">ما هي حسابات التكلفة التي سيتم استخدامها للمصروفات التالية؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-116">Which cost accounts will be used for the following expenses?</span></span>

        - <span data-ttu-id="f1d3a-117">التكلفة</span><span class="sxs-lookup"><span data-stu-id="f1d3a-117">Cost</span></span>
        - <span data-ttu-id="f1d3a-118">توزيع كشف الرواتب</span><span class="sxs-lookup"><span data-stu-id="f1d3a-118">Payroll allocation</span></span>
        - <span data-ttu-id="f1d3a-119">الأعمال قيد التنفيذ (WIP)-قيمة التكلفة</span><span class="sxs-lookup"><span data-stu-id="f1d3a-119">WIP-cost value</span></span>
        - <span data-ttu-id="f1d3a-120">عنصر التكلفة</span><span class="sxs-lookup"><span data-stu-id="f1d3a-120">Cost-item</span></span>
        - <span data-ttu-id="f1d3a-121">الأعمال قيد التنفيذ (WIP) - عنصر قيمة التكلفة</span><span class="sxs-lookup"><span data-stu-id="f1d3a-121">WIP-cost value-item</span></span>
        - <span data-ttu-id="f1d3a-122">الخسارة المتكبدة</span><span class="sxs-lookup"><span data-stu-id="f1d3a-122">Accrued loss</span></span>
        - <span data-ttu-id="f1d3a-123">الأعمال قيد التنفيذ (WIP) - الخسارة المتكبدة</span><span class="sxs-lookup"><span data-stu-id="f1d3a-123">WIP-accrued loss</span></span>

    - <span data-ttu-id="f1d3a-124">ما هي حسابات الإيرادات التي سيتم استخدامها للمصادر التالية من الإيرادات؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-124">Which revenue accounts will be used for the following sources of revenue?</span></span>

        - <span data-ttu-id="f1d3a-125">الإيرادات المفوترة</span><span class="sxs-lookup"><span data-stu-id="f1d3a-125">Invoiced revenue</span></span>
        - <span data-ttu-id="f1d3a-126">الإيرادات المستحقة - قيمة المبيعات</span><span class="sxs-lookup"><span data-stu-id="f1d3a-126">Accrued revenue-sales value</span></span>
        - <span data-ttu-id="f1d3a-127">الأعمال قيد التنفيذ (WIP) - قيمة المبيعات</span><span class="sxs-lookup"><span data-stu-id="f1d3a-127">WIP-sales value</span></span>
        - <span data-ttu-id="f1d3a-128">الإيراد المستحق-الإنتاج</span><span class="sxs-lookup"><span data-stu-id="f1d3a-128">Accrued revenue-production</span></span>
        - <span data-ttu-id="f1d3a-129">الأعمال قيد التنفيذ (WIP) - الإنتاج</span><span class="sxs-lookup"><span data-stu-id="f1d3a-129">WIP-production</span></span>
        - <span data-ttu-id="f1d3a-130">الإيراد المستحق - الربح</span><span class="sxs-lookup"><span data-stu-id="f1d3a-130">Accrued revenue-profit</span></span>
        - <span data-ttu-id="f1d3a-131">الأعمال قيد التنفيذ (WIP) - الربح</span><span class="sxs-lookup"><span data-stu-id="f1d3a-131">WIP-profit</span></span>
        - <span data-ttu-id="f1d3a-132">الإيراد المستحق - الاشتراك</span><span class="sxs-lookup"><span data-stu-id="f1d3a-132">Accrued revenue-subscription</span></span>
        - <span data-ttu-id="f1d3a-133">الأعمال قيد التنفيذ (WIP) - الاشتراك</span><span class="sxs-lookup"><span data-stu-id="f1d3a-133">WIP-subscription</span></span>

- <span data-ttu-id="f1d3a-134">ما هو نوع المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-134">What is the expense type?</span></span>
- <span data-ttu-id="f1d3a-135">ما هي طريقة الدفع الافتراضية لفئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-135">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="f1d3a-136">هل يجب تفصيل بنود المصروفات في فئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-136">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="f1d3a-137">ما هو الحساب الرئيسي الافتراضي لفئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-137">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="f1d3a-138">ما هي مجموعة ضريبة مبيعات الصنف الافتراضية لفئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-138">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="f1d3a-139">هل يتم السماح بطرق دفع إضافية لفئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-139">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="f1d3a-140">وإذا كان الأمر كذلك، فما هي؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-140">If so, what are they?</span></span>
- <span data-ttu-id="f1d3a-141">هل يوجد هناك فئات فرعية في فئة المصروفات هذه؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-141">Are there subcategories in this expense category?</span></span> <span data-ttu-id="f1d3a-142">إذا كان هناك فئات فرعية، فيجب أيضًا أن تحسم أمرك بشأن القرارات التالية:</span><span class="sxs-lookup"><span data-stu-id="f1d3a-142">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="f1d3a-143">هل يتم استبعاد أي من الفئات الفرعية من استرداد الضريبة؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-143">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="f1d3a-144">ما هي مجموعة ضريبة مبيعات الصنف للفئات الفرعية؟</span><span class="sxs-lookup"><span data-stu-id="f1d3a-144">What is the item sales tax group of the subcategories?</span></span>
