---
title: تصحيحات مجمعة للقيم الفعلية التي تم إنشاؤها بواسطة إدخالات الوقت والمصروفات الموافق عليها
description: يشرح هذه الموضوع كيف يمكن للمسؤول إجراء تصحيحات فردية أو مجمعة لإدخالات الوقت أو المصروفات التي تمت الموافقة عليها في السابق إذا لم تكن الفوترة مكتملة.
author: rumant
manager: AnnBe
ms.date: 04/02/2020
ms.topic: article
ms.service: dynamics-ax-applications
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
search.app:
- ProjectOperations
ms.openlocfilehash: 6d6c03cc74d47ca3ae7c2bd7d0aa0720bb2f3c01
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070820"
---
# <a name="bulk-corrections-of-actuals-created-by-approved-time-and-expense-entries"></a><span data-ttu-id="8bdc8-103">تصحيحات مجمعة للقيم الفعلية التي تم إنشاؤها بواسطة إدخالات الوقت والمصروفات الموافق عليها</span><span class="sxs-lookup"><span data-stu-id="8bdc8-103">Bulk corrections of actuals created by approved time and expense entries</span></span>

<span data-ttu-id="8bdc8-104">في بعض الأحيان، قد يتم إدخال إدخالات الوقت أو المصروفات بشكل غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-104">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="8bdc8-105">على سبيل المثال، قد يحدد أحد المستشارين تاريخًا صحيح عند إنشاء إدخال الوقت أو قد يقوم بتبديل الأرقام عند إدخال المصروفات.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-105">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="8bdc8-106">إذا تعذر على المستشار إجراء التحديثات على الإدخالات المقدمة، فبإمكان المسؤول أي يصحح الإدخال مباشرة لمشروع ما.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-106">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="8bdc8-107">لإكمال الإجراءات الواردة في هذا الموضوع، ستحتاج إلى أذونات المسؤول.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-107">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="8bdc8-108">تصحيح إدخالات الوقت الموافق عليها</span><span class="sxs-lookup"><span data-stu-id="8bdc8-108">Correct approved time entries</span></span>     

<span data-ttu-id="8bdc8-109">أكمل الخطوات التالية لتصحيح إدخالات وقت فردية أو متعددة لمشروع.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-109">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="8bdc8-110">في منطقة **المبيعات** ، حدد **المعاملات‬** ، ثم حدد **الوقت الموافق عليه‬**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-110">In the **Sales** area, select **Transactions** , and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="8bdc8-111">في قائمة **الوقت الموافق عليه‬** ، حدد موقع إدخال وقت أو أكثر تمت الموافقة عليها يجب تصحيحه.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-111">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="8bdc8-112">يمكنك استخدام عامل التصفية لتحديد موقع الإدخالات ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-112">You can use the filter to locate related entries.</span></span> <span data-ttu-id="8bdc8-113">على سبيل المثال، يمكنك إجراء التصفية حسب معرف المشروع، وتحديد جميع إدخالات الوقت الموافق عليها لمعرف المشروع هذا.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-113">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="8bdc8-114">حدد **تصحيح الإدخالات**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-114">Select **Correct entries**.</span></span> <span data-ttu-id="8bdc8-115">يتم إنشاء دفتر يومية تصحيح جديد تلقائيًا ، مع النوع المعين **تصحيح الوقت**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-115">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="8bdc8-116">تُضاف الإدخالات التي حددتها إلى دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-116">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="8bdc8-117">في الصفحة **دفتر يومية جديد** ، أدخل **وصفاً** لدفتر يومية التصحيح، ثم حدد علامة التبويب **تصحيحات إدخال الوقت**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-117">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  
5. <span data-ttu-id="8bdc8-118">في القسم **القيم الجديدة لإدخالات الوقت** ، قم بتحديث الحقول بواسطة المعلومات الصحيحة كما تقتضي الحاجة.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-118">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="8bdc8-119">على سبيل المثال، يمكنك تغيير المشروع المعين أو المورد القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-119">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="8bdc8-120">حدد **معاينة**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-120">Select **Preview**.</span></span> <span data-ttu-id="8bdc8-121">في مربع الحوار ، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-121">In the dialog box, select **OK**.</span></span> <span data-ttu-id="8bdc8-122">على علامة التبويب‏‎ **أسطر دفتر اليومية** ، يمكنك عرض قائمة بالقيم الفعلية الأصلية المرتبطة بإدخالات الوقت المحددة التي تم إلغاؤها والبنود المقابلة التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-122">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="8bdc8-123">كرر الخطوتين 5 و6 إن كان هناك حاجة إلى إجراء تصحيحات إضافية.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-123">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="8bdc8-124">ستكون لدى جميع القيم الفعلية التي تم تصحيحها القيم نفسها التي حددتها في القسم **القيم الجديدة لإدخالات الوقت‬**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-124">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="8bdc8-125">إذا ظهرت التصحيحات كما هو متوقع‏‎، فحدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-125">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="8bdc8-126">في مربع الحوار ، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-126">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="8bdc8-127">عد إلى منطقة **المبيعات** ، وحدد **المشاريع** ، ثم افتح المشروع الذي قمت بتحديث إدخالات الوقت له.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-127">Return to the **Sales** area, select **Projects** , and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="8bdc8-128">في صفحة **المشاريع** ، على علامة تبويب **القيم الفعلية** ، استعرض التغييرات التي قمت بها.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-128">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="8bdc8-129">إذا لم تظهر علام تبويب **القيم الفعلية** ، فحدد **ذو صلة** > **القيم الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-129">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="8bdc8-130">في القائمة **طريقة العرض المقترنة الفعلية‬** ، يمكنك أن ترى أن إدخالات الوقت الأصلية الملغاة ما زالت مدرجة، كما هو الحال مع إدخالات الوقت المناظرة التي تم تصحيحها.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-130">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="8bdc8-131">على سبيل المثال، في الرسم التالي، هناك بندان لديهما كمية 8.00 وأرصدة دائنة مدرجة في عمود المبلغ.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-131">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="8bdc8-132">علاوةً على ذلك، هناك بندان لديهما كمية من-8.00 ويعرضان مبالغ مضافة إلى الرصيد في عمود المبلغ.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-132">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="8bdc8-133">تؤدي هذه التصحيحات إلى جعل الكمية صفرية.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-133">These corrections bring the quantity to zero.</span></span>

