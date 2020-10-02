---
title: إنشاء دفاتر يومية التصحيح وتأكيدها
description: يقدم هذا الموضوع معلومات عن كيفية إنشاء دفاتر يومية التصحيح وتأكيدها.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 274f99527804b0db81b26201a22eb5a8cbe86c9a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896940"
---
# <a name="create-and-confirm-correction-journals"></a><span data-ttu-id="cf7fb-103">إنشاء دفاتر يومية التصحيح وتأكيدها</span><span class="sxs-lookup"><span data-stu-id="cf7fb-103">Create and confirm Correction journals</span></span>

<span data-ttu-id="cf7fb-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="cf7fb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cf7fb-105">في بعض الأحيان، قد يتم إدخال إدخالات الوقت أو المصروفات بشكل غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-105">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="cf7fb-106">على سبيل المثال، قد يحدد أحد المستشارين تاريخًا صحيح عند إنشاء إدخال الوقت أو قد يقوم بتبديل الأرقام عند إدخال المصروفات.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-106">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="cf7fb-107">إذا تعذر على المستشار إجراء التحديثات على الإدخالات المقدمة، فبإمكان المسؤول أي يصحح الإدخال مباشرة لمشروع ما.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-107">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="cf7fb-108">لإكمال الإجراءات الواردة في هذا الموضوع، ستحتاج إلى أذونات المسؤول.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-108">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="cf7fb-109">تصحيح إدخالات الوقت الموافق عليها</span><span class="sxs-lookup"><span data-stu-id="cf7fb-109">Correct approved time entries</span></span>     

<span data-ttu-id="cf7fb-110">أكمل الخطوات التالية لتصحيح إدخالات وقت فردية أو متعددة لمشروع.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-110">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="cf7fb-111">في منطقة **المبيعات**، حدد **المعاملات‬**، ثم حدد **الوقت الموافق عليه‬**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-111">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="cf7fb-112">في قائمة **الوقت الموافق عليه‬**، حدد موقع إدخال وقت أو أكثر تمت الموافقة عليها يجب تصحيحه.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-112">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="cf7fb-113">يمكنك استخدام عامل التصفية لتحديد موقع الإدخالات ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-113">You can use the filter to locate related entries.</span></span> <span data-ttu-id="cf7fb-114">على سبيل المثال، يمكنك إجراء التصفية حسب معرف المشروع، وتحديد جميع إدخالات الوقت الموافق عليها لمعرف المشروع هذا.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-114">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="cf7fb-115">حدد **تصحيح الإدخالات**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-115">Select **Correct entries**.</span></span> <span data-ttu-id="cf7fb-116">يتم إنشاء دفتر يومية تصحيح جديد تلقائيًا ، مع النوع المعين **تصحيح الوقت**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-116">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="cf7fb-117">تُضاف الإدخالات التي حددتها إلى دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-117">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="cf7fb-118">في الصفحة **دفتر يومية جديد**، أدخل **وصفاً** لدفتر يومية التصحيح، ثم حدد علامة التبويب **تصحيحات إدخال الوقت**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-118">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  

