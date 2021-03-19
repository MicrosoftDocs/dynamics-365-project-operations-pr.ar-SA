---
title: تقدم المشروع واستهلاك التكلفة‬
description: يقدم هذا الموضوع معلومات حول تعقب تقدم المشروع واستهلاك التكلفة.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/21/2020
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
ms.openlocfilehash: 73b23aad2976c8ccbb542fc2dda1d96dd9f5714b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283622"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="a1f3a-103">تقدم المشروع واستهلاك التكلفة‬</span><span class="sxs-lookup"><span data-stu-id="a1f3a-103">Project progress and cost consumption</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a1f3a-104">تختلف الحاجة إلى تعقب التقدم مقابل جدول حسب الصناعة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="a1f3a-105">تتبع بعض الصناعات مستوى حبيبيًا ، بينما تتبع صناعات أخرى مستوى أعلى.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="a1f3a-106">يوضح هذا الموضوع كيفية الجدولة من أجل تلبية متطلبات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="a1f3a-107">طريقة عرض تعقب الجهود</span><span class="sxs-lookup"><span data-stu-id="a1f3a-107">Effort tracking view</span></span>

<span data-ttu-id="a1f3a-108">تتعقب طريقة عرض **تعقب الجهد** تقدم المهام في الجدولة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="a1f3a-109">وتقوم بمقارنة ساعات المجهود الفعلي في تنفيذ مهمة بساعات الجهد المخططة للمهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-109">It compares the actual effort hours spent on a task to the task's planned effort hours.</span></span> <span data-ttu-id="a1f3a-110">يستخدم Project Service Automation الصيغ التالية لحساب مقاييس التتبع:</span><span class="sxs-lookup"><span data-stu-id="a1f3a-110">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="a1f3a-111">بشكل مبدئي عند إنشاء المهمة: سيتم تعيين التكلفة المخططة إلى التكلفة المقدرة عند الاكتمال.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-111">Initially on the task creation: Planned cost will be set to the Estimated cost at complete.</span></span> <span data-ttu-id="a1f3a-112">بعد تسجيل القيم الفعلية على المهمة، سيتم حساب ما يلي في طريقه عرض التعقب الخاصة بالجهد</span><span class="sxs-lookup"><span data-stu-id="a1f3a-112">Once Actuals are recorded on the task, the following will be calculation on the Tracking view for Effort</span></span>

- <span data-ttu-id="a1f3a-113">النسبة المئوية للتقدم = الجهد الفعلي المبذول حتى تاريخه ÷ التقدير عند الاكتمال (EAC)</span><span class="sxs-lookup"><span data-stu-id="a1f3a-113">Progress percentage = Actual effort spent to date ÷ Estimate at complete (EAC)</span></span> 
- <span data-ttu-id="a1f3a-114">التقدير للإكمال (ETC) = التقدير عند الاكتمال (EAC) - الجهد الفعلي المبذول حتى تاريخه</span><span class="sxs-lookup"><span data-stu-id="a1f3a-114">Estimate to complete (ETC) = Estimate at complete (EAC)  – Actual effort spent to date</span></span> 
- <span data-ttu-id="a1f3a-115">التقدير عند الاكتمال (EAC) = الجهد المتبقي + الجهد الفعلي المبذول حتى تاريخه</span><span class="sxs-lookup"><span data-stu-id="a1f3a-115">EAC = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="a1f3a-116">تباين الجهد المتوقع = الجهد المخطط - التقدير عند الاكتمال</span><span class="sxs-lookup"><span data-stu-id="a1f3a-116">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="a1f3a-117">يُظهر Project Service Automation تقديرًا لتباين الجهد في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-117">Project Service Automation shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="a1f3a-118">إذا كان التقدير عند الاكتمال أكثر من الجهد المخطط له ، فمن المتوقع أن تستغرق المهمة وقتًا أكثر مما كان مخططًا له في الأصل.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-118">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="a1f3a-119">ولذلك، فإنه متأخر في الجدولة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-119">Therefore, it's behind schedule.</span></span> <span data-ttu-id="a1f3a-120">إذا كان التقدير عند الاكتمال أقل من الجهد المخطط له ، فمن المتوقع أن تستغرق المهمة وقتًا أقل مما كان مخططًا له في الأصل.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-120">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="a1f3a-121">ولذلك، فإنه متقدم في الجدولة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-121">Therefore, it's ahead of schedule.</span></span>

## <a name="reprojecting-effort"></a><span data-ttu-id="a1f3a-122">إعادة تخطيط الجهود</span><span class="sxs-lookup"><span data-stu-id="a1f3a-122">Reprojecting effort</span></span>