![طريقة العرض المقترنة الفعلية](https://github.com/MicrosoftDocs/dynamics-365-customer-engagement-pr/blob/bulk-corrections-actuals-created-by-approved-time-expense-entries.md/time-actuals.png)
 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="8bdc8-135">تصحيح إدخالات المصروفات الموافق عليها</span><span class="sxs-lookup"><span data-stu-id="8bdc8-135">Correct approved expense entries</span></span>

<span data-ttu-id="8bdc8-136">أكمل الخطوات التالية لتصحيح واحد أو أكثر من إدخالات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="8bdc8-137">في منطقة **المبيعات** ، في جزء التنقل الأيمن، ضمن **المعاملات** ، حدد **المصروفات الموافق عليها‬**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-137">In the **Sales** area, in the left navigation pane, under **Transactions** , select **Approved Expenses**.</span></span>

2. <span data-ttu-id="8bdc8-138">في قائمة **المصروفات الموافق عليها‬** ، حدد المشروع الذي تريد تصحيحه، ثم حدد **تصحيح الإدخالات**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="8bdc8-139">سيتم إنشاء دفتر يومية تصحيح جديد تلقائيًا ، مع النوع المعين **تصحيح المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="8bdc8-140">في الصفحة **دفتر يومية جديد** ، أدخل **وصفًا** للتصحيح، وعلى علامة التبويب **تصحيح المصروفات** في القسم **القيم الجديدة للمصروفات‬** ، حدد حقول البيانات التي تريد تصحيحها لبند المصروفات المحدد.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="8bdc8-141">على سبيل المثال، يمكنك تعيين المصروفات إلى **مشروع** آخرـ أو تصحيح **فئة المصروفات** أو **تاريخ المصروفات** أو **المورد القابل للحجز**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-141">For example, you can assign the expense to another **Project** , or correct the **Expense Category** , **Expense Date** , or **Bookable Resource**.</span></span>

4. <span data-ttu-id="8bdc8-142">حدد **معاينة**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-142">Select **Preview**.</span></span> <span data-ttu-id="8bdc8-143">في مربع الحوار ، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="8bdc8-144">تحقق من التصحيحات على علامة التبويب‏‎ **أسطر دفتر اليومية**. يمكنك عرض قائمة بالقيم الفعلية الأصلية المرتبطة بإدخالات المصروفات المحددة التي تم إلغاؤها والبنود المقابلة التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="8bdc8-145">إذا كانت القيم الصحيحة كما هو متوقع‏‎، فحدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="8bdc8-146">في مربع الحوار ، حدد **موافق.**</span><span class="sxs-lookup"><span data-stu-id="8bdc8-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="8bdc8-147">إذا لم تظهر القيم كما هو متوقع، فحدد‏‎ **إلغاء** للعودة إلى قائمة **المصروفات الموافق عليها**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="8bdc8-148">كرر الخطوات من 2 إلى 5.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="8bdc8-149">ستكون لدى القيم الفعلية التي تم تصحيحها القيم نفسها التي حددتها في القسم **القيم الجديدة لإدخالات المصروفات‬**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="8bdc8-150">بعد التأكد دفتر يومية التصحيح، عد إلى المشروع (المشاريع) الذي قمت بتحديثه لاستعراض تغييراتك.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="8bdc8-151">في صفحة المشروع، على علامة تبويب **القيم الفعلية** ، راجع **طريقة العرض المقترنة الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="8bdc8-152">في طريقة العرض هذه، تكون الإدخالات الأصلية والإدخالات المصححة مدرجة.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="8bdc8-153">يوضح الرسم التالي مبالغ إدخالات المصروفات الأصلية ومبالغ إدخالات المصروفات المصححة المناظرة.</span><span class="sxs-lookup"><span data-stu-id="8bdc8-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 

![القيم الفعلية للمصروفات](https://user-images.githubusercontent.com/60806505/77122219-4cd52900-69fa-11ea-8349-ccd2ffebf640.png)
