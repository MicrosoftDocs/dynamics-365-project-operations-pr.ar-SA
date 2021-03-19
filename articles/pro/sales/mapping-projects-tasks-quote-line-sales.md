---
title: تعيين المشاريع والمهام لبند عرض أسعار قائمة على المشروع
description: يقدم هذا الموضوع معلومات حول كيفية تعيين المشاريع والمهام إلى بند مهمة يعتمد على المشروع.
author: rumant
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d714304f408050babae1a6ba74268979e0b6ea4b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272732"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a><span data-ttu-id="3a691-103">تعيين المشاريع والمهام لبند عرض أسعار قائمة على المشروع</span><span class="sxs-lookup"><span data-stu-id="3a691-103">Map projects and tasks to a project-based quote line</span></span>

<span data-ttu-id="3a691-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="3a691-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3a691-105">في بنود عرض الأسعار المستندة إلى المشروع، يمكنك تعيين المهام محددة لأحد المشروعات والمقترنة بالفعل ببند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3a691-105">On project-based quote lines, you can map the specific tasks of a project that is already associated to a quote line.</span></span>

<span data-ttu-id="3a691-106">عند القيام بتعيين المهام إلى بند عرض الأسعار، يتم تطبيق العناصر التالية التي قمت بتعريفها في بند عرض الأسعار على هذه المهام فقط:</span><span class="sxs-lookup"><span data-stu-id="3a691-106">When you map tasks to a quote line, the following items you defined on the quote line will only apply to those tasks:</span></span>

- <span data-ttu-id="3a691-107">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="3a691-107">Billing method</span></span>
- <span data-ttu-id="3a691-108">خيارات الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="3a691-108">Chargeability options</span></span>
- <span data-ttu-id="3a691-109">حدود يجب عدم تجاوزها</span><span class="sxs-lookup"><span data-stu-id="3a691-109">Not-to-exceed limits</span></span>
- <span data-ttu-id="3a691-110">العملاء</span><span class="sxs-lookup"><span data-stu-id="3a691-110">Customers</span></span>

<span data-ttu-id="3a691-111">على سبيل المثال، قد يكون لديك مشروع توجد فيه مرحلة واحدة بسعر ثابت بينما كافة المراحل الأخرى مقدرة حسب الوقت والمواد.</span><span class="sxs-lookup"><span data-stu-id="3a691-111">For example, you might have a project where one phase is fixed price and all the other phases are time and materials.</span></span> <span data-ttu-id="3a691-112">في هذه الحالة، يمكنك إقران المرحلة الأولى، وكافة المهام التابعة لها، ببند عرض الأسعار الخاص بهذه المرحلة باستخدام أسلوب فوترة بسعر ثابت.</span><span class="sxs-lookup"><span data-stu-id="3a691-112">In this case, you can associate the first phase, and all of its child tasks, to the quote line for that phase with a fixed price billing method.</span></span> <span data-ttu-id="3a691-113">يمكنك بعد ذلك إقران كافة المراحل الأخرى ببند عرض الأسعار المستند إلى المواد والوقت.</span><span class="sxs-lookup"><span data-stu-id="3a691-113">You can then associate all the other phases to the time and materials-based quote line.</span></span>

## <a name="associate-tasks-to-project-based-quote-lines"></a><span data-ttu-id="3a691-114">إقران المهام ببنود عرض أسعار مستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="3a691-114">Associate tasks to project-based quote lines</span></span>

<span data-ttu-id="3a691-115">يمكنك إقران المهام ببنود عرض الأسعار من المواقع التالية:</span><span class="sxs-lookup"><span data-stu-id="3a691-115">You can associate tasks with quote lines from the following locations:</span></span>

- <span data-ttu-id="3a691-116">صفحة **المشروع** > علامة تبويب **فوترة المهمة** (المثلي)</span><span class="sxs-lookup"><span data-stu-id="3a691-116">**Project** page > **Task billing** tab (optimal)</span></span>
- <span data-ttu-id="3a691-117">صفحة **بند عرض الأسعار** > علامة تبويب **المهام الخاضعة للرسوم**</span><span class="sxs-lookup"><span data-stu-id="3a691-117">**Quote Line** page > **Chargeable tasks** tab</span></span> 

### <a name="from-the-project-page"></a><span data-ttu-id="3a691-118">من صفحة المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-118">From the Project page</span></span>

<span data-ttu-id="3a691-119">توفر صفحة **المشروع** تجربة مثلي لإقران المهام ببنود عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3a691-119">The **Project** page provides the optimal experience for associating tasks to quote lines.</span></span> <span data-ttu-id="3a691-120">يمكنك استخدام هذه الصفحة لتحديد مهام متعددة وإقرانها جميعًا، بالإضافة إلى المهام التابعة لها، ببند عرض الأسعار المحدد.</span><span class="sxs-lookup"><span data-stu-id="3a691-120">You can use this page to select multiple tasks and associate all of them, plus their child tasks, to the selected quote line.</span></span>

