---
title: كيف يمكنني تعيين مورد قابل للحجز لمهمة في تطبيق الويب
description: نظرة عامة حول الطرق التي يمكنك من خلالها تعيين موارد قابلة للحجز.
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 32a04ddef901515cd77262b5ae6be2458cb6b00c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993266"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="62f7d-103">كيف يمكنني تعيين مورد قابل للحجز لتنفيذ مهمة في تطبيق ويب (الإصدار v2.x من تطبيق Project Service)؟‬</span><span class="sxs-lookup"><span data-stu-id="62f7d-103">How do I assign a bookable resource to a task in the web app (Project Service app v2.x)?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="62f7d-104">هناك طريقتان لتعيين مورد لتنفيذ مهمة في Project Service.</span><span class="sxs-lookup"><span data-stu-id="62f7d-104">There are two ways to assign a resource to a task in Project Service.</span></span> <span data-ttu-id="62f7d-105">يمكنك حجز مورد كعضو فريق وتعيينه لتنفيذ مهمة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-105">You can book a resource as a team member and then assign it to a task.</span></span> <span data-ttu-id="62f7d-106">أو، يمكنك إنشاء عضو فريق عام من خلال تعيينات الأدوار على المهام، وإنشاء فريق، ثم تنفيذ متطلبات المساعدة بواسطة مورد مسمى.</span><span class="sxs-lookup"><span data-stu-id="62f7d-106">Or, you can create a generic team member through role assignment on tasks, generate a team, and then fulfill the backing requirements with a named resource.</span></span>

<span data-ttu-id="62f7d-107">إذا كنت ترغب في تعيين مورد قابل للحجز لتنفيذ مهمة، فيجب أن يتوفر لعضو فريق الموارد القابلة للحجز حجوزات متوفرة كافية.</span><span class="sxs-lookup"><span data-stu-id="62f7d-107">Note that if you’d like to assign a bookable resource to a task, the bookable resource team member must have enough available bookings.</span></span> <span data-ttu-id="62f7d-108">يجب أن تكون حالة الحجز المورد "الحجز المحدد‬" ونوع الالتزام "ملتزم‬".</span><span class="sxs-lookup"><span data-stu-id="62f7d-108">The status of the booking must be Commit Type Hard Book and Status Committed.</span></span> <span data-ttu-id="62f7d-109">في حالة عدم وجود عدد كافٍ من الحجوزات للمورد، تزيل خدمة Project Service التعيين وتعرض رسالة الخطأ التالية:</span><span class="sxs-lookup"><span data-stu-id="62f7d-109">If there aren’t enough bookings for the resource, Project Service removes the assignment and displays the following error message:</span></span>

<span data-ttu-id="62f7d-110">*يتعذر تعيين مورد إلى هذه المهمة - لا تتوفر لدى المورد التالي (الموارد التالية) ساعات كافية محجوزة للعمل على مشروع*</span><span class="sxs-lookup"><span data-stu-id="62f7d-110">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project*</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="62f7d-111">حجز مورد كعضو فريق وتعيينه لتنفيذ مهمة</span><span class="sxs-lookup"><span data-stu-id="62f7d-111">Book a resource as a team member and then assign the resource to a task</span></span>

<span data-ttu-id="62f7d-112">باستخدام هذه الطريقة، يمكنك إضافة مورد إلى فريق المشروع ثم تعيين المهام إلى المورد في جدول المشروع.</span><span class="sxs-lookup"><span data-stu-id="62f7d-112">With this method you add a resource to the project team and then assign tasks to the resource in the project schedule.</span></span> <span data-ttu-id="62f7d-113">وإليك كيفية القيام بذلك:</span><span class="sxs-lookup"><span data-stu-id="62f7d-113">Here’s how you do this:</span></span>
1.  <span data-ttu-id="62f7d-114">على شبكة أعضاء الفريق، أضف عضو فريق جديدًا بتحديد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="62f7d-114">On the team member grid, add a new team member by selecting **New**.</span></span>
2.  <span data-ttu-id="62f7d-115">في شاشة الإنشاء السريع لعضو الفريق، حدد اسم المورد القابل للحجز وعيّن له دورًا.</span><span class="sxs-lookup"><span data-stu-id="62f7d-115">On the Team Member Quick Create screen, select the bookable resource name and set a role.</span></span>
3.  <span data-ttu-id="62f7d-116">حدد التاريخين **من** و **إلى**.</span><span class="sxs-lookup"><span data-stu-id="62f7d-116">Select the **From** and **To** dates.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="62f7d-117">![لقطه شاشة لإضافة عضو فريق](media/FAQ-Resources-to-Tasks2-1.png "لقطه شاشة لإضافة عضو فريق")</span><span class="sxs-lookup"><span data-stu-id="62f7d-117">![Screenshot of adding team member](media/FAQ-Resources-to-Tasks2-1.png "Screenshot of adding team member")</span></span>
 
