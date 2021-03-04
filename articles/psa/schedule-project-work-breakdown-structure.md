---
title: جدولة مشروع مع هيكل تنظيم العمل
description: كيفية جدولة مشروع مع هيكل تنظيم العمل في Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: cf12cc3bcf061e1daffafb248cfd76809c6444ec
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149797"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a><span data-ttu-id="f6ee4-103">جدولة مشروع مع هيكل تنظيم العمل (Project Service)</span><span class="sxs-lookup"><span data-stu-id="f6ee4-103">Schedule a project with a work breakdown structure (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="f6ee4-104">يقوم جدول المشروع بالتبليغ عن العمل الذي يحتاج إلى تنفيذ والموارد التي ستنفذ العمل والإطار الزمني الذي يجب إكمال العمل ضمنه.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-104">A project schedule communicates what work needs to be performed, which resources will perform the work, and the timeframe in which that work needs to be completed.</span></span> <span data-ttu-id="f6ee4-105">يعكس جدول المشروع جميع الأعمال المرتبطة بتسليم المشروع في الوقت المحدد.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-105">The project schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="f6ee4-106">إحدى الخطوات الأولى في مرحلة بدء المشروع هي وضع جدول مشروع.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-106">One of the first steps in the initiation phase of the project is to come up with a project schedule.</span></span> <span data-ttu-id="f6ee4-107">لإنشاء جدول مشروع، تحتاج إلى إنشاء هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-107">To establish a project schedule, you need to create a work breakdown structure.</span></span>  
  
 <span data-ttu-id="f6ee4-108">أنشئ هيكل مشروع مع هيكل تنظيم العمل، مما يساعدك على:</span><span class="sxs-lookup"><span data-stu-id="f6ee4-108">Create a project structure with a work breakdown structure, which helps you:</span></span>  
  
- <span data-ttu-id="f6ee4-109">تنظيم العمل في مهام قابلة للإدارة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-109">Break down work into manageable tasks</span></span>  
  
- <span data-ttu-id="f6ee4-110">تقدير الوقت اللازم لإتمام المهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-110">Estimate the time required to complete a task</span></span>  
  
- <span data-ttu-id="f6ee4-111">تعيين تبعيات المهمة ومدة المهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-111">Set task dependencies and task duration</span></span>  
  
- <span data-ttu-id="f6ee4-112">تحديد الأدوار المطلوبة لإكمال كل مهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-112">Determine the roles required to complete each task</span></span>  
  
  <span data-ttu-id="f6ee4-113">يتميز جدول المشروع في هيكل تنظيم العمل بشكل وأسلوب عرض مألوفين، ويكتمل مع مخطط جانت التفاعلي.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-113">The project schedule in the work breakdown structure has a familiar look and feel, complete with an interactive Gantt chart.</span></span>  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a><span data-ttu-id="f6ee4-114">إنشاء هيكل تنظيم العمل لمشروع</span><span class="sxs-lookup"><span data-stu-id="f6ee4-114">Create a work breakdown structure for a project</span></span>  
 <span data-ttu-id="f6ee4-115">أنشئ هيكل تنظيم العمل لتمثيل تسلسل المهام في المشروع.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-115">Create a work breakdown structure to represent the sequence of tasks in a project.</span></span> <span data-ttu-id="f6ee4-116">يتضمن هيكل تنظيم العمل المهام، ومتطلبات كل مهمة، ومعلومات التكلفة والإيراد.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-116">The work breakdown structure includes tasks, requirements for each task, and revenue and cost information.</span></span> <span data-ttu-id="f6ee4-117">في هيكل تنظيم العمل، يمكنك إضافة:</span><span class="sxs-lookup"><span data-stu-id="f6ee4-117">In your work breakdown structure, you can add:</span></span>  
  
-   <span data-ttu-id="f6ee4-118">تسلسل المهام في تدرج هرمي</span><span class="sxs-lookup"><span data-stu-id="f6ee4-118">The sequence of tasks in a hierarchy</span></span>  
  
-   <span data-ttu-id="f6ee4-119">المهام الأخرى، إن وجدت، التي يجب إكمالها قبل بدء مهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-119">Other tasks, if any, that must be completed before a task can be started</span></span>  
  
