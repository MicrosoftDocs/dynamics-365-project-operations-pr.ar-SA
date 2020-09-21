---
title: كيف يمكنني إجراء "حجز مبدئي" للموارد في إصدار التطبيق 2.x؟
description: توضح هذه المقالة كيفية إجراء حجز مبدئي لأعضاء فريق المشروع باستخدام Project Service.
author: JohnPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.prod: Applies to Project Service version 2.x
ms.technology: ''
ms.assetid: 27063de4-cb0c-436f-970e-c87ebcab92db
ms.author: john.burrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: aad119c0907cdd31220a0d73e6e7d99ee63e2e13
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748665"
---
# <a name="how-do-i-soft-book-resources-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="f3a1a-103">كيف يمكنني إجراء "حجز مبدئي" للموارد في تطبيق ويب (الإصدار v2.x من تطبيق Project Service)؟</span><span class="sxs-lookup"><span data-stu-id="f3a1a-103">How do I "soft book" resources in the web app (Project Service app v2.x)?</span></span>

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="f3a1a-104">يمكنك إجراء "حجز مبدئي" لأحد الموارد في فريق المشروع لإظهار أنك تخطط لتعيين المورد للعمل على مشروع.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-104">You can tentatively schedule or "soft book" a resource onto a project team to show you plan to assign the resource to a project.</span></span> <span data-ttu-id="f3a1a-105">لا تستهلك الحجوزات المبدئية القدرة الإنتاجية المتوفرة لدى المورد.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-105">Soft bookings don’t consume a resource’s available capacity.</span></span> <span data-ttu-id="f3a1a-106">لا يمكن تعيين أعضاء الفريق الذين تم إجراء حجز مبدئي لهم لتنفيذ مهام المشروع.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-106">Soft-booked team members can’t be assigned to project tasks.</span></span> <span data-ttu-id="f3a1a-107">المورد الذي يمكن تعيينه لتنفيذ المهام هو فقط المورد بحالة "الحجز المحدد‬" ونوع الالتزام "ملتزم‬" (مع افتراض بأن لدى هذا المورد ساعات حجز محدد كافية لتغطية مجهود التعيين).</span><span class="sxs-lookup"><span data-stu-id="f3a1a-107">Only resources with the Status Hard Booked and Commit Type Committed can be assigned to tasks (assuming they have enough hard booking hours to cover the assignment effort).</span></span>

<span data-ttu-id="f3a1a-108">يظهر أعضاء فريق المشروع الذين تم إجراء حجز مبدئي لهم في شبكة "أعضاء فريق" وتظهر ساعات الحجز المبدئي في عمود "الحجز المبدئي".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-108">Soft-booked project team members show up in the Team Member grid with their soft-booked hours shown in the Soft Book column.</span></span> <span data-ttu-id="f3a1a-109">كما يظهر هؤلاء في لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-109">They also show up on the schedule board.</span></span> <span data-ttu-id="f3a1a-110">ومرة أخرى، لا توجد أي إشارة إلى استهلاك القدرة الإنتاجية لأن الحجز المبدئي لا يستهلك القدرة الإنتاجية للمورد.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-110">Again, they don’t indicate any consumption of capacity as soft-booking doesn’t consume capacity of a resource.</span></span>

<span data-ttu-id="f3a1a-111">هناك ثلاث طرق لإجراء حجز مبدئي لعضو الفريق للعمل على مشروع باستخدام الإصدار 2.x من Project Service.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-111">There are three ways to soft-book a team member onto a project with Project Service version 2.x.</span></span> <span data-ttu-id="f3a1a-112">يمكنك إجراء حجز مبدئي باستخدام لوحة الجدولة أو باستخدام ميزة المحافظة على الحجوزات‬ أو عن طريق إنشاء مورد عام.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-112">You can soft-book with the schedule board, use the Maintain Bookings feature, or by creating a generic resource.</span></span> <span data-ttu-id="f3a1a-113">هذه الطرق موضحة أدناه.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-113">These methods are described below.</span></span>

## <a name="soft-book-with-the-schedule-board"></a><span data-ttu-id="f3a1a-114">إجراء حجز مبدئي باستخدام لوحة الجدولة</span><span class="sxs-lookup"><span data-stu-id="f3a1a-114">Soft-book with the schedule board</span></span>

