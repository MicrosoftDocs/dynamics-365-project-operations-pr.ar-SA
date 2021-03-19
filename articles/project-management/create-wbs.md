---
title: إنشاء هيكل تنظيم العمل
description: يوضح هذا الموضوع كيفية إنشاء هيكل تنظيم عمل (WBS) يشمل التحكم الأساسي في واجهة الجدولة الجديدة.
author: ruhercul
manager: tfehr
ms.date: 01/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 695bbc2ae1ba1e762472b5f5fa853c89017d2f52
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286997"
---
# <a name="create-a-work-breakdown-structure-wbs"></a><span data-ttu-id="01b71-103">إنشاء هيكل تنظيم العمل (WBS)</span><span class="sxs-lookup"><span data-stu-id="01b71-103">Create a work breakdown structure (WBS)</span></span>

<span data-ttu-id="01b71-104">يوضح جدول المشروع ما العمل الذي يجب إكماله، والموارد التي ستؤدي العمل، والإطار الزمني الذي يجب إكمال العمل فيه.</span><span class="sxs-lookup"><span data-stu-id="01b71-104">A project schedule communicates what work must be completed, which resources will do the work, and the timeframe in which the work must be completed.</span></span> <span data-ttu-id="01b71-105">يعكس الجدول جميع الأعمال المرتبطة بتسليم المشروع في الوقت المحدد.</span><span class="sxs-lookup"><span data-stu-id="01b71-105">The schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="01b71-106">في Dynamics 365 Project Operations، قم بإنشاء جدول مشروع من خلال:</span><span class="sxs-lookup"><span data-stu-id="01b71-106">In Dynamics 365 Project Operations, you create a project schedule by:</span></span>

  - <span data-ttu-id="01b71-107">تنظيم العمل إلى مهام قابلة للإدارة.</span><span class="sxs-lookup"><span data-stu-id="01b71-107">Breaking the work down into manageable tasks.</span></span>
  - <span data-ttu-id="01b71-108">تقدير الوقت اللازم للقيام بكل مهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-108">Estimating the time that is required to do each task.</span></span>
  - <span data-ttu-id="01b71-109">إعداد تبعيات المهام.</span><span class="sxs-lookup"><span data-stu-id="01b71-109">Setting task dependencies.</span></span>
  - <span data-ttu-id="01b71-110">إعداد مدد المهام.</span><span class="sxs-lookup"><span data-stu-id="01b71-110">Setting task durations.</span></span>
  - <span data-ttu-id="01b71-111">تقدير الموارد العامة التي ستنفذ المهام.</span><span class="sxs-lookup"><span data-stu-id="01b71-111">Estimating the generic resources that will do the tasks.</span></span> 

<span data-ttu-id="01b71-112">يتم إنشاء جدول المشروع في علامة التبويب **الجدولة** في صفحة **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="01b71-112">The project schedule is created on the **Schedule** tab on the **Project** page.</span></span>

## <a name="tasks"></a><span data-ttu-id="01b71-113">المهام</span><span class="sxs-lookup"><span data-stu-id="01b71-113">Tasks</span></span>

<span data-ttu-id="01b71-114">تتمثل الخطوة الأولى في إنشاء جدول مشروع في تقسيم العمل إلى أجزاء قابلة للإدارة.</span><span class="sxs-lookup"><span data-stu-id="01b71-114">The first step in creating a project schedule is to break the work down into manageable portions.</span></span> <span data-ttu-id="01b71-115">تدعم الجدولة في Project Operations الميزات التالية:</span><span class="sxs-lookup"><span data-stu-id="01b71-115">The schedule in Project Operations supports the following features:</span></span>

- <span data-ttu-id="01b71-116">المهام الموجزة أو مهام الحاوية</span><span class="sxs-lookup"><span data-stu-id="01b71-116">Summary or container tasks</span></span>
- <span data-ttu-id="01b71-117">مهام العقدة الطرفية</span><span class="sxs-lookup"><span data-stu-id="01b71-117">Leaf node tasks</span></span>