4.  <span data-ttu-id="62f7d-118">حدد أحد أساليب التوزيع التالية لحجز المورد:</span><span class="sxs-lookup"><span data-stu-id="62f7d-118">Select one of the following allocation methods for booking the resource:</span></span>
    - <span data-ttu-id="62f7d-119">**القدرة الإنتاجية الكاملة** هذا الأسلوب يحجز القدرة الإنتاجية الكاملة للمورد لتواريخ "من" و"إلى" المحددة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-119">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="62f7d-120">**النسبة المئوية للقدرة الإنتاجية‬** هذا الأسلوب يحجز المورد للنسبة المئوية من القدرة الإنتاجية لتواريخ "من" و"إلى" المحددة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-120">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="62f7d-121">**توزيع بالتساوي حسب الساعات‬‬** هذا الأسلوب يحجز المورد لعدد محدد من الساعات، ويؤدي إلى توزيع الوقت بطريقة متساوية لكل يوم على مدى تواريخ "من" و"إلى" المحددة.‬</span><span class="sxs-lookup"><span data-stu-id="62f7d-121">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing it evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="62f7d-122">**الحمل في البداية حسب الساعات‬** هذا الأسلوب يحجز المورد لعدد محدد من الساعات، ويؤدي إلى توزيع الحمل في البداية لساعات العمل لكل يوم على مدى تواريخ "من" و"إلى" المحددة.‬</span><span class="sxs-lookup"><span data-stu-id="62f7d-122">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>

    <span data-ttu-id="62f7d-123">لا تحدد **بلا** لأن هذا الأسلوب يضيف المورد إلى الفريق، ولكنه لا ينشئ أية حجوزات تستوعب القدرة الإنتاجية للمورد.</span><span class="sxs-lookup"><span data-stu-id="62f7d-123">Don’t select **None** because it adds the resource to the team but doesn’t create any bookings that absorb the resource's capacity.</span></span>
5.  <span data-ttu-id="62f7d-124">حدد **حفظ.**.</span><span class="sxs-lookup"><span data-stu-id="62f7d-124">Select **Save**.</span></span>

    <span data-ttu-id="62f7d-125">تجدر الإشارة إلى أن ساعات الحجز يجب أن تكون كافية لتغطية ساعات المجهود ونطاقات التواريخ الخاصة بالمهام التي تعيّن المورد لتنفيذها.</span><span class="sxs-lookup"><span data-stu-id="62f7d-125">Note that the hours of the booking must be enough to cover the effort hours and date ranges of the tasks that you assign this resource to.</span></span> <span data-ttu-id="62f7d-126">إذا لم تكن متماشية، فلا يمكنك تعيين المورد لتنفيذ المهمة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-126">If they aren’t in alignment, you can’t assign the resource to the task.</span></span>

