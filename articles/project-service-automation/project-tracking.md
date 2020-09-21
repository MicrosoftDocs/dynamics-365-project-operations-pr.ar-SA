---
title: تقدم المشروع واستهلاك التكلفة‬
description: يقدم هذا الموضوع معلومات حول كيفية تعقب تقدم المشروع واستهلاك التكلفة.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748713"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="a8bf9-103">تقدم المشروع واستهلاك التكلفة‬</span><span class="sxs-lookup"><span data-stu-id="a8bf9-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a8bf9-104">تختلف الحاجة إلى تعقب التقدم مقابل جدول حسب الصناعة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="a8bf9-105">تتبع بعض الصناعات مستوى حبيبيًا ، بينما تتبع صناعات أخرى مستوى أعلى.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="a8bf9-106">يوضح هذا الموضوع كيفية الجدولة من أجل تلبية متطلبات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="a8bf9-107">طريقة عرض تعقب الجهود</span><span class="sxs-lookup"><span data-stu-id="a8bf9-107">Effort tracking view</span></span>

<span data-ttu-id="a8bf9-108">تتعقب طريقة عرض **تعقب الجهد** تقدم المهام في الجدولة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="a8bf9-109">فهو يقارن ساعات الجهد الفعلي التي تم إنفاقها في مهمة ما مع ساعات الجهد المخططة لتلك المهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-109">It compares the actual effort hours that have been spent on a task to the planned effort hours for that task.</span></span> <span data-ttu-id="a8bf9-110">يستخدم PSA الصيغ التالية لحساب مقاييس التتبع:</span><span class="sxs-lookup"><span data-stu-id="a8bf9-110">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="a8bf9-111">نسبة التقدم = الجهد الفعلي المبذول حتى تاريخه ÷ الجهد المخطط للمهمة</span><span class="sxs-lookup"><span data-stu-id="a8bf9-111">Progress percentage = Actual effort spent to date ÷ Planned effort for the task</span></span> 
- <span data-ttu-id="a8bf9-112">التقدير للإكمال (ETC) = الجهد المخطط - الجهد الفعلي المبذول حتى تاريخه</span><span class="sxs-lookup"><span data-stu-id="a8bf9-112">Estimate to complete (ETC) = Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="a8bf9-113">التقدير عند الاكتمال (EAC) = الجهد المتبقي + الجهد الفعلي المبذول حتى تاريخه</span><span class="sxs-lookup"><span data-stu-id="a8bf9-113">Estimate at complete (EAC) = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="a8bf9-114">تباين الجهد المتوقع = الجهد المخطط - التقدير عند الاكتمال</span><span class="sxs-lookup"><span data-stu-id="a8bf9-114">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="a8bf9-115">يُظهر PSA إسقاطًا لفرق الجهد في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-115">PSA shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="a8bf9-116">إذا كان التقدير عند الاكتمال أكثر من الجهد المخطط له ، فمن المتوقع أن تستغرق المهمة وقتًا أكثر مما كان مخططًا له في الأصل.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="a8bf9-117">ولذلك، فإنه متأخر في الجدولة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-117">Therefore, it's behind schedule.</span></span> <span data-ttu-id="a8bf9-118">إذا كان التقدير عند الاكتمال أقل من الجهد المخطط له ، فمن المتوقع أن تستغرق المهمة وقتًا أقل مما كان مخططًا له في الأصل.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-118">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="a8bf9-119">ولذلك، فإنه متقدم في الجدولة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-119">Therefore, it's ahead of schedule.</span></span>

## <a name="re-projecting-effort"></a><span data-ttu-id="a8bf9-120">جهد إعادة التخطيط</span><span class="sxs-lookup"><span data-stu-id="a8bf9-120">Re-projecting effort</span></span>

<span data-ttu-id="a8bf9-121">من الشائع أن يقوم مدير المشروع بمراجعة التقديرات الأصلية للمهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-121">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="a8bf9-122">عمليات إعادة تخطيط المشروع هي تصور مدير المشروع للتقديرات ، بالنظر إلى الوضع الحالي للمشروع.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-122">Project re-projections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="a8bf9-123">ومع ذلك ، لا نوصي بأن يقوم مديرو المشاريع بتغيير أرقام خط الأساس ، لأن خط الأساس للمشروع يمثل مصدر الحقيقة المحدد لجدول المشروع وتقدير التكلفة ، وقد وافق جميع أصحاب المصلحة في المشروع على ذلك.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-123">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="a8bf9-124">هناك طريقتان يمكن لمدير المشروع من خلالهما إعادة تخطيط الجهود في المهام:</span><span class="sxs-lookup"><span data-stu-id="a8bf9-124">There are two ways that a project manager can re-project effort on tasks:</span></span>