### <a name="summary-tasks"></a><span data-ttu-id="01b71-118">مهام الملخص</span><span class="sxs-lookup"><span data-stu-id="01b71-118">Summary tasks</span></span>

<span data-ttu-id="01b71-119">يمكن لمهام الملخص تخزين مهام ملخص أخرى أو مهام العقدة الطرفية.</span><span class="sxs-lookup"><span data-stu-id="01b71-119">Summary tasks can store other summary tasks or leaf node tasks.</span></span> <span data-ttu-id="01b71-120">وليس لديهم جهد عمل أو تكلفة خاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="01b71-120">They have no work effort or cost of their own.</span></span> <span data-ttu-id="01b71-121">بدلاً من ذلك ، فإن جهد العمل والتكلفة هما مجموعة من جهد العمل وتكلفة مهام الحاوية الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="01b71-121">Instead, their work effort and cost are a rollup of the work effort and cost of their container tasks.</span></span> <span data-ttu-id="01b71-122">تاريخ بدء مهمة التلخيص هو تاريخ بدء مهام الحاوية ، وتاريخ الانتهاء هو تاريخ الانتهاء من مهام الحاوية.</span><span class="sxs-lookup"><span data-stu-id="01b71-122">The start date of the summary task is the start date of the container tasks, and the end date is the end date of the container tasks.</span></span> <span data-ttu-id="01b71-123">يمكن تحرير اسم مهمة الملخص، لكن لا يمكن تحرير خصائص الجدولة، بما في ذلك الجهد والتواريخ والمدة.</span><span class="sxs-lookup"><span data-stu-id="01b71-123">The name of a summary task can be edited, but scheduling properties, including effort, dates, and duration, can't be edited.</span></span> <span data-ttu-id="01b71-124">إذا قمت بحذف مهمة تلخيصية ، يمكنك أيضًا حذف جميع مهام الحاوية الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="01b71-124">If you delete a summary task, you also delete all its container tasks.</span></span>

### <a name="leaf-node-tasks"></a><span data-ttu-id="01b71-125">مهام العقدة الطرفية</span><span class="sxs-lookup"><span data-stu-id="01b71-125">Leaf node tasks</span></span>

<span data-ttu-id="01b71-126">تمثل مهام عقدة الورقة العمل الأكثر تفصيلاً في المشروع.</span><span class="sxs-lookup"><span data-stu-id="01b71-126">Leaf node tasks represent the most granular work on the project.</span></span> <span data-ttu-id="01b71-127">إنها تتميز بمجهود مقدّر والموارد وتواريخ بدء وانتهاء مخططين ومدة.</span><span class="sxs-lookup"><span data-stu-id="01b71-127">They have an estimated effort, resources, planned start and end dates, and a duration.</span></span>

## <a name="create-a-task-hierarchy"></a><span data-ttu-id="01b71-128">إنشاء تدرج هرمي للمهام</span><span class="sxs-lookup"><span data-stu-id="01b71-128">Create a task hierarchy</span></span>

### <a name="add-a-task"></a><span data-ttu-id="01b71-129">أضف مهمة</span><span class="sxs-lookup"><span data-stu-id="01b71-129">Add a task</span></span>

<span data-ttu-id="01b71-130">أكمل الخطوات التالية لإضافة مهمة واحدة أو أكثر.</span><span class="sxs-lookup"><span data-stu-id="01b71-130">Complete the following steps to add one or more tasks.</span></span>