-   <span data-ttu-id="f6ee4-120">تاريخ البدء وتاريخ الانتهاء ومدة المهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-120">The starting date, ending date, and duration of a task</span></span>  
  
-   <span data-ttu-id="f6ee4-121">عدد الساعات المطلوبة لمهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-121">The number of hours required for a task</span></span>  
  
-   <span data-ttu-id="f6ee4-122">أي مستويات تعليم ومهارات مطلوبة للعامل</span><span class="sxs-lookup"><span data-stu-id="f6ee4-122">Any required worker skills and education</span></span>  
  
-   <span data-ttu-id="f6ee4-123">العاملون المكلفون بتنفيذ مهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-123">The workers who are assigned to a task</span></span>  
  
-   <span data-ttu-id="f6ee4-124">الإيرادات والتكاليف المقدرة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-124">Estimated revenue and costs</span></span>  
  
## <a name="task-types"></a><span data-ttu-id="f6ee4-125">أنواع المهام</span><span class="sxs-lookup"><span data-stu-id="f6ee4-125">Task types</span></span>  
<span data-ttu-id="f6ee4-126">ستستخدم أنواع المهام التالية عند إنشاء هيكل تنظيم العمل:</span><span class="sxs-lookup"><span data-stu-id="f6ee4-126">You’ll use the following types of tasks when creating your work breakdown structure:</span></span>  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| <span data-ttu-id="f6ee4-127">**عقدة الجذر للمشروع**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-127">**Project root node**</span></span> | <span data-ttu-id="f6ee4-128">المهمة الموجزة للمشروع الأعلى مستوى.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-128">The top-level summary task for the project.</span></span> <span data-ttu-id="f6ee4-129">يتم إنشاء كافة مهام المشروع تحتها.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-129">All other project tasks are created under it.</span></span> <span data-ttu-id="f6ee4-130">اسم المهمة الجذر هو اسم المشروع.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-130">The name of the root task is the project name.</span></span> <span data-ttu-id="f6ee4-131">يستند المجهود والتواريخ ومدة عقدة الجذر إلى القيم الموجودة في التدرج الهرمي أدناها.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-131">The effort, dates, and duration of the root node are based on the values on the hierarchy below it.</span></span> <span data-ttu-id="f6ee4-132">لا يمكنك تحرير خصائص عقدة الجذر أو حذف عقدة الجذر.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-132">You can’t edit root node properties or delete the root node.</span></span> | 
| <span data-ttu-id="f6ee4-133">**المهام الموجزة أو مهام الحاوية**</span><span class="sxs-lookup"><span data-stu-id="f6ee4-133">**Summary or container tasks**</span></span> | <span data-ttu-id="f6ee4-134">المهمة الموجزة هي مهمة لديها مهام فرعية تحتها.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-134">A summary task is a task that has sub-tasks under it.</span></span> <span data-ttu-id="f6ee4-135">لا تتضمن المهمة الموجزة أي مجهود عمل أو تكلفة خاصة بها.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-135">A summary task doesn’t have any work effort or cost of its own.</span></span> <span data-ttu-id="f6ee4-136">يُعتبر مجهود العمل في المهمة الموجزة وتكلفتها القيمة المحتسبة لمهامها الفرعية.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-136">Its work effort and cost are a rollup of its sub-tasks.</span></span> <span data-ttu-id="f6ee4-137">يمكنك تغيير اسم المهمة الموجزة، ولكن لا يمكنك تغيير المجهود أو التواريخ أو المدة، إذ يتم احتساب هذه العناصر تلقائيًا.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-137">You can change the name of a summary task, but you can’t change the effort, dates, or duration, because those are automatically calculated.</span></span> <span data-ttu-id="f6ee4-138">يؤدي حذف مهمة موجزة إلى حذف المهمة وكافة مهامها الفرعية.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-138">Deleting a summary task deletes the task and all of its sub-tasks.</span></span>|  
| <span data-ttu-id="f6ee4-139">**مهام العقدة الطرفية**</span><span class="sxs-lookup"><span data-stu-id="f6ee4-139">**Leaf node tasks**</span></span> | <span data-ttu-id="f6ee4-140">تمثل مهمة العقدة الطرفية العمل الأكثر تفصيلاً في المشروع.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-140">A leaf node task represents the most detailed work on the project.</span></span> <span data-ttu-id="f6ee4-141">إنها تتميز بمجهود مقدّر وعدد من الموارد المخططة وتواريخ بدء وانتهاء مخططين ومدة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-141">It has an estimated effort, a planned number of resources, planned start and end dates, and a duration.</span></span>|

  
## <a name="task-hierarchy"></a><span data-ttu-id="f6ee4-142">التدرج الهرمي للمهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-142">Task hierarchy</span></span>  
 <span data-ttu-id="f6ee4-143">لديك الخيارات التالية عند إنشاء تدرج هرمي لمهمة:</span><span class="sxs-lookup"><span data-stu-id="f6ee4-143">You have the following options when creating a task hierarchy:</span></span>  
  
