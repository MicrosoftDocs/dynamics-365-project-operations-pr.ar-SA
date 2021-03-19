---
title: تغييرات إدارة الموارد (Project Service Automation 3.x)
description: يوفر هذا الموضوع معلومات حول التغييرات التي تتم على منطقة إدارة الموارد.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 5f88d7309a5e1171629a72e749bfc01abb64c62a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284747"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="0382c-103">تغييرات إدارة الموارد (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="0382c-103">Resource management changes (Project Service Automation 3.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

<span data-ttu-id="0382c-104">توفر أقسام هذه الموضوع معلومات حول التغييرات التي تم إجراؤها على منطقة إدارة الموارد في الإصدار 3.x من Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="0382c-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="0382c-105">تقديرات المشروع</span><span class="sxs-lookup"><span data-stu-id="0382c-105">Project estimates</span></span>

<span data-ttu-id="0382c-106">وبدلاً من كون تقديرات المشروع مستندة إلى كيان **msdyn\_projecttask** (**Project Task**)، تستند تقديرات المشروع إلى كيان **msdyn\_resourceassignment** (**تعيين المورد**).</span><span class="sxs-lookup"><span data-stu-id="0382c-106">Instead of being based on the **msdyn\_projecttask** entity (**Project Task**), project estimates are based on the **msdyn\_resourceassignment** entity (**Resource Assignment**).</span></span> <span data-ttu-id="0382c-107">أصبحت تعيينات الموارد "مصدر الحقيقة" لجدولة المهام وأسعارها.</span><span class="sxs-lookup"><span data-stu-id="0382c-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="0382c-108">مهام البنود</span><span class="sxs-lookup"><span data-stu-id="0382c-108">Line tasks</span></span>

<span data-ttu-id="0382c-109">في PSA 3. x، مهام البنود قديمة (مهملة).</span><span class="sxs-lookup"><span data-stu-id="0382c-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="0382c-110">تشير التعيينات الآن إلى المهمة بالكامل بدلاً من مهام البنود.</span><span class="sxs-lookup"><span data-stu-id="0382c-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="0382c-111">يوضح المثال التالي كيفية تعيين مهمة تُسمى "مهمة الاختبار" لأعضاء الفريق A وB في الإصدارين السابقين من PSA وفي الإصدار 3.x من PSA.</span><span class="sxs-lookup"><span data-stu-id="0382c-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="0382c-112">**قبل PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="0382c-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="0382c-113">مهمة الاختبار</span><span class="sxs-lookup"><span data-stu-id="0382c-113">Test task</span></span>

        - <span data-ttu-id="0382c-114">مهمة الاختبار - مهمة البند 1</span><span class="sxs-lookup"><span data-stu-id="0382c-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="0382c-115">التعيين إلى A</span><span class="sxs-lookup"><span data-stu-id="0382c-115">Assignment to A</span></span>

        - <span data-ttu-id="0382c-116">مهمة الاختبار - مهمة البند 2</span><span class="sxs-lookup"><span data-stu-id="0382c-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="0382c-117">التعيين إلى B</span><span class="sxs-lookup"><span data-stu-id="0382c-117">Assignment to B</span></span>

- <span data-ttu-id="0382c-118">**PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="0382c-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="0382c-119">مهمة الاختبار</span><span class="sxs-lookup"><span data-stu-id="0382c-119">Test task</span></span>

        - <span data-ttu-id="0382c-120">التعيين إلى A</span><span class="sxs-lookup"><span data-stu-id="0382c-120">Assignment to A</span></span>
        - <span data-ttu-id="0382c-121">التعيين إلى B</span><span class="sxs-lookup"><span data-stu-id="0382c-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="0382c-122">التعيين غير المعين</span><span class="sxs-lookup"><span data-stu-id="0382c-122">Unassigned assignment</span></span>

<span data-ttu-id="0382c-123">في PSA 3.x، التعيين غير المعين هو تعيين يتم تعيينه لعضو فريق **فارغ** ومورد **فارغ**.</span><span class="sxs-lookup"><span data-stu-id="0382c-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="0382c-124">يمكن أن تحدث التعيينات غير المعينة في سيناريوهين:</span><span class="sxs-lookup"><span data-stu-id="0382c-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="0382c-125">إذا تم إنشاء مهمة، ولكن لم يتم تعيينها بعد إلى أي عضو من أعضاء الفريق، يتم دومًا إنشاء تعيين غير معين.</span><span class="sxs-lookup"><span data-stu-id="0382c-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="0382c-126">إذا تمت إزالة كافة المعين لهم في إحدى المهام، ستتم إعادة إنشاء تعيين غير معين لهذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="0382c-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="0382c-127">جدولة الحقول في كيان مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="0382c-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="0382c-128">تم إهمال الحقول في كيان **msdyn\_projecttask** أو تم نقلها إلى كيان **msdyn\_resourceassignment** أو تتم الإشارة إليها الآن من كيان **msdyn\_projectteam** (**عضو فريق المشروع**).</span><span class="sxs-lookup"><span data-stu-id="0382c-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity (**Project Team Member**).</span></span>