1. <span data-ttu-id="01b71-131">انتقل إلى **Projects** وحدد وافتح سجل المشروع الذي ترغب في إنشاء جدولة له.</span><span class="sxs-lookup"><span data-stu-id="01b71-131">Go to **Projects** and select and open the project record for which you want to create a schedule.</span></span> 
2. <span data-ttu-id="01b71-132">حدد علامة تبويب **المهام**.</span><span class="sxs-lookup"><span data-stu-id="01b71-132">Select the **Tasks** tab.</span></span> 
3. <span data-ttu-id="01b71-133">حدد **إضافة مهمة جديدة**، وأدخل اسمًا للمهمة، ثم اضغط على Enter.</span><span class="sxs-lookup"><span data-stu-id="01b71-133">Select **Add new task**, enter a name for the task, and then press Enter.</span></span>
2. <span data-ttu-id="01b71-134">أدخل اسم مهمة آخر واضغط على Enter مرة أخرى حتى يصبح لديك قائمة كاملة بالمهام.</span><span class="sxs-lookup"><span data-stu-id="01b71-134">Enter another task name and press Enter again until you have a full list of tasks.</span></span>

### <a name="manage-hierarchy-of-a-task"></a><span data-ttu-id="01b71-135">إدارة التسلسل الهرمي لمهمة ما</span><span class="sxs-lookup"><span data-stu-id="01b71-135">Manage hierarchy of a task</span></span>

<span data-ttu-id="01b71-136">عند تحريك مهمة لأسفل، تصبح تابعة للمهمة التي فوقها مباشرةً.</span><span class="sxs-lookup"><span data-stu-id="01b71-136">When a task is indented, it becomes a child of the task that is directly above it.</span></span> <span data-ttu-id="01b71-137">ثم تتم إعادة حساب الجدول الزمني للمهمة بحيث يستند إلى معرف الجدول الأصلي الجديد ويتبع مخطط ترقيم المخطط التفصيلي.</span><span class="sxs-lookup"><span data-stu-id="01b71-137">The schedule ID of the task is then recalculated so that it's based on the schedule ID of its new parent and follows the outline numbering scheme.</span></span> <span data-ttu-id="01b71-138">المهمة الأصل هي الآن مهمة ملخص.</span><span class="sxs-lookup"><span data-stu-id="01b71-138">The parent task is now a summary task.</span></span> <span data-ttu-id="01b71-139">ولذلك، تصبح قيمة محتسبة للمهام التابعة لها.</span><span class="sxs-lookup"><span data-stu-id="01b71-139">Therefore, it becomes a rollup of its child tasks.</span></span> <span data-ttu-id="01b71-140">عندما تتم ترقية إحدى المهام، فإنها تصبح غير تابعة للمهمة الأصلية لها.</span><span class="sxs-lookup"><span data-stu-id="01b71-140">When a task is promoted, it's no longer a child of the task that was its parent.</span></span> <span data-ttu-id="01b71-141">ثم يتم بعد ذلك إعادة حساب معرف الجدول حتى يعكس عمق وموضع المهمة اللذين تم تحديثهما في التدرج الهرمي.</span><span class="sxs-lookup"><span data-stu-id="01b71-141">The schedule ID is then recalculated so that it reflects the task's updated depth and position in the hierarchy.</span></span> <span data-ttu-id="01b71-142">تتم إعادة حساب الجهد والتكلفة والتواريخ الخاصة بالمهمة الأصل السابقة التالي لا تتضمن هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-142">The effort, cost, and dates of the previous parent task are recalculated so that they don't include this task.</span></span>

<span data-ttu-id="01b71-143">أكمل الخطوات التالية لترقية مهمة أو تحريكها إلى مستوى أدنى.</span><span class="sxs-lookup"><span data-stu-id="01b71-143">Complete the following steps to indent or promote a task.</span></span>

