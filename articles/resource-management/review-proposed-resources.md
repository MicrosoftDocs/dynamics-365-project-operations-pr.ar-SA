---
title: مراجعة الموارد المقترحة
description: يوفر هذا الموضوع معلومات حول كيفية اقتراح موارد المشاريع.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
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
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 212b80a7fde8368eedd7572dd5f9278cc53fae98
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897345"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="390c9-103">مراجعة الموارد المقترحة</span><span class="sxs-lookup"><span data-stu-id="390c9-103">Review proposed resources</span></span>

<span data-ttu-id="390c9-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="390c9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="390c9-105">يمكن لمديري الموارد اقتراح مورد لمدير المشروع باستخدام طلب مورد.</span><span class="sxs-lookup"><span data-stu-id="390c9-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="390c9-106">من شبكة الطلبات أو الطلب نفسه، حدد **البحث عن الموارد**.</span><span class="sxs-lookup"><span data-stu-id="390c9-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="390c9-107">في صفحة **مساعد الجدولة**، حدد المورد، ثم في جزء **إنشاء حجز المورد**، في حقل **حالة الحجز**، حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="390c9-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="390c9-108">تحدث تحديثات الحالة التالية:</span><span class="sxs-lookup"><span data-stu-id="390c9-108">The following status updates occur:</span></span>

- <span data-ttu-id="390c9-109">في صفحة **مساعد الجدولة**، يتم تحديث مؤشرات الحالة للإشارة إلى اقتراح الحجز، وليس حجزه بشكل ثابت.</span><span class="sxs-lookup"><span data-stu-id="390c9-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="390c9-110">في طلب المورد، تم تغيير الحالة إلى **في حاجة إلى المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="390c9-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="390c9-111">في علامة التبويب **فريق** في المشروع، يتم تغيير قيمة **حالة الطلب** لعضو الفريق العام إلى **في حاجة إلى المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="390c9-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="390c9-112">يمكن لمدير المشروع إما قبول الاقتراح أو رفضه.</span><span class="sxs-lookup"><span data-stu-id="390c9-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="390c9-113">عندما تقوم إدارات الموارد بمعالجة طلبات الموارد، يمكنها استخدام أي طريقة من الطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="390c9-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="390c9-114">اقترح موارد متعددة لتلبية الطلب في حالة عدم توفر مورد واحد لاستيفاء الساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="390c9-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="390c9-115">يتم بعد ذلك تقسيم الساعات المقترحة بين الموارد المتعددة التي يمكن أن تفي بالساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="390c9-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="390c9-116">في هذا السيناريو، لا يمكن أن تتداخل الساعات.</span><span class="sxs-lookup"><span data-stu-id="390c9-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="390c9-117">اقتراح موارد أقل مما هو مطلوب.</span><span class="sxs-lookup"><span data-stu-id="390c9-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="390c9-118">في هذا السيناريو، تكون سعة المورد المقترحة أقل من الساعات المطلوبة التي حددها الطالب.</span><span class="sxs-lookup"><span data-stu-id="390c9-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="390c9-119">وبالتالي، عندما يقبل الطالب الموارد المقترحة، يتم إنشاء متطلبات مورد غير مستوفاة لالتقاط الطلب المتبقي.</span><span class="sxs-lookup"><span data-stu-id="390c9-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="390c9-120">احجز موارد متعددة لتلبية الطلب في حالة عدم توفر مورد واحد لإكمال العمل.</span><span class="sxs-lookup"><span data-stu-id="390c9-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="390c9-121">حجز موارد أقل مما هو مطلوب.</span><span class="sxs-lookup"><span data-stu-id="390c9-121">Book fewer resources than are required.</span></span> <span data-ttu-id="390c9-122">في هذا السيناريو ، تكون الساعات المحجوزة أقل من الساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="390c9-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="390c9-123">يرشدك النظام لاقتراح الموارد بدلاً من الحجوزات، ومن ثم يمكن للطالب التحقق من الطلب المتبقي وتتبعه.</span><span class="sxs-lookup"><span data-stu-id="390c9-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="390c9-124">الاستخدام القابل للفوترة</span><span class="sxs-lookup"><span data-stu-id="390c9-124">Billable utilization</span></span>