| <span data-ttu-id="0382c-129">الحقل المهمل في \_projecttask (مهمة المشروع)</span><span class="sxs-lookup"><span data-stu-id="0382c-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="0382c-130">حقل جديد في msdyn\_resourceassignment (تعيين المورد)</span><span class="sxs-lookup"><span data-stu-id="0382c-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="0382c-131">تعليق</span><span class="sxs-lookup"><span data-stu-id="0382c-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="0382c-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="0382c-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="0382c-133">بلا</span><span class="sxs-lookup"><span data-stu-id="0382c-133">None</span></span> | |
| <span data-ttu-id="0382c-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="0382c-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="0382c-135">بلا</span><span class="sxs-lookup"><span data-stu-id="0382c-135">None</span></span> | |
| <span data-ttu-id="0382c-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="0382c-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="0382c-137">بلا</span><span class="sxs-lookup"><span data-stu-id="0382c-137">None</span></span> | |
| <span data-ttu-id="0382c-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="0382c-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="0382c-139">بلا</span><span class="sxs-lookup"><span data-stu-id="0382c-139">None</span></span> | |
| <span data-ttu-id="0382c-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="0382c-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="0382c-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="0382c-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="0382c-142">تم تغيير تنسيق بنية بيانات منهج كائن JavaScript ‏(JSON) المخزنة في الحقل.</span><span class="sxs-lookup"><span data-stu-id="0382c-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="0382c-143">مخطط الجدولة</span><span class="sxs-lookup"><span data-stu-id="0382c-143">Schedule contour</span></span>

<span data-ttu-id="0382c-144">يتم تخزين مخطط الجدولة في حقل **العمل المخطط** (**msdyn\_plannedwork**) في كلٍّ من كياني **تعيين المورد** (**msdyn\_resourceassignment**).</span><span class="sxs-lookup"><span data-stu-id="0382c-144">The schedule contour is stored in the **Planned Work** field (**msdyn\_plannedwork**) of each **Resource Assignment** entity (**msdyn\_resourceassignment**).</span></span>

### <a name="structure"></a><span data-ttu-id="0382c-145">هيكل</span><span class="sxs-lookup"><span data-stu-id="0382c-145">Structure</span></span>

<span data-ttu-id="0382c-146">تتكون البنية الجديدة لمخطط الجدولة من شرائح زمنية مرنة يتم تعريفها لكل يوم من الجدولة.</span><span class="sxs-lookup"><span data-stu-id="0382c-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="0382c-147">تحتوي كل شريحة زمنية على الخصائص التالية:</span><span class="sxs-lookup"><span data-stu-id="0382c-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="0382c-148">**البداية** – بدء ساعات العمل لليوم وفقًا لتقويم المشروع.</span><span class="sxs-lookup"><span data-stu-id="0382c-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="0382c-149">**النهاية** – انتهاء ساعات العمل لليوم وفقًا لتقويم المشروع.</span><span class="sxs-lookup"><span data-stu-id="0382c-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="0382c-150">**الساعات** -عدد الساعات التي تم تعيينها في اليوم.</span><span class="sxs-lookup"><span data-stu-id="0382c-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="0382c-151">**مثال**</span><span class="sxs-lookup"><span data-stu-id="0382c-151">**Example**</span></span>

<span data-ttu-id="0382c-152">يستخدم هذا المثال تقويم مشروع حيث يكون يوم العمل من 9 صباحًا إلى 5 مساءً في المنطقة الزمنية UTC-8.</span><span class="sxs-lookup"><span data-stu-id="0382c-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="0382c-153">الجدولة التلقائية والجدولة اليدوية</span><span class="sxs-lookup"><span data-stu-id="0382c-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="0382c-154">وإذا كانت المهمة مجدولة تلقائيًا، فسيتم تحميل الساعات في المقدمة وقد تنخفض مده المهمة.</span><span class="sxs-lookup"><span data-stu-id="0382c-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="0382c-155">**مثال**</span><span class="sxs-lookup"><span data-stu-id="0382c-155">**Example**</span></span>

<span data-ttu-id="0382c-156">تتم جدولة المهمة التالية تلقائيًا لمدة 18 ساعة خلال ثلاثه أيام (من 3 ديسمبر 2018 إلى 5 ديسمبر 2018).</span><span class="sxs-lookup"><span data-stu-id="0382c-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="0382c-157">وإذا كانت المهمة مجدولة يدويًا، يتم توزيع الساعات بالتساوي على كافة التواريخ.</span><span class="sxs-lookup"><span data-stu-id="0382c-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="0382c-158">**مثال**</span><span class="sxs-lookup"><span data-stu-id="0382c-158">**Example**</span></span>