<span data-ttu-id="a1f3a-123">من الشائع أن يقوم مدير المشروع بمراجعة التقديرات الأصلية للمهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-123">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="a1f3a-124">عمليات إعادة تخطيط المشروع هي تصور مدير المشروع للتقديرات ، بالنظر إلى الوضع الحالي للمشروع.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-124">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="a1f3a-125">ومع ذلك ، لا نوصي بأن يقوم مديرو المشاريع بتغيير أرقام خط الأساس ، لأن خط الأساس للمشروع يمثل مصدر الحقيقة المحدد لجدول المشروع وتقدير التكلفة ، وقد وافق جميع أصحاب المصلحة في المشروع على ذلك.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-125">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="a1f3a-126">هناك طريقتان يمكن لمدير المشروع من خلالهما إعادة تخطيط الجهود في المهام:</span><span class="sxs-lookup"><span data-stu-id="a1f3a-126">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="a1f3a-127">تجاوز التقدير للإكمال (ETC) الافتراضي مع تقدير جديد للجهد الفعلي المتبقي في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-127">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="a1f3a-128">تجاوز النسبة المئوية للتقدم الافتراضي مع تقدير جديد للتقدم الحقيقي في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-128">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="a1f3a-129">يؤدي كل من هاتين الطريقتين إلى إعادة حساب التقدير للإكمال للمهمة والتقدير عند الاكتمال ونسبة التقدم وتباين الجهد المتوقع في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-129">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="a1f3a-130">يتم أيضًا إعادة حساب التقدير عند الاكتمال والتقدير للإكمال والنسبة المئوية للتقدم في مهام الملخص، وتنتج إسقاطًا جديدًا لتباين الجهد.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-130">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="reprojection-of-effort-on-summary-tasks"></a><span data-ttu-id="a1f3a-131">إعادة تخطيط الجهد في مهام الملخص</span><span class="sxs-lookup"><span data-stu-id="a1f3a-131">Reprojection of effort on summary tasks</span></span>

<span data-ttu-id="a1f3a-132">يمكن إعادة تخطيط الجهد في مهام الملخص أو مهام الحاوية.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-132">Effort on summary tasks or container tasks can be reprojected.</span></span> <span data-ttu-id="a1f3a-133">بغض النظر عما إذا كان المستخدم يعيد تخطيط المشاريع باستخدام الجهد المتبقي أو النسبة المئوية للتقدم في مهام الملخص، تبدأ مجموعة الحسابات التالية:</span><span class="sxs-lookup"><span data-stu-id="a1f3a-133">Regardless of whether the user reprojects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="a1f3a-134">التقدير عند الاكتمال، والتقدير للإكمال، ويتم حساب النسبة المئوية للتقدم في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-134">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="a1f3a-135">يتم توزيع التقدير عند الاكتمال الجديد إلى المهام التابعة بنفس النسبة التي كان عليها التقدير عند الاكتمال الأصلي في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-135">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="a1f3a-136">يتم حساب التقدير عند الاكتمال الجديد في المهام الفردية وصولاً إلى مهام العقدة الطرفية.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-136">The new EAC on each of the individual tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="a1f3a-137">تحتوي المهام الفرعية المتأثرة وصولاً إلى العقد الورقية على التقدير للإكمال وتتم إعادة حساب النسبة المئوية للتقدم بناءً على قيمة التقدير عند الاكتمال.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-137">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="a1f3a-138">ينتج عن هذا عرض جديد لتباين الجهد للمهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-138">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="a1f3a-139">تتم إعادة حساب عمليات التقدير عند الاكتمال للمهام التلخيصية طوال الطريق إلى عقدة الجذر.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-139">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="a1f3a-140">طريقة عرض تعقب التكلفة</span><span class="sxs-lookup"><span data-stu-id="a1f3a-140">Cost tracking view</span></span> 

<span data-ttu-id="a1f3a-141">تقارن طريقة عرض **تعقب التكلفة** التكلفة الفعلية التي تم قضاؤها في مهمة ما بالتكلفة المخططة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-141">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost.</span></span> 

