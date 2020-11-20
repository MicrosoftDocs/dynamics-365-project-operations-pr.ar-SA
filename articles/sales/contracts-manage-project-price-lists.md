---
title: إدارة قوائم أسعار المشروع على عقود المشروع
description: يقدم هذا الموضوع معلومات حول إدارة قوائم أسعار المشروع على عقود المشروع.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 030684576e1f53d27921907b07c9e5e0c5efe612
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4133265"
---
# <a name="manage-project-price-lists-on-project-contracts"></a><span data-ttu-id="3f6b6-103">إدارة قوائم أسعار المشروع على عقود المشروع</span><span class="sxs-lookup"><span data-stu-id="3f6b6-103">Manage project price lists on project contracts</span></span>

<span data-ttu-id="3f6b6-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="3f6b6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3f6b6-105">تم تصميم عقود المشروع في Dynamics 365 Project Operations لدعم قوائم أسعار المبيعات متعددة السريان على أحد العقود.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-105">Project contracts in Dynamics 365 Project Operations are designed to support multiple date effective sales price lists on a contract.</span></span> <span data-ttu-id="3f6b6-106">في Project Operations، يوجد كيان جديد مقترن يسمى **قوائم أسعار المشروع**.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-106">In Project Operations, there is a new associated entity called **Project Price Lists**.</span></span> <span data-ttu-id="3f6b6-107">توجد في هذا الكيان علاقة واحد إلى متعدد بعقد مشروع.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-107">This entity has a one-to-many relationship to a project contract.</span></span>

<span data-ttu-id="3f6b6-108">يتم استخدام قوائم أسعار المشروعات لتسعير حركات الوقت والمصروفات في مشروع ما.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-108">Project price lists are used to price time and expense transactions on a project.</span></span> <span data-ttu-id="3f6b6-109">عندما يتضمن أحد العقود قائمة أسعار مشروع أو أكثر، يتم استخدام قوائم الأسعار هذه لعرض تقديرات الوقت والمصروفات والقيم الفعلية على المشاريع المقترنة بالعقد من خلال شروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-109">When a contract has one or more project price lists, these price lists are used to price for time and expense estimates and actuals on projects that are associated to the contract through the contract line.</span></span>

<span data-ttu-id="3f6b6-110">في حال عدم وجود قوائم أسعار مشروع على عقد مشروع، سترى رسالة تحذير تفيد بعدم وجود قوائم أسعار المشروع ولن يتم تسعير التقديرات وعمل المشروع الفعلي والمصروفات.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-110">When there are no project price lists on a project contract, you will see a warning message that there are no project price lists and your estimates, actual project work, and expenses will not be priced.</span></span> <span data-ttu-id="3f6b6-111">لن يكون هناك أي سعر لقيم المبيعات.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-111">There will be no price for sales values.</span></span>

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a><span data-ttu-id="3f6b6-112">إقران قائمه أسعار  مشروع على عقد مشروع أو إلغاء إقرانها</span><span class="sxs-lookup"><span data-stu-id="3f6b6-112">Associate or unassociate a project price list on a project contract</span></span>

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-and-expenses"></a><span data-ttu-id="3f6b6-113">إنشاء قائمة أسعار معينه أو إقرانها لتقدير العمل والمصروفات القائمة على المشروع</span><span class="sxs-lookup"><span data-stu-id="3f6b6-113">Create or associate a specific price list for estimating project-based work and expenses</span></span>

1. <span data-ttu-id="3f6b6-114">في عقد المشروع، حدد علامة التبويب **قوائم أسعار المشروع**.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-114">On the project contract, select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="3f6b6-115">في الشبكة الفرعية، حدد **حدد + إضافة قائمة أسعار مشروع جديدة**.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-115">In the subgrid, select **+ Add New Project Price List**.</span></span>
3. <span data-ttu-id="3f6b6-116">علي شريط تمرير **الإنشاء السريع**، حدد قائمة أسعار.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-116">On the **Quick Create** slider, select a price list.</span></span> 

  <span data-ttu-id="3f6b6-117">تعرض القائمة المنسدلة كافة قوائم الأسعار التي تم تعيين السياق لها إلى **المبيعات**، حيث تتطابق العملة على قائمة الأسعار مع العملة على العقد.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-117">The drop-down list shows all price lists that have the context set to **Sales**, where the currency on the price list matches the currency on the contract.</span></span>
  