1. <span data-ttu-id="3a691-121">في علامة التبويب **عام** لبند عرض الأسعار المستند إلى المشروع، تحقق من ملء حقل **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="3a691-121">On the **General** tab of a project–based quote line, verify the **Project** field is filled out.</span></span>
2. <span data-ttu-id="3a691-122">في حقل **المهام المضمنة**، قم بتحديد **المهام المحددة فقط**.</span><span class="sxs-lookup"><span data-stu-id="3a691-122">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="3a691-123">احفظ بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-123">Save the project-based quote line.</span></span> <span data-ttu-id="3a691-124">عند تحديث النموذج، يتم عرض علامة تبويب **المهام الخاضعة للرسوم**.</span><span class="sxs-lookup"><span data-stu-id="3a691-124">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="3a691-125">في علامة التبويب **عام**، حدد ارتباط المشروع من حقل **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="3a691-125">On the **General** tab, select the link for the project from the **Project** field.</span></span>
5. <span data-ttu-id="3a691-126">في صفحة **المشروع**، حدد علامة التبويب **فوترة المهمة**.</span><span class="sxs-lookup"><span data-stu-id="3a691-126">On the **Project** page, select the **Task billing** tab.</span></span>
6. <span data-ttu-id="3a691-127">في الشبكة الثانية، والتي تنطبق على إعداد الفوترة الخاص بالمهمة، حدد مهمة واحدة أو أكثر ثم حدد **إقران بنود عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="3a691-127">In the second grid, which applies to task-specific billing setup, select one or more tasks and then select **Associate quote lines**.</span></span>
7. <span data-ttu-id="3a691-128">في صفحة مربع الحوار التي تظهر، حدد بند عرض الأسعار الذي يعرض بنود عروض الأسعار المستندة إلى المشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3a691-128">In the dialog page that appears, select a quote line that displays project-based quote lines on the quote.</span></span>
8. <span data-ttu-id="3a691-129">في حقل **نوع الفاتورة**، حدد ما إذا كانت هذه المهام خاضعة للرسوم أم غير خاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="3a691-129">In the **Billing type** field, indicate if these tasks are chargeable or non-chargeable.</span></span>
9. <span data-ttu-id="3a691-130">حدد خانة الاختيار للإشارة إلى ما إذا كان ينبغي أن يتضمن الاقتران مهام فرعية للمهام المحددة.</span><span class="sxs-lookup"><span data-stu-id="3a691-130">Select the check box to indicate if the association should include child tasks of the selected tasks.</span></span> <span data-ttu-id="3a691-131">سيؤدي تحديد خانة الاختيار إلى إقران المهام التابعة للمهام المحددة ببند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3a691-131">Checking the box will associate the child tasks of the selected tasks to the quote line.</span></span>
10. <span data-ttu-id="3a691-132">حدد **موافق** لغلق مربع الحوار.</span><span class="sxs-lookup"><span data-stu-id="3a691-132">Select **OK** to close the dialog.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="3a691-133">من صفحة بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="3a691-133">From the Quote line page</span></span>

<span data-ttu-id="3a691-134">يمكنك إقران مهام المشروع ببنود عرض الأسعار من علامة التبويب **المهام الخاضعة للرسوم** في صفحة **بند عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="3a691-134">You can associate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

>[!NOTE]
><span data-ttu-id="3a691-135">يوجد أفضل مكان لإقران مهام المشروع مع بنود عرض الأسعار في علامة التبويب **فوترة المهمة** في صفحة **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="3a691-135">The optimal place to associate project tasks to quote lines is on the **Task billing** tab on the **Project** page.</span></span> <span data-ttu-id="3a691-136">إذا قمت بإقران مهام من علامة التبويب **المهام الخاضعة للرسوم** في صفحة **بند عرض الأسعار**، يجب عليك إقران كل مشروع يدويًا.</span><span class="sxs-lookup"><span data-stu-id="3a691-136">If you associate tasks from the **Chargeable tasks** tab on **Quote line** page, you must manually associate each project.</span></span>

1. <span data-ttu-id="3a691-137">في علامة التبويب **عام** لبند عرض الأسعار المستند إلى المشروع، تحقق من وجود مشروع محدد في حقل **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="3a691-137">On the **General** tab of a project–based quote line, verify that there is a project selected in the **Project** field.</span></span>
2. <span data-ttu-id="3a691-138">في حقل **المهام المضمنة**، قم بتحديد **المهام المحددة فقط**.</span><span class="sxs-lookup"><span data-stu-id="3a691-138">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="3a691-139">احفظ بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-139">Save the project-based quote line.</span></span> <span data-ttu-id="3a691-140">عند تحديث النموذج، يتم عرض علامة تبويب **المهام الخاضعة للرسوم**.</span><span class="sxs-lookup"><span data-stu-id="3a691-140">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="3a691-141">في علامة التبويب **مهام خاضعة للرسوم**، حدد **إضافة مهمة بند عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="3a691-141">On the **Chargeable tasks** tab, select **Add a quote line task**.</span></span>
5. <span data-ttu-id="3a691-142">في صفحة **مهمة بند عرض الأسعار**، في حقل **المهام**، حدد المهمة وفي حقل **نوع الفاتورة**، حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="3a691-142">On the **Quote line task** page, in the **Tasks** field, select the task and in the **Billing type** field, select **Save**.</span></span> 
6. <span data-ttu-id="3a691-143">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="3a691-143">Close the page.</span></span> <span data-ttu-id="3a691-144">المهمة المحددة مقترنة الآن ببند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3a691-144">The selected task is now associated to the quote line.</span></span>

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a><span data-ttu-id="3a691-145">إلغاء إقران المهام ببنود عرض أسعار مستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="3a691-145">Disassociate tasks from project–based quote lines</span></span>