<span data-ttu-id="f3a1a-115">لإجراء حجز مبدئي باستخدام لوحة الجدولة‬، اتبع هذا الإجراء:</span><span class="sxs-lookup"><span data-stu-id="f3a1a-115">To soft-book with the schedule board, follow this procedure:</span></span> 
1. <span data-ttu-id="f3a1a-116">افتح لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-116">Open the schedule board.</span></span>
2. <span data-ttu-id="f3a1a-117">حدد علامة تبويب "المشروع" في لوحة "متطلبات الحجز‬" السفلى في لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-117">Select the Project tab on the bottom Booking Requirements panel of the schedule board.</span></span>
3. <span data-ttu-id="f3a1a-118">ابحث عن المشروع الذي تريد إجراء حجز مبدئي لأحد الموارد للعمل عليه.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-118">Find the project you wish to soft-book a resource on.</span></span> <span data-ttu-id="f3a1a-119">إذا كان لديك العديد من المشاريع، فانقر فوق رأس العمود "المشروع"، ثم استخدم عامل التصفية للبحث عن مشروعك.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-119">If you have many projects, click on the Project column header and then use the filter to find your project.</span></span>
4. <span data-ttu-id="f3a1a-120">انقر فوق المشروع، ثم اعمل على سحبه وإفلاته في شبكة الوقت الخاصة بالمورد.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-120">Click on the project, then drag and drop it on the resource’s time grid.</span></span>
5. <span data-ttu-id="f3a1a-121">يؤدي هذا إلى فتح لوحة "إنشاء حجز مورد‬" إلى اليسار.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-121">This opens the Create Resource Booking panel on the right.</span></span> <span data-ttu-id="f3a1a-122">اضبط تاريخي البدء والانتهاء، وحدد "مبدئي" لحالة الحجز، ثم حدد الساعات.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-122">Adjust the start and end date, select the Booking Status as Soft and set the hours.</span></span> 
6. <span data-ttu-id="f3a1a-123">انقر فوق "حجز".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-123">Click Book.</span></span>
7. <span data-ttu-id="f3a1a-124">بالعودة إلى المشروع، سيظهر المورد الآن كعضو فريق وستظهر ساعات الحجز المبدئي في عمود "الحجز المبدئي".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-124">Back on the project, the resource will now show as a team member with the soft booked hours in the Soft Book column.</span></span>

<span data-ttu-id="f3a1a-125">لاحظ أنه لا يمكنك تعيين هذا المورد لتنفيذ المهام في هيكل تنظيم العمل (WBS) إذ يجب إجراء حجز محدد له على الفريق لكي يتم تعيينه.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-125">Note that you can’t assign them to tasks on the work breakdown structure (WBS) as resources must be hard booked on the team to be assigned.</span></span>

## <a name="soft-book-using-the-maintain-bookings-feature"></a><span data-ttu-id="f3a1a-126">إجراء حجز مبدئي باستخدام ميزة المحافظة على الحجوزات‬</span><span class="sxs-lookup"><span data-stu-id="f3a1a-126">Soft-book using the Maintain Bookings feature</span></span>

