---
title: جداول المشاريع
description: يقدم هذا الموضوع معلومات عن كيفية إنشاء جدول.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 3/01/2019
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
ms.openlocfilehash: 2877f12a9ea3d288c4cf41f406cd8ca3e6cee821
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148402"
---
# <a name="project-schedules"></a><span data-ttu-id="83068-103">جداول المشاريع</span><span class="sxs-lookup"><span data-stu-id="83068-103">Project schedules</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="83068-104">يوضح جدول المشروع ما العمل الذي يجب إكماله ، والموارد التي ستؤدي العمل ، والإطار الزمني الذي يجب الانتهاء من العمل فيه.</span><span class="sxs-lookup"><span data-stu-id="83068-104">A project schedule communicates what work must be completed, which resources will do the work, and the timeframe that the work must be finished in.</span></span> <span data-ttu-id="83068-105">يعكس جميع الأعمال المرتبطة بتسليم المشروع في الوقت المحدد.</span><span class="sxs-lookup"><span data-stu-id="83068-105">It reflects all the work that is associated with delivering the project on time.</span></span> <span data-ttu-id="83068-106">في Dynamics 365 Project Service Automation، يمكنك إنشاء جدول مشروع وذلك بتقسيم العمل إلى المهام القابلة للإدارة وتقدير الوقت المطلوب لتنفيذ كل مهمة وتعيين تبعيات المهام وتعيين مدد المهام وتقدير الموارد العامة التي ستقوم بتنفيذ المهام.</span><span class="sxs-lookup"><span data-stu-id="83068-106">In Dynamics 365 Project Service Automation, you create a project schedule by breaking the work down into manageable tasks, estimating the time that is required to do each task, setting task dependencies, setting task durations, and estimating the generic resources that will do the tasks.</span></span> <span data-ttu-id="83068-107">يتم إنشاء جدول المشروع في علامة التبويب **الجدولة** في صفحة المشروع.</span><span class="sxs-lookup"><span data-stu-id="83068-107">The project schedule is created on the **Schedule** tab of the project page.</span></span>
 
## <a name="tasks"></a><span data-ttu-id="83068-108">المهام</span><span class="sxs-lookup"><span data-stu-id="83068-108">Tasks</span></span>

<span data-ttu-id="83068-109">تتمثل الخطوة الأولى في إنشاء جدول مشروع في تقسيم العمل إلى أجزاء قابلة للإدارة.</span><span class="sxs-lookup"><span data-stu-id="83068-109">The first step in creating a project schedule is to break the work down into manageable portions.</span></span> <span data-ttu-id="83068-110">يدعم الجدول في PSA الميزات التالية:</span><span class="sxs-lookup"><span data-stu-id="83068-110">The schedule in PSA supports the following features:</span></span>

- <span data-ttu-id="83068-111">عقدة الجذر للمشروع.</span><span class="sxs-lookup"><span data-stu-id="83068-111">Project root node</span></span>
- <span data-ttu-id="83068-112">المهام الموجزة أو مهام الحاوية</span><span class="sxs-lookup"><span data-stu-id="83068-112">Summary or container tasks</span></span>
- <span data-ttu-id="83068-113">مهام العقدة الطرفية</span><span class="sxs-lookup"><span data-stu-id="83068-113">Leaf node tasks</span></span>

### <a name="project-root-node"></a><span data-ttu-id="83068-114">عقدة الجذر للمشروع.</span><span class="sxs-lookup"><span data-stu-id="83068-114">Project root node</span></span>