1. <span data-ttu-id="01b71-144">في صفحة **المشروع**، في علامة تبويب **المهام**، أسفل **مهام الملخص**، حدد النقاط العمودية الثلاثة باسم المهمة، ثم حدد **إنشاء مهمة فرعية**.</span><span class="sxs-lookup"><span data-stu-id="01b71-144">On the **Project** page, on the **Tasks** tab, under **Summary tasks**, select the three vertical dots by the task name, and then select **Make subtask**.</span></span> 
2. <span data-ttu-id="01b71-145">حدد المهمة المراد ترقيتها أو تحريكها إلى مستوى أدنى.</span><span class="sxs-lookup"><span data-stu-id="01b71-145">Select the task to indent or promote.</span></span> <span data-ttu-id="01b71-146">لتحديد أكثر من مهمة واحدة، حدد مهمة، واضغط مع الاستمرار على Ctrl، ثم حدد مهام أخرى.</span><span class="sxs-lookup"><span data-stu-id="01b71-146">To select more than one task, select a task, press and hold Ctrl, and then select additional tasks.</span></span>
2. <span data-ttu-id="01b71-147">حدد **تحريك إلى مستوى أدنى** أو **ترقية المهمة الفرعية** لنقل المهام أسفل مهام الملخص أو خارجها.</span><span class="sxs-lookup"><span data-stu-id="01b71-147">Select **Indent** or **Promote subtask**  to move tasks under or out from under summary tasks.</span></span>

### <a name="move-tasks-up-and-down"></a><span data-ttu-id="01b71-148">تحريك المهام لأعلى ولأسفل</span><span class="sxs-lookup"><span data-stu-id="01b71-148">Move tasks up and down</span></span>

<span data-ttu-id="01b71-149">يمكن تحريك المهام إلى أي مستوى في هيكل تنظيم العمل بإحدى طريقتين:</span><span class="sxs-lookup"><span data-stu-id="01b71-149">Tasks can me moved to any level in the work breakdown structure in one of two ways:</span></span>

- <span data-ttu-id="01b71-150">حدد مهمة أو أكثر واسحبها إلى الموقع المطلوب.</span><span class="sxs-lookup"><span data-stu-id="01b71-150">Select one more tasks and drag them to the desired location.</span></span>
- <span data-ttu-id="01b71-151">حدد واحدة أو أكثر من المهام، انقر باليمين فوق وحدد **قص**، ثم حدد الخلية الوجهة في الجدولة، ثم انقر بالماوس الأيمن فوق وحدد **لصق**.</span><span class="sxs-lookup"><span data-stu-id="01b71-151">Select one or more tasks, right-click and select **Cut**, select the destination cell in the schedule, and then right-click and select **Paste**.</span></span>

## <a name="task-attributes"></a><span data-ttu-id="01b71-152">سمات المهمة</span><span class="sxs-lookup"><span data-stu-id="01b71-152">Task attributes</span></span>

<span data-ttu-id="01b71-153">يصف اسم المهمة العمل الذي يجب إكماله.</span><span class="sxs-lookup"><span data-stu-id="01b71-153">A task's name describes the work that must be completed.</span></span> <span data-ttu-id="01b71-154">في Project Operations، تصف السمات المرتبطة بالمهمة جدول المهمة ومتطلبات التوظيف الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="01b71-154">In Project Operations, the attributes associated with a task describe the schedule of the task and its staffing requirements.</span></span>

## <a name="schedule-attributes"></a><span data-ttu-id="01b71-155">سمات الجدولة</span><span class="sxs-lookup"><span data-stu-id="01b71-155">Schedule attributes</span></span>

<span data-ttu-id="01b71-156">تحدد سمات **المجهود** و **تاريخ البدء** و **تاريخ الانتهاء** و **المدة** الجدول الخاص بالمهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-156">The **Effort**, **Start date**, **End date**, and **Duration** attributes define the schedule for the task.</span></span>

<span data-ttu-id="01b71-157">يعرض الجدول التالي سمات جدولة إضافية.</span><span class="sxs-lookup"><span data-stu-id="01b71-157">The following table shows additional schedule attributes.</span></span>

