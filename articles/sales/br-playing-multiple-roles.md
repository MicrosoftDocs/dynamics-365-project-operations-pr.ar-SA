---
title: تقدير مبيعات المشروع وتكاليفه عندما يملأ مورد قابل للحجز عدة أدوار في المشروع
description: يشرح هذا الموضوع كيفية استخدام أبعاد التسعير لدعم تقديرات التسعير والتكلفة لمورد يقوم بتعبئة أدوار متعددة في مشروع.
author: rumant
manager: tfehr
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: da17f0f58623128d51fda0f5529182cd37ea41b9
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531343"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-on-a-project"></a><span data-ttu-id="13300-103">تقدير مبيعات المشروع وتكاليفه عندما يملأ مورد قابل للحجز عدة أدوار في المشروع</span><span class="sxs-lookup"><span data-stu-id="13300-103">Estimate project sales and costs when a bookable resource fills multiple roles on a project</span></span> 

<span data-ttu-id="13300-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬، نشر خفيف - التعامل مع الفواتير الأولية‬، وProject Operations للسيناريوهات المستندة إلى المنتجات المخزنة/الإنتاج_</span><span class="sxs-lookup"><span data-stu-id="13300-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing, Project Operations for stocked/production-based scenarios_</span></span> 

<span data-ttu-id="13300-105">غالبًا ما تحتاج الشركات القائمة على المشروعات إلى مورد واحد لملء أدوار متعددة في المشروع.</span><span class="sxs-lookup"><span data-stu-id="13300-105">Project-based companies often have the need for one resource to fill multiple roles on a project.</span></span> <span data-ttu-id="13300-106">يمكن تسعير كل دور وتكلفته بشكل مختلف.</span><span class="sxs-lookup"><span data-stu-id="13300-106">Each role can be priced and costed differently.</span></span> <span data-ttu-id="13300-107">هذا يعني أن وقت المورد نفسه في مشروع ما يمكن أن يحصل على تقدير مالي مختلف اعتمادًا على أسعار الفاتورة والتكلفة لكل دور.</span><span class="sxs-lookup"><span data-stu-id="13300-107">This means that the same resource's time on a project could get a different financial estimate depending on the bill and cost rates for each role.</span></span> <span data-ttu-id="13300-108">يمكنك إعداد القيم في سجل عضو الفريق للمورد المسمى بتجاوزات مختلفة لكل مهمة من المهام التي تم تعيين عضو الفريق لها.</span><span class="sxs-lookup"><span data-stu-id="13300-108">You can set up the values on the team member record for the named resource with different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="13300-109">يرشدك المثال التالي إلى كيفية قيام التجاوز البسيط للقيمة بالسماح للمورد بأدوار متعددة في مشروع بمعدلات تكلفة وفواتير مختلفة.</span><span class="sxs-lookup"><span data-stu-id="13300-109">The following example walks you through how the simple override of a value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="13300-110">إنشاء مهام</span><span class="sxs-lookup"><span data-stu-id="13300-110">Create tasks</span></span>
<span data-ttu-id="13300-111">لإنشاء المهام ، تحتاج إلى إضافة المهام ، بالإضافة إلى المهام الموجزة ، وبعد ذلك تحتاج إلى تعيين المهمة قبل إضافة مدة المهمة.</span><span class="sxs-lookup"><span data-stu-id="13300-111">To create tasks, you need to add tasks, as well as summary tasks, after which you need to assign the task before you add task duration.</span></span> 

### <a name="add-tasks-and-summary-tasks"></a><span data-ttu-id="13300-112">أضف المهام والمهام الموجزة</span><span class="sxs-lookup"><span data-stu-id="13300-112">Add tasks and summary tasks</span></span>
<span data-ttu-id="13300-113">لإضافة مهمة ، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="13300-113">To add a task, complete the following steps.</span></span>

