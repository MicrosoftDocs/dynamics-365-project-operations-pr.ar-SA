---
title: إدارة قوائم أسعار المشروع على عقود المشروع
description: يقدم هذا الموضوع معلومات حول إدارة قوائم أسعار المشروع على عقود المشروع.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3313eef74b5e7a0624b32d2a336cd986dfdda839
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010365"
---
# <a name="manage-project-price-lists-on-project-contracts"></a><span data-ttu-id="32899-103">إدارة قوائم أسعار المشروع على عقود المشروع</span><span class="sxs-lookup"><span data-stu-id="32899-103">Manage project price lists on project contracts</span></span>

<span data-ttu-id="32899-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="32899-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="32899-105">تم تصميم عقود المشروع في Dynamics 365 Project Operations لدعم قوائم أسعار المبيعات متعددة السريان على أحد العقود.</span><span class="sxs-lookup"><span data-stu-id="32899-105">Project contracts in Dynamics 365 Project Operations are designed to support multiple date effective sales price lists on a contract.</span></span> <span data-ttu-id="32899-106">في Project Operations، يوجد كيان جديد مقترن يسمى **قوائم أسعار المشروع**.</span><span class="sxs-lookup"><span data-stu-id="32899-106">In Project Operations, there is a new associated entity called **Project Price Lists**.</span></span> <span data-ttu-id="32899-107">توجد في هذا الكيان علاقة واحد إلى متعدد بعقد مشروع.</span><span class="sxs-lookup"><span data-stu-id="32899-107">This entity has a one-to-many relationship to a project contract.</span></span>

<span data-ttu-id="32899-108">تُستخدم قوائم أسعار المشروع لتسعير حركات الوقت والمواد والمصروفات على مشروع.</span><span class="sxs-lookup"><span data-stu-id="32899-108">Project price lists are used to price time, material, and expense transactions on a project.</span></span> <span data-ttu-id="32899-109">عندما يتضمن العقد قائمة أسعار مشروع واحدة أو أكثر، يتم استخدام قوائم الأسعار هذه لتسعير الوقت والمواد وتقديرات المصاريف والقيم الفعلية على المشاريع المقترنة بالعقد من خلال شروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="32899-109">When a contract has one or more project price lists, these price lists are used to price for time, material, expense estimates, and actuals on projects that are associated to the contract through the contract line.</span></span>

<span data-ttu-id="32899-110">في حالة عدم وجود قوائم أسعار مشروع في عقد مشروع، تظهر لك رسالة تحذير تشير إلى عدم وجود قوائم أسعار مشروع ولن يتم تسعير تقديراتك وعمل المشروع الفعلي والمصروفات المسجلة.</span><span class="sxs-lookup"><span data-stu-id="32899-110">When there are no project price lists on a project contract, you will see a warning message that there are no project price lists and your estimates, actual project work, material, and expenses logged will not be priced.</span></span> <span data-ttu-id="32899-111">لن يكون هناك أي سعر لقيم المبيعات.</span><span class="sxs-lookup"><span data-stu-id="32899-111">There will be no price for sales values.</span></span>

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a><span data-ttu-id="32899-112">إقران قائمه أسعار  مشروع على عقد مشروع أو إلغاء إقرانها</span><span class="sxs-lookup"><span data-stu-id="32899-112">Associate or unassociate a project price list on a project contract</span></span>

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-material-and-expenses"></a><span data-ttu-id="32899-113">إنشاء قائمة أسعار معينة أو إقرانها لتقدير العمل والمواد والمصروفات المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="32899-113">Create or associate a specific price list for estimating project-based work, material, and expenses</span></span>

1. <span data-ttu-id="32899-114">في عقد المشروع، حدد علامة التبويب **قوائم أسعار المشروع**.</span><span class="sxs-lookup"><span data-stu-id="32899-114">On the project contract, select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="32899-115">في الشبكة الفرعية، حدد **حدد + إضافة قائمة أسعار مشروع جديدة**.</span><span class="sxs-lookup"><span data-stu-id="32899-115">In the subgrid, select **+ Add New Project Price List**.</span></span>
3. <span data-ttu-id="32899-116">علي شريط تمرير **الإنشاء السريع**، حدد قائمة أسعار.</span><span class="sxs-lookup"><span data-stu-id="32899-116">On the **Quick Create** slider, select a price list.</span></span> 

  <span data-ttu-id="32899-117">تعرض القائمة المنسدلة كافة قوائم الأسعار التي تم تعيين السياق لها إلى **المبيعات**، حيث تتطابق العملة على قائمة الأسعار مع العملة على العقد.</span><span class="sxs-lookup"><span data-stu-id="32899-117">The drop-down list shows all price lists that have the context set to **Sales**, where the currency on the price list matches the currency on the contract.</span></span>
  
