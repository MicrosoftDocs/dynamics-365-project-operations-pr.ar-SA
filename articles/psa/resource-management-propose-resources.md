---
title: اقتراح موارد المشاريع
description: يوفر هذا الموضوع معلومات حول اقتراح موارد المشاريع.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 02e47338e34a37e05455e2bc6e6a175210ed6bc7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997945"
---
# <a name="propose-project-resources"></a><span data-ttu-id="2e643-103">اقتراح موارد المشاريع</span><span class="sxs-lookup"><span data-stu-id="2e643-103">Propose project resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="2e643-104">يمكن لمديري الموارد اقتراح مورد لمدير المشروع باستخدام طلب مورد.</span><span class="sxs-lookup"><span data-stu-id="2e643-104">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="2e643-105">من شبكة الطلبات أو الطلب نفسه، حدد **البحث عن الموارد**.</span><span class="sxs-lookup"><span data-stu-id="2e643-105">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="2e643-106">في صفحة **مساعد الجدولة**، حدد المورد، ثم في جزء **إنشاء حجز المورد**، في حقل **حالة الحجز**، حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="2e643-106">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

    ![تحديد المورد المقترح](media/Resource-Management-image62.png)

<span data-ttu-id="2e643-108">تحدث تحديثات الحالة التالية:</span><span class="sxs-lookup"><span data-stu-id="2e643-108">The following status updates occur:</span></span>

- <span data-ttu-id="2e643-109">في صفحة **مساعد الجدولة**، يتم تحديث مؤشرات الحالة للإشارة إلى اقتراح الحجز، وليس حجزه بشكل ثابت.</span><span class="sxs-lookup"><span data-stu-id="2e643-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>

    ![مؤشرات الحالة الخاصة بالحجز المقترح في صفحة مساعد الجدولة](media/Resource-Management-image63.png)

- <span data-ttu-id="2e643-111">في طلب المورد، تم تغيير الحالة إلى **في حاجة إلى المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="2e643-111">On the resource request, the status is changed to **Needs Review**.</span></span>

    ![تغيير حالة طلب المورد إلى في حاجة إلى المراجعة](media/Resource-Management-image64.png)

- <span data-ttu-id="2e643-113">في علامة التبويب **فريق** في المشروع، يتم تغيير قيمة **حالة الطلب** لعضو الفريق العام إلى **في حاجة إلى المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="2e643-113">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

    ![تغيير حالة طلب عضو الفريق العام إلى في حاجة إلى التغيير في علامة التبويب فريق](media/Resource-Management-image48.png)

<span data-ttu-id="2e643-115">يمكن لمدير المشروع إما قبول الاقتراح أو رفضه.</span><span class="sxs-lookup"><span data-stu-id="2e643-115">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="2e643-116">عندما تقوم إدارات الموارد بمعالجة طلبات الموارد، يمكنها استخدام أي طريقة من الطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="2e643-116">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="2e643-117">اقترح موارد متعددة لتلبية الطلب في حالة عدم توفر مورد واحد لاستيفاء الساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="2e643-117">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="2e643-118">يتم بعد ذلك تقسيم الساعات المقترحة بين الموارد المتعددة التي يمكن أن تفي بالساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="2e643-118">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="2e643-119">في هذا السيناريو، لا يمكن أن تتداخل الساعات.</span><span class="sxs-lookup"><span data-stu-id="2e643-119">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="2e643-120">اقتراح موارد أقل مما هو مطلوب.</span><span class="sxs-lookup"><span data-stu-id="2e643-120">Propose fewer resources than are required.</span></span> <span data-ttu-id="2e643-121">في هذا السيناريو، تكون سعة المورد المقترحة أقل من الساعات المطلوبة التي حددها الطالب.</span><span class="sxs-lookup"><span data-stu-id="2e643-121">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="2e643-122">وبالتالي، عندما يقبل الطالب الموارد المقترحة، يتم إنشاء متطلبات مورد غير مستوفاة لالتقاط الطلب المتبقي.</span><span class="sxs-lookup"><span data-stu-id="2e643-122">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="2e643-123">احجز موارد متعددة لتلبية الطلب في حالة عدم توفر مورد واحد لإكمال العمل.</span><span class="sxs-lookup"><span data-stu-id="2e643-123">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="2e643-124">حجز موارد أقل مما هو مطلوب.</span><span class="sxs-lookup"><span data-stu-id="2e643-124">Book fewer resources than are required.</span></span> <span data-ttu-id="2e643-125">في هذا السيناريو ، تكون الساعات المحجوزة أقل من الساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="2e643-125">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="2e643-126">يرشدك النظام لاقتراح الموارد بدلاً من الحجوزات، ومن ثم يمكن للطالب التحقق من الطلب المتبقي وتتبعه.</span><span class="sxs-lookup"><span data-stu-id="2e643-126">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="2e643-127">الاستخدام القابل للفوترة</span><span class="sxs-lookup"><span data-stu-id="2e643-127">Billable utilization</span></span>