<span data-ttu-id="83068-115">عقدة جذر المشروع هي مهمة الملخص ذات المستوى الأعلى للمشروع.</span><span class="sxs-lookup"><span data-stu-id="83068-115">The project root node is the top-level summary task for the project.</span></span> <span data-ttu-id="83068-116">يتم إنشاء كافة مهام المشروع تحتها.</span><span class="sxs-lookup"><span data-stu-id="83068-116">All other project tasks are created under it.</span></span> <span data-ttu-id="83068-117">يتم تعيين اسم العقدة الجذر إلى اسم المشروع دائمًا.</span><span class="sxs-lookup"><span data-stu-id="83068-117">The name of the root node is always set to the project name.</span></span> <span data-ttu-id="83068-118">يتم تلخيص المجهود والتواريخ ومدة عقدة الجذر استنادًا إلى القيم الموجودة في التدرج الهرمي أدناها.</span><span class="sxs-lookup"><span data-stu-id="83068-118">The effort, dates, and duration of the root node are summarized based on the values in the hierarchy below it.</span></span> <span data-ttu-id="83068-119">لا يمكنك تحرير خصائص العقدة الجذر.</span><span class="sxs-lookup"><span data-stu-id="83068-119">You can't edit the properties of the root node.</span></span> <span data-ttu-id="83068-120">لا يمكنك أيضًا حذف العقدة الجذر.</span><span class="sxs-lookup"><span data-stu-id="83068-120">You also can't delete the root node.</span></span>

### <a name="summary-or-container-tasks"></a><span data-ttu-id="83068-121">المهام الموجزة أو مهام الحاوية</span><span class="sxs-lookup"><span data-stu-id="83068-121">Summary or container tasks</span></span> 

<span data-ttu-id="83068-122">تشتمل مهام الملخص على مهام فرعية أو مهام حاوية ضمنها.</span><span class="sxs-lookup"><span data-stu-id="83068-122">Summary tasks have sub-tasks or container tasks under them.</span></span> <span data-ttu-id="83068-123">وليس لديهم جهد عمل أو تكلفة خاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="83068-123">They have no work effort or cost of their own.</span></span> <span data-ttu-id="83068-124">بدلاً من ذلك ، فإن جهد العمل والتكلفة هما مجموعة من جهد العمل وتكلفة مهام الحاوية الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="83068-124">Instead, their work effort and cost are a rollup of the work effort and cost of their container tasks.</span></span> <span data-ttu-id="83068-125">تاريخ بدء مهمة التلخيص هو تاريخ بدء مهام الحاوية ، وتاريخ الانتهاء هو تاريخ الانتهاء من مهام الحاوية.</span><span class="sxs-lookup"><span data-stu-id="83068-125">The start date of the summary task is the start date of the container tasks, and the end date is the end date of the container tasks.</span></span> <span data-ttu-id="83068-126">يمكن تحرير اسم مهمة تلخيصية ، لكن لا يمكن تحرير خصائص الجدولة (الجهد والتواريخ والمدة).</span><span class="sxs-lookup"><span data-stu-id="83068-126">The name of a summary task can be edited, but scheduling properties (effort, dates, and duration) can't be edited.</span></span> <span data-ttu-id="83068-127">إذا قمت بحذف مهمة تلخيصية ، يمكنك أيضًا حذف جميع مهام الحاوية الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="83068-127">If you delete a summary task, you also delete all its container tasks.</span></span>

### <a name="leaf-node-tasks"></a><span data-ttu-id="83068-128">مهام العقدة الطرفية</span><span class="sxs-lookup"><span data-stu-id="83068-128">Leaf node tasks</span></span>

<span data-ttu-id="83068-129">تمثل مهام عقدة الورقة العمل الأكثر تفصيلاً في المشروع.</span><span class="sxs-lookup"><span data-stu-id="83068-129">Leaf node tasks represent the most granular work on the project.</span></span> <span data-ttu-id="83068-130">إنها تتميز بمجهود مقدّر والموارد وتواريخ بدء وانتهاء مخططين ومدة.</span><span class="sxs-lookup"><span data-stu-id="83068-130">They have an estimated effort, resources, planned start and end dates, and a duration.</span></span>
 
## <a name="creating-a-task-hierarchy"></a><span data-ttu-id="83068-131">إنشاء التدرج الهرمي للمهام</span><span class="sxs-lookup"><span data-stu-id="83068-131">Creating a task hierarchy</span></span>

<span data-ttu-id="83068-132">يمكنك إنشاء تدرج هرمي للمهام باستخدام الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="83068-132">You can create a task hierarchy by using the following options:</span></span>

