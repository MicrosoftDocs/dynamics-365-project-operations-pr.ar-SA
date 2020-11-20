---
title: اعتبارات ترقية هيكل تنظيم العمل
description: يقدم هذا الموضوع معلومات حول ترقية هيكل تنظيم العمل من الإصدار 2.x حتى الإصدار 3.x من Project Service Automation.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: 0b75fd372732f42a3557aaa5eccec1f24a644941
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121787"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="17d4c-103">اعتبارات ترقية هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="17d4c-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="17d4c-104">يقدم هذا الموضوع معلومات حول ترقية هيكل تنظيم العمل من الإصدار 2.x حتى الإصدار 3.x من Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="17d4c-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="17d4c-105">يحدد هذا الموضوع الحالة السليمة لمشروع في Project Service Automation (PSA) المطلوب للترقية الناجحة.</span><span class="sxs-lookup"><span data-stu-id="17d4c-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="17d4c-106">كما توجد أيضا معلومات حول حالات الحظر الشائعة التي ستؤدي إلى فشل الترقية.</span><span class="sxs-lookup"><span data-stu-id="17d4c-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="17d4c-107">للحصول على مزيد من المعلومات حول تعريف مهام المشروع ووظائفها في جدول مشروع، راجع[جداول المشروع](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="17d4c-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="17d4c-108">الكيانات الرئيسية</span><span class="sxs-lookup"><span data-stu-id="17d4c-108">Key entities</span></span>
<span data-ttu-id="17d4c-109">بالنسبة لهيكل تنظيم عمل دقيق تم تحميله بالفعل بالموارد، تكون الكيانات التالية مطلوبة:</span><span class="sxs-lookup"><span data-stu-id="17d4c-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="17d4c-110">المشروع</span><span class="sxs-lookup"><span data-stu-id="17d4c-110">Project</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [<span data-ttu-id="17d4c-111">فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="17d4c-111">Project Team</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [<span data-ttu-id="17d4c-112">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="17d4c-112">Project Task</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [<span data-ttu-id="17d4c-113">تعيينات الموارد</span><span class="sxs-lookup"><span data-stu-id="17d4c-113">Resource Assignments</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [<span data-ttu-id="17d4c-114">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="17d4c-114">Project Task Dependency</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [<span data-ttu-id="17d4c-115">الموارد القابلة للحجز</span><span class="sxs-lookup"><span data-stu-id="17d4c-115">Bookable Resources</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

