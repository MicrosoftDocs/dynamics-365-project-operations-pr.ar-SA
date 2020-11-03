---
title: إدارة المناطق الزمنية
description: عند إنشاء مشروع، فإن المنطقة الزمنية الخاصة به تستند إلى المنطقة الزمنية المحددة في قالب ساعة العمل الذي يتم تطبيقه.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 27f58f0dacc3404119a719547ad374629c740740
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070582"
---
# <a name="manage-time-zones"></a><span data-ttu-id="6f09e-103">إدارة المناطق الزمنية</span><span class="sxs-lookup"><span data-stu-id="6f09e-103">Manage time zones</span></span>

<span data-ttu-id="6f09e-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="6f09e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


## <a name="projects"></a><span data-ttu-id="6f09e-105">المشروعات</span><span class="sxs-lookup"><span data-stu-id="6f09e-105">Projects</span></span>

<span data-ttu-id="6f09e-106">عند إنشاء مشروع، فإن المنطقة الزمنية تستند إلى المنطقة الزمنية المحددة في قالب ساعة العمل المطبق.</span><span class="sxs-lookup"><span data-stu-id="6f09e-106">When a project is created, the time zone is based on the time zone defined in the applied work hour template.</span></span> <span data-ttu-id="6f09e-107">في نموذج **المشروع** ، تكون التواريخ دائمًا ما تكون مرتبطة بالمنطقة الزمنية للمستخدم الذي سجل دخوله في كل علامة تبويب، باستثناء علامة تبويب **المهمة**. عند عرض هيكل تنظيم العمل، يتم عرض التواريخ دائما في المنطقة الزمنية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="6f09e-107">On the **Project** for, the dates are always relative to the time zone of the user that is logged in on each tab, except the **Task** tab. When you view the work breakdown structure, the dates will always be displayed in the project’s time zone.</span></span>

## <a name="tasks"></a><span data-ttu-id="6f09e-108">المهام</span><span class="sxs-lookup"><span data-stu-id="6f09e-108">Tasks</span></span>

<span data-ttu-id="6f09e-109">عند إنشاء مهمة، يتم التحكم في وقت البدء ووقت الانتهاء والساعات/اليوم من خلال ساعات عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="6f09e-109">When a task is created, the start time, end time, and hours/day is controlled by the working hours of the project.</span></span> <span data-ttu-id="6f09e-110">على سبيل المثال، إذا تم إنشاء مهمة لمشروع خصصت المنطقة الزمنية له بـ -8 PST، وكانت تحتوي على ساعات العمل التالية: 9:00 ص 5:00 م من الإثنين إلى الجمعة، فإن أي مهمة يتم إنشاؤها دون تعيين سوف تحترم وقت البدء ووقت الانتهاء لتقويم المشروع.</span><span class="sxs-lookup"><span data-stu-id="6f09e-110">For example, if a task is created with a project whose time zone is -8 PST and has the following working hours: 9:00 AM to 5:00 PM Monday to Friday, any task created without an assignment will respect the start time and end time of the project calendar.</span></span>

## <a name="manage-resources-with-time-zones"></a><span data-ttu-id="6f09e-111">إدارة الموارد حسب المناطق الزمنية</span><span class="sxs-lookup"><span data-stu-id="6f09e-111">Manage resources with time zones</span></span>

<span data-ttu-id="6f09e-112">للحصول على نتائج دقيقة ومتوقعة عند استخدام **توسيع الحجز** ، يوجد اثنين من المتطلبات الأساسية التي يجب يلزم تلبيتها:</span><span class="sxs-lookup"><span data-stu-id="6f09e-112">For accurate and predictable results when using **Extend Booking** , there are two key prerequisites that must be met:</span></span>  

- <span data-ttu-id="6f09e-113">يجب على المستخدم تكوين المنطقة الزمنية للجهاز الخاصة به لمطابقة المنطقة الزمنية المحددة في **إعدادات التخصيص** الخاصة بالنظام.</span><span class="sxs-lookup"><span data-stu-id="6f09e-113">The user must configure their device's time zone to match the time zone defined in the system's **Personalization Settings**.</span></span>
 
  ![إعدادات المنطقة الزمنية في Windows 10](media/reconcile-assignments-03.png)

  ![إعدادات المنطقة الزمنية في إعدادات التخصيص](media/reconcile-assignments-04.png)
 
- <span data-ttu-id="6f09e-116">يجب وجود دقيقة واحدة على الأقل من وقت المورد القابل للحجز تتداخل مع المخططات الزمنية المستخدمة لتعريف التمديد المطلوب.</span><span class="sxs-lookup"><span data-stu-id="6f09e-116">The bookable resource must have at least one minute of working time that overlaps with the contours that are used to define the requested extension.</span></span> <span data-ttu-id="6f09e-117">على سبيل المثال، الموارد التالية التي تقع ساعات العمل الخاص بها بين 9:00 ص و 7:00 م.</span><span class="sxs-lookup"><span data-stu-id="6f09e-117">For example, the following resources with working hours that fall between 9:00 AM and 7:00 PM.</span></span> 

  ![مقارنة حدود الموارد](media/reconcile-assignments-05.png)

<span data-ttu-id="6f09e-119">يبين الجدول التالي:</span><span class="sxs-lookup"><span data-stu-id="6f09e-119">The following table shows:</span></span>