- <span data-ttu-id="a8bf9-125">تجاوز التقدير للإكمال (ETC) الافتراضي مع تقدير جديد للجهد الفعلي المتبقي في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-125">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="a8bf9-126">تجاوز النسبة المئوية للتقدم الافتراضي مع تقدير جديد للتقدم الحقيقي في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-126">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="a8bf9-127">يؤدي كل من هاتين الطريقتين إلى إعادة حساب التقدير للإكمال للمهمة والتقدير عند الاكتمال ونسبة التقدم وتباين الجهد المتوقع في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-127">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="a8bf9-128">يتم أيضًا إعادة حساب التقدير عند الاكتمال والتقدير للإكمال والنسبة المئوية للتقدم في مهام الملخص، وتنتج إسقاطًا جديدًا لتباين الجهد.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-128">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="re-projection-of-effort-on-summary-tasks"></a><span data-ttu-id="a8bf9-129">إعادة تخطيط الجهد في مهام الملخص</span><span class="sxs-lookup"><span data-stu-id="a8bf9-129">Re-projection of effort on summary tasks</span></span>

<span data-ttu-id="a8bf9-130">يمكن إعادة تخطيط الجهد في مهام الملخص أو مهام الحاوية.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-130">Effort on summary tasks or container tasks can be re-projected.</span></span> <span data-ttu-id="a8bf9-131">بغض النظر عما إذا كان المستخدم يعيد تخطيط المشاريع باستخدام الجهد المتبقي أو النسبة المئوية للتقدم في مهام الملخص، تبدأ مجموعة الحسابات التالية:</span><span class="sxs-lookup"><span data-stu-id="a8bf9-131">Regardless of whether the user re-projects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="a8bf9-132">التقدير عند الاكتمال، والتقدير للإكمال، ويتم حساب النسبة المئوية للتقدم في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-132">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="a8bf9-133">يتم توزيع التقدير عند الاكتمال الجديد إلى المهام التابعة بنفس النسبة التي كان عليها التقدير عند الاكتمال الأصلي في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-133">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="a8bf9-134">يتم حساب التقدير عند الاكتمال الجديد في المهام الفردية وصولاً إلى مهام العقدة الطرفية.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-134">The new EAC on each of the individualt tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="a8bf9-135">تحتوي المهام الفرعية المتأثرة وصولاً إلى العقد الورقية على التقدير للإكمال وتتم إعادة حساب النسبة المئوية للتقدم بناءً على قيمة التقدير عند الاكتمال.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-135">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="a8bf9-136">ينتج عن هذا عرض جديد لتباين الجهد للمهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-136">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="a8bf9-137">تتم إعادة حساب عمليات التقدير عند الاكتمال للمهام التلخيصية طوال الطريق إلى عقدة الجذر.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-137">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="a8bf9-138">طريقة عرض تعقب التكلفة</span><span class="sxs-lookup"><span data-stu-id="a8bf9-138">Cost tracking view</span></span> 

<span data-ttu-id="a8bf9-139">تقارن طريقة عرض **تعقب التكلفة** التكلفة الفعلية التي تم قضاؤها في مهمة ما بالتكلفة المخطط لها في مهمة ما.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-139">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="a8bf9-140">تعرض طريقة العرض هذه تكاليف العمالة فقط ولا تشمل التكاليف من تقديرات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-140">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="a8bf9-141">يستخدم PSA الصيغ التالية لحساب مقاييس التتبع:</span><span class="sxs-lookup"><span data-stu-id="a8bf9-141">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="a8bf9-142">النسبة المئوية للتكلفة المستهلكة = التكلفة الفعلية المنفقة حتى تاريخه ÷ التكلفة المخططة للمهمة</span><span class="sxs-lookup"><span data-stu-id="a8bf9-142">Percentage of cost consumed = Actual cost spent to date ÷ Planned cost for the task</span></span>
- <span data-ttu-id="a8bf9-143">تكلفة الإكمال (CTC) = التكلفة المخططة - التكلفة الفعلية المنفقة تاريخه</span><span class="sxs-lookup"><span data-stu-id="a8bf9-143">Cost to complete (CTC) = Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="a8bf9-144">التقدير عند الاكتمال = تكلفة الإكمال + التكلفة الفعلية المنفقة حتى تاريخه</span><span class="sxs-lookup"><span data-stu-id="a8bf9-144">EAC = CTC + Actual cost spent to date</span></span>
- <span data-ttu-id="a8bf9-145">تباين التكلفة التقديرية = التكلفة المخططة - التقدير عند الاكتمال</span><span class="sxs-lookup"><span data-stu-id="a8bf9-145">Projected cost variance = Planned cost – EAC</span></span>