- <span data-ttu-id="f6ee4-144">**إضافة مهمة**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-144">**Add task**.</span></span>   <span data-ttu-id="f6ee4-145">يمكنك إضافة مهمة في الموضع الذي تختاره في التدرج الهرمي للمهمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-145">You can add a task at a position you choose in the task hierarchy.</span></span> <span data-ttu-id="f6ee4-146">إذا لم تقم بتحديد موضع، فستظهر المهمة في النهاية.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-146">If you don’t select a position, your new task appears at the end.</span></span>  
  
- <span data-ttu-id="f6ee4-147">**تحريك المهمة إلى مستوى أدنى**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-147">**Indent task**.</span></span>   <span data-ttu-id="f6ee4-148">يمكنك تحريك مهمة إلى مستوى أدنى لجعلها مهمة تابعة للمهمة الموجودة فوقها مباشرة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-148">Indent a task to make it a child of the task directly above it.</span></span>  
  
- <span data-ttu-id="f6ee4-149">**تحريك المهمة إلى مستوى أعلى**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-149">**Outdent task**.</span></span>   <span data-ttu-id="f6ee4-150">يمكنك تحريك المهمة إلى مستوى أعلى بحيث لا تعود مهمة فرعية لمهمتها الأصلية الأساسية.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-150">Outdent a task to make it so it’s no longer a sub-task of its original parent task.</span></span>  
  
- <span data-ttu-id="f6ee4-151">**تحريك لأعلى وتحريك لأسفل**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-151">**Move up and Move down**.</span></span>   <span data-ttu-id="f6ee4-152">تحريك المهام للأعلى وللأسفل في التدرج الهرمي للمهمة الأصلية.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-152">Move tasks up and down in the hierarchy of its parent task.</span></span> <span data-ttu-id="f6ee4-153">لا يؤثر تحريك مهمة للأعلى أو للأسفل على مجهودها أو تكلفتها أو تواريخها أو مدتها.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-153">Moving a task up or down has no effect on its effort, cost, dates, or duration.</span></span>  
  
## <a name="task-attributes"></a><span data-ttu-id="f6ee4-154">سمات المهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-154">Task attributes</span></span>  
 <span data-ttu-id="f6ee4-155">يصف اسم المهمة العمل الذي يجب إكماله.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-155">A task’s name describes the work that needs to be completed.</span></span> <span data-ttu-id="f6ee4-156">يمكنك استخدام سمات مهمة مختلفة لوصف الجدول واحتياجات التوظيف للمهمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-156">You use various task attributes to describe the schedule and staffing requirements for the task.</span></span>  
  
### <a name="schedule-attributes"></a><span data-ttu-id="f6ee4-157">سمات الجدولة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-157">Schedule attributes</span></span>

 - <span data-ttu-id="f6ee4-158">قم بتعيين قيم إلى **ساعات المجهود** و **عدد الموارد** و **تاريخ البدء** و **تاريخ الانتهاء** و **المدة** لتحديد جدول للمهمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-158">Assign values to **Effort hours**, **Number of resources**, **Start date**, **End date**, and **Duration** to determine the schedule for the task.</span></span> 
 - <span data-ttu-id="f6ee4-159">**المجهود** عبارة عن تقدير للساعات التي يستغرقها إكمال المهمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-159">**Effort** is an estimate of the hours it takes to complete the task.</span></span>
 - <span data-ttu-id="f6ee4-160">**عدد الموارد** عبارة عن تقدير يضعه مدير المشروع في المهمة للمساعدة في التوصل إلى أفضل جدول محتمل.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-160">**Number of resources** is an estimate that the project manager puts in the task to help come up with the best possible schedule.</span></span> 
 - <span data-ttu-id="f6ee4-161">**المدة** (بالأيام) تشير إلى عدد أيام العمل الذي سوف يستغرقه إكمال المهمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-161">**Duration** (in days) indicates the number of work days it will take to complete the task.</span></span>  
  
