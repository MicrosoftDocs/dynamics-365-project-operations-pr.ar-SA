---
title: إنشاء عقود متقدمة للفوترة استنادًا إلى التقدم
description: يشرح هذا الموضوع كيفية إنشاء عقود المشروع بحيث يمكنك إنشاء الفواتير للعملاء، استنادًا إلى النسبة المئوية للعمل المكتمل.
author: RadhikaRS
ms.date: 03/26/2020
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 3b445488100e0a8335a05505405953b173ff836c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999655"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a><span data-ttu-id="cc40b-103">إنشاء عقود متقدمة للفوترة استنادًا إلى التقدم</span><span class="sxs-lookup"><span data-stu-id="cc40b-103">Create advanced contracts for billing based on progress</span></span>
[!include [banner](../includes/banner.md)]

<span data-ttu-id="cc40b-104">يشرح هذا الموضوع كيفية إنشاء عقود المشروع بحيث يمكنك إنشاء الفواتير للعملاء، استنادًا إلى النسبة المئوية للعمل المكتمل.</span><span class="sxs-lookup"><span data-stu-id="cc40b-104">This topic explains how to create project contracts so that you can create invoices for customers, based on a percentage of completed work.</span></span> <span data-ttu-id="cc40b-105">يتم حساب مبالغ الفواتير بشكل تلقائي لفئات الموازنة للعمل الذي أعددته للمشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-105">Invoice amounts are automatically calculated for the budget categories of work that you set up for a project.</span></span> <span data-ttu-id="cc40b-106">يتم تعيين توقيت الفاتورة عند التفاوض على عقد المشروع مع العميل.</span><span class="sxs-lookup"><span data-stu-id="cc40b-106">The invoice timing is set when you negotiate the project contract with the customer.</span></span>

<span data-ttu-id="cc40b-107">استخدم الإجراءات الموجودة في هذا الموضوع لإعداد عقد ومشروع مقترن وقواعد الفوترة التي تقوم بحساب مبالغ الفواتير لفئات الموازنة للعمل الذي أعددته للمشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-107">Use the procedures in this topic to set up a contract, an associated project, and the billing rules that calculate invoice amounts for the budget categories of work that you set up for the project.</span></span>

<span data-ttu-id="cc40b-108">بعد أن تنتهي من إنشاء العقد والمشروع، يمكنك إعداد التفاصيل الخاصة بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-108">After you've created the contract and the project, you can set up the details of the project.</span></span> <span data-ttu-id="cc40b-109">على سبيل المثال، يمكنك تعريف الأنشطة وتعيين عاملين للمشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-109">For example, you can define activities and assign workers to the project.</span></span>

## <a name="example"></a><span data-ttu-id="cc40b-110">مثال</span><span class="sxs-lookup"><span data-stu-id="cc40b-110">Example</span></span>

<span data-ttu-id="cc40b-111">تعمل مؤسستك في مجال تطوير البرامج.</span><span class="sxs-lookup"><span data-stu-id="cc40b-111">Your organization is a software development firm.</span></span> <span data-ttu-id="cc40b-112">أنت توافق على تطوير حزمة محاسبية لكشوف الرواتب لأحد العملاء مقابل رسم إجمالي من 20000 دولار أمريكي (USD).</span><span class="sxs-lookup"><span data-stu-id="cc40b-112">You agree to develop a payroll accounting package for a customer for a total fee of 20,000 US dollars (USD).</span></span> <span data-ttu-id="cc40b-113">توافق مؤسستك على فوترة العميل بينما تكمل نسبًا مئوية معينة من المشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-113">Your organization agrees to invoice the customer as you complete specific percentages of the project.</span></span> <span data-ttu-id="cc40b-114">يمكنك إعداد فئات المشروع التالية للعمل، بحيث يمكنك استخدامها في عملية الفوترة:</span><span class="sxs-lookup"><span data-stu-id="cc40b-114">You set up the following project categories for the work, so that you can use them in the billing process:</span></span>

- <span data-ttu-id="cc40b-115">تقديم استشارات</span><span class="sxs-lookup"><span data-stu-id="cc40b-115">Consulting</span></span>
- <span data-ttu-id="cc40b-116">تصميم</span><span class="sxs-lookup"><span data-stu-id="cc40b-116">Design</span></span>
- <span data-ttu-id="cc40b-117">التثبيت</span><span class="sxs-lookup"><span data-stu-id="cc40b-117">Installation</span></span>