- <span data-ttu-id="83068-133">الزر **إضافة مهمة**</span><span class="sxs-lookup"><span data-stu-id="83068-133">**Add task** button</span></span>
- <span data-ttu-id="83068-134">الزر **تحريك المهمة إلى مستوى أدنى**.</span><span class="sxs-lookup"><span data-stu-id="83068-134">**Indent task** button</span></span>
- <span data-ttu-id="83068-135">الزر **تحريك المهمة إلى مستوى أعلى**.</span><span class="sxs-lookup"><span data-stu-id="83068-135">**Outdent task** button</span></span>
- <span data-ttu-id="83068-136">الزران **تحريك لأعلى** و **تحريك لأسفل**</span><span class="sxs-lookup"><span data-stu-id="83068-136">**Move up** and **Move down** buttons</span></span>
- <span data-ttu-id="83068-137">اختصارات لوحة المفاتيح وذوي الاحتياجات الخاصة</span><span class="sxs-lookup"><span data-stu-id="83068-137">Accessibility and keyboard shortcuts</span></span>

### <a name="add-task"></a><span data-ttu-id="83068-138">إضافة مهمة</span><span class="sxs-lookup"><span data-stu-id="83068-138">Add task</span></span>

<span data-ttu-id="83068-139">يتيح لك الزر **إضافة مهمة** إمكانية إنشاء مهمة جديدة في التدرج الهرمي.</span><span class="sxs-lookup"><span data-stu-id="83068-139">The **Add task** button lets you create a new task in the hierarchy.</span></span> <span data-ttu-id="83068-140">إذا لم تقم بتحديد موضع، فإنه يتم إدراج المهمة في النهاية.</span><span class="sxs-lookup"><span data-stu-id="83068-140">If you don't select a position, the task is inserted at the end.</span></span> 

<span data-ttu-id="83068-141">يتم تعيين معرف الجدول لكل مهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-141">A schedule ID is assigned to every task.</span></span> <span data-ttu-id="83068-142">يمثل معرف الجدول عمق وموضع المهمة في التدرج الهرمي.</span><span class="sxs-lookup"><span data-stu-id="83068-142">The schedule ID represents the task's depth and position in the hierarchy.</span></span> <span data-ttu-id="83068-143">ويستخدم ترقيم المخططات التفصيلية.</span><span class="sxs-lookup"><span data-stu-id="83068-143">It uses outline numbering.</span></span> <span data-ttu-id="83068-144">بالنسبة للمهام الموجودة في المستوي الأول أسفل العقدة الجذر للمشروع ، يتم استخدام نظام ترقيم من 1 و2 و3 وهكذا.</span><span class="sxs-lookup"><span data-stu-id="83068-144">For tasks in the first level under the project root node, a numbering scheme of 1, 2, 3, and so on, is used.</span></span> <span data-ttu-id="83068-145">بالنسبة للمهام ضمن المستوى الأول، يتم استخدام نظام ترقيم من 1.1 و1.2 و1.3 وهكذا.</span><span class="sxs-lookup"><span data-stu-id="83068-145">For tasks under the first level, a numbering scheme of 1.1, 1.2, 1.3, and so on, is used.</span></span>

### <a name="indent-task"></a><span data-ttu-id="83068-146">تحريك المهمة إلى مستوى أدنى</span><span class="sxs-lookup"><span data-stu-id="83068-146">Indent task</span></span>

<span data-ttu-id="83068-147">عند تحريك مهمة لأسفل، تصبح تابعة للمهمة التي فوقها مباشرةً.</span><span class="sxs-lookup"><span data-stu-id="83068-147">When a task is indented, it becomes a child of the task that is directly above it.</span></span> <span data-ttu-id="83068-148">ثم تتم إعادة حساب الجدول الزمني للمهمة بحيث يستند إلى معرف الجدول الأصلي الجديد ويتبع مخطط ترقيم المخطط التفصيلي.</span><span class="sxs-lookup"><span data-stu-id="83068-148">The schedule ID of the task is then recalculated so that it's based on the schedule ID of its new parent and follows the outline numbering scheme.</span></span> <span data-ttu-id="83068-149">تعتبر المهمة الأصل الآن مهمة ملخص أو مهمة حاوية.</span><span class="sxs-lookup"><span data-stu-id="83068-149">The parent task is now a summary task or a container task.</span></span> <span data-ttu-id="83068-150">ولذلك، تصبح قيمة محتسبة للمهام التابعة لها.</span><span class="sxs-lookup"><span data-stu-id="83068-150">Therefore, it becomes a rollup of its child tasks.</span></span>

