---
title: حجز لمشروع
description: يوفر هذا الموضوع معلومات حول كيفية حجز موارد لمشروع.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 19128264ed3db7efeeba948155f0ddbdc806c2a0
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907821"
---
# <a name="book-to-a-project"></a><span data-ttu-id="ebab8-103">حجز لمشروع</span><span class="sxs-lookup"><span data-stu-id="ebab8-103">Book to a project</span></span>

<span data-ttu-id="ebab8-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="ebab8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ebab8-105">يحتاج مدير المشروع أو مدير الموارد في بعض الأحيان إلى تخصيص مورد لمشروع من دون تعريف متطلبات معينة من عضو فريق عام.</span><span class="sxs-lookup"><span data-stu-id="ebab8-105">There are times where a Project manager or Resource manager will need to allocate a resource to project without a specific requirement being defined from a generic team member.</span></span> <span data-ttu-id="ebab8-106">يمكن تحقيق ذلك من خلال طريقة من ثلاث طرق.</span><span class="sxs-lookup"><span data-stu-id="ebab8-106">This can be achieved in one of three ways.</span></span>

- <span data-ttu-id="ebab8-107">الحجز من شبكة أعضاء الفريق</span><span class="sxs-lookup"><span data-stu-id="ebab8-107">Book from the team member grid</span></span>
- <span data-ttu-id="ebab8-108">الحجز من لوحة الجدولة</span><span class="sxs-lookup"><span data-stu-id="ebab8-108">Book from the schedule board</span></span>
- <span data-ttu-id="ebab8-109">الحجز من نموذج **المشروع**</span><span class="sxs-lookup"><span data-stu-id="ebab8-109">Book from the **Project** form</span></span>

## <a name="book-from-the-team-member-grid"></a><span data-ttu-id="ebab8-110">الحجز من شبكة أعضاء الفريق</span><span class="sxs-lookup"><span data-stu-id="ebab8-110">Book from the team member grid</span></span>

<span data-ttu-id="ebab8-111">إذا كانت مؤسستك تعمل في وضع تخصيص الموارد المختلط، فيمكن لمدير المشروع حجز مورد للمشروع بشكل مباشر من خلال إكمال الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="ebab8-111">If your organization is operating in hybrid Resource allocation mode, the Project manager can book a resource directly to the project by completing the following steps.</span></span>

1. <span data-ttu-id="ebab8-112">من المشروع، انتقل إلى شبكة أعضاء الفريق وحدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="ebab8-112">From the project, go to the team member grid and select **New**.</span></span>
2. <span data-ttu-id="ebab8-113">حدد اسم المنصب ودور المورد.</span><span class="sxs-lookup"><span data-stu-id="ebab8-113">Define the position name and the role of the resource.</span></span>
3. <span data-ttu-id="ebab8-114">حدد المورد القابل للحجز من البحث المتوفر.</span><span class="sxs-lookup"><span data-stu-id="ebab8-114">Select the bookable resource from the available lookup.</span></span>
4. <span data-ttu-id="ebab8-115">بعد تحديد المورد، قم بتعريف معلومات الحقل التالية لحجز المورد:</span><span class="sxs-lookup"><span data-stu-id="ebab8-115">After you select the resource, define the following field information to book the resource:</span></span>

    - <span data-ttu-id="ebab8-116">تاريخ البدء</span><span class="sxs-lookup"><span data-stu-id="ebab8-116">Start date</span></span>
    - <span data-ttu-id="ebab8-117">تاريخ الانتهاء</span><span class="sxs-lookup"><span data-stu-id="ebab8-117">Finish date</span></span>
    - <span data-ttu-id="ebab8-118">أسلوب التخصيص</span><span class="sxs-lookup"><span data-stu-id="ebab8-118">Allocation method</span></span>
    - <span data-ttu-id="ebab8-119">الساعات، إذا كانت قابلة للتطبيق</span><span class="sxs-lookup"><span data-stu-id="ebab8-119">Hours, if applicable</span></span>
    - <span data-ttu-id="ebab8-120">الموافق على المشروع</span><span class="sxs-lookup"><span data-stu-id="ebab8-120">Project approver</span></span>

6. <span data-ttu-id="ebab8-121">حدد **حفظ وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="ebab8-121">Select **Save and Close**</span></span>

## <a name="book-from-the-schedule-board"></a><span data-ttu-id="ebab8-122">الحجز من لوحة الجدولة</span><span class="sxs-lookup"><span data-stu-id="ebab8-122">Book from the schedule board</span></span>

<span data-ttu-id="ebab8-123">عندما يحتاج مدير الموارد إلى حجز مورد لمشروع بشكل مباشر، يمكنه استخدام لوحة الجدولة ومتطلبات المشروع.</span><span class="sxs-lookup"><span data-stu-id="ebab8-123">When a Resource manager needs to book a resource directly to a project, they can use the schedule board and the project requirement.</span></span> <span data-ttu-id="ebab8-124">متطلبات المشروع هي عبارة عن متطلبات الموارد المتوفرة دائمًا لحجزها.</span><span class="sxs-lookup"><span data-stu-id="ebab8-124">The project requirement is a resource requirement that is always available to be booked against.</span></span> <span data-ttu-id="ebab8-125">للحجز مباشرةً من نموذج المشروع أو من لوحة الجدولة، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="ebab8-125">To book directly to a project form the schedule board, complete the following steps.</span></span>