4. <span data-ttu-id="32899-118">أدخل وصفًا لاقتران قائمة أسعار المشروع، وحدد **حفظ**، ثم أغلق شريط تمرير **الإنشاء السريع**.</span><span class="sxs-lookup"><span data-stu-id="32899-118">Enter a description for the project price list association, select **Save**, and then close the **Quick Create** slider.</span></span>

   <span data-ttu-id="32899-119">يتم إنشاء اقتران قائمة أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="32899-119">A project price list association is created.</span></span>
   
5. <span data-ttu-id="32899-120">كرر الخطوات من 1 إلى 4 لإقران أكثر من قائمة أسعار مشروع واحدة بعقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="32899-120">Repeat steps 1-4 to associate more than one project price list to the project contract.</span></span> <span data-ttu-id="32899-121">أنشئ قوائم أسعار مشروع متعددة فقط إذا كان سريان التاريخ يختلف على كل قائمة أسعار مشروع مقترنة.</span><span class="sxs-lookup"><span data-stu-id="32899-121">Only create multiple project price lists if you have different date effectivity on each of the associated project price list.</span></span>

> [!NOTE]
> <span data-ttu-id="32899-122">لا يدعم Project Operations تداخل سريان تاريخ قوائم أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="32899-122">Project Operations doesn't support overlapping the date effectivity of the project price lists.</span></span> <span data-ttu-id="32899-123">عند وجود قوائم أسعار مشروع متعددة لحركة بتاريخ محدد، سيتم تعيين السعر في هذه الحركة إلى صفر بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="32899-123">If there are multiple project prices lists for a transaction with a given date, the price on that transaction will be defaulted to zero.</span></span>

### <a name="remove-a-project-price-list-association"></a><span data-ttu-id="32899-124">إزالة اقتران قائمة أسعار المشروع</span><span class="sxs-lookup"><span data-stu-id="32899-124">Remove a project price list association</span></span>

- <span data-ttu-id="32899-125">حدد قائمة أسعار المشروع، ثم حدد **حذف قائمة أسعار مشروع العقد** على الشبكة الفرعية.</span><span class="sxs-lookup"><span data-stu-id="32899-125">Select the project price list, and then select **Delete Contract Project Price List** on the subgrid.</span></span> 

  <span data-ttu-id="32899-126">تُزال قائمة الأسعار من قوائم أسعار المشروع في العقد.</span><span class="sxs-lookup"><span data-stu-id="32899-126">The price list is removed from the project price lists on the contract.</span></span> <span data-ttu-id="32899-127">لن يتم حذف قائمة الأسعار بحد ذاتها.</span><span class="sxs-lookup"><span data-stu-id="32899-127">The price list itself will not be deleted.</span></span> <span data-ttu-id="32899-128">سيتم حذف الاقتران بالعقد فقط.</span><span class="sxs-lookup"><span data-stu-id="32899-128">Only the association to the contract will be deleted.</span></span>

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a><span data-ttu-id="32899-129">إعداد تعيين قوائم أسعار المشروع على عقد إلى قوائم الأسعار الافتراضية بشكل تلقائي</span><span class="sxs-lookup"><span data-stu-id="32899-129">Set up automatic defaulting of project price lists on a contract</span></span>

<span data-ttu-id="32899-130">يمكن إعداد قائمة أسعار مشروع كقائمة الأسعار الافتراضية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="32899-130">A project price list can be set up as the default project price list.</span></span> <span data-ttu-id="32899-131">يضمن هذا الإعداد أن تبدأ دائمًا كافة العقود في مؤسستك بقائمة أسعار مشروع قياسية لفترة الأسعار هذه.</span><span class="sxs-lookup"><span data-stu-id="32899-131">This setup ensures that all contracts in your organization always start with a standard project price list for that price period.</span></span>

### <a name="set-up-the-organizational-default-for-project-price-lists"></a><span data-ttu-id="32899-132">إعداد التعيين الافتراضي التنظيمي لقوائم أسعار المشروع</span><span class="sxs-lookup"><span data-stu-id="32899-132">Set up the organizational default for project price lists</span></span>