### <a name="staffing-attributes"></a><span data-ttu-id="f6ee4-162">سمات التوظيف</span><span class="sxs-lookup"><span data-stu-id="f6ee4-162">Staffing attributes</span></span>

 - <span data-ttu-id="f6ee4-163">تصف خيارات **الدور** و **الوحدة التنظيمية للمورد‬** و **عدد الموارد** و **الموارد** متطلبات التوظيف الخاصة بالمهمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-163">**Role**, **Resource organizational unit**, **Number of resources**, and **Resources** describe the staffing requirements for the task.</span></span> 
 - <span data-ttu-id="f6ee4-164">**الدور** يصف نوع المورد المطلوب لتنفيذ المهمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-164">**Role** describes the type of resource needed to perform the task.</span></span> 
 - <span data-ttu-id="f6ee4-165">**الوحدة التنظيمية للمورد** تشير إلى الوحدة التنظيمية التي ينبغي تعيين الموارد منها لهذه المهمة؛ يؤثر ذلك أيضًا على تقدير التكلفة والمبيعات للمهمة، إذ يتم حسابه عند تحديد سعر مبيعات الوحدة للمورد.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-165">**Resource organizational unit** indicates the organizational unit from which resources should be staffed for that task; this also impacts the cost and sales estimate of the task, since this is accounted for when determining the unit sales price for the resource.</span></span> 
 - <span data-ttu-id="f6ee4-166">**الموارد** تحتوي على مورد عام أو مورد مسمى عندما يتم العثور على واحد.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-166">**Resources** holds a generic resource or a named resource when one is found.</span></span>  
  
## <a name="task-dependencies"></a><span data-ttu-id="f6ee4-167">تبعيات المهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-167">Task dependencies</span></span>  
 <span data-ttu-id="f6ee4-168">يمكنك إنشاء علاقات نشاط سابق بين مهمة واحدة أو أكثر في هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-168">You can create predecessor relationships between one or more tasks in the work breakdown structure.</span></span> <span data-ttu-id="f6ee4-169">يمكنك تعيين قيمة واحدة أو أكثر لحقل المهمة السابقة على المهام للإشارة إلى المهام التي سوف يعتمد عليها.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-169">You can set one or more values for the predecessor field on tasks to indicate the tasks that it will be dependent on.</span></span> <span data-ttu-id="f6ee4-170">عند تعيين قيمة مهمة سابقة لمهمة، يمكن بدء المهمة فقط عند إكمال كافة المهام السابقة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-170">When you assign a predecessor value to a task, the task can only start when all the predecessor tasks have completed.</span></span> <span data-ttu-id="f6ee4-171">سيؤدي تعيين هذه التبعية على مهمة إلى إعادة حساب تاريخ البدء المخطط للمهمة كتاريخ الانتهاء الأخير لكافة المهام السابقة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-171">Setting this dependency on a task will result in the recalculation of the planned start date of the task as the latest end of all of its predecessors.</span></span> <span data-ttu-id="f6ee4-172">الآثار ذات الصلة بالنشاط السابق على الجدول لا تتحدد بوضع المهمة المحدد في المهمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-172">Predecessor-related impacts on a schedule are not limited by the task mode defined on the task.</span></span>  
  
## <a name="task-mode"></a><span data-ttu-id="f6ee4-173">وضع المهمة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-173">Task mode</span></span>  
 <span data-ttu-id="f6ee4-174">وضع المهمة هو أحد العوامل الهامة التي تحدد جدولة مهام العقدة الطرفية.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-174">Task mode is one of the important factors that determine scheduling leaf node tasks.</span></span> <span data-ttu-id="f6ee4-175">هناك وضعان للمهمة في كل مهمة: وضع الجدولة التلقائية ووضع الجدولة اليدوية.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-175">There are two task modes for every task: auto scheduling mode and manual scheduling mode.</span></span>  
  
