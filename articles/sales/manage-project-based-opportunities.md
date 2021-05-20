---
title: إدارة فرص مستندة إلى مشروع
description: يقدم هذا الموضوع معلومات حول كيفية التعامل مع الفرص المرتبطة بالمشروعات.
author: rumant
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5ce9ad1458d338d63469c3d6fddb98b9cbbced31
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948359"
---
# <a name="manage-project-based-opportunities"></a><span data-ttu-id="bec7c-103">إدارة فرص مستندة إلى مشروع</span><span class="sxs-lookup"><span data-stu-id="bec7c-103">Manage project-based opportunities</span></span>

<span data-ttu-id="bec7c-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="bec7c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bec7c-105">تعمل عادةً الشركات القائمة على المشاريع على نشر عمليات التسليم لديها عبر عدة بلدان ومناطق جغرافية.</span><span class="sxs-lookup"><span data-stu-id="bec7c-105">Project-based companies typically have their operations for delivery spread across multiple countries and geographies.</span></span> <span data-ttu-id="bec7c-106">بإمكان تكلفة تنفيذ المشروع وتسليمه أن تختلف استنادًا إلى المنطقة الجغرافية أو القسم الذي يدير عملية التسليم.</span><span class="sxs-lookup"><span data-stu-id="bec7c-106">The cost of the project execution and delivery can vary  based on which geography or division manages the delivery.</span></span> <span data-ttu-id="bec7c-107">وبإمكان هذا الأمر أن يؤثر بدوره على هوامش الصفقة.</span><span class="sxs-lookup"><span data-stu-id="bec7c-107">In turn, this can impact the margins of the deal.</span></span> <span data-ttu-id="bec7c-108">تتضمن عملية تسليم الخدمات المستندة إلى المشروع كميات كبيرة من وقت الموارد البشرية ومصروفات باهظة للسفر وتكاليف الموارد ومصروفات أخرى.</span><span class="sxs-lookup"><span data-stu-id="bec7c-108">Delivery of project-based services typically involves large quantities of human resource time, considerable expenses for travel, material costs, and other expenses.</span></span>

<span data-ttu-id="bec7c-109">تم تصميم الفرص القائمة على المشروع في Dynamics 365 Project Operations مع ملحقات إلى Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="bec7c-109">Project-based opportunities in Dynamics 365 Project Operations are designed with extensions to Dynamics 365 Sales.</span></span> <span data-ttu-id="bec7c-110">يوفر الموضوع تفاصيل حول الحقول المختلفة ومنطق الأعمال المضمن في الوظائف الإضافية المطلوبة من قِبل الشركات القائمة على المشاريع لإدارة الفرص القائمة على المشاريع.</span><span class="sxs-lookup"><span data-stu-id="bec7c-110">The topic provides details about the different fields and business logic included in the additional functionality that is required by project-based companies to manage project-based opportunities.</span></span>

## <a name="view-all-project-based-opportunities"></a><span data-ttu-id="bec7c-111">عرض جميع الفرص المستندة إلى مشروع</span><span class="sxs-lookup"><span data-stu-id="bec7c-111">View all project-based opportunities</span></span>

<span data-ttu-id="bec7c-112">يمكن رؤية قائمة بكافة الفرص المستندة إلى المشروع من صفحة قائمة **الفرصة**.</span><span class="sxs-lookup"><span data-stu-id="bec7c-112">A list of all the project-based opportunities can be seen from the **Opportunity** list page.</span></span> 

1. <span data-ttu-id="bec7c-113">انتقل إلى **المبيعات** > **الفرص**.</span><span class="sxs-lookup"><span data-stu-id="bec7c-113">Go to **Sales** > **Opportunities**.</span></span>
2. <span data-ttu-id="bec7c-114">استخدم **محدد طريقة العرض** لتحديد طرق عرض مُصفاة أخرى للفرص.</span><span class="sxs-lookup"><span data-stu-id="bec7c-114">Use the **View switcher** to select other filtered views of the opportunities.</span></span> <span data-ttu-id="bec7c-115">يمكنك إنشاء طرق عرض خاصة بك باستخدام معايير التصفية المخصصة لتكوين خيارات طرق العرض والتنقل هذه.</span><span class="sxs-lookup"><span data-stu-id="bec7c-115">You can create your own views with custom filter criteria to configure these views and navigation options.</span></span>

<span data-ttu-id="bec7c-116">يمكن إنشاء فرص المشروع أو حذفها من صفحة القائمة أو صفحة التفاصيل هذه.</span><span class="sxs-lookup"><span data-stu-id="bec7c-116">Project Opportunities can be created or deleted from this list page or the detail page.</span></span>