6.  <span data-ttu-id="62f7d-127">في هيكل تنظيم العمل (WBS) للمهمة، انقر فوق القائمة المنسدلة لخلية المورد.</span><span class="sxs-lookup"><span data-stu-id="62f7d-127">On the work breakdown structure (WBS) for the task, click the resource cell dropdown.</span></span> <span data-ttu-id="62f7d-128">ثم:</span><span class="sxs-lookup"><span data-stu-id="62f7d-128">Then:</span></span> 

    1. <span data-ttu-id="62f7d-129">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="62f7d-129">Select **Add**.</span></span>
    2. <span data-ttu-id="62f7d-130">حدد القائمة المنسدلة تحت **الموارد** وحدد عضو الفريق الذي أضفته أعلاه.</span><span class="sxs-lookup"><span data-stu-id="62f7d-130">Select the dropdown under **Resources** and select the team member you added above.</span></span>
    3. <span data-ttu-id="62f7d-131">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="62f7d-131">Select **OK**.</span></span> <span data-ttu-id="62f7d-132">تم الآن تعيين عضو الفريق لتنفيذ المهمة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-132">The team member is now assigned to the task.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="62f7d-133">![لقطه شاشة لإضافة موارد باستخدام WBS](media/FAQ-Resources-to-Tasks2-2.png "لقطه شاشة لإضافة موارد باستخدام WBS")</span><span class="sxs-lookup"><span data-stu-id="62f7d-133">![Screenshot of adding resources with WBS](media/FAQ-Resources-to-Tasks2-2.png "Screenshot of adding resources with WBS")</span></span>
 
<span data-ttu-id="62f7d-134">على شبكة أعضاء الفريق، سوف ترى تجميع الساعات المعينة للمورد ضمن "الساعات المعينة‬".</span><span class="sxs-lookup"><span data-stu-id="62f7d-134">On the team member grid, you’ll see the aggregate of the resource’s assigned hours under Assigned Hours.</span></span> <span data-ttu-id="62f7d-135">وسيكون عددها أقل من الساعات المحجوزة للمورد أو مساويًا لها.</span><span class="sxs-lookup"><span data-stu-id="62f7d-135">It will be less than or equal to the booked hours for the resource.</span></span> 

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="62f7d-136">![لقطه شاشة للساعات المعينة لأحد الموارد](media/FAQ-Resources-to-Tasks2-3.png "لقطه شاشة للساعات المعينة لأحد الموارد")</span><span class="sxs-lookup"><span data-stu-id="62f7d-136">![Screenshot of assigned hours for a resource](media/FAQ-Resources-to-Tasks2-3.png "Screenshot of assigned hours for a resource")</span></span>
 
<span data-ttu-id="62f7d-137">إذا كان موعد بدء المهمة التي تحاول تعيينها إلى المورد يقع بعد تاريخ انتهاء حجوزات الموارد، فلن يظهر المورد في القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-137">If the task you’re attempting to assign to the resource starts after the end date of the resources bookings, the resource won’t appear in the dropdown.</span></span>

<span data-ttu-id="62f7d-138">لاحظ أنه يمكنك تعيين أحد الموارد بحيث يعمل لساعات تزيد عن عدد ساعاته المحجوزة إذا كان لديه قدرة إنتاجية متبقية غير معينة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-138">Note that you can assign a resource to more hours than their booked hours if the resource has some remaining unassigned capacity.</span></span> <span data-ttu-id="62f7d-139">وفي هذه الحالة، سيكون المورد في وضع المعيّن بشكل جزئي إلى حجوزاته.</span><span class="sxs-lookup"><span data-stu-id="62f7d-139">In this case the resource will only be partially assigned up to their bookings.</span></span> <span data-ttu-id="62f7d-140">يمكنك الاطلاع على ساعات المهام المتبقية غير المعينة هذه عن طريق إضافة العمود "الساعات الناقصة‬" إلى هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="62f7d-140">You can see these remaining unassigned task hours by adding the Unstaffed Hours column to the work breakdown structure.</span></span>

<span data-ttu-id="62f7d-141">إذا تم تعيين الموارد إلى ساعاتهم المحجوزة (تساوي ساعاتهم المحجوزة ساعاتهم المعينة)، سوف ترى رسالة الخطأ التالية عندما تحاول تعيين مهام إضافية لهم:</span><span class="sxs-lookup"><span data-stu-id="62f7d-141">If resources are assigned to their booked hours (their booked hours equals their assigned hours), you’ll see the following error message when you attempt to assign them further tasks:</span></span>