4. <span data-ttu-id="3f6b6-118">أدخل وصفًا لاقتران قائمة أسعار المشروع، وحدد **حفظ**، ثم أغلق شريط تمرير **الإنشاء السريع**.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-118">Enter a description for the project price list association, select **Save**, and then close the **Quick Create** slider.</span></span>

   <span data-ttu-id="3f6b6-119">يتم إنشاء اقتران قائمة أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-119">A project price list association is created.</span></span>
   
5. <span data-ttu-id="3f6b6-120">كرر الخطوات من 1 إلى 4 لإقران أكثر من قائمة أسعار مشروع واحدة بعقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-120">Repeat steps 1-4 to associate more than one project price list to the project contract.</span></span> <span data-ttu-id="3f6b6-121">أنشئ قوائم أسعار مشروع متعددة فقط إذا كان سريان التاريخ يختلف على كل قائمة أسعار مشروع مقترنة.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-121">Only create multiple project price lists if you have different date effectivity on each of the associated project price list.</span></span>

> [!NOTE]
> <span data-ttu-id="3f6b6-122">لا يدعم Project Operations تداخل سريان تاريخ قوائم أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-122">Project Operations doesn't support overlapping the date effectivity of the project price lists.</span></span> <span data-ttu-id="3f6b6-123">عند وجود قوائم أسعار مشروع متعددة لحركة بتاريخ محدد، سيتم تعيين السعر في هذه الحركة إلى صفر بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-123">If there are multiple project prices lists for a transaction with a given date, the price on that transaction will be defaulted to zero.</span></span>

### <a name="remove-a-project-price-list-association"></a><span data-ttu-id="3f6b6-124">إزالة اقتران قائمة أسعار المشروع</span><span class="sxs-lookup"><span data-stu-id="3f6b6-124">Remove a project price list association</span></span>

- <span data-ttu-id="3f6b6-125">حدد قائمة أسعار المشروع، ثم حدد **حذف قائمة أسعار مشروع العقد** على الشبكة الفرعية.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-125">Select the project price list, and then select **Delete Contract Project Price List** on the subgrid.</span></span> 

  <span data-ttu-id="3f6b6-126">تُزال قائمة الأسعار من قوائم أسعار المشروع في العقد.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-126">The price list is removed from the project price lists on the contract.</span></span> <span data-ttu-id="3f6b6-127">لن يتم حذف قائمة الأسعار بحد ذاتها.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-127">The price list itself will not be deleted.</span></span> <span data-ttu-id="3f6b6-128">سيتم حذف الاقتران بالعقد فقط.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-128">Only the association to the contract will be deleted.</span></span>

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a><span data-ttu-id="3f6b6-129">إعداد تعيين قوائم أسعار المشروع على عقد إلى قوائم الأسعار الافتراضية بشكل تلقائي</span><span class="sxs-lookup"><span data-stu-id="3f6b6-129">Set up automatic defaulting of project price lists on a contract</span></span>

<span data-ttu-id="3f6b6-130">يمكن إعداد قائمة أسعار المشروع كقائمة افتراضية على عقد مشروع.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-130">A project price list can be set up as the default list on a project contract.</span></span> <span data-ttu-id="3f6b6-131">يمكن لهذا الإعداد أن يساعد على التأكد من أن جميع العقود في مؤسستك تبدأ دائمًا بقائمة أسعار قياسية لفترة السعر هذه.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-131">This setup can help ensure that all contracts in your organization always start with a standard price list for that price period.</span></span>

### <a name="set-up-the-organizational-default-for-project-price-lists"></a><span data-ttu-id="3f6b6-132">إعداد التعيين الافتراضي التنظيمي لقوائم أسعار المشروع</span><span class="sxs-lookup"><span data-stu-id="3f6b6-132">Set up the organizational default for project price lists</span></span>

