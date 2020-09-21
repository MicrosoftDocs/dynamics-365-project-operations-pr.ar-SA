---
title: إنشاء حجز مشروع من لوحة الجدولة
description: يقدم هذا الموضوع معلومات حول كيفية إنشاء حجز مشروع من لوحة الجدولة.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.prod: Dynamics 365 Project Service Automation 2.x and 3.x
ms.technology: ''
ms.assetid: bbc1bbe2-3482-4b84-9e89-f7e0e585ade8
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 7b6c7e07ea6451e0654ccf1ba7be10e7b38e0d09
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748714"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a><span data-ttu-id="c7ceb-103">إنشاء حجز مشروع من لوحة الجدولة</span><span class="sxs-lookup"><span data-stu-id="c7ceb-103">Create a project booking from the Schedule board</span></span>

<span data-ttu-id="c7ceb-104">يمكنك حجز مورد للعمل على مشروع مباشرة على علامة التبويب **فريق المشروع** للمشروع أو عن طريق إنشاء متطلبات المورد من تعيين عضو فريق عام ثم تنفيذ المتطلبات الناشئة بواسطة أحد أعضاء فريق مشروع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-104">You can book a resource onto a project directly from the **Team** tab of the project or by generating a resource requirement from a generic team member assignment and then fulfilling the generated requirement with a project team member.</span></span>

<span data-ttu-id="c7ceb-105">يمكنك أيضًا حجز مورد للعمل على مشروع مباشرة من لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-105">You can also book a resource onto a project directly from the Schedule board.</span></span> <span data-ttu-id="c7ceb-106">وهناك ثلاث طرق للتعامل للقيام بذلك:</span><span class="sxs-lookup"><span data-stu-id="c7ceb-106">There are three ways to do this:</span></span>

- <span data-ttu-id="c7ceb-107">**‏‫الحجز من متطلبات موارد ناشئة‬:** يمكنك إنشاء مطلب مورد بعد إنشاء مورد عام وتعيين المهام داخل مشروع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-107">**Book from a generated resource requirement:** You can generate a resource requirement after you create a generic resource and assign tasks within a project.</span></span>

- <span data-ttu-id="c7ceb-108">**الحجز من المتطلبات الأساسية‬:** تظهر المتطلبات الاساسية في لوحة الجدولة بعلامة تبويب " **المشروع** ".</span><span class="sxs-lookup"><span data-stu-id="c7ceb-108">**Book from the primary requirement:** The primary requirements show up on the Schedule board on the **Project** tab.</span></span> 

- <span data-ttu-id="c7ceb-109">**‏‫الحجز من متطلبات موارد جديدة‬:** يمكنك إنشاء مطلب مورد من الصفر وإقرانه بمشروع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-109">**Book from a new resource requirement:** You can create a resource requirement from scratch and associate it with a project.</span></span> <span data-ttu-id="c7ceb-110">في لوحة الجدولة، تظهر متطلبات الموارد على علامة التبويب **المتطلبات المفتوحة‬**.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-110">On the Schedule board, the resource requirement shows up on the **Open Requirements** tab.</span></span>

## <a name="book-from-a-generated-resource-requirement"></a><span data-ttu-id="c7ceb-111">الحجز من متطلبات موارد ناشئة</span><span class="sxs-lookup"><span data-stu-id="c7ceb-111">Book from a generated resource requirement</span></span>

<span data-ttu-id="c7ceb-112">يمكنك إنشاء مورد عام وتعيينه مهمة أو أكثر داخل مشروع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-112">You can create a generic resource and assign it one or more tasks within a project.</span></span> <span data-ttu-id="c7ceb-113">بعد ذلك يمكنك إنشاء متطلب مورد من عضو الفريق العام.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-113">Then you can generate a resource requirement from the generic team member.</span></span> 