<span data-ttu-id="62f7d-142">*يتعذر تعيين مورد إلى هذه المهمة - لا تتوفر لدى المورد التالي (الموارد التالية) ساعات كافية محجوزة للعمل على مشروع.*</span><span class="sxs-lookup"><span data-stu-id="62f7d-142">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project.*</span></span>

<span data-ttu-id="62f7d-143">بالإضافة إلى ذلك، يُضاف عضو فريق مدير المشروع الافتراضي الذي تمت إضافته إلى الفريق عندما أنشأت المشروع من دون أي حجوزات ولا يمكن تعيينه للعمل على أي مهمة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-143">Additionally, the default project manager team member that is added to the team when you create the project is added without any bookings and can’t be assigned to any task.</span></span> <span data-ttu-id="62f7d-144">ولن يظهر في قائمة المورد المنسدلة للمهام.</span><span class="sxs-lookup"><span data-stu-id="62f7d-144">They won’t show up in the resource dropdown for tasks.</span></span>

<span data-ttu-id="62f7d-145">إذا أردت تعيين هذا المورد، فيجب إزالته من الفريق ثم إعادة إضافته باستخدام أسلوب توزيع آخر غير "بلا".</span><span class="sxs-lookup"><span data-stu-id="62f7d-145">If you want to assign this resource, you need to remove them from the team and then re-add them with an allocation method other than None.</span></span> <span data-ttu-id="62f7d-146">ويعود سبب إضافته إلى الفريق عند إنشاء المشروع إلى وجود موافق على المشروع واحد على الأقل بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="62f7d-146">The reason they’re added to the team when the project is created is so that a project has at least one project approver by default.</span></span>

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a><span data-ttu-id="62f7d-147">إنشاء عضو فريق عام من خلال تعيينات الأدوار على المهام</span><span class="sxs-lookup"><span data-stu-id="62f7d-147">Create a generic team member through role assignment on tasks</span></span>

<span data-ttu-id="62f7d-148">يضمن هذا الأسلوب وجود حجوزات كافية للمهام لدى الموارد.</span><span class="sxs-lookup"><span data-stu-id="62f7d-148">This method assures that resources have enough bookings for tasks.</span></span> <span data-ttu-id="62f7d-149">أولاً، تنشئ موردًا نائبًا أو عامًا يصف خصائص المورد المسمى الذي تريده في النهاية أن يعمل على المهام عن طريق إنشاء فريق بعد تعيين الأدوار إلى المهام.</span><span class="sxs-lookup"><span data-stu-id="62f7d-149">First, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks by generating a team after assigning roles to tasks.</span></span> <span data-ttu-id="62f7d-150">وإليك كيفية القيام بذلك:</span><span class="sxs-lookup"><span data-stu-id="62f7d-150">Here’s how you do this:</span></span>

1. <span data-ttu-id="62f7d-151">في هيكل تنظيم العمل، حدد مهمة.</span><span class="sxs-lookup"><span data-stu-id="62f7d-151">On the work breakdown structure, select a task.</span></span>
2. <span data-ttu-id="62f7d-152">حدد أيقونة القائمة المنسدلة **الدور المعين** في خلية المورد.</span><span class="sxs-lookup"><span data-stu-id="62f7d-152">Select the **Assigned Role** dropdown icon in the resource cell.</span></span>
3. <span data-ttu-id="62f7d-153">حدد القائمة المنسدلة **الدور** وحدد الدور للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="62f7d-153">Select the **Role** dropdown and select the role for the generic resource.</span></span>
4. <span data-ttu-id="62f7d-154">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="62f7d-154">Select **OK**.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="62f7d-155">![لقطه شاشة لاستخدام WBS‏‎ لإضافة مورد](media/FAQ-Resources-to-Tasks2-4.png "لقطه شاشة لاستخدام WBS‏‎ لإضافة مورد")</span><span class="sxs-lookup"><span data-stu-id="62f7d-155">![Screenshot of using WBS to add resource](media/FAQ-Resources-to-Tasks2-4.png "Screenshot of using WBS to add resource")</span></span>
 
