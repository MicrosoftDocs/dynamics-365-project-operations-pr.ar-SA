---
title: عرض استخدام الموارد الخاضع للرسوم
description: يوفر هذا الموضوع معلومات حول طريقة عرض استخدام الموارد.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
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
ms.openlocfilehash: a1d1db532c65b2a13f3cf4e1281a5987490b96df
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122147"
---
# <a name="view-chargeable-utilization-for-resources"></a><span data-ttu-id="97419-103">عرض استخدام الموارد الخاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="97419-103">View chargeable utilization for resources</span></span>
 
<span data-ttu-id="97419-104">توضح طريقه عرض **الاستخدام** الموجودة في صفحة **استخدام مورد Project Service** الاستخدام الخاضع للرسوم لكل مورد قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="97419-104">The **Utilization View** on the **Project Service Resource Utilization** page shows the chargeable utilization for each bookable resource.</span></span> <span data-ttu-id="97419-105">ولأن طريقة العرض تستند إلى لوحة الجدولة، فسوف تعثر على العديد من الوظائف نفسها هناك.</span><span class="sxs-lookup"><span data-stu-id="97419-105">Because the view is based on the schedule board, you’ll find many of the same functions.</span></span>

> ![لقطة شاشة لطريقة عرض الاستخدام](media/FAQ-utilization-1.png)
 

<span data-ttu-id="97419-107">يعمل حساب الاستخدام الخاضع للرسوم يعمل كما يلي:</span><span class="sxs-lookup"><span data-stu-id="97419-107">The chargeable utilization calculation works as follows:</span></span>

   <span data-ttu-id="97419-108">الاستخدام الخاضع للرسوم = (الساعات الفعلية الخاضعة للرسوم) / (القدرة الإنتاجية للمورد).</span><span class="sxs-lookup"><span data-stu-id="97419-108">Chargeable utilization = (Chargeable actual hours) / (resource capacity)</span></span>

<span data-ttu-id="97419-109">تمثل الخلايا الاستخدام الخاضع للرسوم المحتسب للفترة المحددة (الأيام أو الأسابيع أو الشهور).</span><span class="sxs-lookup"><span data-stu-id="97419-109">The cells represent the calculated chargeable utilization for the selected period (days, weeks, or months).</span></span>

<span data-ttu-id="97419-110">توضح الألوان في كل خلية الاستخدام الخاضع للرسوم لأحد الموارد مقارنة بالاستخدام المستهدف الخاضع للرسوم.</span><span class="sxs-lookup"><span data-stu-id="97419-110">The colors in each cell show the chargeable utilization for a resource as compared to their target chargeable utilization.</span></span> 

<span data-ttu-id="97419-111">يمكن تعيين الاستخدام المستهدف إلى الدور الافتراضي للمورد أو المورد الفردي بحد ذاته.</span><span class="sxs-lookup"><span data-stu-id="97419-111">The target utilization can be set on the resource’s default role or on the individual resource itself.</span></span> <span data-ttu-id="97419-112">تنظر عملية الحساب إلى الفرد بحثًا عن الهدف أولاً، ثم الدور الافتراضي للمورد.</span><span class="sxs-lookup"><span data-stu-id="97419-112">The calculation looks at the individual for the target first, and then to the resource’s default role.</span></span>

## <a name="set-target-on-a-resource"></a><span data-ttu-id="97419-113">تعيين هدف لمورد</span><span class="sxs-lookup"><span data-stu-id="97419-113">Set target on a resource</span></span>

1. <span data-ttu-id="97419-114">انتقل إلى **الموارد** \> **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="97419-114">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="97419-115">حدد أحد الوارد لفتح السجل.</span><span class="sxs-lookup"><span data-stu-id="97419-115">Select a resource to open the record.</span></span> 
3. <span data-ttu-id="97419-116">من علامة التبويب **Project Service**، يمكنك أيضًا تعيين الاستخدام المستهدف للمورد.</span><span class="sxs-lookup"><span data-stu-id="97419-116">On the **Project Service** tab, you can set the resource’s target utilization.</span></span>