<span data-ttu-id="390c9-125">يمكن للموارد أن تشتمل على الاستخدام القابل للفوترة للهدف.</span><span class="sxs-lookup"><span data-stu-id="390c9-125">Resources can have a target billable utilization.</span></span> <span data-ttu-id="390c9-126">ويتم تحديد هذا الاستخدام الهدف كسمة في دور افتراضي لأحد الموارد أو تعيينه في سجل المورد القابل للحجز الفردي.</span><span class="sxs-lookup"><span data-stu-id="390c9-126">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="390c9-127">وتعتمد عمليات احتساب الاستخدام على الساعات الفعلية التي قامت الموارد بالإبلاغ عنها من خلال استخدام إدخالات الوقت المعتمدة.</span><span class="sxs-lookup"><span data-stu-id="390c9-127">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="390c9-128">تُستخدم الصيغ التالية لحساب الاستخدام:</span><span class="sxs-lookup"><span data-stu-id="390c9-128">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="390c9-129">الاستخدام القابل للفوترة = الساعات الفعلية الخاضعة للرسوم ÷ القدرة الإنتاجية للمورد.</span><span class="sxs-lookup"><span data-stu-id="390c9-129">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="390c9-130">الاستخدام غير القابل للفوترة = الوقت الفعلي مع معرف نوع الفوترة = غير خاضع للرسوم أو التكميلي أو غير المتوفر ÷ القدرة الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="390c9-130">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="390c9-131">داخلي = الوقت الفعلي بلا عقد مبيعات ÷ القدرة الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="390c9-131">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="390c9-132">القدرة الإنتاجية للمورد = ساعات عمل المورد - خارج المكتب - غير أيام العمل</span><span class="sxs-lookup"><span data-stu-id="390c9-132">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="390c9-133">يمكنك العثور على طريقة عرض **استخدام الموارد** في جزء **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="390c9-133">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="390c9-134">تمثل كل خلية في الشبكة النسبة المئوية للاستخدام القابل للفوترة من المورد في فترة، مثل اليوم أو الأسبوع أو الشهر.</span><span class="sxs-lookup"><span data-stu-id="390c9-134">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="390c9-135">تُستخدم الصيغ التالية لتلوين الخلايا:</span><span class="sxs-lookup"><span data-stu-id="390c9-135">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="390c9-136">**أخضر:** الاستخدام القابل للفوترة \>= الاستخدام الهدف للمورد</span><span class="sxs-lookup"><span data-stu-id="390c9-136">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="390c9-137">**أصفر:** الاستخدام الهدف – 20 \<= الاستخدام القابل للفوترة \< الاستخدام الهدف</span><span class="sxs-lookup"><span data-stu-id="390c9-137">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="390c9-138">**أحمر:** الاستخدام القابل للفوترة \< الاستخدام الهدف – 20</span><span class="sxs-lookup"><span data-stu-id="390c9-138">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="390c9-139">ونظرًا لأن طريقة عرض **استخدام المورد** تستند إلى لوحة الجدولة، فيمكنك استخدام إمكانات تصفية لوحة الجدولة لتصفية النتائج.</span><span class="sxs-lookup"><span data-stu-id="390c9-139">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="390c9-140">تتطلب الشبكة أن تقوم بتعيين استخدام الهدف لكل من الدور أو المورد الفردي.</span><span class="sxs-lookup"><span data-stu-id="390c9-140">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="390c9-141">لإجراء هذا الإعداد، انتقل إلى **الموارد**\>**أدوار الموارد**.</span><span class="sxs-lookup"><span data-stu-id="390c9-141">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="390c9-142">بالإضافة إلى ذلك، يجب تعيين دور افتراضي لكل مورد قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="390c9-142">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="390c9-143">انتقل إلى **الموارد** \> **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="390c9-143">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="390c9-144">في علامة التبويب **Project Service**، تحقق من تحديد دور مورد، ومن تعيين حقل **افتراضي** له إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="390c9-144">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="390c9-145">يمكنك إضافة أدوار إضافية حيث **افتراضي = لا**.</span><span class="sxs-lookup"><span data-stu-id="390c9-145">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="390c9-146">يتم استخدام الدور حيث **افتراضي = نعم** لتقييم استخدام المورد مقابل الهدف لذلك الدور.</span><span class="sxs-lookup"><span data-stu-id="390c9-146">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="390c9-147">من علامة التبويب **Project Service**، يمكنك أيضًا تعيين استخدام هدف فردي للمورد.</span><span class="sxs-lookup"><span data-stu-id="390c9-147">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="390c9-148">ويقوم حساب الاستخدام بعد ذلك باستخدام هذه الطريقة لتقييم هدف المورد بدلاً من هدف الدور الافتراضي للمورد.</span><span class="sxs-lookup"><span data-stu-id="390c9-148">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="390c9-149">يتم عرض الاستخدام لمورد فقط إذا قام ذلك المورد بالموافقة، ويتم عرض الوقت الخاضع للرسوم خلال الفترة في الشبكة.</span><span class="sxs-lookup"><span data-stu-id="390c9-149">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="390c9-150">توفر الموارد</span><span class="sxs-lookup"><span data-stu-id="390c9-150">Resource availability</span></span>