| <span data-ttu-id="01b71-158">**اسم العرض النهائي**</span><span class="sxs-lookup"><span data-stu-id="01b71-158">**Final display name**</span></span> | <span data-ttu-id="01b71-159">**الوصف النهائي**</span><span class="sxs-lookup"><span data-stu-id="01b71-159">**Final description**</span></span> |
| --- | --- |
| <span data-ttu-id="01b71-160">الجهد المكتمل (بالساعات)</span><span class="sxs-lookup"><span data-stu-id="01b71-160">Effort Completed (Hours)</span></span> | <span data-ttu-id="01b71-161">العمل المكتمل للمهمة بالساعات.</span><span class="sxs-lookup"><span data-stu-id="01b71-161">Completed work for the task in hours.</span></span> |
| <span data-ttu-id="01b71-162">المدة</span><span class="sxs-lookup"><span data-stu-id="01b71-162">Duration</span></span> | <span data-ttu-id="01b71-163">يعرض المدة بالأيام للمهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-163">Displays the duration in days for the task.</span></span> |
| <span data-ttu-id="01b71-164">الجهد الإجمالي</span><span class="sxs-lookup"><span data-stu-id="01b71-164">Total Effort</span></span> | <span data-ttu-id="01b71-165">إجمالي العمل للمهمة بالساعات</span><span class="sxs-lookup"><span data-stu-id="01b71-165">Total work for the task in hours.</span></span> |
| <span data-ttu-id="01b71-166">إنهاء</span><span class="sxs-lookup"><span data-stu-id="01b71-166">Finish</span></span> | <span data-ttu-id="01b71-167">تاريخ ووقت الانتهاء</span><span class="sxs-lookup"><span data-stu-id="01b71-167">Finish date and time.</span></span> |
| <span data-ttu-id="01b71-168">تم الإكمال بنسبة %</span><span class="sxs-lookup"><span data-stu-id="01b71-168">% Complete</span></span> | <span data-ttu-id="01b71-169">النسبة المئوية للمهمة المكتملة.</span><span class="sxs-lookup"><span data-stu-id="01b71-169">The percentage of the task that is complete.</span></span> |
| <span data-ttu-id="01b71-170">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="01b71-170">Project Bucket</span></span> | <span data-ttu-id="01b71-171">يمكن تجميع لوحه المهمة حسب المستودع بحيث يكون لكل مستودع عموده الخاص.</span><span class="sxs-lookup"><span data-stu-id="01b71-171">The task board can be grouped by bucket so each bucket has its own column.</span></span> |
| <span data-ttu-id="01b71-172">الجهد المتبقي (ساعات)</span><span class="sxs-lookup"><span data-stu-id="01b71-172">Effort Remaining (Hours)</span></span> | <span data-ttu-id="01b71-173">العمل المتبقي للمهمة بالساعات.</span><span class="sxs-lookup"><span data-stu-id="01b71-173">The remaining work for the task in hours.</span></span> |
| <span data-ttu-id="01b71-174">البدء</span><span class="sxs-lookup"><span data-stu-id="01b71-174">Start</span></span> | <span data-ttu-id="01b71-175">تاريخ ووقت البدء.</span><span class="sxs-lookup"><span data-stu-id="01b71-175">Start date and time.</span></span> |
| <span data-ttu-id="01b71-176">الاسم </span><span class="sxs-lookup"><span data-stu-id="01b71-176">Name</span></span> | <span data-ttu-id="01b71-177">اسم المهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-177">The name of the task.</span></span> |
| <span data-ttu-id="01b71-178">البطاقة/رقم البطاقة</span><span class="sxs-lookup"><span data-stu-id="01b71-178">ID</span></span> | <span data-ttu-id="01b71-179">معرف المهمة في هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="01b71-179">The ID of the task in the work breakdown structure.</span></span> |