<span data-ttu-id="a8bf9-146">يتم إظهار عرض لتباين التكلفة في المهمة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-146">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="a8bf9-147">إذا كان التقدير عند الاكتمال أكبر من التكلفة المخطط لها، فمن المتوقع أن تكلف المهمة مبلغًا أكبر مما كان مخططًا له في الأصل.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-147">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="a8bf9-148">وبالتالي، فإن الاتجاه أكبر من الموازنة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-148">Therefore, it's trending over budget.</span></span> <span data-ttu-id="a8bf9-149">إذا كان التقدير عند الاكتمال أقل من التكلفة المخطط لها، فمن المتوقع أن تكلف المهمة مبلغًا أقل مما كان مخططًا له في الأصل.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-149">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="a8bf9-150">وبالتالي، فإن الاتجاه أقل من الموازنة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-150">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-re-projection-of-cost"></a><span data-ttu-id="a8bf9-151">إعادة تخطيط التكلفة من قِبل مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="a8bf9-151">Project manager’s re-projection of cost</span></span>

<span data-ttu-id="a8bf9-152">وعندما تتم إعادة تخطيط الجهد، يتم حساب تكلفة الإكمال والتقدير عند الاكتمال والنسبة المئوية للتكلفة المستهلكة وتباين التكلفة المعروض في طريقة عرض **تعقب التكاليف**.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-152">When effort is re-projected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="a8bf9-153">ملخص حالة المشروع</span><span class="sxs-lookup"><span data-stu-id="a8bf9-153">Project status summary</span></span>

<span data-ttu-id="a8bf9-154">يُظهر تعقب البيانات في طريقتي عرض **تعقب الجهد** و**تعقب التكلفة** مستى التقدم واستهلاك التكلفة في مستويات العقدة الجذر للمشروع ومهام الملخص والعقدة الطرفية.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-154">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="a8bf9-155">يعرض قسم **الحالة** في صفحة **كيان المشروع** ملخصًا لحالة المشروع.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-155">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="a8bf9-156">حقول ملخص الحالة</span><span class="sxs-lookup"><span data-stu-id="a8bf9-156">Status summary fields</span></span>

<span data-ttu-id="a8bf9-157">يعتبر حقل **حالة المشروع الإجمالية** حقلا قابلا للتحرير يوضح الحالة الإجمالية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-157">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="a8bf9-158">وهو يستخدم ترميز اللون، مثل الأخضر، والأصفر، والأحمر، للإشارة إلى زيادة المخاطرة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-158">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="a8bf9-159">يتيح حقل **التعليقات** لمدير المشروع إدخال تعليقات معينة حول الحالة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-159">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="a8bf9-160">حقل **تم تحديث الحالة في‬** غير قابل للتحرير والقيمة عبارة عن طابع زمني يشير إلى الوقت الأخير الذي تم فيه تحديث الحالة.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-160">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="a8bf9-161">يتم تعيين حقلب **أداء الجدولة** و**أداء التكلفة** من تاريخ التعقب.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-161">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="a8bf9-162">عندما يكون الجدول وتباين التكلفة للعقدة الجذر في طريقة عرض **تعقب الجهد** إيجابيين، يمكنك تعيين هذه الحقول إلى **متقدم**.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-162">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="a8bf9-163">عندما يكون الجدول وتباين التكلفة للعقدة الجذر سالبين، يمكنك تعيينهما إلى **متأخر**.</span><span class="sxs-lookup"><span data-stu-id="a8bf9-163">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