1. <span data-ttu-id="13300-114">انتقل إلى **المشاريع** وافتح المشروع الذي تريد إضافة المهام إليه.</span><span class="sxs-lookup"><span data-stu-id="13300-114">Go to **Projects** and open the project to which you want to add tasks.</span></span>
2. <span data-ttu-id="13300-115">حدد **إضافة مهمة جديدة**.</span><span class="sxs-lookup"><span data-stu-id="13300-115">Select **Add new task**.</span></span> <span data-ttu-id="13300-116">قم بتسمية المهمة ثم اضغط على **Enter**.</span><span class="sxs-lookup"><span data-stu-id="13300-116">Name the task, and then press **Enter**.</span></span>
3. <span data-ttu-id="13300-117">أدخل اسم مهمة آخر واضغط على **Enter**.</span><span class="sxs-lookup"><span data-stu-id="13300-117">Enter another task name and press **Enter**.</span></span> <span data-ttu-id="13300-118">كرر هذا حتى تحصل على قائمة كاملة بالمهام.</span><span class="sxs-lookup"><span data-stu-id="13300-118">Repeat this until you have a full list of tasks.</span></span>
3. <span data-ttu-id="13300-119">لوضع مسافة بادئة للمهام ضمن مهام **الملخص**، حدد ثلاث نقاط عمودية باسم المهمة، ثم حدد **إنشاء مهمة فرعية**.</span><span class="sxs-lookup"><span data-stu-id="13300-119">To indent tasks under **Summary** tasks, select the three vertical dots by the task name, and then select **Make subtask**.</span></span> 

  > [!TIP]
  > <span data-ttu-id="13300-120">لتحديد أكثر من مهمة ، حدد مهمة ، واضغط مع الاستمرار على **Ctrl**، ثم حدد مهمة أخرى.</span><span class="sxs-lookup"><span data-stu-id="13300-120">To select more than one task, select a task, press and hold **Ctrl**, and then select another task.</span></span>
  >
  > <span data-ttu-id="13300-121">يمكنك أيضا اختيار **ترقية المهمة الفرعية** لنقل المهام من مهام **الملخص**.</span><span class="sxs-lookup"><span data-stu-id="13300-121">You can also choose **Promote subtask** to move tasks out from under **Summary** tasks.</span></span>

### <a name="assign-tasks"></a><span data-ttu-id="13300-122">تعيين المهام</span><span class="sxs-lookup"><span data-stu-id="13300-122">Assign tasks</span></span>

<span data-ttu-id="13300-123">أكمل الخطوات التالية لتعيين المهام.</span><span class="sxs-lookup"><span data-stu-id="13300-123">Complete the following steps to assign tasks.</span></span>

1. <span data-ttu-id="13300-124">في العمود **معين إلى** لمهمة، حدد رمز الشخص.</span><span class="sxs-lookup"><span data-stu-id="13300-124">In the  **Assigned to**  column for a task, select the person icon.</span></span>
2. <span data-ttu-id="13300-125">اختر أحد أعضاء الفريق من القائمة أو أدخل نصًا للبحث عن اسم.</span><span class="sxs-lookup"><span data-stu-id="13300-125">Choose a team member from the list or enter text to search for a name.</span></span>

### <a name="add-task-duration-and-columns"></a><span data-ttu-id="13300-126">أضف مدة المهمة والأعمدة</span><span class="sxs-lookup"><span data-stu-id="13300-126">Add task duration and columns</span></span>

<span data-ttu-id="13300-127">غالبًا ما يكون من الأسهل البدء في إنشاء مشروعك مع المدة.</span><span class="sxs-lookup"><span data-stu-id="13300-127">It's often easiest to begin constructing your project with duration.</span></span> <span data-ttu-id="13300-128">أكمل الخطوات التالية لإضافة مدة المهمة.</span><span class="sxs-lookup"><span data-stu-id="13300-128">Complete the following steps to add a task duration.</span></span>

1. <span data-ttu-id="13300-129">في عمود **المدة** لمهمة، اكتب عدد الأيام التي تعتقد أن الأمر سيستغرقها لإنجاز المهمة.</span><span class="sxs-lookup"><span data-stu-id="13300-129">In the **Duration** column for a task, type the number of days you think it will take to accomplish the task.</span></span> <span data-ttu-id="13300-130">إذا كنت تريد استخدام وحدة زمنية مختلفة ، فأدخل رقمًا بالإضافة إلى الكلمة **ساعات** أو **أسابيع** أو **أشهر**.</span><span class="sxs-lookup"><span data-stu-id="13300-130">If you want to use a different unit of time, enter a number plus the word **hours**, **weeks**, or **months**.</span></span>
2. <span data-ttu-id="13300-131">إذا كنت تريد أن تظهر مهمتك كمعلم رئيسي على شكل معين في طريقة عرض **الجدول الزمني**، في عمود **المدة**، أدخل **0 من الأيام** .</span><span class="sxs-lookup"><span data-stu-id="13300-131">If you want your task to appear as a diamond-shaped milestone in the **Timeline** view, in the **Duration** column, enter **0 days** .</span></span>
3. <span data-ttu-id="13300-132">اضغط على **Enter** للانتقال إلى حقل **المدة** الخاص بالمهمة التالية وتابع إدخال المدد الزمنية.</span><span class="sxs-lookup"><span data-stu-id="13300-132">Press **Enter**  to go to the next task's **Duration** field and continue entering durations.</span></span>

  > [!NOTE]
  > <span data-ttu-id="13300-133">لا يمكنك إدخال مدة للمهام الموجزة.</span><span class="sxs-lookup"><span data-stu-id="13300-133">You can't enter a duration for summary tasks.</span></span>