- <span data-ttu-id="6f09e-120">قالب تقويم مشروع</span><span class="sxs-lookup"><span data-stu-id="6f09e-120">A project calendar template</span></span>
- <span data-ttu-id="6f09e-121">المورد A: هذا المورد له التقويم نفسه وهو في المنطقة الزمنية نفسها حيث يوجد المشروع.</span><span class="sxs-lookup"><span data-stu-id="6f09e-121">Resource A: This resource has the same calendar and is in the same time zone as the project.</span></span> <span data-ttu-id="6f09e-122">سيكون وقت بدء الحجوزات 9:00 ص.</span><span class="sxs-lookup"><span data-stu-id="6f09e-122">The start time of the bookings will be 9:00 AM.</span></span>
- <span data-ttu-id="6f09e-123">المورد ب: يقع هذا المورد في منطقة زمنية مختلفة عن المشروع ويبدأ عند 7:00 ص في المنطقة الزمنية الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="6f09e-123">Resource B: This resource is located in a different time zone than the project and starts at 7:00 AM in their time zone.</span></span> <span data-ttu-id="6f09e-124">ومع ذلك، ستبدأ الحجوزات عند الساعة 9:00 ص لأن هذا الوقت هو أقرب وقت بدء لحدود التعيين.</span><span class="sxs-lookup"><span data-stu-id="6f09e-124">However, the bookings will begin at 9:00 AM as that is the earliest start time of the assignment contour.</span></span>
- <span data-ttu-id="6f09e-125">الموارد جـ و د: يتم تحديد موقع الموارد في مناطق زمنية مختلفة، على أن تكون مختلفة عن بعضها البعض وعن المشروع، ولا يتم بدء حجوزاتها قبل تاريخ البدء الخاص بها المتوفر.</span><span class="sxs-lookup"><span data-stu-id="6f09e-125">Resources C and D: The resources are located in different time zones, both different from each other and the project, and their bookings start no earlier than their respective available start times.</span></span>

|<span data-ttu-id="6f09e-126">الكيان</span><span class="sxs-lookup"><span data-stu-id="6f09e-126">Entity</span></span>  |<span data-ttu-id="6f09e-127">التقويم</span><span class="sxs-lookup"><span data-stu-id="6f09e-127">Calendar</span></span>  |
|-|-|
|<span data-ttu-id="6f09e-128">قالب تقويم مشروع</span><span class="sxs-lookup"><span data-stu-id="6f09e-128">Project calendar template</span></span>   | ![تقويم المشروع](media/reconcile-assignments-06.png) |
|<span data-ttu-id="6f09e-130">المورد A</span><span class="sxs-lookup"><span data-stu-id="6f09e-130">Resource A</span></span>  | ![تقويم المورد A](media/reconcile-assignments-06.png) |
|<span data-ttu-id="6f09e-132">المورد B</span><span class="sxs-lookup"><span data-stu-id="6f09e-132">Resource B</span></span>  |  ![تقويم المورد B](media/reconcile-assignments-07.png) |
|<span data-ttu-id="6f09e-134">المورد C</span><span class="sxs-lookup"><span data-stu-id="6f09e-134">Resource C</span></span>  |  ![تقويم المورد C](media/reconcile-assignments-08.png) |
|<span data-ttu-id="6f09e-136">المورد D</span><span class="sxs-lookup"><span data-stu-id="6f09e-136">Resource D</span></span>  | ![تقويم المورد D](media/reconcile-assignments-09.png)  |
 
<span data-ttu-id="6f09e-138">وعند الانتقال إلى طريقة عرض **التسوية** ، يتم عرض تعيينات الموارد وغيرها من حالات نقص الحجز المرتبطة.</span><span class="sxs-lookup"><span data-stu-id="6f09e-138">When you navigate to the **Reconciliation** view, the resource assignments and the associated booking shortages are displayed.</span></span>

![طريقة عرض التسوية قبل التمديد](media/reconcile-assignments-10.png)

<span data-ttu-id="6f09e-140">وبعد أن يتم استخدام وظيفة توسيع الحجز لكل مورد، يتم بنجاح توسيع الحجوزات لكل مورد لأن ساعات عمل كل مورد تتداخل مع المخططات الزمنية للنقص.</span><span class="sxs-lookup"><span data-stu-id="6f09e-140">After the extend booking functionality has been used for each resource, bookings are successfully extended for each resource because each resource’s working hours overlapped with the contours of the shortage.</span></span>

![طريقة عرض التسوية بعد تمديد الحجز](media/reconcile-assignments-11.png) 

<span data-ttu-id="6f09e-142">لاحظ أن نظرة عن كثب على تفاصيل الحجوزات توضح الاختلافات في وقت بدء الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="6f09e-142">Notice that a closer look at the details of the bookings shows differences in the start time of the bookings.</span></span> <span data-ttu-id="6f09e-143">تبدأ الحجوزات في وقت لا يسبق البدء الخاص بالمخطط الزمني للتعيين وليس قبل وقت البدء المتوفر للمورد.</span><span class="sxs-lookup"><span data-stu-id="6f09e-143">The bookings start no earlier than the start time of the assignment contour and no earlier than the available start time of the resource.</span></span>

![حجوزات جديدة للموارد في لوحة الجدولة](media/reconcile-assignments-12.png)