### <a name="outdent-task"></a><span data-ttu-id="83068-151">تحريك المهمة إلى مستوى أعلى</span><span class="sxs-lookup"><span data-stu-id="83068-151">Outdent task</span></span> 

<span data-ttu-id="83068-152">عندما يتم تحريك أحدي المهام إلى مستوى أعلى، تصبح المهمة تابعة للمهمة الأصلية.</span><span class="sxs-lookup"><span data-stu-id="83068-152">When a task is outdented, it's no longer a child of the task that was its parent.</span></span> <span data-ttu-id="83068-153">ثم يتم بعد ذلك إعادة حساب معرف الجدول حتى يعكس عمق وموضع المهمة اللذين تم تحديثهما في التدرج الهرمي.</span><span class="sxs-lookup"><span data-stu-id="83068-153">The schedule ID is then recalculated so that it reflects the task's updated depth and position in the hierarchy.</span></span> <span data-ttu-id="83068-154">تتم إعادة حساب الجهد والتكلفة والتواريخ الخاصة بالمهمة الأصل السابقة التالي لا تتضمن هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-154">The effort, cost, and dates of the previous parent task are recalculated so that they don't include this task.</span></span>

### <a name="move-up-and-move-down"></a><span data-ttu-id="83068-155">تحريك لأعلى وتحريك لأسفل</span><span class="sxs-lookup"><span data-stu-id="83068-155">Move up and Move down</span></span> 

<span data-ttu-id="83068-156">ويقوم الزران **تحريك لأعلى** و **تحريك لأسفل** بتغيير موضع المهمة في التدرج الهرمي الأصل.</span><span class="sxs-lookup"><span data-stu-id="83068-156">The **Move up** and **Move down** buttons change the position of a task within its parent hierarchy.</span></span> <span data-ttu-id="83068-157">لا تؤثر التغييرات من هذا النوع على مجهود المهمة أو تكلفتها أو تواريخها أو مدتها.</span><span class="sxs-lookup"><span data-stu-id="83068-157">Changes of this type don't affect the task's effort, cost, dates, or duration.</span></span> <span data-ttu-id="83068-158">يتأثر فقط معرف الجدول الخاص بالمهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-158">Only the task's schedule ID is affected.</span></span> <span data-ttu-id="83068-159">تتم إعادة حساب معرف الجدول حتى يعكس الموضع الجديد للمهمة في قائمة المهام التابعة للأصل.</span><span class="sxs-lookup"><span data-stu-id="83068-159">The schedule ID is recalculated so that it reflects the task's new position in the parent's list of child tasks.</span></span>

### <a name="accessibility-and-keyboard-shortcuts"></a><span data-ttu-id="83068-160">اختصارات لوحة المفاتيح وذوي الاحتياجات الخاصة</span><span class="sxs-lookup"><span data-stu-id="83068-160">Accessibility and keyboard shortcuts</span></span>