<span data-ttu-id="13300-134">يمكنك إضافة أعمدة إلى مشروعك لتقديم مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="13300-134">You can add columns to your project to provide more details.</span></span> <span data-ttu-id="13300-135">للقيام بذلك، حدد **إضافة عمود**.</span><span class="sxs-lookup"><span data-stu-id="13300-135">To do this, select **Add column**.</span></span> 

<span data-ttu-id="13300-136">لمزيد من المعلومات، راجع [إنشاء مشروع](https://support.microsoft.com/en-us/office/create-a-project-a5b5e823-fb2e-45fd-be00-7d84422d9749).</span><span class="sxs-lookup"><span data-stu-id="13300-136">For more information, see [Create a project](https://support.microsoft.com/en-us/office/create-a-project-a5b5e823-fb2e-45fd-be00-7d84422d9749).</span></span>

## <a name="set-up-the-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="13300-137">قم بإعداد الدور والوحدة التنظيمية لعضو فريق المشروع العام</span><span class="sxs-lookup"><span data-stu-id="13300-137">Set up the role and organization unit for a generic project team member</span></span>
<span data-ttu-id="13300-138">أكمل الخطوات التالية لإعداد دور ووحدة تنظيمية لعضو فريق عام.</span><span class="sxs-lookup"><span data-stu-id="13300-138">Complete the following steps to set up a role and organizational unit for a generic team member.</span></span>

1. <span data-ttu-id="13300-139">في صفحة **المهام**، حدد صف **المهمة** لـ **المهمة أ**.</span><span class="sxs-lookup"><span data-stu-id="13300-139">On the **Tasks** page, select the **Task** row for **Task A**.</span></span> 
2. <span data-ttu-id="13300-140">في **معين إلى**، حدد **إضافة مورد عام**.</span><span class="sxs-lookup"><span data-stu-id="13300-140">In **Assigned To**, select **Add generic resource**.</span></span> <span data-ttu-id="13300-141">يؤدي هذا إلى فتح صفحة **الإنشاء السريع لعضو الفريق**.</span><span class="sxs-lookup"><span data-stu-id="13300-141">This opens the **Team Member Quick Create** page.</span></span>
3. <span data-ttu-id="13300-142">في صفحة **الإنشاء السريع لعضو الفريق**، حدد سمات عضو الفريق العام الذي يمكنه تنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="13300-142">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="13300-143">حدد الدور المناسب والوحدة التنظيمية المناسبة، ثم حدد **حفظ وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="13300-143">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="13300-144">يتم إنشاء عضو فريق عام ويتم تعيينه إلى هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="13300-144">A generic team member is created and assigned to this task.</span></span> 
5. <span data-ttu-id="13300-145">كرر الخطوات 1-4 لـ **المهمة ب**. ومع ذلك، يجب أن تشتمل **المهمة ب** على دور مختلف والوحدة التنظيمية المعينة لعضو الفريق العام مقارنةً بـ **المهمة A**.</span><span class="sxs-lookup"><span data-stu-id="13300-145">Repeat steps 1-4 for **Task B**. However, **Task B** must have a different role and organizational unit assigned for the generic team member than **Task A**.</span></span> 

## <a name="set-up-the-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="13300-146">إعداد الدور والوحدة التنظيمية لمهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="13300-146">Set up the role and organization unit for a project task</span></span>
<span data-ttu-id="13300-147">أكمل الخطوات التالية لإعداد دور ووحدة تنظيمية لمهمة.</span><span class="sxs-lookup"><span data-stu-id="13300-147">Complete the following steps to set up a role and organizational unit for a task.</span></span>

1. <span data-ttu-id="13300-148">بعد قيامك بإنشاء **المهمة أ**، حدد المهمة، ثم حدد الرمز **i** لفتح جزء **تفاصيل المهمة**.</span><span class="sxs-lookup"><span data-stu-id="13300-148">After you create **Task A**, select the task, and then select the **i** icon to open the **Task Details** pane.</span></span> 
2. <span data-ttu-id="13300-149">في جزء **تفاصيل المهمة**، قم بالتمرير إلى الأسفل وحدد **عرض التفاصيل** لفتح صفحة **تفاصيل المهمة**.</span><span class="sxs-lookup"><span data-stu-id="13300-149">On the **Task Details** pane, scroll to the bottom and select **View Details** to open the **Task Details** page.</span></span>
3. <span data-ttu-id="13300-150">في صفحة **تفاصيل المهمة**، في **الدور** و **الوحدة التنظيمية**، أضف القيم المطلوبة لتنفيذ هذه المهمة للمورد.</span><span class="sxs-lookup"><span data-stu-id="13300-150">On the **Task Details** page, in **Role** and **Organizational Unit**, add the values that are required to perform this task for the resource.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="13300-151">إذا أكملت هذا السيناريو باستخدام بيانات العرض التوضيحي لـ Project Operations، فحدد **العميل المتوقع الاستشاري** للدور، و **Fabrikam US** باعتبارها الوحدة التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="13300-151">If you complete this scenario using the Project Operations demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

4. <span data-ttu-id="13300-152">حدد **المهمة ب**، ثم حدد المهمة.</span><span class="sxs-lookup"><span data-stu-id="13300-152">Select **Task B**, and then select the task.</span></span>
5. <span data-ttu-id="13300-153">حدد الرمز **i** لفتح جزء **تفاصيل المهمة**.</span><span class="sxs-lookup"><span data-stu-id="13300-153">Select the **i** icon to open **Task Details** pane.</span></span> 
6. <span data-ttu-id="13300-154">في جزء **تفاصيل المهمة**، قم بالتمرير إلى الأسفل وحدد **عرض التفاصيل** لفتح صفحة **تفاصيل المهمة**.</span><span class="sxs-lookup"><span data-stu-id="13300-154">On the **Task Details** pane, scroll to the bottom and select **View details** to open the **Task Details** page.</span></span>
7. <span data-ttu-id="13300-155">في صفحة **تفاصيل المهمة**، في **الدور** و **الوحدة التنظيمية**، أضف القيم المطلوبة لتنفيذ هذه المهمة للمورد.</span><span class="sxs-lookup"><span data-stu-id="13300-155">On the **Task Details** page, in **Role** and **Organizational Unit**, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="13300-156">يجب أن تكون القيم الموجودة في **الدور** و **الوحدة التنظيمية** لـ **المهمة ب** مختلفة عن تلك الخاصة بـ **المهمة أ**.</span><span class="sxs-lookup"><span data-stu-id="13300-156">The values in **Role** and **Organizational Unit** for **Task B** must be different than those for **Task A**.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="13300-157">إذا أكملت هذا السيناريو باستخدام بيانات العرض التوضيحي لـ Project Operations، فحدد **فني الشبكة** للدور، و **Fabrikam US** باعتبارها الوحدة التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="13300-157">If you complete this scenario using the Project Operations demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

8. <span data-ttu-id="13300-158">احفظ صفحة **تفاصيل المهمة**، ثم أغلقها.</span><span class="sxs-lookup"><span data-stu-id="13300-158">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behavior"></a><span data-ttu-id="13300-159">سلوك عضو الفريق والتقديرات</span><span class="sxs-lookup"><span data-stu-id="13300-159">Team member and estimates behavior</span></span> 
<span data-ttu-id="13300-160">لفهم السلوك في شبكة **عضو الفريق** والتقديرات، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="13300-160">To understand the behavior on the **Team Member** grid and the estimates, complete the following steps.</span></span>

1. <span data-ttu-id="13300-161">في شبكة **عضو الفريق**، حدد عضوي الفريق العامين، ثم حدد **إنشاء متطلبات**.</span><span class="sxs-lookup"><span data-stu-id="13300-161">On the **Team Member** grid, select the two generic team members, and then select **Generate Requirements**.</span></span> <span data-ttu-id="13300-162">سيؤدي ذلك إلى إنشاء متطلبات الموارد.</span><span class="sxs-lookup"><span data-stu-id="13300-162">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="13300-163">حدد صف عضو الفريق لدور **المستشار الرئيسي‬‏‫**، ثم حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="13300-163">Select the team member row for **Consulting Lead**, and then select **Book**.</span></span> <span data-ttu-id="13300-164">يتم فتح لوحة الجدولة مع قائمة من الموارد.</span><span class="sxs-lookup"><span data-stu-id="13300-164">The schedule board opens with a list of resources.</span></span> <span data-ttu-id="13300-165">حدد موردًا ثم حدد **حجز** لحجز المورد لهذا المتطلب.</span><span class="sxs-lookup"><span data-stu-id="13300-165">Select a resource and then select **Book** to book the resource to that requirement.</span></span>
3. <span data-ttu-id="13300-166">حدد صف عضو الفريق لدور **فني الشبكة‬‏‫**، ثم حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="13300-166">Select the team member row for **Network Technician**, and then select **Book**.</span></span> <span data-ttu-id="13300-167">يتم فتح لوحة الجدولة مع قائمة من الموارد.</span><span class="sxs-lookup"><span data-stu-id="13300-167">The schedule board opens with a list of resources.</span></span> <span data-ttu-id="13300-168">حدد نفس المورد مثل السابق، ثم حدد **حجز** لحجز المورد لهذا المتطلب.</span><span class="sxs-lookup"><span data-stu-id="13300-168">Select the same resource as above and then select **Book** to book the resource to that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="13300-169">شبكة أعضاء الفريق</span><span class="sxs-lookup"><span data-stu-id="13300-169">Team Member grid</span></span> 

<span data-ttu-id="13300-170">في شبكة **عضو الفريق**، يتم حذف اثنين من السجلات لأعضاء الفريق العامين ويتم استبدالها بمورد واحد فقط.</span><span class="sxs-lookup"><span data-stu-id="13300-170">On the **Team Member** grid, the two generic team member records are deleted and replaced with only one resource.</span></span> <span data-ttu-id="13300-171">هناك مجموعة واحدة من القيم لهذا المورد ، وهي مجموعة افتراضية من القيم لـ **الدور** و **الوحدة التنظيمية**.</span><span class="sxs-lookup"><span data-stu-id="13300-171">There is one set of values for that resource, which are a default set of values for **Role** and **Organizational Unit**.</span></span>

<span data-ttu-id="13300-172">عندما تقوم بتوسيع الصف لسجل عضو الفريق هذا ، يمكنك رؤية التعيينات المميزة في سجل عضو الفريق لكلتا المهمتين.</span><span class="sxs-lookup"><span data-stu-id="13300-172">When you expand the row for that team member record, you can see distinct assignments on the team member record for both tasks.</span></span> <span data-ttu-id="13300-173">يتضمن كل صف تعيينات قيمًا خاصة بالمهمة لكل من **الدور** و **الوحدة التنظيمية**.</span><span class="sxs-lookup"><span data-stu-id="13300-173">Each assignment row has task-specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="13300-174">شبكة التقديرات</span><span class="sxs-lookup"><span data-stu-id="13300-174">Estimates grid</span></span> 

<span data-ttu-id="13300-175">في شبكة **التقديرات**، يتم تسعير كلٍّ من التعيينات لنفس المورد بشكل مختلف.</span><span class="sxs-lookup"><span data-stu-id="13300-175">On the **Estimates** grid, both assignments for the same resource are priced differently.</span></span> <span data-ttu-id="13300-176">يتم تسعير تعيين المورد في **المهمة أ** باستخدام قيمة سمة **الدور** الخاصة بـ **العميل المتوقع الاستشاري**.</span><span class="sxs-lookup"><span data-stu-id="13300-176">The assignment for the resource on **Task A** is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="13300-177">يتم تسعير تعيين المورد نفسه في **المهمة ب** باستخدام قيمة سمة **الدور** الخاصة بـ **فني الشبكة**.</span><span class="sxs-lookup"><span data-stu-id="13300-177">The assignment for the same resource on **Task B** is priced using the **Role** attribute value of **Network Technician**.</span></span>