## <a name="business-process-flow-for-project-based-deals"></a><span data-ttu-id="bec7c-117">سير إجراءات العمل للصفقات المعتمدة على المشروع</span><span class="sxs-lookup"><span data-stu-id="bec7c-117">Business process flow for project-based deals</span></span>

<span data-ttu-id="bec7c-118">يتم دعم سير إجراءات العمل التالي للصفقات المعتمدة على المشروعات في Project Operations:</span><span class="sxs-lookup"><span data-stu-id="bec7c-118">The following business process flows are supported for project-based deals in Project Operations:</span></span>

- <span data-ttu-id="bec7c-119">إجراءات العمل من العميل المتوقع إلى الفرصة</span><span class="sxs-lookup"><span data-stu-id="bec7c-119">Lead to Opportunity business process</span></span>
- <span data-ttu-id="bec7c-120">عملية مبيعات الفرصة</span><span class="sxs-lookup"><span data-stu-id="bec7c-120">Opportunity sales process</span></span>

### <a name="lead-to-opportunity-business-process"></a><span data-ttu-id="bec7c-121">عملية الأعمال من العميل المتوقع إلى الفرصة</span><span class="sxs-lookup"><span data-stu-id="bec7c-121">Lead to opportunity business process</span></span> 
<span data-ttu-id="bec7c-122">تدعم عملية الأعمال من العميل المتوقع إلى الفرصة المراحل التالية:</span><span class="sxs-lookup"><span data-stu-id="bec7c-122">The lead to opportunity business process supports the following stages:</span></span>

| <span data-ttu-id="bec7c-123">مرحلة</span><span class="sxs-lookup"><span data-stu-id="bec7c-123">Stage</span></span> | <span data-ttu-id="bec7c-124">الكيان المعين</span><span class="sxs-lookup"><span data-stu-id="bec7c-124">Mapped entity</span></span> | <span data-ttu-id="bec7c-125">الوظائف</span><span class="sxs-lookup"><span data-stu-id="bec7c-125">Functionality</span></span> |
| --- | --- | --- |
| <span data-ttu-id="bec7c-126">تأهيل</span><span class="sxs-lookup"><span data-stu-id="bec7c-126">Qualify</span></span> | <span data-ttu-id="bec7c-127">عميل متوقع</span><span class="sxs-lookup"><span data-stu-id="bec7c-127">Lead</span></span> | <span data-ttu-id="bec7c-128">تأهيل عميل متوقع لإنشاء حساب وجهة اتصال وفرصة.</span><span class="sxs-lookup"><span data-stu-id="bec7c-128">Qualify the lead to create an account, contact, and an opportunity.</span></span> |
| <span data-ttu-id="bec7c-129">تطوير</span><span class="sxs-lookup"><span data-stu-id="bec7c-129">Develop</span></span> | <span data-ttu-id="bec7c-130">الفرصة</span><span class="sxs-lookup"><span data-stu-id="bec7c-130">Opportunity</span></span> | <span data-ttu-id="bec7c-131">تطوير الفرصة لإضافة المزيد من المعلومات حول العمل المتضمن وحملة الأسهم والمنافسة.</span><span class="sxs-lookup"><span data-stu-id="bec7c-131">Develop the opportunity to add more information on the work involved, key stakeholders, and competition.</span></span> |
| <span data-ttu-id="bec7c-132">اقتراح</span><span class="sxs-lookup"><span data-stu-id="bec7c-132">Propose</span></span> | <span data-ttu-id="bec7c-133">الفرصة</span><span class="sxs-lookup"><span data-stu-id="bec7c-133">Opportunity</span></span> | <span data-ttu-id="bec7c-134">تطوير الاقتراح والحصول على موافقة من فريق المراجعة الداخلي.</span><span class="sxs-lookup"><span data-stu-id="bec7c-134">Develop the proposal and get approval from the internal review team.</span></span> |
| <span data-ttu-id="bec7c-135">إقفال</span><span class="sxs-lookup"><span data-stu-id="bec7c-135">Close</span></span> | <span data-ttu-id="bec7c-136">الفرصة</span><span class="sxs-lookup"><span data-stu-id="bec7c-136">Opportunity</span></span> | <span data-ttu-id="bec7c-137">الفوز بفرصة لإغلاق الصفقة.</span><span class="sxs-lookup"><span data-stu-id="bec7c-137">Win the opportunity to close the deal.</span></span> |