> [!NOTE]
> <span data-ttu-id="a1f3a-142">تعرض طريقة العرض هذه تكاليف العمالة فقط ولا تشمل التكاليف من تقديرات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-142">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="a1f3a-143">يستخدم Project Service Automation الصيغ التالية لحساب مقاييس التتبع:</span><span class="sxs-lookup"><span data-stu-id="a1f3a-143">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="a1f3a-144">عند إنشاء مهمة، تكون التكلفة المخططة مستوية للتكلفة المقدرة عند الاكتمال.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-144">When a task is created, the planned cost is equal to the estimated cost at complete.</span></span> <span data-ttu-id="a1f3a-145">بعد تسجيل القيم الفعلية على المهمة، سيتم حساب ما يلي في طريقه عرض **التعقب** الخاصة بالتكلفة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-145">After actuals are recorded on the task, the following is calculated on the **Tracking** view for cost:</span></span>

 - <span data-ttu-id="a1f3a-146">النسبة المئوية للتكلفة المستهلكة = التكلفة الفعلية المنفقة حتى تاريخه ÷ التكلفة المقدرة عند الاكتمال للمهمة</span><span class="sxs-lookup"><span data-stu-id="a1f3a-146">Percentage of cost consumed = Actual cost spent to date ÷ Estimated cost at complete for the task</span></span>
 - <span data-ttu-id="a1f3a-147">تكلفة الإكمال (CTC) = التكلفة المقدرة عند الاكتمال - التكلفة الفعلية التي تم إنفاقها حتى تاريخه</span><span class="sxs-lookup"><span data-stu-id="a1f3a-147">Cost to complete (CTC) = Estimated cost at complete – Actual cost spent to date</span></span>
 - <span data-ttu-id="a1f3a-148">التكلفة المقدرة عند الاكتمال = تكلفة الإكمال (CTC) + التكلفة الفعلية التي تم إنفاقها حتى تاريخه</span><span class="sxs-lookup"><span data-stu-id="a1f3a-148">Estimated cost at complete = CTC + Actual cost spent to date</span></span>
 - <span data-ttu-id="a1f3a-149">تباين التكلفة المقدرة = التكلفة المخططة - التكلفة المقدرة عند الاكتمال</span><span class="sxs-lookup"><span data-stu-id="a1f3a-149">Projected cost variance = Planned cost – Estimated cost at complete</span></span>

<span data-ttu-id="a1f3a-150">يتم إظهار عرض لتباين التكلفة في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-150">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="a1f3a-151">إذا كانت التكلفة المقدرة عند الاكتمال أكبر من التكلفة المخططة، فمن المتوقع أن تكلف المهمة مبلغًا أكبر مما كان مخططًا له في الأصل.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-151">If the estimated cost at complete is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="a1f3a-152">وبالتالي، فإن الاتجاه أكبر من الموازنة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-152">Therefore, it's trending over budget.</span></span> <span data-ttu-id="a1f3a-153">إذا كانت التكلفة المقدرة عند الاكتمال أقل من التكلفة المخططة، فمن المتوقع أن تكلف المهمة مبلغًا أقل مما كان مخططًا له في الأصل، والاتجاه أقل من الموازنة.‬</span><span class="sxs-lookup"><span data-stu-id="a1f3a-153">If the Estimated cost at complete is less than the planned cost, the task is projected to cost less than was originally planned and is trending under budget.</span></span>

## <a name="project-managers-reprojection-of-cost"></a><span data-ttu-id="a1f3a-154">إعادة تخطيط التكلفة من قِبل مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="a1f3a-154">Project manager’s reprojection of cost</span></span>

<span data-ttu-id="a1f3a-155">عند إعادة تقدير الجهد، يتم حساب تكلفة الإكمال (CTC) والتكلفة المقدرة عند الاكتمال والنسبة المئوية للتكلفة المستهلكة وتباين التكلفة المقدرة في طريقة عرض **تعقب التكاليف**.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-155">When effort is reprojected, the CTC, Estimated cost at complete, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="a1f3a-156">ملخص حالة المشروع</span><span class="sxs-lookup"><span data-stu-id="a1f3a-156">Project status summary</span></span>

<span data-ttu-id="a1f3a-157">يُظهر تعقب البيانات في طريقتي عرض **تعقب الجهد** و **تعقب التكلفة** مستى التقدم واستهلاك التكلفة في مستويات العقدة الجذر للمشروع ومهام الملخص والعقدة الطرفية.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-157">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="a1f3a-158">يعرض قسم **الحالة** في صفحة **كيان المشروع** ملخصًا لحالة المشروع.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-158">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="a1f3a-159">حقول ملخص الحالة</span><span class="sxs-lookup"><span data-stu-id="a1f3a-159">Status summary fields</span></span>

<span data-ttu-id="a1f3a-160">يعتبر حقل **حالة المشروع الإجمالية** حقلا قابلا للتحرير يوضح الحالة الإجمالية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-160">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="a1f3a-161">وهو يستخدم ترميز اللون، مثل الأخضر، والأصفر، والأحمر، للإشارة إلى زيادة المخاطرة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-161">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="a1f3a-162">يتيح حقل **التعليقات** لمدير المشروع إدخال تعليقات معينة حول الحالة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-162">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="a1f3a-163">حقل **تم تحديث الحالة في‬** غير قابل للتحرير والقيمة عبارة عن طابع زمني يشير إلى الوقت الأخير الذي تم فيه تحديث الحالة.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-163">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="a1f3a-164">يتم تعيين حقلب **أداء الجدولة** و **أداء التكلفة** من تاريخ التعقب.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-164">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="a1f3a-165">عندما يكون الجدول وتباين التكلفة للعقدة الجذر في طريقة عرض **تعقب الجهد** إيجابيين، يمكنك تعيين هذه الحقول إلى **متقدم**.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-165">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="a1f3a-166">عندما يكون الجدول وتباين التكلفة للعقدة الجذر سالبين، يمكنك تعيينهما إلى **متأخر**.</span><span class="sxs-lookup"><span data-stu-id="a1f3a-166">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]