5. <span data-ttu-id="cf7fb-119">في القسم **القيم الجديدة لإدخالات الوقت**، قم بتحديث الحقول بواسطة المعلومات الصحيحة كما تقتضي الحاجة.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-119">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="cf7fb-120">على سبيل المثال، يمكنك تغيير المشروع المعين أو المورد القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-120">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="cf7fb-121">حدد **معاينة**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-121">Select **Preview**.</span></span> <span data-ttu-id="cf7fb-122">في مربع الحوار ، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-122">In the dialog box, select **OK**.</span></span> <span data-ttu-id="cf7fb-123">على علامة التبويب‏‎ **أسطر دفتر اليومية** ، يمكنك عرض قائمة بالقيم الفعلية الأصلية المرتبطة بإدخالات الوقت المحددة التي تم إلغاؤها والبنود المقابلة التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-123">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="cf7fb-124">كرر الخطوتين 5 و6 إن كان هناك حاجة إلى إجراء تصحيحات إضافية.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-124">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="cf7fb-125">ستكون لدى جميع القيم الفعلية التي تم تصحيحها القيم نفسها التي حددتها في القسم **القيم الجديدة لإدخالات الوقت‬**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-125">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="cf7fb-126">إذا ظهرت التصحيحات كما هو متوقع‏‎، فحدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-126">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="cf7fb-127">في مربع الحوار ، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-127">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="cf7fb-128">عد إلى منطقة **المبيعات**، وحدد **المشاريع**، ثم افتح المشروع الذي قمت بتحديث إدخالات الوقت له.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-128">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="cf7fb-129">في صفحة **المشاريع**، على علامة تبويب **القيم الفعلية**، استعرض التغييرات التي قمت بها.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-129">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="cf7fb-130">إذا لم تظهر علام تبويب **القيم الفعلية**، فحدد **ذو صلة** > **القيم الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-130">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="cf7fb-131">في القائمة **طريقة العرض المقترنة الفعلية‬**، يمكنك أن ترى أن إدخالات الوقت الأصلية الملغاة ما زالت مدرجة، كما هو الحال مع إدخالات الوقت المناظرة التي تم تصحيحها.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-131">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="cf7fb-132">على سبيل المثال، في الرسم التالي، هناك بندان لديهما كمية 8.00 وأرصدة دائنة مدرجة في عمود المبلغ.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-132">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="cf7fb-133">علاوةً على ذلك، هناك بندان لديهما كمية من-8.00 ويعرضان مبالغ مضافة إلى الرصيد في عمود المبلغ.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-133">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="cf7fb-134">تؤدي هذه التصحيحات إلى جعل الكمية صفرية.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-134">These corrections bring the quantity to zero.</span></span>

 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="cf7fb-135">تصحيح إدخالات المصروفات الموافق عليها</span><span class="sxs-lookup"><span data-stu-id="cf7fb-135">Correct approved expense entries</span></span>

<span data-ttu-id="cf7fb-136">أكمل الخطوات التالية لتصحيح واحد أو أكثر من إدخالات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="cf7fb-137">في منطقة **المبيعات**، في جزء التنقل الأيمن، ضمن **المعاملات**، حدد **المصروفات الموافق عليها‬**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="cf7fb-138">في قائمة **المصروفات الموافق عليها‬**، حدد المشروع الذي تريد تصحيحه، ثم حدد **تصحيح الإدخالات**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="cf7fb-139">سيتم إنشاء دفتر يومية تصحيح جديد تلقائيًا ، مع النوع المعين **تصحيح المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="cf7fb-140">في الصفحة **دفتر يومية جديد**، أدخل **وصفًا** للتصحيح، وعلى علامة التبويب **تصحيح المصروفات** في القسم **القيم الجديدة للمصروفات‬**، حدد حقول البيانات التي تريد تصحيحها لبند المصروفات المحدد.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="cf7fb-141">على سبيل المثال، يمكنك تعيين المصروفات إلى **مشروع** آخرـ أو تصحيح**فئة المصروفات** أو **تاريخ المصروفات** أو **المورد القابل للحجز**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="cf7fb-142">حدد **معاينة**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-142">Select **Preview**.</span></span> <span data-ttu-id="cf7fb-143">في مربع الحوار ، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="cf7fb-144">تحقق من التصحيحات على علامة التبويب‏‎ **أسطر دفتر اليومية**. يمكنك عرض قائمة بالقيم الفعلية الأصلية المرتبطة بإدخالات المصروفات المحددة التي تم إلغاؤها والبنود المقابلة التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="cf7fb-145">إذا كانت القيم الصحيحة كما هو متوقع‏‎، فحدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="cf7fb-146">في مربع الحوار ، حدد **موافق.**</span><span class="sxs-lookup"><span data-stu-id="cf7fb-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="cf7fb-147">إذا لم تظهر القيم كما هو متوقع، فحدد‏‎ **إلغاء** للعودة إلى قائمة **المصروفات الموافق عليها**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="cf7fb-148">كرر الخطوات من 2 إلى 5.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="cf7fb-149">ستكون لدى القيم الفعلية التي تم تصحيحها القيم نفسها التي حددتها في القسم **القيم الجديدة لإدخالات المصروفات‬**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="cf7fb-150">بعد التأكد دفتر يومية التصحيح، عد إلى المشروع (المشاريع) الذي قمت بتحديثه لاستعراض تغييراتك.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="cf7fb-151">في صفحة المشروع، على علامة تبويب **القيم الفعلية**، راجع **طريقة العرض المقترنة الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="cf7fb-152">في طريقة العرض هذه، تكون الإدخالات الأصلية والإدخالات المصححة مدرجة.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="cf7fb-153">يوضح الرسم التالي مبالغ إدخالات المصروفات الأصلية ومبالغ إدخالات المصروفات المصححة المناظرة.</span><span class="sxs-lookup"><span data-stu-id="cf7fb-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 