### <a name="opportunity-sales-process"></a><span data-ttu-id="bec7c-138">عملية مبيعات الفرصة</span><span class="sxs-lookup"><span data-stu-id="bec7c-138">Opportunity sales process</span></span>
<span data-ttu-id="bec7c-139">تعتبر عملية مبيعات الفرصة في Project Operations ملحقًا لسير عمل عملية مبيعات الفرصة في تطبيق Sales.</span><span class="sxs-lookup"><span data-stu-id="bec7c-139">The Opportunity sales process in Project Operations is an extension to the Opportunity sales process business flow in the Sales application.</span></span> <span data-ttu-id="bec7c-140">تم تصميم عملية الأعمال هذه لتكون جاهزة لدعم المراحل التالية في الفرصة المستندة إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="bec7c-140">This business process is designed out-of-the-box to support the following stages in a project-based opportunity.</span></span>

| <span data-ttu-id="bec7c-141">مرحلة</span><span class="sxs-lookup"><span data-stu-id="bec7c-141">Stage</span></span> | <span data-ttu-id="bec7c-142">الكيان المعين</span><span class="sxs-lookup"><span data-stu-id="bec7c-142">Mapped entity</span></span> | <span data-ttu-id="bec7c-143">الوظائف</span><span class="sxs-lookup"><span data-stu-id="bec7c-143">Functionality</span></span> |
| --- | --- | --- |
| <span data-ttu-id="bec7c-144">تأهيل</span><span class="sxs-lookup"><span data-stu-id="bec7c-144">Qualify</span></span> | <span data-ttu-id="bec7c-145">الفرصة</span><span class="sxs-lookup"><span data-stu-id="bec7c-145">Opportunity</span></span> | <span data-ttu-id="bec7c-146">تأهيل عميل متوقع لإنشاء حساب وجهة اتصال وفرصة.</span><span class="sxs-lookup"><span data-stu-id="bec7c-146">Qualify the lead to create an account, contact, and an opportunity.</span></span> |
| <span data-ttu-id="bec7c-147">اقتراح</span><span class="sxs-lookup"><span data-stu-id="bec7c-147">Propose</span></span> | <span data-ttu-id="bec7c-148">اقتباس</span><span class="sxs-lookup"><span data-stu-id="bec7c-148">Quote</span></span> | <span data-ttu-id="bec7c-149">تطوير الاقتراح باستخدام عروض أسعار المشروع والحصول على موافقة من فريق المراجعة الداخلي.</span><span class="sxs-lookup"><span data-stu-id="bec7c-149">Develop the proposal using project quotes and get approval from the internal review team.</span></span> |
| <span data-ttu-id="bec7c-150">عقد</span><span class="sxs-lookup"><span data-stu-id="bec7c-150">Contract</span></span> | <span data-ttu-id="bec7c-151">عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="bec7c-151">Project Contract</span></span> | <span data-ttu-id="bec7c-152">ربح عرض الأسعار لإنشاء العقد وبدء التنفيذ والتسليم في المشروع.</span><span class="sxs-lookup"><span data-stu-id="bec7c-152">Win the quote to create the contract and begin execution and delivery on the project.</span></span> |
| <span data-ttu-id="bec7c-153">إقفال</span><span class="sxs-lookup"><span data-stu-id="bec7c-153">Close</span></span> | <span data-ttu-id="bec7c-154">عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="bec7c-154">Project Contract</span></span> | <span data-ttu-id="bec7c-155">إنجاز العمل بنجاح ثم إغلاق عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="bec7c-155">Finish the work successfully and close the project contract.</span></span> |

> [!NOTE]
> <span data-ttu-id="bec7c-156">إذا بدأت الصفقة المستندة إلى المشروع مع عميل متوقع، فستكون الأسبقية لعملية الأعمال من العميل المتوقع إلى الفرصة‬.</span><span class="sxs-lookup"><span data-stu-id="bec7c-156">If your project-based deal started with a Lead, the Lead to Opportunity business process takes precedence.</span></span>
>
> <span data-ttu-id="bec7c-157">إذا بدأت الصفقة المستندة إلى المشروع مع فرصة، فستكون الأسبقية لعملية مبيعات الفرصة.</span><span class="sxs-lookup"><span data-stu-id="bec7c-157">If your project-based deal started with an Opportunity, the Opportunity sales process takes precedence.</span></span>

<span data-ttu-id="bec7c-158">يمكنك تحرير سير إجراءات عمل المنتج أو إنشاء سير إجراءات عمل خاص بك لتعقب عملية الأعمال حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="bec7c-158">You can edit the product business process flow or create your own business process flows to track your sales process as needed.</span></span> <span data-ttu-id="bec7c-159">للحصول على مزيد من المعلومات حول سير إجراءات العمل، راجع [نظرة عامة حول عمليات سير إجراءات العمل](/dynamics365/customerengagement/on-premises/customize/business-process-flows-overview).</span><span class="sxs-lookup"><span data-stu-id="bec7c-159">For more information about the business process flow, see [Business process flows overview](/dynamics365/customerengagement/on-premises/customize/business-process-flows-overview).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]