<span data-ttu-id="83068-161">إن شبكة **الجدولة** يمكن الوصول اليها بالكامل ويمكن استخدامها مع قارئات الشاشة مثل المسرد أو JAWS أو NVDA.</span><span class="sxs-lookup"><span data-stu-id="83068-161">The **Schedule** grid is fully accessible and can be used with screen readers such as Narrator, JAWS, or NVDA.</span></span> <span data-ttu-id="83068-162">يمكنك التنقل خلال منطقه الشبكة باستخدام مفاتيح الأسهم (كما في Microsoft Excel)، يمكنك استخدام المفتاح Tab للتقدم من خلال عناصر واجهة المستخدم التفاعلية، ويمكنك استخدام مفتاح السهم لأسفل، أو مفتاح Enter، أو Spacebar لتحديد واستدعاء القوائم المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="83068-162">You can move through the grid area by using arrow keys (as in Microsoft Excel), you can use the Tab key to advance through the interactive UI elements, and you can use the Down arrow key, the Enter key, or the Spacebar to select and invoke the drop-down menus.</span></span> <span data-ttu-id="83068-163">وتكون رؤوس الأعمدة أيضا تفاعلية.</span><span class="sxs-lookup"><span data-stu-id="83068-163">The column headers are also interactive.</span></span> <span data-ttu-id="83068-164">يمكنك إخفاء الأعمدة وإظهارها، واستخدام المفتاح Tab ومفاتيح الأسهم للتنقل بين رؤوس الأعمدة، واستخدام أزرار الإجراء على شريط الأدوات.</span><span class="sxs-lookup"><span data-stu-id="83068-164">You can hide and show columns, use the Tab key and arrow keys to move through the column headers, and use the action buttons on the toolbar.</span></span> <span data-ttu-id="83068-165">بالإضافه إلى ذلك، يمكنك استخدام مفاتيح الاختصارات التالية:</span><span class="sxs-lookup"><span data-stu-id="83068-165">In addition, you can use the following keyboard shortcuts:</span></span>

- <span data-ttu-id="83068-166">**تحديث**:‏ ALT+SHIFT+F5</span><span class="sxs-lookup"><span data-stu-id="83068-166">**Refresh**: ALT+SHIFT+F5</span></span>
- <span data-ttu-id="83068-167">**إضافة**:‏ ALT+SHIFT+Insert</span><span class="sxs-lookup"><span data-stu-id="83068-167">**Add**: ALT+SHIFT+Insert</span></span>
- <span data-ttu-id="83068-168">**حذف**:‏ ALT+SHIFT+Delete</span><span class="sxs-lookup"><span data-stu-id="83068-168">**Delete**: ALT+SHIFT+Delete</span></span>
- <span data-ttu-id="83068-169">**تحريك لأعلى/لأسفل**: أسهم‏ ALT+SHIFT+Up/Down</span><span class="sxs-lookup"><span data-stu-id="83068-169">**Move up/down**: ALT+SHIFT+Up/Down arrows</span></span>
- <span data-ttu-id="83068-170">**التحريك لمستوى أدنى/أعلى**: أسهم ALT_SHIFT+Left/Right</span><span class="sxs-lookup"><span data-stu-id="83068-170">**Indent/Outdent**: ALT_SHIFT+Left/Right arrows</span></span>
- <span data-ttu-id="83068-171">**توسيع/طي التدرجات الهرمية**: مفاتيح ALT+SHIFT+Plus/Minus</span><span class="sxs-lookup"><span data-stu-id="83068-171">**Expand/Collapse Hierarchies**: ALT+SHIFT+Plus/Minus keys</span></span>

## <a name="task-attributes"></a><span data-ttu-id="83068-172">سمات المهمة</span><span class="sxs-lookup"><span data-stu-id="83068-172">Task attributes</span></span>

<span data-ttu-id="83068-173">يصف اسم المهمة العمل الذي يجب إكماله.</span><span class="sxs-lookup"><span data-stu-id="83068-173">A task's name describes the work that must be completed.</span></span> <span data-ttu-id="83068-174">في PSA ، تصف السمات المرتبطة بالمهمة جدول المهمة ومتطلبات التوظيف الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="83068-174">In PSA, the attributes that are associated with a task describe the schedule of the task and its staffing requirements.</span></span>

> ![سمات المهمة](media/project-2.png)
 
### <a name="schedule-attributes"></a><span data-ttu-id="83068-176">سمات الجدولة</span><span class="sxs-lookup"><span data-stu-id="83068-176">Schedule attributes</span></span>