1. <span data-ttu-id="3f6b6-133">انتقل إلى **الإعدادات** > **عام**، ثم حدد **المعلمات**.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-133">Go to **Settings** > **General**, and then select **Parameters**.</span></span>
2. <span data-ttu-id="3f6b6-134">في صفحة قائمة **المعلمات النشطة**، حدد ثم انقر نقرًا مزدوجًا فوق السجل لفتحه.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-134">In the **Active Parameters** list page, select and double-click the record to open it.</span></span> <span data-ttu-id="3f6b6-135">أثناء النقر المزدوج، تأكد من أنك لا تنقر فوق قيمة حقل هي عبارة عن ارتباط تشعبي.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-135">While double–clicking, make sure that you are not clicking on a field value that is hyperlink.</span></span> 
3. <span data-ttu-id="3f6b6-136">في صفحة **المعلمات النشطة**، حدد علامة التبويب **قائمة الأسعار**. تعرض شبكة فرعية قائمة بقوائم الأسعار الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-136">On the **Active Parameters** page, select the **Price List** tab. A subgrid shows a list of default price lists.</span></span> <span data-ttu-id="3f6b6-137">هذه قائمة تتضمن قوائم أسعار المبيعات والتكلفة القياسية.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-137">This is a list of standard cost and sales price lists.</span></span> <span data-ttu-id="3f6b6-138">يضمن وجود قائمة أسعار **مبيعات** مقترنة هنا لكل عملة تقوم ببيعها أن تكون قائمة أسعار المبيعات قائمة الأسعار الافتراضية على كل عقد تقوم بإنشائه للعملاء الذين يتعاملون بهذه العملة.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-138">Having a **Sales** price list associated here for every currency that you sell in ensures that the sales price list is the default on any contract that you create for customers that transact in this currency.</span></span>

### <a name="set-up-a-customer-specific-project-price-list"></a><span data-ttu-id="3f6b6-139">إعداد قائمه أسعار مشروع خاصة بالعميل</span><span class="sxs-lookup"><span data-stu-id="3f6b6-139">Set up a customer-specific project price list</span></span>

<span data-ttu-id="3f6b6-140">يمكنك أيضًا إعداد قوائم أسعار مشروع خاصة بالعميل عندما تتفاوض على اتفاقية تسعير رئيسية مع العملاء.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-140">You can also set up customer–specific project price lists when you have negotiated a master pricing agreement with your customers.</span></span>

1. <span data-ttu-id="3f6b6-141">انتقل إلى **المبيعات** > **العملاء**.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-141">Go to **Sales** > **Customers**.</span></span>
2. <span data-ttu-id="3f6b6-142">من قائمة الحسابات النشطة، حدد العميل الذي حصلت منه على قائمة أسعار خاصة.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-142">From the list of active accounts, select the customer for whom have special price list.</span></span>
3. <span data-ttu-id="3f6b6-143">حدد سجل العميل لفتحه، ثم حدد علامة التبويب **قوائم أسعار المشروع**. تعرض شبكة فرعية قائمة بقوائم أسعار المشروع الخاصة بهذا العميل.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-143">Select the customer record to open it and then select the **Project Price Lists** tab. A subgrid shows a list of project price lists specific to this customer.</span></span> 
4. <span data-ttu-id="3f6b6-144">أنشئ اقتران قائمة أسعار جديدة هنا لجعل قائمة أسعار المشروع خاصة بهذا العميل.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-144">Create a new price list association here to have project price list specific to this customer.</span></span>

## <a name="custom-pricing-on-a-project-contract"></a><span data-ttu-id="3f6b6-145">التسعير المخصص على عقد مشروع</span><span class="sxs-lookup"><span data-stu-id="3f6b6-145">Custom pricing on a project contract</span></span>

<span data-ttu-id="3f6b6-146">بعد حصولك على قوائم أسعار مشروع افتراضية خاصة بالعميل والمؤسسة، سيتم إنشاء عقود المشروع مع اقترانات قوائم أسعار المشروع هذه بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-146">After you have organizational and customer-specific default project price lists, your project contracts will be created with these project price list associations automatically.</span></span> <span data-ttu-id="3f6b6-147">ولكن يتم دائمًا نسخ قوائم أسعار المشروع على عقد المشروع مع إلحاق التاريخ واسم العقد بها.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-147">However, project price lists on a project contract are always copied with the date and contract name appended to them.</span></span> <span data-ttu-id="3f6b6-148">عندئذٍ، يمكن لمدراء الحسابات والمشاريع بدء عمليات تحرير على هذه النُسخ.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-148">The account and project managers can then begin making edits to prices on these copies.</span></span> <span data-ttu-id="3f6b6-149">ستنطبق هذه الأسعار المتغيرة على عقد المشروع هذا فقط.</span><span class="sxs-lookup"><span data-stu-id="3f6b6-149">These changed prices will be applicable to this project contract only.</span></span>