<span data-ttu-id="f3a1a-127">لإجراء حجز مبدئي باستخدام ميزة المحافظة على الحجوزات‬، اتبع هذا الإجراء:</span><span class="sxs-lookup"><span data-stu-id="f3a1a-127">To soft-book with Maintain Bookings follow this procedure:</span></span>
1. <span data-ttu-id="f3a1a-128">من شبكة أعضاء الفريق، انقر فوق "جديد".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-128">From the team member grid, Click New.</span></span>
2. <span data-ttu-id="f3a1a-129">حدد المورد القابل للحجز، الدور، من/إلى.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-129">Select the bookable resource, role, from/to.</span></span>
3. <span data-ttu-id="f3a1a-130">حدد أسلوب توزيع غير "بلا":</span><span class="sxs-lookup"><span data-stu-id="f3a1a-130">Select an allocation method other than None:</span></span>
- <span data-ttu-id="f3a1a-131">القدرة الإنتاجية الكاملة</span><span class="sxs-lookup"><span data-stu-id="f3a1a-131">Full Capacity</span></span>
- <span data-ttu-id="f3a1a-132">النسبة المئوية للقدرة الإنتاجية</span><span class="sxs-lookup"><span data-stu-id="f3a1a-132">Percentage Capacity</span></span>
- <span data-ttu-id="f3a1a-133">توزيع بالتساوي حسب الساعات‬</span><span class="sxs-lookup"><span data-stu-id="f3a1a-133">By Hours Distribute Evenly</span></span>
- <span data-ttu-id="f3a1a-134">الحمل في البداية حسب الساعات</span><span class="sxs-lookup"><span data-stu-id="f3a1a-134">By Hours Front Load</span></span>
4. <span data-ttu-id="f3a1a-135">انقر فوق "حفظ".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-135">Click Save.</span></span> <span data-ttu-id="f3a1a-136">سوف تشاهد المورد على شبكة الفريق مع الإشارة إلى ساعات حجزه كحجز محدد.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-136">You’ll see the resource on the team grid and their hours indicated as Hard.</span></span>
5. <span data-ttu-id="f3a1a-137">انقر فوق "المحافظة على الحجوزات‬" للمحافظة على حجوزات المورد.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-137">Maintain the resource’s bookings by clicking Maintain Bookings.</span></span>
6. <span data-ttu-id="f3a1a-138">عندما تفتح لوحة الجدولة، قم بتوسيع المورد لعرض حجوزاته.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-138">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="f3a1a-139">سوف تشاهد الحجز المشار إليه كحجز محدد.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-139">You will see the booking indicated as Hard.</span></span>
7. <span data-ttu-id="f3a1a-140">انقر بزر الماوس الأيمن فوق الحجز، وضمن "تغيير الحالة"، حدد "حجز مبدئي" ثم "مبدئي".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-140">Right-click the booking, under Change Status, select Soft Book and then Soft.</span></span> <span data-ttu-id="f3a1a-141">أصبحت حالة الحجز الآن "مبدئي".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-141">The booking status is now Soft.</span></span>
8. <span data-ttu-id="f3a1a-142">بعد إغلاق لوحة الجدولة، سترى أن ساعات المورد قد تغيرت من "محدد" إلى "مبدئي" على شبكة أعضاء الفريق.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-142">After closing the schedule board, you’ll see that the hours for the resource have changed from Hard to Soft on the team member grid.</span></span>
<span data-ttu-id="f3a1a-143">لاحظ أنك إذا أجريت حجزًا محددًا لمورد في الفريق، ثم قمت بتعيين مهام إليه في هيكل تنظيم العمل (WBS)، عندما تستخدم خيار "المحافظة على الحجوزات" لتغيير حالة الحجز من "محدد" إلى "مبدئي"، سيؤدي ذلك إلى إزالة التعيينات من المهام لذلك المورد، إذ يمكن تعيين الموارد لتنفيذ المهام فقط إذا كانت حالة الحجز "محدد".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-143">Note that if you hard book a resource onto the team and then assign them tasks in the WBS, when you use maintain bookings to change the status of Hard to Soft, it will remove the assignments from the tasks for that resource, as only hard booked resources can be assigned to tasks.</span></span>

## <a name="soft-book-by-creating-a-generic-resource"></a><span data-ttu-id="f3a1a-144">إجراء حجز مبدئي عن طريق إنشاء مورد عام</span><span class="sxs-lookup"><span data-stu-id="f3a1a-144">Soft-book by creating a generic resource</span></span>

<span data-ttu-id="f3a1a-145">يمكنك إنشاء حجز مبدئي عن طريق إنشاء عضو فريق مورد عام والتنفيذ بواسطة لوحة الجدولة أو طلب المورد‬ وتغيير النوع أثناء الحجز.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-145">You can create a soft-booking by generating a generic resource team member, fulfilling with schedule board or Resource Request and changing the type during the booking.</span></span>
<span data-ttu-id="f3a1a-146">للقيام بذلك، استخدم الإجراء التالي:</span><span class="sxs-lookup"><span data-stu-id="f3a1a-146">To do this, use the following procedure:</span></span>