<span data-ttu-id="17d4c-116">لتحديد هيكل تنظيم عمل تم تحميله لمورد، يجب إكمال الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="17d4c-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="17d4c-117">إنشاء مشروع جديد.</span><span class="sxs-lookup"><span data-stu-id="17d4c-117">Create a new project.</span></span> <span data-ttu-id="17d4c-118">لمزيد من المعلومات حول كيفية إنشاء مشروع جديد، راجع [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span><span class="sxs-lookup"><span data-stu-id="17d4c-118">For more information about how to create a new project, see [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span></span>
2. <span data-ttu-id="17d4c-119">إنشاء مهمة واحده أو أكثر.</span><span class="sxs-lookup"><span data-stu-id="17d4c-119">Create one or more tasks.</span></span> <span data-ttu-id="17d4c-120">لمزيد من المعلومات حول كيفية إنشاء مهمة، راجع [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span><span class="sxs-lookup"><span data-stu-id="17d4c-120">For more information about how to create a task, see [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span></span>
3. <span data-ttu-id="17d4c-121">تحديد تبعيات المهام.</span><span class="sxs-lookup"><span data-stu-id="17d4c-121">Define the task dependencies.</span></span> <span data-ttu-id="17d4c-122">لمزيد من المعلومات، راجع [تبعية مهمة المشروع](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span><span class="sxs-lookup"><span data-stu-id="17d4c-122">For more information, see [Project Task Dependency](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span></span>
4. <span data-ttu-id="17d4c-123">تعيين أعضاء فريق المشروع للمشروع.</span><span class="sxs-lookup"><span data-stu-id="17d4c-123">Assign project team members to the project.</span></span> <span data-ttu-id="17d4c-124">لمزيد من المعلومات، راجع [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span><span class="sxs-lookup"><span data-stu-id="17d4c-124">For more information, see [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span></span>
5. <span data-ttu-id="17d4c-125">تعيين أعضاء فريق المشروع للمهام.</span><span class="sxs-lookup"><span data-stu-id="17d4c-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="17d4c-126">لمزيد من المعلومات، راجع [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span><span class="sxs-lookup"><span data-stu-id="17d4c-126">For more information, see [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="17d4c-127">علاقات فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="17d4c-127">Project team relationships</span></span>

<span data-ttu-id="17d4c-128">لضمان إجراء ترقية ناجحة، يجب الاحتفاظ بالعلاقات التالية بشكل صحيح:</span><span class="sxs-lookup"><span data-stu-id="17d4c-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="17d4c-129">يجب أن يكون كافة أعضاء فريق المشروع مقترنين بمورد قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="17d4c-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="17d4c-130">يجب أن يكون كافة أعضاء فريق المشروع مقترنين بنفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="17d4c-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="17d4c-131">علاقات مهام المشروع</span><span class="sxs-lookup"><span data-stu-id="17d4c-131">Project task relationships</span></span>
<span data-ttu-id="17d4c-132">لضمان إجراء ترقية ناجحة، يجب الاحتفاظ بالعلاقات التالية بشكل صحيح:</span><span class="sxs-lookup"><span data-stu-id="17d4c-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="17d4c-133">يجب أن تكون أي مهام مرتبطة مقترنة بنفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="17d4c-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="17d4c-134">يجب أن يكون لكل مهمة بند مهمة أصل.</span><span class="sxs-lookup"><span data-stu-id="17d4c-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="17d4c-135">يجب أن يكون لكل مهمة مشروع أصل.</span><span class="sxs-lookup"><span data-stu-id="17d4c-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="17d4c-136">الشروط الصالحة</span><span class="sxs-lookup"><span data-stu-id="17d4c-136">Valid conditions</span></span>

- <span data-ttu-id="17d4c-137">يجب أن تكون كافة مدد المهام أكبر من أو تساوي (> =) ساعة واحدة وأقل من 1,800,000 دقيقة (1,250 يوم).\*</span><span class="sxs-lookup"><span data-stu-id="17d4c-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="17d4c-138">يجب أن يكون لكافة المهام تاريخ بدء قبل 2000/01/01.\*</span><span class="sxs-lookup"><span data-stu-id="17d4c-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="17d4c-139">يجب أن تحتوي كافة المهام على تاريخ بدء ليس بعد 17 سنة من اليوم الحالي.\*</span><span class="sxs-lookup"><span data-stu-id="17d4c-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="17d4c-140">يجب أن يكون لكافة المهام تاريخ بدء قبل أو يساوي تاريخ الانتهاء.</span><span class="sxs-lookup"><span data-stu-id="17d4c-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="17d4c-141">يجب أن تحتوي كافة أنواع الحركات الموجودة في التصنيفات (المصروفات، والمواد، والضريبة، والوقت) على قيم لـ **الوحدة الافتراضية** و **مجموعة الوحدات**.</span><span class="sxs-lookup"><span data-stu-id="17d4c-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="17d4c-142">ينبغي تجنب تنسيقات التاريخ مع الأحرف.</span><span class="sxs-lookup"><span data-stu-id="17d4c-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="17d4c-143">خطوات تخفيف المخاطر المحتملة</span><span class="sxs-lookup"><span data-stu-id="17d4c-143">Potential mitigation steps</span></span>
- <span data-ttu-id="17d4c-144">استخدم البحث المتقدم لتحديد مهام المشروع التي لا تتضمن معرف مشروع.</span><span class="sxs-lookup"><span data-stu-id="17d4c-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="17d4c-145">استخدم البحث المتقدم لتحديد مهام المشروع حيث المدة المجدولة أكبر من > 1,800,000.</span><span class="sxs-lookup"><span data-stu-id="17d4c-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="17d4c-146">قبل إجراء أي تغييرات على البيانات، يجب عليك التحقق من أي تخصيصات مرتبطة بالكيان والتي من المحتمل أن تكون قد أدت إلى وجود البيانات في حالة سيئة.</span><span class="sxs-lookup"><span data-stu-id="17d4c-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="17d4c-147">يجب معالجة هذه التخصيصات قبل متابعة أي تحديثات ذات صلة بالبيانات.</span><span class="sxs-lookup"><span data-stu-id="17d4c-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="17d4c-148">بالنسبة إلى المحددة التي تم عزلها، ضع في اعتبارك حذف هذه المهام إذا لم تكن مطلوبة أو إذا كان يجب ربطها بالمشروع الأصلي الصحيح.</span><span class="sxs-lookup"><span data-stu-id="17d4c-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="17d4c-149">بالنسبة إلى مهام تتجاوز مدتها 1,250، عليك أن تأخذ في الاعتبار إضافة مهام متعددة لتمثيل المدة الإجمالية، إذا كان ذلك ممكنًا.</span><span class="sxs-lookup"><span data-stu-id="17d4c-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="17d4c-150">العناصر المميزة بعلامة نجمية (\*) لها حدود لأن إدارة علاقات العملاء (CRM) تدعم 7,320 عملية فقط من عمليات توسيع التكرار.</span><span class="sxs-lookup"><span data-stu-id="17d4c-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="17d4c-151">يجب أن تبقى دون هذا الحد.</span><span class="sxs-lookup"><span data-stu-id="17d4c-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="17d4c-152">علاقات تعيينات الموارد</span><span class="sxs-lookup"><span data-stu-id="17d4c-152">Resource Assignment relationships</span></span>
<span data-ttu-id="17d4c-153">لضمان إجراء ترقية ناجحة، يجب الاحتفاظ بالعلاقات التالية بشكل صحيح:</span><span class="sxs-lookup"><span data-stu-id="17d4c-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="17d4c-154">يجب أن تكون كافة تعيينات الموارد الموجودة في هيكل تنظيم العمل مرتبطة بنفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="17d4c-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="17d4c-155">يجب أن تكون كافة تعيينات الموارد الموجودة في هيكل تنظيم العمل مرتبطة بأعضاء فريق المشروع في نفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="17d4c-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="17d4c-156">خطوات تخفيف المخاطر المحتملة</span><span class="sxs-lookup"><span data-stu-id="17d4c-156">Potential mitigation steps</span></span>
- <span data-ttu-id="17d4c-157">حدد كافة المهام التي تقع خارج الشروط الموضحة أعلاه.</span><span class="sxs-lookup"><span data-stu-id="17d4c-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="17d4c-158">ينبغي حذف تعيينات الموارد التي لم تعد صالحة.</span><span class="sxs-lookup"><span data-stu-id="17d4c-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="17d4c-159">علاقات تبعيات مهام المشاريع</span><span class="sxs-lookup"><span data-stu-id="17d4c-159">Project task dependency relationships</span></span>
<span data-ttu-id="17d4c-160">لضمان إجراء ترقية ناجحة، يجب الاحتفاظ بالعلاقات التالية بشكل صحيح:</span><span class="sxs-lookup"><span data-stu-id="17d4c-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="17d4c-161">يجب أن تكون كافة تبعيات مهام المشروع مرتبطة بنفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="17d4c-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="17d4c-162">لا يمكن أن يكون لمهمة نفس التبعية مشار إليها أكثر من مرة.</span><span class="sxs-lookup"><span data-stu-id="17d4c-162">A task can't have the same dependency referenced more than once.</span></span>