### <a name="from-the-project-page"></a><span data-ttu-id="3a691-146">من صفحة المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-146">From the Project page</span></span>

<span data-ttu-id="3a691-147">توفر هذه الطريق التجربة المثلي لإلغاء إقران المهام ببنود عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3a691-147">This method provides the most optimal experience for disassociating tasks from quote lines.</span></span> <span data-ttu-id="3a691-148">يمكنك تحديد مهام متعددة وإلغاء إقرانها جميعًا، بالإضافة إلى المهام التابعة لها، من بند عرض الأسعار المحدد.</span><span class="sxs-lookup"><span data-stu-id="3a691-148">You can select multiple tasks and disassociate all of the them, plus their child tasks, from the selected quote line.</span></span>

1. <span data-ttu-id="3a691-149">في علامة التبويب **عام** لبند عرض الأسعار المستند إلى المشروع، في حقل **المشروع** حدد ارتباط المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-149">On the **General** tab of a project–based quote line, in the **Project** field, select the project link.</span></span>
2. <span data-ttu-id="3a691-150">في صفحة **المشروع**، حدد علامة التبويب **فوترة المهمة**.</span><span class="sxs-lookup"><span data-stu-id="3a691-150">On the **Project** page, select the **Task billing** tab.</span></span>
3. <span data-ttu-id="3a691-151">في الشبكة الثانية، والتي تنطبق على إعداد الفوترة الخاص بالمهمة، حدد مهمة واحدة أو أكثر، ثم حدد **إلغاء إقران بنود عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="3a691-151">In the second grid, which applies to task-specific billing setup, select one or more tasks, and then select **Disassociate quote lines**.</span></span>
4. <span data-ttu-id="3a691-152">في صفحه مربع الحوار التي تظهر، حدد بند عرض أسعار.</span><span class="sxs-lookup"><span data-stu-id="3a691-152">In the dialog page that appears, select a quote line.</span></span>
5. <span data-ttu-id="3a691-153">حدد خانة الاختيار للإشارة إلى ما إذا كان ينبغي أيضًا إزالة الاقتران من المهام الفرعية للمهام المحددة.</span><span class="sxs-lookup"><span data-stu-id="3a691-153">Select the check box to indicate whether the association should also be removed from child tasks of the selected tasks.</span></span> <span data-ttu-id="3a691-154">سيؤدي تحديد خانة الاختيار أيضًا إلى إلغاء إقران المهام التابعة للمهام المحددة ببند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3a691-154">Checking the box will also disassociate the child tasks of the selected tasks to the quote line.</span></span>
6. <span data-ttu-id="3a691-155">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="3a691-155">Select **OK**.</span></span> <span data-ttu-id="3a691-156">تخبرك رسالة تحذير بأنك إذا قمت بإزالة هذا الاقتران، فقد يتم عكس أية قيم فعلية سابقه تم تسجيلها مسبقا في المهمة.</span><span class="sxs-lookup"><span data-stu-id="3a691-156">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
7. <span data-ttu-id="3a691-157">حدد **موافق** للمتابعة وإزالة الاقتران بين المهمة وبند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-157">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="3a691-158">من صفحة بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="3a691-158">From the Quote line page</span></span>

<span data-ttu-id="3a691-159">يمكنك أيضًا إلغاء إقران مهام المشروع ببنود عرض الأسعار من علامة التبويب **المهام الخاضعة للرسوم** في صفحة **بند عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="3a691-159">You can also disassociate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

1. <span data-ttu-id="3a691-160">في علامة التبويب **مهام خاضعة للرسوم**، حدد **حذف مهمة بند عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="3a691-160">On the **Chargeable tasks** tab, select **Delete a quote line task**.</span></span>
2. <span data-ttu-id="3a691-161">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="3a691-161">Select **OK**.</span></span> <span data-ttu-id="3a691-162">تخبرك رسالة تحذير بأنك إذا قمت بإزالة هذا الاقتران، فقد يتم عكس أية قيم فعلية سابقه تم تسجيلها مسبقا في المهمة.</span><span class="sxs-lookup"><span data-stu-id="3a691-162">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
3. <span data-ttu-id="3a691-163">حدد **موافق** للمتابعة وإزالة الاقتران بين المهمة وبند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-163">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

>[!NOTE]
> <span data-ttu-id="3a691-164">لا يؤدي هذا الإجراء إلى حذف المهمة من المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-164">This procedure doesn't delete the task from the project.</span></span> <span data-ttu-id="3a691-165">فهو يؤدي فقط إلى إزالة اقتران المهمة من بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="3a691-165">It only removes the task association from the project-based quote line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]