1. <span data-ttu-id="32899-133">انتقل إلى **الإعدادات** > **عام**، ثم حدد **المعلمات**.</span><span class="sxs-lookup"><span data-stu-id="32899-133">Go to **Settings** > **General**, and then select **Parameters**.</span></span>
2. <span data-ttu-id="32899-134">في صفحة قائمة **المعلمات النشطة**، حدد ثم انقر نقرًا مزدوجًا فوق السجل لفتحه.</span><span class="sxs-lookup"><span data-stu-id="32899-134">In the **Active Parameters** list page, select and double-click the record to open it.</span></span> <span data-ttu-id="32899-135">أثناء النقر المزدوج، تأكد من أنك لا تنقر فوق قيمة حقل هي عبارة عن ارتباط تشعبي.</span><span class="sxs-lookup"><span data-stu-id="32899-135">While double–clicking, make sure that you are not clicking on a field value that is hyperlink.</span></span> 
3. <span data-ttu-id="32899-136">في صفحة **المعلمات النشطة**، حدد علامة التبويب **قائمة الأسعار**. تعرض شبكة فرعية قائمة بقوائم الأسعار الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="32899-136">On the **Active Parameters** page, select the **Price List** tab. A subgrid shows a list of default price lists.</span></span> <span data-ttu-id="32899-137">هذه قائمة تتضمن قوائم أسعار المبيعات والتكلفة القياسية.</span><span class="sxs-lookup"><span data-stu-id="32899-137">This is a list of standard cost and sales price lists.</span></span> <span data-ttu-id="32899-138">يضمن وجود قائمة أسعار **مبيعات** مقترنة هنا لكل عملة تقوم ببيعها أن تكون قائمة أسعار المبيعات قائمة الأسعار الافتراضية على كل عقد تقوم بإنشائه للعملاء الذين يتعاملون بهذه العملة.</span><span class="sxs-lookup"><span data-stu-id="32899-138">Having a **Sales** price list associated here for every currency that you sell in ensures that the sales price list is the default on any contract that you create for customers that transact in this currency.</span></span>

### <a name="set-up-a-customer-specific-project-price-list"></a><span data-ttu-id="32899-139">إعداد قائمه أسعار مشروع خاصة بالعميل</span><span class="sxs-lookup"><span data-stu-id="32899-139">Set up a customer-specific project price list</span></span>

<span data-ttu-id="32899-140">يمكنك أيضًا إعداد قوائم أسعار مشروع خاصة بالعميل عندما تتفاوض على اتفاقية تسعير رئيسية مع العملاء.</span><span class="sxs-lookup"><span data-stu-id="32899-140">You can also set up customer–specific project price lists when you have negotiated a master pricing agreement with your customers.</span></span>

1. <span data-ttu-id="32899-141">انتقل إلى **المبيعات** > **العملاء**.</span><span class="sxs-lookup"><span data-stu-id="32899-141">Go to **Sales** > **Customers**.</span></span>
2. <span data-ttu-id="32899-142">من قائمة الحسابات النشطة، حدد العميل الذي حصلت منه على قائمة أسعار خاصة.</span><span class="sxs-lookup"><span data-stu-id="32899-142">From the list of active accounts, select the customer for whom have special price list.</span></span>
3. <span data-ttu-id="32899-143">حدد سجل العميل لفتحه، ثم حدد علامة التبويب **قوائم أسعار المشروع**. تعرض شبكة فرعية قائمة بقوائم أسعار المشروع الخاصة بهذا العميل.</span><span class="sxs-lookup"><span data-stu-id="32899-143">Select the customer record to open it and then select the **Project Price Lists** tab. A subgrid shows a list of project price lists specific to this customer.</span></span> 
4. <span data-ttu-id="32899-144">أنشئ اقتران قائمة أسعار جديدة هنا لجعل قائمة أسعار المشروع خاصة بهذا العميل.</span><span class="sxs-lookup"><span data-stu-id="32899-144">Create a new price list association here to have project price list specific to this customer.</span></span>

## <a name="custom-pricing-on-a-project-contract"></a><span data-ttu-id="32899-145">التسعير المخصص على عقد مشروع</span><span class="sxs-lookup"><span data-stu-id="32899-145">Custom pricing on a project contract</span></span>

<span data-ttu-id="32899-146">بعد حصولك على قوائم أسعار مشروع افتراضية خاصة بالعميل والمؤسسة، سيتم إنشاء عقود المشروع مع اقترانات قوائم أسعار المشروع هذه بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="32899-146">After you have organizational and customer-specific default project price lists, your project contracts will be created with these project price list associations automatically.</span></span> <span data-ttu-id="32899-147">ولكن يتم دائمًا نسخ قوائم أسعار المشروع على عقد المشروع مع إلحاق التاريخ واسم العقد بها.</span><span class="sxs-lookup"><span data-stu-id="32899-147">However, project price lists on a project contract are always copied with the date and contract name appended to them.</span></span> <span data-ttu-id="32899-148">عندئذٍ، يمكن لمدراء الحسابات والمشاريع بدء عمليات تحرير على هذه النُسخ.</span><span class="sxs-lookup"><span data-stu-id="32899-148">The account and project managers can then begin making edits to prices on these copies.</span></span> <span data-ttu-id="32899-149">ستنطبق هذه الأسعار المتغيرة على عقد المشروع هذا فقط.</span><span class="sxs-lookup"><span data-stu-id="32899-149">These changed prices will be applicable to this project contract only.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
