---
title: مراجعة الموارد المقترحة
description: يوفر هذا الموضوع معلومات حول كيفية اقتراح موارد المشاريع.
author: ruhercul
ms.date: 11/05/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 987ea08c77c1824182856c0d52ee0cd15e7029b9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000735"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="a06af-103">مراجعة الموارد المقترحة</span><span class="sxs-lookup"><span data-stu-id="a06af-103">Review proposed resources</span></span>

<span data-ttu-id="a06af-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="a06af-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a06af-105">يمكن لمديري الموارد اقتراح مورد لمدير المشروع باستخدام طلب مورد.</span><span class="sxs-lookup"><span data-stu-id="a06af-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="a06af-106">من شبكة الطلبات أو الطلب نفسه، حدد **البحث عن الموارد**.</span><span class="sxs-lookup"><span data-stu-id="a06af-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="a06af-107">في صفحة **مساعد الجدولة**، حدد المورد، ثم في جزء **إنشاء حجز المورد**، في حقل **حالة الحجز**، حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="a06af-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="a06af-108">تحدث تحديثات الحالة التالية:</span><span class="sxs-lookup"><span data-stu-id="a06af-108">The following status updates occur:</span></span>

- <span data-ttu-id="a06af-109">في صفحة **مساعد الجدولة**، يتم تحديث مؤشرات الحالة للإشارة إلى اقتراح الحجز، وليس حجزه بشكل ثابت.</span><span class="sxs-lookup"><span data-stu-id="a06af-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="a06af-110">في طلب المورد، تم تغيير الحالة إلى **في حاجة إلى المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="a06af-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="a06af-111">في علامة التبويب **فريق** في المشروع، يتم تغيير قيمة **حالة الطلب** لعضو الفريق العام إلى **في حاجة إلى المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="a06af-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="a06af-112">يمكن لمدير المشروع إما قبول الاقتراح أو رفضه.</span><span class="sxs-lookup"><span data-stu-id="a06af-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="a06af-113">عندما تقوم إدارات الموارد بمعالجة طلبات الموارد، يمكنها استخدام أي طريقة من الطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="a06af-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="a06af-114">اقترح موارد متعددة لتلبية الطلب في حالة عدم توفر مورد واحد لاستيفاء الساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="a06af-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="a06af-115">يتم بعد ذلك تقسيم الساعات المقترحة بين الموارد المتعددة التي يمكن أن تفي بالساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="a06af-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="a06af-116">في هذا السيناريو، لا يمكن أن تتداخل الساعات.</span><span class="sxs-lookup"><span data-stu-id="a06af-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="a06af-117">اقتراح موارد أقل مما هو مطلوب.</span><span class="sxs-lookup"><span data-stu-id="a06af-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="a06af-118">في هذا السيناريو، تكون سعة المورد المقترحة أقل من الساعات المطلوبة التي حددها الطالب.</span><span class="sxs-lookup"><span data-stu-id="a06af-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="a06af-119">وبالتالي، عندما يقبل الطالب الموارد المقترحة، يتم إنشاء متطلبات مورد غير مستوفاة لالتقاط الطلب المتبقي.</span><span class="sxs-lookup"><span data-stu-id="a06af-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="a06af-120">احجز موارد متعددة لتلبية الطلب في حالة عدم توفر مورد واحد لإكمال العمل.</span><span class="sxs-lookup"><span data-stu-id="a06af-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="a06af-121">حجز موارد أقل مما هو مطلوب.</span><span class="sxs-lookup"><span data-stu-id="a06af-121">Book fewer resources than are required.</span></span> <span data-ttu-id="a06af-122">في هذا السيناريو ، تكون الساعات المحجوزة أقل من الساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="a06af-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="a06af-123">يرشدك النظام لاقتراح الموارد بدلاً من الحجوزات، ومن ثم يمكن للطالب التحقق من الطلب المتبقي وتتبعه.</span><span class="sxs-lookup"><span data-stu-id="a06af-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="a06af-124">توفر الموارد</span><span class="sxs-lookup"><span data-stu-id="a06af-124">Resource availability</span></span>

<span data-ttu-id="a06af-125">من المهم أن يمكن لمديري الموارد عرض توافر الموارد وتحديث الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="a06af-125">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="a06af-126">في بعض الحالات، لا يوجد طلب رسمي (طلب مورد)، ولكن يجب أن يستجيب مدير المورد لطلب غير مخطط له من خلال قنوات مثل البريد الإلكتروني أو المكالمة الهاتفية أو الرسالة الفورية.</span><span class="sxs-lookup"><span data-stu-id="a06af-126">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="a06af-127">يستخدم مديرو الموارد لوحة الجدولة لتحديث الموارد والحجوزات.</span><span class="sxs-lookup"><span data-stu-id="a06af-127">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="a06af-128">يتم استخدام ساعات عمل المورد كأساس لحساب توافر المورد.</span><span class="sxs-lookup"><span data-stu-id="a06af-128">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="a06af-129">تستهلك حجوزات الموارد القدرة الإنتاجية للموارد.</span><span class="sxs-lookup"><span data-stu-id="a06af-129">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="a06af-130">وتستخدم لوحة الجدولة الألوان والتظليل لإظهار الحجوزات والتوافر والحجوزات الزائدة، وكذلك حالة الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="a06af-130">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="a06af-131">ويتيح لك الإعداد الموجود في إعدادات لوحة الجدولة عرض وسيلة إيضاح.</span><span class="sxs-lookup"><span data-stu-id="a06af-131">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="a06af-132">وإذا ظهر سهم يشير إلى اليمين بجوار مورد فردي قابل للحجز على لوحة الجدولة، فيمكن توسيع المورد لإظهار تفاصيل العمل الذي تم حجز المورد عليه.</span><span class="sxs-lookup"><span data-stu-id="a06af-132">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="a06af-133">نظرًا لأن Dynamics 365 Project Operations يستخدم محرك Universal Resource Scheduling، إذا كان لديك Dynamics 365 Field Service مثبتًا، فإنه يمكنك عرض تفاصيل حجوزات الموارد الخاصة بالمشاريع وأوامر العمل وأي كيانات أخرى قمت بتوسيع الجدولة إليها.</span><span class="sxs-lookup"><span data-stu-id="a06af-133">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="a06af-134">لعرض مزيد من التفاصيل حول مورد واحد، انقر بزر الماوس الأيمن فوقه لفتح بطاقة المورد.</span><span class="sxs-lookup"><span data-stu-id="a06af-134">To view more details about an individual resource, right-click it to open the resource card.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]