1.  <span data-ttu-id="c7ceb-114">على لوحة الجدولة، سيظهر هذا المورد في علامة تبويب **المتطلبات المفتوحة**. وقد تحتاج إلى استخدام عوامل تصفية الأعمدة على الشبكة إذا كان لديك الكثير من المتطلبات مفتوحة.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-114">On the Schedule board, this resource will show up on the **Open Requirements** tab. You might need to use column filters on the grid if you have many open requirements.</span></span> 

    <span data-ttu-id="c7ceb-115">![افتح علامة تبويب المتطلبات على لوحة الجدولة](media/FAQ-Project-Booking-Schedule-Board-1.png "لقطة شاشة لجدول الحجوزات والتعيينات")</span><span class="sxs-lookup"><span data-stu-id="c7ceb-115">![Open Requirements tab on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-1.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="c7ceb-116">حدد المتطلبات.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-116">Select the requirement.</span></span> <span data-ttu-id="c7ceb-117">سوف تظهر علامة التبويب **بحث عن التوافر‬** في الجزء العلوي من الصف المحدد.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-117">The **Find Availability** tab will appear at the top of the selected row.</span></span>
 
3. <span data-ttu-id="c7ceb-118">عندما تحدد علامة التبويب، يتم فتح وضع "مساعد الجدولة" في لوحة الجدولة ثم تصفية الموارد المتاحة التي تتوافق مع متطلبات الموارد.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-118">When you select the tab, the Schedule Assistant mode of the Schedule board opens and then filters the available resources that meet the resource requirement.</span></span> <span data-ttu-id="c7ceb-119">بعد ذلك، يمكنك حجز مورد.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-119">After that, you can book a resource.</span></span>

4. <span data-ttu-id="c7ceb-120">يمكنك أيضًا سحب وإفلات الصف المحدد من أسفل لوحة الجدولة إلى خلية مورد في الشبكة أعلاه.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-120">You can also drag and drop the selected row from the bottom of the Schedule board to a resource cell in the grid above.</span></span> <span data-ttu-id="c7ceb-121">عند إفلاتها، تفتح لوحة **إنشاء حجز مورد** إلى اليسار.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-121">When you drop it, it opens the **Create Resource Booking** panel on the right.</span></span>

    <span data-ttu-id="c7ceb-122">يؤدي تحديد **حجز** إلى حجز‏‎ المورد في فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-122">Selecting **Book** books the resource onto the project team.</span></span>

![لوحة إنشاء حجز مورد](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a><span data-ttu-id="c7ceb-124">الحجز من المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="c7ceb-124">Book from the Primary Requirement</span></span>

<span data-ttu-id="c7ceb-125">يؤدي إنشاء مشروع في Project Service إلى إنشاء متطلبات الموارد بشكل تلقائي، وتسمى هذه المتطلبات الأساسية.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-125">Creating a project in Project Service automatically creates a resource requirement called the Primary Requirement.</span></span> <span data-ttu-id="c7ceb-126">هذا متطلب فارغ يتم استخدامه لحجز مورد بسرعة باستخدام لوحة الجدولة من دون إنشاء متطلب أو إنشائه من الصفر.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-126">This is an empty requirement that is used to quickly book a resource with the Schedule board without generating a requirement or creating one from scratch.</span></span> <span data-ttu-id="c7ceb-127">وبما أن المتطلب فارغ، ستحتاج إلى تحديد التواريخ بالإضافة إلى أسلوب التوزيع والساعات، إذا كان ذلك ممكنًا.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-127">Because the requirement is empty, you’ll need to specify dates as well as the allocation method and hours, if applicable.</span></span> 

1. <span data-ttu-id="c7ceb-128">لحجز مورد مع المتطلبات الأساسية، على لوحة الجدولة، حدد علامة تبويب **المشروع**. قد تحتاج إلى استخدام عوامل تصفية الأعمدة على عمود **المشروع** إذا كان لديك العديد من المشاريع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-128">To book a resource with the Primary Requirement, on the Schedule board, select the **Project** tab. You might need to use the column filter on the **Project** column if you have many projects.</span></span>

   <span data-ttu-id="c7ceb-129">![عوامل تصفية العمود على لوحة الجدولة](media/FAQ-Project-Booking-Schedule-Board-2.png "لقطة شاشة لجدول الحجوزات والتعيينات")</span><span class="sxs-lookup"><span data-stu-id="c7ceb-129">![Column filters on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-2.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="c7ceb-130">حدد فقط المتطلبات التي لها اسم المشروع ومدتها صفر (0).</span><span class="sxs-lookup"><span data-stu-id="c7ceb-130">Select the requirement that only has the project name as its name and has a duration of zero (0).</span></span>

3. <span data-ttu-id="c7ceb-131">حدد علامة التبويب **بحث عن التوافر‬** التي تظهر على الصف.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-131">Select the **Find Availability** tab that appears on the row.</span></span> <span data-ttu-id="c7ceb-132">يؤدي هذا إلى وضع لوحة الجدولة في وضع "مساعد الجدولة" وعرض الموارد المتوفرة التي يمكن حجزها للمشروع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-132">This puts the Schedule board in Schedule Assistant mode and shows the available resources that can be booked onto the project.</span></span>

4. <span data-ttu-id="c7ceb-133">بما أن **المتطلب الأساسي** عبارة عن متطلب فارغ ومدته صفر (0)، ستحتاج إلى تعيين المدة على لوحة **إنشاء حجز مورد**" عند تحديد مورد وحجزه.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-133">Because a **Primary Requirement** is an empty requirement with zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when selecting and booking a resource.</span></span>

5. <span data-ttu-id="c7ceb-134">يمكنك أيضًا تحديد **المتطلب الأساسي للمشروع** في الجزء السفلي من لوحة الجدولة وسحبه وإفلاته على مورد لحجزه.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-134">You can also select the **Project Primary Requirement** at the bottom of the Schedule board and drag and drop it on a resource to book it.</span></span>
 
    <span data-ttu-id="c7ceb-135">بما أن **المتطلب الأساسي** عبارة عن متطلب فارغ ومدته صفر (0)، ستحتاج إلى تعيين المدة على لوحة **إنشاء حجز مورد**" عندما تقوم بتحديد مورد وحجزه.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-135">Because the **Primary Requirement** is an empty requirement that has zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when you select and book a resource.</span></span>
 
    <span data-ttu-id="c7ceb-136">عند حجز مورد من خلال **المتطلب الأساسي** في لوحة الجدولة، فأنت تضيفه إلى فريق المشروع من دون أية تعيينات.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-136">When you book a resource through the **Primary Requirement** on the Schedule board, you add it to the project team without any assignments.</span></span>
 
## <a name="book-from-a-new-resource-requirement"></a><span data-ttu-id="c7ceb-137">الحجز من متطلبات موارد جديدة</span><span class="sxs-lookup"><span data-stu-id="c7ceb-137">Book from a new resource requirement</span></span>
<span data-ttu-id="c7ceb-138">أكمل الخطوات التالية للحجز من متطلب مورد جديد.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-138">Complete the following steps to book from a new resource requirement.</span></span> 

1. <span data-ttu-id="c7ceb-139">انتقل إلى **متطلبات الموارد** ثم حدد **جديد** لإنشاء متطلب مورد جديد.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-139">Go to **Resource Requirements**, and then select **New** to create a new resource requirement.</span></span>

2. <span data-ttu-id="c7ceb-140">من علامة تبويب **المشروع**، حدد مشروعا لاقران المتطلبات بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-140">On the **Project** tab, select a project to associate the requirement to the project.</span></span>
 
    <span data-ttu-id="c7ceb-141">في لوحة الجدولة، يظهر هذا المتطلب الجديد كـ **متطلب مفتوح** والذي يمكنك استيفاؤه.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-141">On the Schedule board, this new requirement shows as an **Open Requirement** that you can fulfill.</span></span>

3. <span data-ttu-id="c7ceb-142">احجز المورد لإضافته إلى فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-142">Book the resource to add it to the project team.</span></span>

4. <span data-ttu-id="c7ceb-143">الآن وبعد أن تم حجز المورد، يجب تعيين المهام إليه يدويًا.</span><span class="sxs-lookup"><span data-stu-id="c7ceb-143">Now that the resource is booked, you must assign tasks manually.</span></span>