-   <span data-ttu-id="f6ee4-176">**الجدولة الآلية**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-176">**Auto scheduling**.</span></span>   <span data-ttu-id="f6ee4-177">عند تعيين وضع المهمة إلى "تمت الجدولة تلقائيًا‬"، يستخدم محرك جدولة المهمة قواعد الجدولة على سمات المهمة التالية لتحديد الجدول الزمني للمهمة:</span><span class="sxs-lookup"><span data-stu-id="f6ee4-177">When you set the task mode to Automatically Scheduled, the task scheduling engine uses the scheduling rules on the following task attributes to determine the schedule for the task:</span></span>  
  
    -   <span data-ttu-id="f6ee4-178">الأنشطة السابقة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-178">Predecessors</span></span>  
  
    -   <span data-ttu-id="f6ee4-179">المجهود</span><span class="sxs-lookup"><span data-stu-id="f6ee4-179">Effort</span></span>  
  
    -   <span data-ttu-id="f6ee4-180">عدد الموارد</span><span class="sxs-lookup"><span data-stu-id="f6ee4-180">Number of resources</span></span>  
  
    -   <span data-ttu-id="f6ee4-181">تواريخ البدء والانتهاء</span><span class="sxs-lookup"><span data-stu-id="f6ee4-181">Start and end dates</span></span>  
  
-   <span data-ttu-id="f6ee4-182">**قواعد الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-182">**Scheduling rules**.</span></span>   <span data-ttu-id="f6ee4-183">تاريخ بدء مهمة عقدة طرفية ليس لديها مهام سابقة تم تعيينها بشكل افتراضي إلى تاريخ بدء جدولة المشروع.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-183">The start date of a leaf node task that does not have predecessors defaults to the project’s scheduling start date.</span></span> <span data-ttu-id="f6ee4-184">يتم حساب مدة مهمة العقدة الطرفية دائمًا كعدد أيام العمل بين تاريخي البدء والانتهاء.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-184">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="f6ee4-185">عندما تتم جدولة مهمة تلقائيًا، يتبع محرك الجدولة القواعد المذكورة أدناه:</span><span class="sxs-lookup"><span data-stu-id="f6ee4-185">When a task is automatically scheduled, the scheduling engine follows the rules below:</span></span>  
  
    -   <span data-ttu-id="f6ee4-186">يجب أن يكون تاريخي بدء وانتهاء المهمة عبارة عن أيام عمل في كل الأوقات وفقًا لتقويم جدولة المشروع</span><span class="sxs-lookup"><span data-stu-id="f6ee4-186">Start and end dates of a task must always be working days according to the project’s scheduling calendar</span></span>  
  
    -   <span data-ttu-id="f6ee4-187">تاريخ بدء مهمة لديها مهام سابقة تم تعيينها بشكل افتراضي إلى تاريخ الانتهاء الأخير لمهامها السابقة</span><span class="sxs-lookup"><span data-stu-id="f6ee4-187">The start date of a task that has predecessors defaults to the latest end date of its predecessors</span></span>  
  
    -   <span data-ttu-id="f6ee4-188">المجهود = عدد الأشخاص \* مدة \* الساعات في يوم عمل قياسي لتقويم المشروع</span><span class="sxs-lookup"><span data-stu-id="f6ee4-188">Effort = Number of people \* Duration \* hours in a standard work day of the project calendar</span></span>  
  
-   <span data-ttu-id="f6ee4-189">**الجدولة اليدوية**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-189">**Manual scheduling**.</span></span>   <span data-ttu-id="f6ee4-190">في بعض الحالات، قد تحتاج إلى الخروج عن هذه القواعد.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-190">In some cases, you might want to deviate from these rules.</span></span> <span data-ttu-id="f6ee4-191">في هذه الحالات، يمكنك تعيين وضع المهمة للمهمة بحيث تتم جدولتها يدويًا.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-191">In these cases, you can set the task mode for the task to be manually scheduled.</span></span> <span data-ttu-id="f6ee4-192">يؤدي ذلك إلى توقف محرك الجدولة عن حساب القيم لسمات جدولة أخرى.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-192">This stops the scheduling engine from calculating the values for other scheduling attributes.</span></span> <span data-ttu-id="f6ee4-193">يؤثر دائمًا تعيين المهام السابقة على المهام في تاريخ بدء المهمة التابعة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-193">Setting predecessors on tasks always impacts the dependent task’s start date.</span></span>  
  
