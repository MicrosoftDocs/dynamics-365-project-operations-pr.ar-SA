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
ms.openlocfilehash: 1f601be072e84fc04246cd55a260c8004f6fb3e5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289713"
---
# <a name="transfer-project-budgets-at-fiscal-year-end"></a><span data-ttu-id="dcd18-103">نقل موازنات المشروع في نهاية السنة المالية</span><span class="sxs-lookup"><span data-stu-id="dcd18-103">Transfer project budgets at fiscal year end</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="dcd18-104">عند العمل على مشروع متعدد السنوات، قد يكون لديك موازنة متبقية في نهاية السنة المالية.</span><span class="sxs-lookup"><span data-stu-id="dcd18-104">When working on a multi-year project, you might have remaining budget at the end of the fiscal year.</span></span> <span data-ttu-id="dcd18-105">يمكنك نقل مبالغ الموازنة المتبقية إلى سنة مستقبلية، وإنشاء تفاصيل سجل الموازنة للمبالغ الموجودة في الحسابات المقترنة في دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="dcd18-105">You can transfer the remaining budget amounts to a future year, and create budget register details for the amounts in the associated general ledger accounts.</span></span> <span data-ttu-id="dcd18-106">قبل تحويل المبالغ المتبقية، يمكنك مراجعة وتحليل مبالغ الموازنة المتبقية.</span><span class="sxs-lookup"><span data-stu-id="dcd18-106">Before you carry forward the remaining amounts, review and analyze the remaining budget amounts.</span></span>

## <a name="review-and-analyze-remaining-budget-amounts"></a><span data-ttu-id="dcd18-107">مراجعة وتحليل مبالغ الموازنة المتبقية</span><span class="sxs-lookup"><span data-stu-id="dcd18-107">Review and analyze remaining budget amounts</span></span>

<span data-ttu-id="dcd18-108">أكمل الخطوات التالية لمراجعة مبالغ موازنة نهاية السنه للمشاريع، ولكن دون تحويل المبالغ.</span><span class="sxs-lookup"><span data-stu-id="dcd18-108">Complete the following steps to review the year-end budget amounts for projects, but not carry the amounts forward.</span></span>

1. <span data-ttu-id="dcd18-109">انتقل إلى **إدارة المشاريع والمحاسبة‬** > **دوري** > **الموازنات** > **تحويل الموازنات**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-109">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="dcd18-110">في الصفحة **معالجة تحويل موازنة المشروع**، على علامة التبويب **خيارات نهاية السنة**، تأكد من عدم تمكين الخيار **تحويل مبالغ موازنة المشروع المتبقية**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-110">On the **Project budget carry-forward process** page, on the **Year-end options** tab, verify that **Carry forward remaining project budget amounts** is not enabled.</span></span>
3. <span data-ttu-id="dcd18-111">من علامة التبويب **المعلمات**، في حقل **سنه موازنة المشروع**، حدد السنة المالية التي ترغب في عرض مبلغ الموازنة المتبقية لها.</span><span class="sxs-lookup"><span data-stu-id="dcd18-111">On the **Parameters** tab, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
4. <span data-ttu-id="dcd18-112">في حقل **السنة المالية الافتتاحية**، حدد السنة المالية التي ترغب في عرض مبلغ الموازنة المتبقية لها.</span><span class="sxs-lookup"><span data-stu-id="dcd18-112">In the **Opening fiscal year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
5. <span data-ttu-id="dcd18-113">في الحقل **من نموذج التنبؤ**، حدد **الموازنة المتبقية**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-113">In the **From forecast model** field, select **Remaining budget**.</span></span> 
6. <span data-ttu-id="dcd18-114">لتضمين المشاريع التي تتوافق مع معاييرك المحددة والتي ليس لديها موازنة متبقية، حدد **إظهار القيمة الصفرية المتبقية**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-114">To include projects that meet your selected criteria and have no remaining budget, select **Show zero remaining**.</span></span>  
7. <span data-ttu-id="dcd18-115">في علامة التبويب **موازنات محددة**، حدد **استرداد جميع الموازنات** لتحميل جميع الموازنات التي تتطابق مع معاييرك المحددة، ثم حدد **معالجة**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-115">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match your selected criteria, and then select **Process**.</span></span> 
8. <span data-ttu-id="dcd18-116">لتصميم استعلام قاعدة بيانات يقوم بتحميل مجموعة محددة من الموازنات في الجزء، حدد **استرداد موازنات محددة**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-116">To design a database query that loads a specific set of budgets into the pane, select **Retrieve selected budgets**.</span></span>