<span data-ttu-id="83068-177">تحدد سمات **المجهود** و **تاريخ البدء** و **تاريخ الانتهاء** و **المدة** الجدول الخاص بالمهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-177">The **Effort**, **Start date**, **End date**, and **Duration** attributes define the schedule for the task.</span></span>

<span data-ttu-id="83068-178">وتتضمن سمات الجدولة الاضافية ما يلي:</span><span class="sxs-lookup"><span data-stu-id="83068-178">Additional schedule attributes include:</span></span>

- <span data-ttu-id="83068-179">**ساعات المجهود**: أدخل تقديرا للساعات المطلوبة لإكمال المهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-179">**Effort hours**: Enter an estimate of the hours that are required to complete the task.</span></span> 
- <span data-ttu-id="83068-180">**المدة**: حدد عدد أيام الإنجاز المطلوبة لإكمال المهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-180">**Duration**: Specify the number of workdays that are required to complete the task.</span></span>
- <span data-ttu-id="83068-181">**معرف الجدول**: يتم استخدام المعرف الذي تم إنشاؤه تلقائيًا لطلب المهام في التدرج الهرمي.</span><span class="sxs-lookup"><span data-stu-id="83068-181">**Schedule ID**: This automatically generated ID is used to order tasks in the hierarchy.</span></span> <span data-ttu-id="83068-182">تدير التبعيات بين المهام الترتيب الفعلي الذي تم العمل على المهام فيه.</span><span class="sxs-lookup"><span data-stu-id="83068-182">Dependencies between the tasks manage the actual order in which the tasks are worked on.</span></span>
 
### <a name="staffing-attributes"></a><span data-ttu-id="83068-183">سمات التوظيف</span><span class="sxs-lookup"><span data-stu-id="83068-183">Staffing attributes</span></span>

<span data-ttu-id="83068-184">يتم الوصول إلى سمات التوظيف من خلال حقل **الموارد** في الجدول.</span><span class="sxs-lookup"><span data-stu-id="83068-184">Staffing attributes are accessed through the **Resources** field in the schedule.</span></span> <span data-ttu-id="83068-185">يمكنك إما البحث عن مورد موجود، أو النقر فوق **إنشاء** وفي جزء **الإنشاء السريع**، أضف عضو فريق مشروع كمورد جديد.</span><span class="sxs-lookup"><span data-stu-id="83068-185">You can either search for an existing resource, or click **Create** and in the **Quick Create** pane, add a project team member as a new resource.</span></span>

<span data-ttu-id="83068-186">يتم استخدام حقول **الدور** و **وحدة تعيين الموارد‬** و **اسم المنصب** لوصف متطلبات الموظفين للمهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-186">The **Role**, **Resourcing Unit**, and **Position Name** fields are used to describe the staffing requirements for the task.</span></span> <span data-ttu-id="83068-187">يتم استخدام سمات التوظيف هذه مع جداول المهام للعثور على الموارد المتوفرة لتنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-187">These staffing attributes together with the task schedule are used to find available resources to do this task.</span></span>

<span data-ttu-id="83068-188">**الدور** -حدد نوع المورد المطلوب لتنفيذ المهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-188">**Role** - Specify the type of resource that is required to do the task.</span></span>

<span data-ttu-id="83068-189">**وحدة تعيين الموارد** - حدد الوحدة التي ينبغي تعيين الموارد الخاصة بالمهمة منها.</span><span class="sxs-lookup"><span data-stu-id="83068-189">**Resourcing unit** - Specify the unit that resources for the task should be assigned from.</span></span> <span data-ttu-id="83068-190">تؤثر هذه السمة على تقدير التكلفة والمبيعات الخاصة بالمهمة في حالة تعيين التكلفة وسعر الفاتورة للمورد بناء على وحدات تعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="83068-190">This attribute affects the cost and sales estimate for the task if the cost and bill rate for the resource are set based on resourcing units.</span></span>

<span data-ttu-id="83068-191">**اسم المنصب** – ادخل اسما مألوفا للمورد العام الذي يعمل كعنصر نائب للمورد الذي سيقوم بالعمل في النهاية.</span><span class="sxs-lookup"><span data-stu-id="83068-191">**Position name** – Enter a friendly name for the generic resource that serves as a placeholder for the resource that will ultimately do the work.</span></span>