<span data-ttu-id="cc40b-118">يمكنك أيضًا إعداد قواعد الفوترة التي تقوم تلقائيًا بحساب مبالغ الفواتير للنسبة المئوية من عمل المشروع المكتمل في كل فئة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-118">You also set up billing rules that automatically calculate the invoice amounts for the percentage of project work that is completed in each category.</span></span>

<span data-ttu-id="cc40b-119">يقوم مدير الموازنة بإنشاء موازنة لفئات المشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-119">The budget manager creates a budget for the project categories.</span></span> <span data-ttu-id="cc40b-120">يتم حساب مقدار العمل المكتمل بشكل تلقائي كنسبة مئوية من العمل الفعلي مقارنة بالمبالغ المدرجة بالموازنة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-120">The amount of completed work is automatically calculated as a percentage of actual work in comparison to the budgeted amounts.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc40b-121">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="cc40b-121">Prerequisites</span></span>

<span data-ttu-id="cc40b-122">قبل أن تقوم بإنشاء مشروع يستخدم قواعد الفوترة، يجب عليك إعداد التسلسلات الرقمية لقواعد الفوترة ودفتر يومية الرسوم الذي يتم استخدامه لترحيل فواتير التقدم.</span><span class="sxs-lookup"><span data-stu-id="cc40b-122">Before you create a project that uses billing rules, you must set up the number sequences for billing rules and a fee journal that is used to post progress billings.</span></span>

1. <span data-ttu-id="cc40b-123">انتقل إلى **إدارة المشاريع والمحاسبة** \> **الإعداد** \> **معلمات إدارة المشاريع والمحاسبة‬‏‫**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-123">Go to **Project management and accounting** \> **Setup** \> **Project management and accounting parameters**.</span></span>
2. <span data-ttu-id="cc40b-124">في صفحة **معلمات إدارة المشاريع والمحاسبة‬‏‫**، على علامة تبويب **التسلسلات الرقمية**، قم بإعداد التسلسلات الرقمية التي تريد استخدامها عند إنشاء قواعد الفوترة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-124">On the **Project management and accounting parameters** page, on the **Number sequences** tab, set up the number sequence that you want to use when billing rules are created.</span></span>
3. <span data-ttu-id="cc40b-125">انتقل إلى **إدارة المشاريع والمحاسبة** \> **دفاتر اليومية** \> **الرسوم**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-125">Go to **Project management and accounting** \> **Journals** \> **Fee**.</span></span>
4. <span data-ttu-id="cc40b-126">في الصفحة **دفتر يومية الرسوم**، حدد **جديد**، وأدخل اسم دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cc40b-126">On the **Fee journal** page, select **New**, and enter the journal name.</span></span>

## <a name="create-a-contract-for-progress-billings"></a><span data-ttu-id="cc40b-127">إنشاء عقد للفوترة استنادًا إلى التقدم‬</span><span class="sxs-lookup"><span data-stu-id="cc40b-127">Create a contract for progress billings</span></span>

<span data-ttu-id="cc40b-128">استخدم هذا الإجراء لإنشاء عقد مشروع لمشروع ثابت السعر.</span><span class="sxs-lookup"><span data-stu-id="cc40b-128">Use this procedure to create a project contract for a fixed-price project.</span></span> <span data-ttu-id="cc40b-129">يمكنك إنشاء فاتورة مشروع عندما يصل العمل المكتمل على المشروع إلى نسبة مئوية محددة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-129">You create a project invoice when the work that is completed on the project reaches a specified percentage.</span></span>