<span data-ttu-id="62f7d-156">بعد الانتهاء من تعيين أدوار إلى المهام في هيكل تنظيم العمل (WBS)، حدد **إنشاء فريق المشروع**.</span><span class="sxs-lookup"><span data-stu-id="62f7d-156">Once you’ve completed assigning roles to the tasks in the WBS, select **Generate Project Team**.</span></span> <span data-ttu-id="62f7d-157">تنشئ خدمة Project Service الحد الأدنى لعدد أعضاء الفريق العام استنادًا إلى الأدوار والوحدات التنظيمية للموارد وتقويم المشروع عن طريق تجميع تعيينات المهام.</span><span class="sxs-lookup"><span data-stu-id="62f7d-157">Project Service creates the minimum number of generic team members based on the roles, resourcing organization units, and project calendar by aggregating the task assignments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="62f7d-158">![لقطه شاشة لإنشاء فريق مشروع](media/FAQ-Resources-to-Tasks2-5.png "لقطه شاشة لإنشاء فريق مشروع")</span><span class="sxs-lookup"><span data-stu-id="62f7d-158">![Screenshot of generating project team](media/FAQ-Resources-to-Tasks2-5.png "Screenshot of generating project team")</span></span>
 
<span data-ttu-id="62f7d-159">على شبكة أعضاء الفريق، سترى موارد من نوع "مورد عام" مع الدور واسم المنصب.</span><span class="sxs-lookup"><span data-stu-id="62f7d-159">On the Team Member grid, you’ll see resources of the Generic Resource type with the role and position name.</span></span> <span data-ttu-id="62f7d-160">إذا كان تنفيذ العمل يستوجب وجود موردين، تنشئ ميزة "إنشاء فريق" عضوين في الفريق وتستخدم اسم المنصب لتمييزهما عن بعضهما.</span><span class="sxs-lookup"><span data-stu-id="62f7d-160">If two resources are needed for a role to complete the work, the Generate Team feature creates two team members and uses position name to set them apart.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="62f7d-161">![لقطه شاشة لإضافة موردين عامين](media/FAQ-Resources-to-Tasks2-6.png "لقطه شاشة لإضافة موردين عامين")</span><span class="sxs-lookup"><span data-stu-id="62f7d-161">![Screenshot of adding two generic resources](media/FAQ-Resources-to-Tasks2-6.png "Screenshot of adding two generic resources")</span></span>
 
<span data-ttu-id="62f7d-162">يمكنك فتح متطلبات موارد المساعدة لعضو الفريق العام عن طريق تحديد الارتباط تحت "متطلبات الموارد".</span><span class="sxs-lookup"><span data-stu-id="62f7d-162">You can open the backing resource requirement for the generic team member by selecting the link under Resource Requirement.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="62f7d-163">![لقطة شاشة لفتح متطلبات الموارد المساعدة](media/FAQ-Resources-to-Tasks2-7.png "لقطة شاشة لفتح متطلبات الموارد المساعدة")</span><span class="sxs-lookup"><span data-stu-id="62f7d-163">![Screenshot of opening backing resource requirement](media/FAQ-Resources-to-Tasks2-7.png "Screenshot of opening backing resource requirement")</span></span>

<span data-ttu-id="62f7d-164">حدد **حجز** للمورد العام، ثم يمكنك استخدام لوحة الجدولة للبحث عن مورد حقيقي وحجزه.</span><span class="sxs-lookup"><span data-stu-id="62f7d-164">Select **Book** for the generic resource, and then you can use the schedule board to find and book a real resource.</span></span> <span data-ttu-id="62f7d-165">يمكنك أيضًا إرسال متطلبات التنفيذ بواسطة مدير الموارد عن طريق تحديد **إرسال الطلب‬**.</span><span class="sxs-lookup"><span data-stu-id="62f7d-165">You can also submit the requirement for fulfillment by a resource manager by selecting **Submit Request**.</span></span>

<span data-ttu-id="62f7d-166">عند تنفيذ المورد العام بواسطة مورد مسمى، تتم إزالة المورد العام من الفريق ويتم تعيين تعيينات المهام الخاصة بالمورد العام إلى المورد المسمى الذي قام بتنفيذ متطلبات الموارد للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="62f7d-166">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>
 



[!INCLUDE[footer-include](../includes/footer-banner.md)]