1. <span data-ttu-id="f3a1a-147">في هيكل تنظيم العمل (WBS) الخاص بالمشروع، قم بتعيين الأدوار إلى المهام التي ترغب في إنشاء أعضاء فريق عام لها.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-147">On the project WBS, assign roles to the tasks you wish to generate generic team members for.</span></span>
2. <span data-ttu-id="f3a1a-148">انقر فوق "إنشاء فريق المشروع".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-148">Click Generate Project Team.</span></span>
3. <span data-ttu-id="f3a1a-149">في شبكة أعضاء فريق المشروع، حدد المورد العام وانقر فوق "حجز".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-149">On the project team member grid, select the generic resource and click Book.</span></span>
4. <span data-ttu-id="f3a1a-150">في لوحة الجدولة، حدد المورد الذي ترغب في حجزه.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-150">On the schedule board, select the resource that you wish to book.</span></span>
5. <span data-ttu-id="f3a1a-151">في لوحة "إنشاء حجز مورد‬" في لوحة الجدولة، غيّر "حالة الحجز" إلى "مبدئي".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-151">On the schedule board’s Create Resource Booking panel, change the Booking Status to Soft.</span></span>
6. <span data-ttu-id="f3a1a-152">انقر فوق "حجز" أو فوق " "حجز وخروج".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-152">Click Book or Book and Exit.</span></span>

<span data-ttu-id="f3a1a-153">بعد إغلاق لوحة الجدولة، سترى أن المورد المحدد قد أضيف إلى الفريق مع ساعات الحجز المبدئي بالإضافة إلى الساعات المعينة.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-153">After closing the schedule board, you’ll see the selected resource added to the team with Soft booked hours as well as assigned hours.</span></span> <span data-ttu-id="f3a1a-154">سوف ترى أيضًا أن المورد العام يبقى في الفريق كمؤشر على تعيين المهام إلى عضو فريق تم إجراء حجز مبدئي له.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-154">You’ll also see that the generic resource remains on the team as an indicator that the tasks are assigned to a soft-booked team member.</span></span>

<span data-ttu-id="f3a1a-155">عندما تصبح مستعدًا لتغيير مورد عضو فريق بحجز مبدئي إلى عضو فريق بحجز محدد لكي تتمكن من تعيين مهام له، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="f3a1a-155">When you’re ready to change a soft-booked team member resource to a hard-booked team member so that you can assign them to tasks, do the following:</span></span>

1. <span data-ttu-id="f3a1a-156">حدد هذا المورد ثم انقر فوق "المحافظة على الحجوزات".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-156">Select that resource and click Maintain Bookings.</span></span>
2. <span data-ttu-id="f3a1a-157">عندما تفتح لوحة الجدولة، قم بتوسيع المورد لعرض حجوزاته.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-157">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="f3a1a-158">سوف تشاهد الحجز وعليه علامة حجز "مبدئي".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-158">You’ll see the booking marked as Soft.</span></span>
3. <span data-ttu-id="f3a1a-159">انقر بزر الماوس الأيمن فوق الحجز، وضمن "تغيير الحالة"، حدد "حجز محدد" ثم "محدد".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-159">Right-click the booking, under Change Status, select Hard Book and then Hard.</span></span> <span data-ttu-id="f3a1a-160">أصبحت حالة الحجز الآن "محدد".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-160">The booking status is now Hard.</span></span>
4. <span data-ttu-id="f3a1a-161">بعد إغلاق لوحة الجدولة، سترى أن ساعات المورد قد تغيرت من "مبدئي" إلى "محدد" على شبكة أعضاء الفريق.</span><span class="sxs-lookup"><span data-stu-id="f3a1a-161">After closing the schedule board, you’ll see that the hours for the resource have changed from Soft to Hard on the team member grid.</span></span> <span data-ttu-id="f3a1a-162">يمكنك الآن تعيين المورد لتنفيذ المهام (شريطة وجود توافق بين ساعات الحجز المحدد وساعات المجهود في المهمة المطلوب تعيينها).</span><span class="sxs-lookup"><span data-stu-id="f3a1a-162">You may now assign the resource to tasks (provided there is alignment between the hard-booked hours and the effort hours of the task for assignment).</span></span> <span data-ttu-id="f3a1a-163">لاحظ أنك إذا تابعت خطوات التنفيذ للمورد العام في البند 3 أعلاه، فإن عضو الفريق العام سيُزال من الفريق عندما تقوم بتغيير حالة المورد القابل للحجز من "مبدئي" إلى "محدد".</span><span class="sxs-lookup"><span data-stu-id="f3a1a-163">Note that if you followed the generic resource fulfilment steps in item #3 above, when you change the status of the soft-booked bookable resource to hard, the generic team member is removed from the team.</span></span>