1. <span data-ttu-id="cc40b-130">انتقل إلى **إدارة المشاريع والمحاسبة** \> **المشاريع** \> **عقود المشروع**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-130">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="cc40b-131">من صفحة **عقود المشروع**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-131">On the **Project contracts** page, select **New**.</span></span>
3. <span data-ttu-id="cc40b-132">في مربع الحوار **عقد مشروع جديد**، عيّن الحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="cc40b-132">In the **New project contract** dialog box, set the following fields:</span></span>

    - <span data-ttu-id="cc40b-133">**الاسم**</span><span class="sxs-lookup"><span data-stu-id="cc40b-133">**Name**</span></span>
    - <span data-ttu-id="cc40b-134">**نوع التمويل**</span><span class="sxs-lookup"><span data-stu-id="cc40b-134">**Funding type**</span></span>
    - <span data-ttu-id="cc40b-135">**مصدر التمويل**</span><span class="sxs-lookup"><span data-stu-id="cc40b-135">**Funding source**</span></span>
    - <span data-ttu-id="cc40b-136">**عملة المبيعات** - بشكل افتراضي، يتم استخدام هذه العملة لفواتير العملاء المقترنة بعقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-136">**Sales currency** – By default, this currency is used for customer invoices that are associated with the project contract.</span></span> <span data-ttu-id="cc40b-137">ومع ذلك، يمكنك تغيير عملة المبيعات في فاتورة عميل محددة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-137">However, you can change the sales currency on a specific customer invoice.</span></span>

4. <span data-ttu-id="cc40b-138">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-138">Select **OK**.</span></span> <span data-ttu-id="cc40b-139">يتم نسخ المعلومات إلى رأس صفحة **عقود المشروع**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-139">The information is copied to the header of the **Project contracts** page.</span></span>
5. <span data-ttu-id="cc40b-140">في الصفحة **عقود المشروعات**، إملأ بقية المعلومات المطلوبة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-140">On the **Project contracts** page, fill in the rest of the required information for the project.</span></span>

## <a name="create-a-project-for-progress-billings"></a><span data-ttu-id="cc40b-141">إنشاء مشروع للفوترة استنادًا إلى التقدم‬</span><span class="sxs-lookup"><span data-stu-id="cc40b-141">Create a project for progress billings</span></span>

<span data-ttu-id="cc40b-142">اتبع هذه الخطوات لإنشاء مشروع وأي مشاريع فرعية مقترنة بعقد مشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-142">Follow these steps to create a project and any subprojects that are associated with a project contract.</span></span>

1. <span data-ttu-id="cc40b-143">انتقل إلى **إدارة المشاريع والمحاسبة** \> **المشاريع** \> **جميع المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-143">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="cc40b-144">من صفحة **جميع المشاريع**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-144">On the **All projects** page, select **New**.</span></span>
3. <span data-ttu-id="cc40b-145">في مربع الحوار **مشروع جديد**، في حقل **نوع المشروع**، حدد **الوقت والمواد**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-145">In the **New project** dialog box, in the **Project type** field, select **Time and material**.</span></span>
4. <span data-ttu-id="cc40b-146">حدد مجموعة مشاريع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-146">Select a project group.</span></span> <span data-ttu-id="cc40b-147">تحدد مجموعة المشاريع معلومات الترحيل للمشاريع المعينة للمجموعة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-147">A project group defines the posting information for the projects that are assigned to the group.</span></span>
5. <span data-ttu-id="cc40b-148">حدد **إنشاء مشروع**</span><span class="sxs-lookup"><span data-stu-id="cc40b-148">Select **Create project**.</span></span>
6. <span data-ttu-id="cc40b-149">بعد إنشاء المشروع، عيّن مرحلة المشروع إلى **قيد التنفيذ**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-149">After the project is created, set the project stage to **In process**.</span></span>

## <a name="create-a-budget-for-a-project"></a><span data-ttu-id="cc40b-150">إنشاء موازنة لمشروع</span><span class="sxs-lookup"><span data-stu-id="cc40b-150">Create a budget for a project</span></span>

<span data-ttu-id="cc40b-151">تُستخدم فئات الموازنة لحساب مبالغ الفواتير بشكل تلقائي للنسبة المئوية للعمل المكتمل لكل فئة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-151">Budget categories are used to automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="cc40b-152">اتبع هذه الخطوات لإنشاء فئات الموازنة للتكاليف المقدرة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-152">Follow these steps to create budget categories for the estimated costs.</span></span>

1. <span data-ttu-id="cc40b-153">انتقل إلى **إدارة المشاريع والمحاسبة** \> **المشاريع** \> **جميع المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-153">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="cc40b-154">في صفحة **جميع المشاريع**، حدد المشروع المطلوب وافتحه.</span><span class="sxs-lookup"><span data-stu-id="cc40b-154">On the **All projects** page, select and open the project that you want.</span></span>
3. <span data-ttu-id="cc40b-155">من صفحة **المشاريع**، في جزء الإجراءات، ضمن علامة تبويب **الخطة** في مجموعة **الموازنة**، حدد **موازنة المشروع**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-155">On the **Projects** page, on the Action Pane, on the **Plan** tab, in the **Budget** group, select **Project budget**.</span></span>
4. <span data-ttu-id="cc40b-156">من صفحة **موازنة المشروع**، أدخل التكلفة المقدرة لكل فئة في المشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-156">On the **Project budget** page, enter an estimated cost for each category in the project.</span></span>