<span data-ttu-id="2e643-128">يمكن للموارد أن تشتمل على الاستخدام القابل للفوترة للهدف.</span><span class="sxs-lookup"><span data-stu-id="2e643-128">Resources can have a target billable utilization.</span></span> <span data-ttu-id="2e643-129">ويتم تحديد هذا الاستخدام الهدف كسمة في دور افتراضي لأحد الموارد أو تعيينه في سجل المورد القابل للحجز الفردي.</span><span class="sxs-lookup"><span data-stu-id="2e643-129">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="2e643-130">وتعتمد عمليات احتساب الاستخدام على الساعات الفعلية التي قامت الموارد بالإبلاغ عنها من خلال استخدام إدخالات الوقت المعتمدة.</span><span class="sxs-lookup"><span data-stu-id="2e643-130">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="2e643-131">تُستخدم الصيغ التالية لحساب الاستخدام:</span><span class="sxs-lookup"><span data-stu-id="2e643-131">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="2e643-132">الاستخدام القابل للفوترة = الساعات الفعلية الخاضعة للرسوم ÷ القدرة الإنتاجية للمورد.</span><span class="sxs-lookup"><span data-stu-id="2e643-132">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="2e643-133">الاستخدام غير القابل للفوترة = الوقت الفعلي مع معرف نوع الفوترة = غير خاضع للرسوم أو التكميلي أو غير المتوفر ÷ القدرة الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="2e643-133">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="2e643-134">داخلي = الوقت الفعلي بلا عقد مبيعات ÷ القدرة الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="2e643-134">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="2e643-135">القدرة الإنتاجية للمورد = ساعات عمل المورد - خارج المكتب - غير أيام العمل</span><span class="sxs-lookup"><span data-stu-id="2e643-135">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="2e643-136">يمكنك العثور على طريقة عرض **استخدام الموارد** في جزء **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="2e643-136">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

![طريقة عرض استخدام الموارد](media/Resource-Management-image65.png)

<span data-ttu-id="2e643-138">تمثل كل خلية في الشبكة النسبة المئوية للاستخدام القابل للفوترة من المورد في فترة، مثل اليوم أو الأسبوع أو الشهر.</span><span class="sxs-lookup"><span data-stu-id="2e643-138">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="2e643-139">تُستخدم الصيغ التالية لتلوين الخلايا:</span><span class="sxs-lookup"><span data-stu-id="2e643-139">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="2e643-140">**أخضر:** الاستخدام القابل للفوترة \>= الاستخدام الهدف للمورد</span><span class="sxs-lookup"><span data-stu-id="2e643-140">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="2e643-141">**أصفر:** الاستخدام الهدف – 20 \<= الاستخدام القابل للفوترة \< الاستخدام الهدف</span><span class="sxs-lookup"><span data-stu-id="2e643-141">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="2e643-142">**أحمر:** الاستخدام القابل للفوترة \< الاستخدام الهدف – 20</span><span class="sxs-lookup"><span data-stu-id="2e643-142">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="2e643-143">ونظرًا لأن طريقة عرض **استخدام المورد** تستند إلى لوحة الجدولة، فيمكنك استخدام إمكانات تصفية لوحة الجدولة لتصفية النتائج.</span><span class="sxs-lookup"><span data-stu-id="2e643-143">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="2e643-144">تتطلب الشبكة أن تقوم بتعيين استخدام الهدف لكل من الدور أو المورد الفردي.</span><span class="sxs-lookup"><span data-stu-id="2e643-144">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="2e643-145">لإجراء هذا الإعداد، انتقل إلى **الموارد**\>**أدوار الموارد**.</span><span class="sxs-lookup"><span data-stu-id="2e643-145">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="2e643-146">بالإضافة إلى ذلك، يجب تعيين دور افتراضي لكل مورد قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="2e643-146">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="2e643-147">انتقل إلى **الموارد** \> **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="2e643-147">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="2e643-148">في علامة التبويب **Project Service**، تحقق من تحديد دور مورد، ومن تعيين حقل **افتراضي** له إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="2e643-148">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="2e643-149">يمكنك إضافة أدوار إضافية حيث **افتراضي = لا**.</span><span class="sxs-lookup"><span data-stu-id="2e643-149">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="2e643-150">يتم استخدام الدور حيث **افتراضي = نعم** لتقييم استخدام المورد مقابل الهدف لذلك الدور.</span><span class="sxs-lookup"><span data-stu-id="2e643-150">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