<span data-ttu-id="390c9-151">من المهم أن يمكن لمديري الموارد عرض توافر الموارد وتحديث الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="390c9-151">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="390c9-152">في بعض الحالات، لا يوجد طلب رسمي (طلب مورد)، ولكن يجب أن يستجيب مدير المورد لطلب غير مخطط له من خلال قنوات مثل البريد الإلكتروني أو المكالمة الهاتفية أو الرسالة الفورية.</span><span class="sxs-lookup"><span data-stu-id="390c9-152">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="390c9-153">يستخدم مديرو الموارد لوحة الجدولة لتحديث الموارد والحجوزات.</span><span class="sxs-lookup"><span data-stu-id="390c9-153">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="390c9-154">يتم استخدام ساعات عمل المورد كأساس لحساب توافر المورد.</span><span class="sxs-lookup"><span data-stu-id="390c9-154">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="390c9-155">تستهلك حجوزات الموارد القدرة الإنتاجية للموارد.</span><span class="sxs-lookup"><span data-stu-id="390c9-155">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="390c9-156">وتستخدم لوحة الجدولة الألوان والتظليل لإظهار الحجوزات والتوافر والحجوزات الزائدة، وكذلك حالة الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="390c9-156">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="390c9-157">ويتيح لك الإعداد الموجود في إعدادات لوحة الجدولة عرض وسيلة إيضاح.</span><span class="sxs-lookup"><span data-stu-id="390c9-157">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="390c9-158">وإذا ظهر سهم يشير إلى اليمين بجوار مورد فردي قابل للحجز على لوحة الجدولة، فيمكن توسيع المورد لإظهار تفاصيل العمل الذي تم حجز المورد عليه.</span><span class="sxs-lookup"><span data-stu-id="390c9-158">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="390c9-159">نظرًا لأن Dynamics 365 Project Operations يستخدم محرك Universal Resource Scheduling ، إذا كان لديك Dynamics 365 Field Service مثبتًا، فإنه يمكنك عرض تفاصيل حجوزات الموارد الخاصة بالمشاريع وأوامر العمل وأي كيانات أخرى قمت بتوسيع الجدولة لها.</span><span class="sxs-lookup"><span data-stu-id="390c9-159">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="390c9-160">لعرض مزيد من التفاصيل حول مورد واحد، انقر بزر الماوس الأيمن فوقه لفتح بطاقة المورد.</span><span class="sxs-lookup"><span data-stu-id="390c9-160">To view more details about an individual resource, right-click it to open the resource card.</span></span>