<span data-ttu-id="01b71-180">بصفتك المسؤول، يمكنك تعريف حقول مخصصة على كيان المهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-180">As an administrator, you can define custom fields on the task entity.</span></span> <span data-ttu-id="01b71-181">ومع ذلك، لا يمكن عرض الحقول على شبكة الجدول.</span><span class="sxs-lookup"><span data-stu-id="01b71-181">However the fields can't be displayed on the schedule grid.</span></span> <span data-ttu-id="01b71-182">لرؤية الحقول المخصصة، أضفها إلى صفحة تفاصيل **مهمة المشروع**.</span><span class="sxs-lookup"><span data-stu-id="01b71-182">To see your custom fields, add them to the **Project Task** details page.</span></span>

## <a name="staffing-attributes"></a><span data-ttu-id="01b71-183">سمات التوظيف</span><span class="sxs-lookup"><span data-stu-id="01b71-183">Staffing attributes</span></span>

<span data-ttu-id="01b71-184">يتم الوصول إلى سمات التوظيف من خلال حقل **الموارد** في الجدول.</span><span class="sxs-lookup"><span data-stu-id="01b71-184">Staffing attributes are accessed through the **Resources** field in the schedule.</span></span> <span data-ttu-id="01b71-185">يمكنك إما البحث عن مورد موجود، أو تحديد **إنشاء**، وفي جزء **الإنشاء السريع**، أضف عضو فريق مشروع كمورد جديد.</span><span class="sxs-lookup"><span data-stu-id="01b71-185">You can either search for an existing resource, or select **Create**, and in the **Quick Create** pane, add a project team member as a new resource.</span></span>

<span data-ttu-id="01b71-186">يتم استخدام حقول **الدور** و **وحدة تعيين الموارد‬** و **اسم المنصب** لوصف متطلبات الموظفين للمهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-186">The **Role**, **Resourcing Unit**, and **Position Name** fields are used to describe the staffing requirements for the task.</span></span> <span data-ttu-id="01b71-187">يتم استخدام سمات التوظيف هذه، مع جداول المهام للعثور على الموارد المتوفرة لتنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-187">These staffing attributes, together with the task schedule are used to find available resources to do this task.</span></span>

   - <span data-ttu-id="01b71-188">**الدور**: حدد نوع المورد المطلوب لتنفيذ المهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-188">**Role**: Specify the type of resource that is required to do the task.</span></span>
   - <span data-ttu-id="01b71-189">**وحدة تعيين الموارد**: حدد الوحدة التي ينبغي تعيين الموارد الخاصة بالمهمة منها.</span><span class="sxs-lookup"><span data-stu-id="01b71-189">**Resourcing unit**: Specify the unit that resources for the task should be assigned from.</span></span> <span data-ttu-id="01b71-190">تؤثر هذه السمة على تقدير التكلفة والمبيعات الخاصة بالمهمة في حالة تعيين التكلفة وسعر الفاتورة للمورد بناء على وحدات تعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="01b71-190">This attribute affects the cost and sales estimate for the task if the cost and bill rate for the resource are set based on resourcing units.</span></span>
   - <span data-ttu-id="01b71-191">**اسم المنصب**: أدخل اسمًا مألوفا للمورد العام الذي يعمل كعنصر نائب للمورد الذي سيقوم بالعمل في النهاية.</span><span class="sxs-lookup"><span data-stu-id="01b71-191">**Position name**: Enter a name for the generic resource that serves as a placeholder for the resource that will ultimately do the work.</span></span>

<span data-ttu-id="01b71-192">يحتوي حقل **الموارد** على اسم المنصب الخاص بالمورد العام أو المورد المسمى عند العثور على واحد.</span><span class="sxs-lookup"><span data-stu-id="01b71-192">The **Resources** field holds the position name of the generic resource or named resource when one is found.</span></span>