> ![لقطة شاشة لاستخدام علامة التبويب Project Service لتعيين الاستخدام المستهدف](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a><span data-ttu-id="97419-118">تعيين الاستخدام المستهدف لدور</span><span class="sxs-lookup"><span data-stu-id="97419-118">Set target utilization on a role</span></span>

1. <span data-ttu-id="97419-119">انتقل إلى **الموارد** \> **أدوار الموارد**.</span><span class="sxs-lookup"><span data-stu-id="97419-119">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="97419-120">حدد أحد الأدوار وافتح السجل.</span><span class="sxs-lookup"><span data-stu-id="97419-120">Select a role and open the record.</span></span> 
3. <span data-ttu-id="97419-121">عيّن الاستخدام المستهدف للدور.</span><span class="sxs-lookup"><span data-stu-id="97419-121">Set the target utilization for the role.</span></span>

> ![لقطة شاشة لاستخدام أدوار الموارد لتعيين الاستخدام المستهدف](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a><span data-ttu-id="97419-123">حساب الاستخدام الخاضع للرسوم لمورد</span><span class="sxs-lookup"><span data-stu-id="97419-123">Calculate chargeable utilization for a resource</span></span>

<span data-ttu-id="97419-124">لحساب الاستخدام الخاضع للرسوم لأحد الموارد، يجب عليك استكمال بعض المتطلبات المسبقة.</span><span class="sxs-lookup"><span data-stu-id="97419-124">To calculate chargeable utilization for a resource, you will need to complete some pre-requisites.</span></span> 

### <a name="set-default-role-for-individual-resource"></a><span data-ttu-id="97419-125">تعيين الدور الافتراضي لمورد فردي</span><span class="sxs-lookup"><span data-stu-id="97419-125">Set default role for individual resource</span></span>

<span data-ttu-id="97419-126">أولاً، يجب تعيين الاستخدام المستهدف إما على المورد الفردي أو على أدوار المورد.</span><span class="sxs-lookup"><span data-stu-id="97419-126">First, the target utilization must be set on either the individual resource or on resource roles.</span></span> <span data-ttu-id="97419-127">إذا كنت تستخدم أدوار الموارد للأهداف، فيجب أن يكون لدى كل مورد فردي دور افتراضي.</span><span class="sxs-lookup"><span data-stu-id="97419-127">If you are using resource roles for targets, each individual resource must have a default role.</span></span> 

1. <span data-ttu-id="97419-128">لتعيين هذا، انتقل إلى **الموارد** \> **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="97419-128">To set this, go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="97419-129">حدد موردا ، ثم افتح السجل، ثم حدد علامة التبويب **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="97419-129">Select a resource, open the record, and then select the **Project Service** tab.</span></span> 
3. <span data-ttu-id="97419-130">في شبكة **دور المورد**، تأكد من وجود دور واحد للمورد وأنه تم تعيين **الوضع الافتراضي** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="97419-130">In the **Resource Role** grid, make sure there’s one role for the resource and **Is Default** is set to **Yes**.</span></span>
 
### <a name="change-billing-type-for-resource-role"></a><span data-ttu-id="97419-131">تغيير نوع الفوترة لدور المورد</span><span class="sxs-lookup"><span data-stu-id="97419-131">Change billing type for resource role</span></span>

<span data-ttu-id="97419-132">يجب تعيين أدوار الموارد بحيث يكون نوع الفوترة المعين لها **خاضعًا للرسوم**.</span><span class="sxs-lookup"><span data-stu-id="97419-132">The resource roles must be set to have a billing type of **Chargeable**.</span></span> 

1. <span data-ttu-id="97419-133">انتقل إلى **الموارد** \> **أدوار الموارد**.</span><span class="sxs-lookup"><span data-stu-id="97419-133">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="97419-134">افتح السجل الذي تريد تحديثه ثم قم بتعيين النوع الافتراضي للفوترة إلى **خاضع للرسوم**.</span><span class="sxs-lookup"><span data-stu-id="97419-134">Open the record you want to update, and then set the billing type default to **Chargeable**.</span></span>

### <a name="set-working-hours-for-resource-role"></a><span data-ttu-id="97419-135">تعيين ساعات لدور الموارد</span><span class="sxs-lookup"><span data-stu-id="97419-135">Set working hours for resource role</span></span>
 
<span data-ttu-id="97419-136">يجب أن تكون لدى المورد ساعات عمل لحساب القدرة الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="97419-136">The resource must have working hours for the capacity calculation.</span></span> 

1. <span data-ttu-id="97419-137">انتقل إلى **الموارد** \> **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="97419-137">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="97419-138">حدد موردًا لفتح السجل، ثم حدد **إظهار ساعات العمل**.</span><span class="sxs-lookup"><span data-stu-id="97419-138">Select a resource to open the record, and then select **Show Work Hours**.</span></span> 
3. <span data-ttu-id="97419-139">يمكن إجراء تحديث مجمع لقائمة الموارد عن طريق تطبيق **قالب ساعات العمل** من طريقة عرض **قائمة الموارد**.</span><span class="sxs-lookup"><span data-stu-id="97419-139">You can bulk-update the list of resources by applying a **Work Hour Template** from the **Resource List** view.</span></span>

## <a name="troubleshooting-chargeable-actual-hours"></a><span data-ttu-id="97419-140">استكشاف أخطاء الساعات الفعلية الخاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="97419-140">Troubleshooting chargeable actual hours</span></span>

<span data-ttu-id="97419-141">الساعات الفعلية الخاضعة للرسوم مصدرها كيان **القيم الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="97419-141">The chargeable actual hours are sourced from the **Actuals** entity.</span></span> <span data-ttu-id="97419-142">يتم تضمين القيم الفعلية ذات نوع الفوترة **الخاضعة للرسوم** في العملية الحسابية، ولهذا السبب يجب أن تكون لديك مشاريع بحيث تكون القيم الفعلية خاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="97419-142">Actuals with a billing type of **Chargeable** are included in the calculation and, for this reason, you must have projects where the actuals that are chargeable.</span></span>

<span data-ttu-id="97419-143">إذا لم يظهر الاستخدام الخاضع للرسوم، فإليك بعض الأشياء التي يمكن التحقق منها:</span><span class="sxs-lookup"><span data-stu-id="97419-143">If you are not seeing chargeable utilization, here are some things you can check:</span></span>

- <span data-ttu-id="97419-144">لدى المورد ساعات عمل محددة للقدرة الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="97419-144">The resource has working hours defined for capacity.</span></span>
- <span data-ttu-id="97419-145">لدى المورد هدف استخدام محدد بشكل فردي أو دور افتراضي معين له.</span><span class="sxs-lookup"><span data-stu-id="97419-145">The resource has either an individually defined utilization target or has a default role assigned to it.</span></span> <span data-ttu-id="97419-146">لدى الدور هدف استخدام محدد له.</span><span class="sxs-lookup"><span data-stu-id="97419-146">The role has a utilization target defined for it.</span></span>
- <span data-ttu-id="97419-147">لدى القيم الفعلية نوع فوترة **خاضع للرسوم** للفترة التي تتوقع فيها حساب الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="97419-147">Actuals have a billing type of **Chargeable** for the period you are expecting a utilization calculation for.</span></span> <span data-ttu-id="97419-148">افحص ما يلي إذا رأيت قيمًا فعلية بأنواع فوترة خلاف غير خاضعة للرسوم:</span><span class="sxs-lookup"><span data-stu-id="97419-148">Check the following if you are seeing actuals with billing types other than chargeable:</span></span>

  - <span data-ttu-id="97419-149">الدور المستخدم على القيم الفعلية لديه نوع فوترة غير تلك الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="97419-149">The role used on the actual has a default billing type of something other than chargeable.</span></span>
  - <span data-ttu-id="97419-150">تم تعيين الدور في شروط التعاقد الخاصة بالمشروع والتي تدعم المشروع إلى غير خاضع للرسوم.</span><span class="sxs-lookup"><span data-stu-id="97419-150">The role on the project contract line backing the project has been set to non-chargeable.</span></span>
  - <span data-ttu-id="97419-151">‏‏ليس لدى المشروع شروط تعاقد مقترنة به.</span><span class="sxs-lookup"><span data-stu-id="97419-151">The project does not have an associated contract line.</span></span>