<span data-ttu-id="83068-192">يحتوي حقل **الموارد** على اسم المنصب الخاص بالمورد العام أو المورد المسمى عند العثور على واحد.</span><span class="sxs-lookup"><span data-stu-id="83068-192">The **Resources** field holds the position name of the generic resource or named resource when one is found.</span></span>

<span data-ttu-id="83068-193">ويحتوي حقل **الفئة** على القيم التي تشير إلى نوع أكبر من العمل الذي يمكن تجميع المهمة فيه.</span><span class="sxs-lookup"><span data-stu-id="83068-193">The **Category** field holds the values that indicate a broader type of work that the task can be grouped into.</span></span> <span data-ttu-id="83068-194">لا يؤثر هذا الحقل في الجدولة أو الموظفين.</span><span class="sxs-lookup"><span data-stu-id="83068-194">This field doesn't affect scheduling or staffing.</span></span> <span data-ttu-id="83068-195">ويُستخدم لإعداد التقارير فقط.</span><span class="sxs-lookup"><span data-stu-id="83068-195">It's used only for reporting.</span></span>

### <a name="task-dependencies"></a><span data-ttu-id="83068-196">تبعيات المهمة</span><span class="sxs-lookup"><span data-stu-id="83068-196">Task dependencies</span></span> 

<span data-ttu-id="83068-197">يمكنك استخدام الجدول في PSA لإنشاء العلاقات السابقة بين المهام.</span><span class="sxs-lookup"><span data-stu-id="83068-197">You can use the schedule in PSA to create predecessor relationships between tasks.</span></span> <span data-ttu-id="83068-198">يأخذ حقل **النشاط السابق** ضمن **المهام** قيمه واحدة أو أكثر للإشارة إلى المهام التي تعتمد عليها المهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-198">The **Predecessor** field under **Tasks** takes one or more values to indicate the tasks that a task depends on.</span></span> <span data-ttu-id="83068-199">عند تعيين قيم أنشطة سابقة لمهمة، يمكن بدء المهمة فقط بعد إكمال كافة المهام السابقة.</span><span class="sxs-lookup"><span data-stu-id="83068-199">When predecessor values are assigned to a task, the task can start only after all the predecessor tasks have been completed.</span></span> <span data-ttu-id="83068-200">وبسبب التبعية، تتم إعادة تعيين تاريخ البدء المخطط للمهمة إلى تاريخ إتمام المهام السابقة.</span><span class="sxs-lookup"><span data-stu-id="83068-200">Because of the dependency, the planned start date of the task is reset to the date when the predecessor tasks are completed.</span></span>

<span data-ttu-id="83068-201">لا يؤثر وضع المهمة على التحديثات التي يتم إجراؤها على تاريخي البدء والانتهاء للمهام السابقة/التابعة.</span><span class="sxs-lookup"><span data-stu-id="83068-201">The task mode has no effect on updates that are made to the start and end dates of predecessor/dependent tasks.</span></span>

## <a name="task-mode"></a><span data-ttu-id="83068-202">وضع المهمة</span><span class="sxs-lookup"><span data-stu-id="83068-202">Task mode</span></span> 

<span data-ttu-id="83068-203">يحدد وضع المهمة جدولة مهام العقدة الطرفية.</span><span class="sxs-lookup"><span data-stu-id="83068-203">The task mode determines the scheduling of leaf node tasks.</span></span> <span data-ttu-id="83068-204">يدعم PSA وضعي مهام لكل مهمة: الجدولة التلقائية والجدولة اليدوية.</span><span class="sxs-lookup"><span data-stu-id="83068-204">PSA supports two task modes for every task: automatic scheduling and manual scheduling.</span></span>

### <a name="auto-scheduling"></a><span data-ttu-id="83068-205">الجدولة التلقائية</span><span class="sxs-lookup"><span data-stu-id="83068-205">Auto-scheduling</span></span> 
 