<span data-ttu-id="01b71-193">ويحتوي حقل **الفئة** على القيم التي تشير إلى نوع أكبر من العمل الذي يمكن تجميع المهمة فيه.</span><span class="sxs-lookup"><span data-stu-id="01b71-193">The **Category** field holds the values that indicate a broader type of work that the task can be grouped into.</span></span> <span data-ttu-id="01b71-194">لا يؤثر هذا الحقل في الجدولة أو الموظفين.</span><span class="sxs-lookup"><span data-stu-id="01b71-194">This field doesn't affect scheduling or staffing.</span></span> <span data-ttu-id="01b71-195">بدلا من ذلك، يُستخدم الحقل فقط لإعداد التقارير.</span><span class="sxs-lookup"><span data-stu-id="01b71-195">Instead, the field is used only for reporting.</span></span>

## <a name="task-dependencies"></a><span data-ttu-id="01b71-196">تبعيات المهمة</span><span class="sxs-lookup"><span data-stu-id="01b71-196">Task dependencies</span></span>

<span data-ttu-id="01b71-197">يمكنك استخدام الجدول في Project Operations لإنشاء العلاقات السابقة بين المهام.</span><span class="sxs-lookup"><span data-stu-id="01b71-197">You can use the schedule in Project Operations to create predecessor relationships between tasks.</span></span> <span data-ttu-id="01b71-198">يستخدم حقل **النشاط السابق** قيمة واحدة أو أكثر للإشارة إلى المهام التي تعتمد عليها المهمة.</span><span class="sxs-lookup"><span data-stu-id="01b71-198">The **Predecessor** field uses one or more values to indicate the tasks that a task depends on.</span></span> <span data-ttu-id="01b71-199">عند تعيين قيم أنشطة سابقة لمهمة، يمكن بدء المهمة فقط بعد إكمال كافة المهام السابقة.</span><span class="sxs-lookup"><span data-stu-id="01b71-199">When predecessor values are assigned to a task, the task can start only after all of the predecessor tasks have been completed.</span></span> <span data-ttu-id="01b71-200">وبسبب التبعية، تتم إعادة تعيين تاريخ البدء المخطط للمهمة إلى تاريخ إتمام المهام السابقة.</span><span class="sxs-lookup"><span data-stu-id="01b71-200">Because of the dependency, the planned start date of the task is reset to the date when the predecessor tasks are completed.</span></span>

<span data-ttu-id="01b71-201">لا يؤثر وضع المهمة على التحديثات التي يتم إجراؤها على تاريخي البدء والانتهاء للمهام السابقة/التابعة.</span><span class="sxs-lookup"><span data-stu-id="01b71-201">The task mode has no effect on updates that are made to the start and end dates of predecessor/dependent tasks.</span></span>

## <a name="accessibility-and-keyboard-shortcuts"></a><span data-ttu-id="01b71-202">اختصارات لوحة المفاتيح وذوي الاحتياجات الخاصة</span><span class="sxs-lookup"><span data-stu-id="01b71-202">Accessibility and keyboard shortcuts</span></span>

<span data-ttu-id="01b71-203">إن شبكة **الجدولة** يمكن الوصول اليها بالكامل ويمكن استخدامها مع قارئات الشاشة مثل المسرد أو JAWS أو NVDA.</span><span class="sxs-lookup"><span data-stu-id="01b71-203">The **Schedule** grid is fully accessible and can be used with screen readers such as Narrator, JAWS, or NVDA.</span></span> <span data-ttu-id="01b71-204">يمكنك التنقل خلال منطقه الشبكة باستخدام مفاتيح الأسهم (كما في Microsoft Excel)، يمكنك استخدام المفتاح Tab للتقدم من خلال عناصر الواجهة التفاعلية، ويمكنك استخدام مفتاح السهم لأسفل، أو مفتاح Enter، أو Spacebar لتحديد وفتح القوائم المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="01b71-204">You can move through the grid area by using arrow keys (as in Microsoft Excel), you can use the Tab key to advance through the interactive user interface elements, and you can use the Down arrow key, the Enter key, or the Spacebar to select and open the drop-down menus.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]