![تعيين الدور الافتراضي](media/Resource-Management-image67.png)

<span data-ttu-id="2e643-152">من علامة التبويب **Project Service**، يمكنك أيضًا تعيين استخدام هدف فردي للمورد.</span><span class="sxs-lookup"><span data-stu-id="2e643-152">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="2e643-153">ويقوم حساب الاستخدام بعد ذلك باستخدام هذه الطريقة لتقييم هدف المورد بدلاً من هدف الدور الافتراضي للمورد.</span><span class="sxs-lookup"><span data-stu-id="2e643-153">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="2e643-154">يتم عرض الاستخدام لمورد فقط إذا قام ذلك المورد بالموافقة، ويتم عرض الوقت الخاضع للرسوم خلال الفترة في الشبكة.</span><span class="sxs-lookup"><span data-stu-id="2e643-154">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="2e643-155">توفر الموارد</span><span class="sxs-lookup"><span data-stu-id="2e643-155">Resource availability</span></span>

<span data-ttu-id="2e643-156">من المهم أن يمكن لمديري الموارد عرض توافر الموارد وتحديث الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="2e643-156">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="2e643-157">في بعض الحالات، لا يوجد طلب رسمي (طلب مورد)، ولكن يجب أن يستجيب مدير المورد لطلب غير مخطط له من خلال قنوات مثل البريد الإلكتروني أو المكالمة الهاتفية أو الرسالة الفورية.</span><span class="sxs-lookup"><span data-stu-id="2e643-157">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="2e643-158">يستخدم مديرو الموارد لوحة الجدولة لتحديث الموارد والحجوزات.</span><span class="sxs-lookup"><span data-stu-id="2e643-158">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="2e643-159">يتم استخدام ساعات عمل المورد كأساس لحساب توافر المورد.</span><span class="sxs-lookup"><span data-stu-id="2e643-159">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="2e643-160">تستهلك حجوزات الموارد القدرة الإنتاجية للموارد.</span><span class="sxs-lookup"><span data-stu-id="2e643-160">Resource bookings consume the capacity of the resources.</span></span>

![لوحة الجدولة](media/Resource-Management-image68.png)

<span data-ttu-id="2e643-162">وتستخدم لوحة الجدولة الألوان والتظليل لإظهار الحجوزات والتوافر والحجوزات الزائدة، وكذلك حالة الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="2e643-162">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="2e643-163">ويتيح لك الإعداد الموجود في إعدادات لوحة الجدولة عرض وسيلة إيضاح.</span><span class="sxs-lookup"><span data-stu-id="2e643-163">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="2e643-164">وإذا ظهر سهم يشير إلى اليمين بجوار مورد فردي قابل للحجز على لوحة الجدولة، فيمكن توسيع المورد لإظهار تفاصيل العمل الذي تم حجز المورد عليه.</span><span class="sxs-lookup"><span data-stu-id="2e643-164">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

![توسيع المورد القابل للحجز في لوحة الجدولة](media/Resource-Management-image69.png)

<span data-ttu-id="2e643-166">نظرًا لأن Dynamics 365 Project Service Automation يستخدم محرك Universal Resource Scheduling، إذا كان لديك Dynamics 365 Field Service مثبتًا، فإنه يمكنك عرض تفاصيل حجوزات الموارد الخاصة بالمشاريع وأوامر العمل وأي كيانات أخرى قمت بتوسيع الجدولة إليها.</span><span class="sxs-lookup"><span data-stu-id="2e643-166">Because Dynamics 365 Project Service Automation uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

![تفاصيل حجوزات الموارد الخاصة بالمشاريع وأوامر العمل](media/Resource-Management-image70.png)

<span data-ttu-id="2e643-168">لعرض مزيد من التفاصيل حول مورد واحد، انقر بزر الماوس الأيمن فوقه لفتح بطاقة المورد.</span><span class="sxs-lookup"><span data-stu-id="2e643-168">To view more details about an individual resource, right-click it to open the resource card.</span></span>

![بطاقة المورد](media/Resource-Management-image71.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]