## <a name="create-a-work-breakdown-structure"></a><span data-ttu-id="f6ee4-194">إنشاء هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="f6ee4-194">Create a work breakdown structure</span></span>  
  
1.  <span data-ttu-id="f6ee4-195">انتقل إلى **Project Service > المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-195">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="f6ee4-196">انقر فوق المشروع الذي تريد العمل عليه.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-196">Click the project you want to work on.</span></span>  
  
3.  <span data-ttu-id="f6ee4-197">في الشريط عبر الجزء العلوي من الشاشة، حدد السهم لأسفل الموجود بجوار اسم المشروع، ثم انقر فوق "هيكل تنظيم العمل".</span><span class="sxs-lookup"><span data-stu-id="f6ee4-197">In the bar across the top of the screen, select the down arrow next to the project name, and then click Work breakdown structure.</span></span>  
  
4.  <span data-ttu-id="f6ee4-198">لإضافة مهمة، انقر فوق **إضافة مهمة**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-198">To add a task, click **Add Task**.</span></span> <span data-ttu-id="f6ee4-199">املأ الحقول المطلوبة للمهمة، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-199">Fill in the fields for the task, and then click **Save**.</span></span>  
  
5.  <span data-ttu-id="f6ee4-200">تابع إضافة المهام حتى اكتمال هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-200">Continue adding tasks until your work breakdown structure is complete.</span></span> <span data-ttu-id="f6ee4-201">أثناء إنشاء هيكل تنظيم العمل، يمكنك القيام بما يلي لتنظيم المهام:</span><span class="sxs-lookup"><span data-stu-id="f6ee4-201">While creating your work breakdown structure, you can do the following to organize your tasks:</span></span>  
  
    -   <span data-ttu-id="f6ee4-202">حدد مهمة وانقر فوق **التحريك إلى مستوى أدنى** لنقل المهمة تحت مهمة أخرى، أو انقر فوق "تحريك إلى مستوى أعلى" لتحريكها إلى مستوى أعلى.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-202">Select a task and click **Indent** to move it under another task or click Outdent to move it out a level.</span></span>  
  
    -   <span data-ttu-id="f6ee4-203">حدد مهمة وانقر فوق **تحريك لأعلى** أو **تحريك لأسفل** لتحريكها لأعلى أو لأسفل في القائمة.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-203">Select a task and click **Move Up** or **Move Down** to move it up or down in the list.</span></span>  
  
    -   <span data-ttu-id="f6ee4-204">انقر فوق **إخفاء جانت** لإخفاء مخطط جانت، وانقر فوق **عرض جانت** لعرضه مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-204">Click **Hide Gantt** to hide the Gantt chart, and click **Show Gantt** to display it again.</span></span>  
  
    -   <span data-ttu-id="f6ee4-205">حدد فترة زمنية مختلفة لمخطط جانت في **مقياس الوقت**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-205">Select a different period of time for the Gantt chart in **Time Scale**.</span></span>  
  
6.  <span data-ttu-id="f6ee4-206">لإضافة الأدوار التي قمت بتحديدها في هيكل تنظيم العمل إلى أعضاء فريق المشروع، انقر فوق **إنشاء فريق المشروع**.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-206">To add the roles you specified in your work breakdown structure to your project’s team members, click **Generate Project Team**.</span></span>  
  
7.  <span data-ttu-id="f6ee4-207">انقر فوق الزر **حفظ** في الزاوية السفلية اليسرى من الشاشة عندما تنتهي من إدخال التغييرات.</span><span class="sxs-lookup"><span data-stu-id="f6ee4-207">Click **Save** at the bottom right corner of the screen when you’re done making changes.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="f6ee4-208">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="f6ee4-208">See Also</span></span>  
 [<span data-ttu-id="f6ee4-209">دليل مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="f6ee4-209">Project manager guide</span></span>](../psa/project-manager-guide.md)