<span data-ttu-id="0382c-159">تتم جدولة المهمة التالية يدويًا لمدة 18 ساعة خلال ثلاثه أيام (من 3 ديسمبر 2018 إلى 5 ديسمبر 2018).</span><span class="sxs-lookup"><span data-stu-id="0382c-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="0382c-160">وحدة التعيين</span><span class="sxs-lookup"><span data-stu-id="0382c-160">Assignment unit</span></span>

<span data-ttu-id="0382c-161">تم إهمال وحده التعيين في PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="0382c-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="0382c-162">أصبحت ساعات مجهود المهام مقسومة بشكل متساو في كل يوم، بين كافة الموارد المعينة.</span><span class="sxs-lookup"><span data-stu-id="0382c-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="0382c-163">**مثال**</span><span class="sxs-lookup"><span data-stu-id="0382c-163">**Example**</span></span>

<span data-ttu-id="0382c-164">في هذا المثال، يتم تعيين المهمة إلى موردين وتتم جدولتها تلقائيًا لمده 36 ساعة من ثلاثه أيام (من 3 ديسمبر 2018 إلى 5 ديسمبر 2018).</span><span class="sxs-lookup"><span data-stu-id="0382c-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="0382c-165">التعيين 1:</span><span class="sxs-lookup"><span data-stu-id="0382c-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="0382c-166">التعيين 2:</span><span class="sxs-lookup"><span data-stu-id="0382c-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="0382c-167">أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="0382c-167">Pricing dimensions</span></span>

<span data-ttu-id="0382c-168">في PSA 3.x، تمت إزالة حقول أبعاد التسعير الخاصة بالمورد (مثل **الدور** و **الوحدة التنظيمية**) من كيان **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="0382c-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit**) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="0382c-169">يمكن استرداد هذه الحقول الآن من عضو فريق المشروع المقابل (**msdyn\_projectteam**) في تعيين المورد (**msdyn\_resourceassignment**) عند إنشاء تقديرات المشروع.</span><span class="sxs-lookup"><span data-stu-id="0382c-169">These fields can now be retrieved from the corresponding project team member (**msdyn\_projectteam**) of the resource assignment (**msdyn\_resourceassignment**) when project estimates are generated.</span></span> <span data-ttu-id="0382c-170">تمت إضافة الحقل الجديد **msdyn\_organizationalunit** إلى كيان **msdyn\_projectteam**.</span><span class="sxs-lookup"><span data-stu-id="0382c-170">A new field, **msdyn\_organizationalunit**, has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="0382c-171">الحقل المهمل في \_projecttask (مهمة المشروع)</span><span class="sxs-lookup"><span data-stu-id="0382c-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="0382c-172">حقل من msdyn\_projectteam (عضو فريق المشروع) تم استخدامه بدلاً من ذلك</span><span class="sxs-lookup"><span data-stu-id="0382c-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="0382c-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="0382c-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="0382c-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="0382c-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="0382c-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="0382c-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="0382c-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="0382c-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="0382c-177">المخططات</span><span class="sxs-lookup"><span data-stu-id="0382c-177">Contours</span></span>

<span data-ttu-id="0382c-178">تم إهمال حقول مخططات التسعير والتقدير في كيان **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="0382c-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="0382c-179">وتم نقلها إلى كيان **msdyn\_resourceassignment**.</span><span class="sxs-lookup"><span data-stu-id="0382c-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="0382c-180">الحقل المهمل في \_projecttask (مهمة المشروع)</span><span class="sxs-lookup"><span data-stu-id="0382c-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="0382c-181">حقل جديد في msdyn\_resourceassignment (تعيين المورد)</span><span class="sxs-lookup"><span data-stu-id="0382c-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="0382c-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="0382c-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="0382c-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="0382c-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="0382c-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="0382c-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="0382c-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="0382c-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="0382c-186">تمت إضافة الحقول التالية إلى كيان **msdyn\_resourceassignment**:</span><span class="sxs-lookup"><span data-stu-id="0382c-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="0382c-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="0382c-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="0382c-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="0382c-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="0382c-189">لم يتم تغيير الحقول التالية للتكاليف والمبيعات الفعلية والمتبقية والمخطط لها في كيان **msdyn\_projecttask**:</span><span class="sxs-lookup"><span data-stu-id="0382c-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="0382c-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="0382c-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="0382c-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="0382c-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="0382c-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="0382c-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="0382c-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="0382c-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="0382c-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="0382c-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="0382c-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="0382c-195">msdyn\_remainingsales</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]