## <a name="create-billing-rules-for-progress-billings"></a><span data-ttu-id="cc40b-157">إنشاء قواعد الفوترة للفوترة استنادًا إلى التقدم‬‬</span><span class="sxs-lookup"><span data-stu-id="cc40b-157">Create billing rules for progress billings</span></span>

1. <span data-ttu-id="cc40b-158">انتقل إلى **إدارة المشاريع والمحاسبة** \> **المشاريع** \> **عقود المشروع**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-158">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="cc40b-159">في صفحة **عقود المشروع**، حدد عقد مشروع، ثم افتحه.</span><span class="sxs-lookup"><span data-stu-id="cc40b-159">On the **Project contracts** page, select and open a project contract.</span></span>
3. <span data-ttu-id="cc40b-160">في صفحة عقود المشروع، على علامة التبويب السريعة **قواعد الفوترة**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-160">On the project contract page, on the **Billing rules** FastTab, select **Add**.</span></span>
4. <span data-ttu-id="cc40b-161">في صفحة **قاعدة الفوترة**، في حقل **نوع البند**، حدد **التقدم**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-161">On the **Billing rule** page, in the **Line type** field, select **Progress**.</span></span>
5. <span data-ttu-id="cc40b-162">على علامة التبويب السريعة **تفاصيل بنود قاعدة الفوترة**، في الحقل **قيمة العقد**، أدخل القيمة الإجمالية للعقد.</span><span class="sxs-lookup"><span data-stu-id="cc40b-162">On the **Billing rule line details** FastTab, in the **Contract value** field, enter the total value of the contract.</span></span>
6. <span data-ttu-id="cc40b-163">في الحقل **الفئة**، حدد الفئة المراد ترحيل حركة الرسوم اليها.</span><span class="sxs-lookup"><span data-stu-id="cc40b-163">In the **Category** field, select the category to post the fee transaction to.</span></span>
7. <span data-ttu-id="cc40b-164">في الحقل **المشروع**، حدد المشروع الذي يستخدم قاعدة الفوترة هذه.</span><span class="sxs-lookup"><span data-stu-id="cc40b-164">In the **Project** field, select the project that uses this billing rule.</span></span>
8. <span data-ttu-id="cc40b-165">اختياري: قم بتعيين قاعدة الفوترة إلى المشروعات الإضافية.</span><span class="sxs-lookup"><span data-stu-id="cc40b-165">Optional: Assign the billing rule to additional projects.</span></span> <span data-ttu-id="cc40b-166">على علامة التبويب السريعة **المشروع**، في قسم **المشاريع المتوفرة**، حدد مشروعًا، ثم حدد زر السهم الأيمن لإضافة المشروع إلى قسم **المشاريع المحددة**.</span><span class="sxs-lookup"><span data-stu-id="cc40b-166">On the **Project** FastTab, in the **Available projects** section, select a project, and then select the right arrow button to add the project to the **Selected projects** section.</span></span>
9. <span data-ttu-id="cc40b-167">اختياري: احسب مبلغ النسبة المئوية التي يحتجزها العميل من الدفعات على الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="cc40b-167">Optional: Calculate the percentage amount that the customer withholds from payments on an invoice.</span></span> <span data-ttu-id="cc40b-168">على علامة التبويب السريعة **شروط احتجاز الدفع**، حدد مصدر التمويل، ثم في الحقل **النسبة المئوية للاحتجاز**، أدخل النسبة المئوية للاحتجاز.</span><span class="sxs-lookup"><span data-stu-id="cc40b-168">On the **Payment retention terms** FastTab, select the funding source, and then, in the **Retention percentage** field, enter the retention percentage.</span></span>
10. <span data-ttu-id="cc40b-169">كرر هذه الخطوات لإنشاء قواعد فوترة إضافية لعقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="cc40b-169">Repeat these steps to create additional billing rules for the project contract.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]