<span data-ttu-id="83068-206">عند تعيين وضع المهمة إلى **تمت الجدولة تلقائيًا**، يستخدم محرك جدولة المهمة قواعد الجدولة على سمات المهمة التالية لتحديد الجدول الزمني للمهمة.</span><span class="sxs-lookup"><span data-stu-id="83068-206">When task mode is set to **Automatically Scheduled** for a task, the task scheduling engine uses the scheduling rules on task attributes to determine the schedule for the task.</span></span>

#### <a name="scheduling-rules"></a><span data-ttu-id="83068-207">قواعد الجدولة</span><span class="sxs-lookup"><span data-stu-id="83068-207">Scheduling rules</span></span>

<span data-ttu-id="83068-208">بشكل افتراضي، لا تشتمل مهمة عقدة طرفية على مهام سابقة، تم تعيين تاريخ البدء الخاص بها إلى تاريخ البدء المجدول للمشروع.</span><span class="sxs-lookup"><span data-stu-id="83068-208">By default, if a leaf node task doesn't have predecessors, its start date is set to the project's scheduled start date.</span></span> <span data-ttu-id="83068-209">يتم حساب مدة مهمة العقدة الطرفية دائمًا كعدد أيام العمل بين تاريخي البدء والانتهاء.</span><span class="sxs-lookup"><span data-stu-id="83068-209">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="83068-210">عندما تتم جدولة مهمة تلقائيًا، يتبع محرك الجدولة القواعد التالية:</span><span class="sxs-lookup"><span data-stu-id="83068-210">When a task is automatically scheduled, the scheduling engine follows these rules:</span></span>

- <span data-ttu-id="83068-211">يجب أن يكون تاريخي بدء وانتهاء المهمة عبارة عن أيام عمل وفقًا لتقويم جدولة المشروع.</span><span class="sxs-lookup"><span data-stu-id="83068-211">The start and end dates of the task must be working days, according to the project's scheduling calendar.</span></span> 
- <span data-ttu-id="83068-212">بالنسبة إلى أي مهمة لها مهام سابقة، يتم تعيين تاريخ البدء تلقائيًا على آخر تاريخ نهاية لسابقاتها.</span><span class="sxs-lookup"><span data-stu-id="83068-212">For any task that has predecessor tasks, the start date is automatically set to the latest end date of its predecessors.</span></span>
- <span data-ttu-id="83068-213">يتم حساب الجهد باستخدام هذه الصيغة: عدد الأشخاص × المدة × ساعة في يوم عمل قياسي في تقويم المشروع.</span><span class="sxs-lookup"><span data-stu-id="83068-213">Effort is calculated by using this formula: Number of people × Duration × Hours in a standard workday in the project calendar.</span></span>

### <a name="manual-scheduling"></a><span data-ttu-id="83068-214">الجدولة اليدوية</span><span class="sxs-lookup"><span data-stu-id="83068-214">Manual scheduling</span></span>

<span data-ttu-id="83068-215">إذا كانت قواعد الجدولة التلقائية لا تفي بمتطلباتك، فيمكنك تعيين وضع المهمة للهمهة المُراد **جدولتها يدويًا**.</span><span class="sxs-lookup"><span data-stu-id="83068-215">If the rules of automatic scheduling don't meet your requirements, you can set the task mode for the task to **Manually Scheduled**.</span></span> <span data-ttu-id="83068-216">يؤدي هذا الإعداد إلى توقف محرك الجدولة عن حساب القيم لسمات جدولة أخرى.</span><span class="sxs-lookup"><span data-stu-id="83068-216">This setting stops the scheduling engine from calculating the values of other scheduling attributes.</span></span> <span data-ttu-id="83068-217">وبغض النظر عن وضع المهمة، إذا قمت بتعيين المهام السابقة على المهام، فسيؤثر دائمًا على تاريخ البدء للمهمة التابعة.</span><span class="sxs-lookup"><span data-stu-id="83068-217">Regardless of the task mode, if you set predecessors on tasks, you always affect the dependent task's start date.</span></span>