<span data-ttu-id="dcd18-117">لمزيد من المعلومات حول بند معين في الجزء، حدد البند، ثم حدد **عرض تفاصيل الموازنة** أو **عرض الحسابات**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-117">For more information about a specific line in the pane, select the line, and then select **View budget details** or **View accounts**.</span></span>

## <a name="carry-forward-remaining-budget-amounts"></a><span data-ttu-id="dcd18-118">تحويل مبالغ الموازنة المتبقية</span><span class="sxs-lookup"><span data-stu-id="dcd18-118">Carry forward remaining budget amounts</span></span> 

<span data-ttu-id="dcd18-119">عند معالجة مبالغ الموازنة المتبقية، يمكنك إنشاء حركات في دفتر الأستاذ العام للمبالغ التي تقوم بتحويلها.</span><span class="sxs-lookup"><span data-stu-id="dcd18-119">When you process remaining budget amounts, you can create transactions in the general ledger for the amounts that you are carrying forward.</span></span> <span data-ttu-id="dcd18-120">لإنشاء حركات دفتر أستاذ عام، استكمل الخطوات في القسم [تحويل مبالغ الموازنة وإنشاء حركات دفتر الأستاذ العام](#carry-forward).</span><span class="sxs-lookup"><span data-stu-id="dcd18-120">To create general ledger transactions, complete the steps in the section, [Carry forward budget amounts and create general ledger transactions](#carry-forward).</span></span> 

> [!NOTE]
> <span data-ttu-id="dcd18-121">يتم نقل مبالغ الموازنة التي يتم تحويلها إلى نموذج التنبؤ المحدد في صفحة **نماذج التنبؤ** كنموذج تنبؤ التحويل.</span><span class="sxs-lookup"><span data-stu-id="dcd18-121">Budget amounts that are carried forward are transferred to the forecast model that is selected in the **Forecast models** page as the carry-forward forecast model.</span></span>  

## <a name="carry-forward-budget-amounts-and-create-general-ledger-transactions"></a><a name="carry-forward"></a><span data-ttu-id="dcd18-122">تحويل مبالغ الموازنة وإنشاء حركات دفتر الأستاذ العام</span><span class="sxs-lookup"><span data-stu-id="dcd18-122">Carry forward budget amounts and create general ledger transactions</span></span>

1.  <span data-ttu-id="dcd18-123">حدد **إدارة المشاريع والمحاسبة‬** > **دوري** > **الموازنات** > **تحويل الموازنات**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-123">Select **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="dcd18-124">في الصفحة **معالجة تحويل موازنة المشروع**، حدد **نهاية السنة**، ثم قم بتمكين الخيارين **تحويل مبالغ موازنة المشروع المتبقية‬‏‫** و **إنشاء إدخالات سجل الموازنة في دفتر الأستاذ العام**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-124">On the **Project budget carry-forward process** page, select **Year-end**, and then enable **Carry forward remaining project budget amounts** and **Create budget register entries in general ledger**.</span></span> 
3. <span data-ttu-id="dcd18-125">في علامة تبويب **المعلمات**، في مجموعة حقول **معلمات المشروع**، حدد الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="dcd18-125">On the **Parameters** tab, in the **Project parameters** field group, select the following:</span></span>

   - <span data-ttu-id="dcd18-126">**سنة موازنة المشروع**: حدد بداية السنة المالية التي ترغب في عرض مبالغ الموازنة المتبقية لها.</span><span class="sxs-lookup"><span data-stu-id="dcd18-126">**Project budget year**: Select the beginning of the fiscal year for which you want to view the remaining budget amounts.</span></span> 
   - <span data-ttu-id="dcd18-127">**الأرباح والخسائر**: أنشئ حركات الأرباح والخسائر في دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="dcd18-127">**Profit and loss**: Create profit and loss transactions in the general ledger.</span></span> 
   -  <span data-ttu-id="dcd18-128">**الاعمال قيد التنفيذ**: أنشئ حركات الاعمال قيد التنفيذ في دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="dcd18-128">**WIP**: Create Work in Progress (WIP) transactions in the general ledger.</span></span>
   -  <span data-ttu-id="dcd18-129">**كشف الرواتب**: أنشئ حركات توزيع كشوف الرواتب في دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="dcd18-129">**Payroll**: Create payroll allocation transactions in the general ledger.</span></span> 

5. <span data-ttu-id="dcd18-130">في مجموعة حقول **دفتر الأستاذ العام**، أدخل المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="dcd18-130">In the **General ledger** field group, provide the following information:</span></span> 

   - <span data-ttu-id="dcd18-131">في حقل **السنة المالية الافتتاحية**، حدد السنة المالية التي تريد أن تنقل إليها مبالغ الموازنة المتبقية للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="dcd18-131">In the **Opening fiscal year** field, select the fiscal year that you want to transfer remaining budget amounts to for the projects.</span></span> <span data-ttu-id="dcd18-132">القيمة الافتراضية هي عام واحد بعد القيمة في الحقل **سنة موازنة المشروع**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-132">The default value is one year after the value in the **Project budget year** field.</span></span>
   -  <span data-ttu-id="dcd18-133">في الحقل **فترة التحويل**، حدد الفترة التي تريد إنشاء تفاصيل سجل الموازنة لها في دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="dcd18-133">In the **Carry-forward period** field, select the period that you want to create the budget register details for in the general ledger.</span></span> <span data-ttu-id="dcd18-134">هذه هي عادةً الفترة الأولى في السنة المالية الافتتاحية‬‏‫.</span><span class="sxs-lookup"><span data-stu-id="dcd18-134">This is typically the first period in the opening fiscal year.</span></span>

6. <span data-ttu-id="dcd18-135">في مجموعة حقول **نسخ من/إلى**، أدخل المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="dcd18-135">In the **Copy from/to** field group, provide the following information:</span></span>

   - <span data-ttu-id="dcd18-136">في الحقل **من نموذج التنبؤ**، حدد نموذج التنبؤ بموازنة المشروع المقترن بمبالغ الموازنة المتبقية التي ترغب في نقلها إلى المشاريع.</span><span class="sxs-lookup"><span data-stu-id="dcd18-136">In the **From forecast model** field, select the project budget forecast model associated with the remaining budget amounts you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="dcd18-137">في الحقل **إلى نموذج موازنة دفتر الأستاذ**، حدد نموذج موازنة دفتر الأستاذ المقترن بمبالغ الموازنة المتبقية التي ترغب في نقلها إلى دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="dcd18-137">In the **To ledger budget model** field, select the ledger budget model associated with the budget amounts you want to transfer to the general ledger.</span></span> 
   -  <span data-ttu-id="dcd18-138">حدد **نقل عملة المبيعات** لاستخدام عملة المبيعات الخاصة بالمشروع في حركات دفتر الأستاذ العام التي يتم إنشاؤها عند نقل مبالغ الموازنة للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="dcd18-138">Select **Transfer sales currency** to use the project's sales currency for the general ledger transactions that are created when you transfer the budget amounts for the projects.</span></span> <span data-ttu-id="dcd18-139">وعندما لا يكون الخيار محددًا، تستخدم الحركات عملة المحاسبة.</span><span class="sxs-lookup"><span data-stu-id="dcd18-139">When the option is not selected, the transactions use the accounting currency.</span></span> 
   -  <span data-ttu-id="dcd18-140">حدد **إظهار القيمة الصفرية المتبقية** لتضمين المشاريع التي ليس لديها مبالغ متبقية في الموازنة، ولكنها تستوفي المعايير الأخرى التي تحددها في المشاريع المعروضة في الجزء السفلي.</span><span class="sxs-lookup"><span data-stu-id="dcd18-140">Select **Show zero remaining** to include projects that have no remaining budget amounts, but meet the other criteria that you select in the projects displayed in the bottom pane.</span></span>

7. <span data-ttu-id="dcd18-141">في علامة التبويب **موازنات محددة**، حدد **استرداد جميع الموازنات** لتحميل جميع الموازنات التي تتطابق مع معاييرك المحددة.</span><span class="sxs-lookup"><span data-stu-id="dcd18-141">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match the criteria you selected.</span></span> <span data-ttu-id="dcd18-142">إذا كنت تفضل تصميم استعلام قاعدة بيانات يقوم بتحميل مجموعة محددة من موازنات المشروع إلى الجزء، فحدد **استرداد موازنات محددة**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-142">If you prefer to design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>
8. <span data-ttu-id="dcd18-143">بالنسبة لكل مشروع تريد معالجته، حدد الخيار الموجود في بداية السطر للمشروع.</span><span class="sxs-lookup"><span data-stu-id="dcd18-143">For each project that you want to process, select the option at the beginning of the line for the project.</span></span>

    > [!TIP]
    > <span data-ttu-id="dcd18-144">لتحديد كافة المشروعات أو معظمها، حدد خانة الاختيار الموجودة في الزاوية العلوية اليسرى.</span><span class="sxs-lookup"><span data-stu-id="dcd18-144">To select all or most of the projects, select the check mark in the top upper-left corner.</span></span> <span data-ttu-id="dcd18-145">لاستثناء معالجة أي مشروع، قم بإلغاء تحديد خانة الاختيار الخاصة بذلك المشروع.</span><span class="sxs-lookup"><span data-stu-id="dcd18-145">To exclude processing any project, clear the check mark for that project.</span></span>

9. <span data-ttu-id="dcd18-146">لنقل مبالغ الموازنة المتبقية للمشاريع المحددة إلى السنة المالية المحددة وإنشاء تفاصيل سجل الموازنة في دفتر الأستاذ العام، حدد **معالجة**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-146">To transfer the remaining budget amounts for the selected projects to the selected fiscal year and create budget register details in the general ledger, select **Process**.</span></span>

## <a name="carry-forward-budget-amounts-without-creating-general-ledger-transactions"></a><span data-ttu-id="dcd18-147">تحويل مبالغ الموازنة من دون إنشاء حركات دفتر الأستاذ العام</span><span class="sxs-lookup"><span data-stu-id="dcd18-147">Carry forward budget amounts without creating general ledger transactions</span></span>

1. <span data-ttu-id="dcd18-148">انتقل إلى **إدارة المشاريع والمحاسبة‬** > **دوري** > **الموازنات** > **تحويل الموازنات**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-148">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span>
2. <span data-ttu-id="dcd18-149">في الصفحة **معالجة تحويل موازنة المشروع**، في حقل **خيارات نهاية السنة**، حدد **تحويل مبالغ موازنة المشروع المتبقية**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-149">On the **Project budget carry-forward process** page, in the **Year-end options** field, select **Carry forward remaining project budget amounts**.</span></span>
3. <span data-ttu-id="dcd18-150">من مجموعة **المعلمات**، في حقل **سنه موازنة المشروع**، حدد السنة المالية التي ترغب في عرض مبالغ الموازنة المتبقية لها.</span><span class="sxs-lookup"><span data-stu-id="dcd18-150">In the **Parameters** group, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amounts.</span></span>
4. <span data-ttu-id="dcd18-151">في المجموعة **نسخ من/إلى**، أدخل المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="dcd18-151">In the **Copy from/to** group, provide the following information:</span></span>

   - <span data-ttu-id="dcd18-152">في الحقل **من نموذج التنبؤ**، حدد نموذج التنبؤ بموازنة المشروع المقترن بمبالغ الموازنة المتبقية التي ترغب في نقلها إلى المشاريع.</span><span class="sxs-lookup"><span data-stu-id="dcd18-152">In the **From forecast model** field, select the project budget forecast model that is associated with the remaining budget amounts that you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="dcd18-153">حدد **إظهار القيمة الصفرية المتبقية** لتضمين المشاريع التي ليس لديها موازنة متبقية، ولكنها تتوافق مع المعايير الأخرى التي حددتها.</span><span class="sxs-lookup"><span data-stu-id="dcd18-153">Select **Show zero remaining** to include projects that have no remaining budget amounts, but that meet the other criteria you selected.</span></span>
   - <span data-ttu-id="dcd18-154">في المجموعة **موازنات محددة**، حدد **استرداد جميع الموازنات** لتحميل جميع الموازنات التي تتطابق مع معاييرك المحددة.</span><span class="sxs-lookup"><span data-stu-id="dcd18-154">In the **Select Budgets** group, select **Retrieve all budgets** to load all budgets that match the criteria that you selected.</span></span> <span data-ttu-id="dcd18-155">لتصميم استعلام قاعدة بيانات يقوم بتحميل مجموعة محددة من موازنات المشروع في الجزء، حدد **استرداد موازنات محددة**.</span><span class="sxs-lookup"><span data-stu-id="dcd18-155">To design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>

5. <span data-ttu-id="dcd18-156">بالنسبة لكل مشروع تريد معالجته، حدد الخيار الموجود في بداية السطر للمشروع.</span><span class="sxs-lookup"><span data-stu-id="dcd18-156">For each project that you want to process, select the option at the beginning of the line for the project.</span></span> 
6. <span data-ttu-id="dcd18-157">حدد **معالجة** لنقل مبالغ الموازنة المتبقية للمشاريع المحددة إلى السنة المالية المحددة.</span><span class="sxs-lookup"><span data-stu-id="dcd18-157">Select **Process** to transfer the remaining budget amounts for the selected projects to the selected fiscal year.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]