1. <span data-ttu-id="ebab8-126">انتقل إلى لوحة الجدولة وعلى الصفحة اليمنى، قم بتصفية الموارد التي تراعيها للمتطلبات.</span><span class="sxs-lookup"><span data-stu-id="ebab8-126">Navigate to the schedule board and on the left page, filter for the resources you are considering for the requirement.</span></span>
2. <span data-ttu-id="ebab8-127">في الجزء السفلي، حدد علامة التبويب **المشروع** لعرض قائمة بمتطلبات المشروع.</span><span class="sxs-lookup"><span data-stu-id="ebab8-127">In the bottom pane, select the **Project** tab to view a list of project requirements.</span></span>
3. <span data-ttu-id="ebab8-128">اسحب المتطلبات إلى المورد وقم بتعريف المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="ebab8-128">Drag the requirement onto a resource and define the following information:</span></span>

    - <span data-ttu-id="ebab8-129">تاريخ البدء</span><span class="sxs-lookup"><span data-stu-id="ebab8-129">Start date</span></span>
    - <span data-ttu-id="ebab8-130">تاريخ الانتهاء</span><span class="sxs-lookup"><span data-stu-id="ebab8-130">Finish date</span></span>
    - <span data-ttu-id="ebab8-131">حالة الحجز</span><span class="sxs-lookup"><span data-stu-id="ebab8-131">Booking status</span></span>
    - <span data-ttu-id="ebab8-132">أسلوب الحجز</span><span class="sxs-lookup"><span data-stu-id="ebab8-132">Booking method</span></span>
    - <span data-ttu-id="ebab8-133">المدة</span><span class="sxs-lookup"><span data-stu-id="ebab8-133">Duration</span></span>

## <a name="book-from-the-project-form"></a><span data-ttu-id="ebab8-134">الحجز من نموذج المشروع</span><span class="sxs-lookup"><span data-stu-id="ebab8-134">Book from the Project form</span></span>

<span data-ttu-id="ebab8-135">بصفتك مدير المشروع، قد تحتاج إلى حجز مورد لمشروع، ولكنك تعرف المعايير فقط بدلاً من اسم المورد.</span><span class="sxs-lookup"><span data-stu-id="ebab8-135">As a Project manager, you might need to book a resource to a project, but only know the criteria rather than the name of the resource.</span></span> <span data-ttu-id="ebab8-136">أكمل الخطوات التالية لاستخدام مساعد الجدولة للعثور على مورد استنادًا إلى اي سمات متوفرة للمورد.</span><span class="sxs-lookup"><span data-stu-id="ebab8-136">Complete the following steps to use the schedule assistant to find a resource based on any available attributes of the resource.</span></span> 

1. <span data-ttu-id="ebab8-137">انتقل إلى المشروع وحدد **حجز** لفتح مساعد الجدولة.</span><span class="sxs-lookup"><span data-stu-id="ebab8-137">Navigate to the project and select **Book** to open the Schedule Assistant.</span></span>
2. <span data-ttu-id="ebab8-138">باستخدام عوامل التصفية الموجودة على الجانب الأيمن من مساعد الجدولة، قم بتضييق المعايير وحدد **بحث.**</span><span class="sxs-lookup"><span data-stu-id="ebab8-138">Using the filters on the left side of the Schedule Assistant, narrow the criteria and select **Search.**</span></span>
3. <span data-ttu-id="ebab8-139">استنادًا إلى الموارد المرتجعة في النتائج، يمكنك حجز مورد.</span><span class="sxs-lookup"><span data-stu-id="ebab8-139">Based on resources returned in the results, you can book a resource.</span></span>

> [!NOTE]
> <span data-ttu-id="ebab8-140">لا ينشئ هذا الأسلوب أي حجوزات للمورد.</span><span class="sxs-lookup"><span data-stu-id="ebab8-140">This method doesn't create any bookings for the resource.</span></span> <span data-ttu-id="ebab8-141">بدلاً من ذلك، يضيف المورد إلى الفريق.</span><span class="sxs-lookup"><span data-stu-id="ebab8-141">Instead, it adds the resource to the team.</span></span> <span data-ttu-id="ebab8-142">بعد إضافة عضو الفريق إلى المشروع، بإمكان مدير المشروع المحافظة على الحجوزات أو توسيعها لإضافة الحجوزات المطلوبة إلى المورد.</span><span class="sxs-lookup"><span data-stu-id="ebab8-142">After the team member has been added to the project, the project manager can use maintain bookings or extend bookings to add the required bookings to the resource.</span></span>
