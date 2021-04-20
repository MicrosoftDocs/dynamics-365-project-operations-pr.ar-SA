---
title: استخدام واجهات برمجة تطبيقات الجدولة لتنفيذ عمليات مع كيانات الجدولة
description: يوفر هذا الموضوع معلومات و عينات لاستخدام واجهات برمجة تطبيقات الجدولة.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868113"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="165f0-103">استخدام واجهات برمجة تطبيقات الجدولة لتنفيذ عمليات مع كيانات الجدولة</span><span class="sxs-lookup"><span data-stu-id="165f0-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="165f0-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="165f0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="165f0-105">تتوفر بعض الوظائف المذكورة في هذا الموضوع أو كلها كجزء من إصدار أولي.</span><span class="sxs-lookup"><span data-stu-id="165f0-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="165f0-106">إن المحتوى والوظائف خاضعة للتغيير.</span><span class="sxs-lookup"><span data-stu-id="165f0-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="165f0-107">كيانات الجدولة</span><span class="sxs-lookup"><span data-stu-id="165f0-107">Scheduling entities</span></span>

<span data-ttu-id="165f0-108">توفر واجهات برمجة تطبيقات جدولة القدرة على تنفيذ عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="165f0-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="165f0-109">تُدار هذه الكيانات من خلال محرك جدولة في المشروع للويب.</span><span class="sxs-lookup"><span data-stu-id="165f0-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="165f0-110">كانت عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة** مقيدة في إصدارات Dynamics 365 Project Operations السابقة.</span><span class="sxs-lookup"><span data-stu-id="165f0-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="165f0-111">يوفر الجدول التالي قائمة كاملة تتضمن **كيانات الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="165f0-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="165f0-112">اسم الكيان</span><span class="sxs-lookup"><span data-stu-id="165f0-112">Entity name</span></span>  | <span data-ttu-id="165f0-113">اسم منطقي للكيان</span><span class="sxs-lookup"><span data-stu-id="165f0-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="165f0-114">Project</span><span class="sxs-lookup"><span data-stu-id="165f0-114">Project</span></span> | <span data-ttu-id="165f0-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="165f0-115">msdyn_project</span></span> |
| <span data-ttu-id="165f0-116">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="165f0-116">Project Task</span></span>  | <span data-ttu-id="165f0-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="165f0-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="165f0-118">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="165f0-118">Project Task Dependency</span></span>  | <span data-ttu-id="165f0-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="165f0-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="165f0-120">تعيين المورد</span><span class="sxs-lookup"><span data-stu-id="165f0-120">Resource Assignment</span></span> | <span data-ttu-id="165f0-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="165f0-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="165f0-122">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="165f0-122">Project Bucket</span></span>  | <span data-ttu-id="165f0-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="165f0-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="165f0-124">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="165f0-124">Project Team Member</span></span> | <span data-ttu-id="165f0-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="165f0-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="165f0-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="165f0-126">OperationSet</span></span>

<span data-ttu-id="165f0-127">إن OperationSet عبارة نمط وحدة عمل يمكن استخدامه عندما يكون من الضروري معالجة طلبات متعددة تؤثر على الجدولة ضمن حركة.</span><span class="sxs-lookup"><span data-stu-id="165f0-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="165f0-128">واجهات برمجة تطبيقات الجدولة</span><span class="sxs-lookup"><span data-stu-id="165f0-128">Schedule APIs</span></span>

<span data-ttu-id="165f0-129">فيما يلي قائمة بواجهات برمجة تطبيقات الجدولة الحالية.</span><span class="sxs-lookup"><span data-stu-id="165f0-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="165f0-130">**msdyn_CreateProjectV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء مشروع.</span><span class="sxs-lookup"><span data-stu-id="165f0-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="165f0-131">يتم إنشاء مستودع المشروع والمشروع الافتراضي في الحال.</span><span class="sxs-lookup"><span data-stu-id="165f0-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="165f0-132">**msdyn_CreateTeamMemberV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء عضو فريق مشروع.</span><span class="sxs-lookup"><span data-stu-id="165f0-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="165f0-133">يتم إنشاء سجل عضو الفريق على الفور.</span><span class="sxs-lookup"><span data-stu-id="165f0-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="165f0-134">**msdyn_CreateOperationSetV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لجدولة طلبات متعددة يجب تنفيذها ضمن حركة.</span><span class="sxs-lookup"><span data-stu-id="165f0-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="165f0-135">**msdyn_PSSCreateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء كيان.</span><span class="sxs-lookup"><span data-stu-id="165f0-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="165f0-136">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية الإنشاء.</span><span class="sxs-lookup"><span data-stu-id="165f0-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="165f0-137">**msdyn_PSSUpdateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لتحديث كيان.</span><span class="sxs-lookup"><span data-stu-id="165f0-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="165f0-138">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية التحديث.</span><span class="sxs-lookup"><span data-stu-id="165f0-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="165f0-139">**msdyn_PSSDeleteV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لحذف كيان.</span><span class="sxs-lookup"><span data-stu-id="165f0-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="165f0-140">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية الحذف.</span><span class="sxs-lookup"><span data-stu-id="165f0-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="165f0-141">**msdyn_ExecuteOperationSetV1**: يتم استخدام واجهة برمجة التطبيقات هذه لتنفيذ جميع العمليات ضمن مجموعة عمليات معينة.</span><span class="sxs-lookup"><span data-stu-id="165f0-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="165f0-142">استخدام واجهات برمجة تطبيقات لجدولة مع OperationSet</span><span class="sxs-lookup"><span data-stu-id="165f0-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="165f0-143">نظرًا لاستخدام السجلات مع كل من **CreateProjectV1** و **CreateTeamMemberV1** على الفور، لا يمكن استخدام واجهات برمجة التطبيقات هذه في **OperationSet** بشكل مباشر.</span><span class="sxs-lookup"><span data-stu-id="165f0-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="165f0-144">ومع ذلك، يمكنك استخدام واجهة برمجة التطبيقات لإنشاء السجلات المطلوبة، وإنشاء  **OperationSet**، ثم استخدام هذه السجلات المنشأة مسبقًا في **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="165f0-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="165f0-145">العمليات المدعومة</span><span class="sxs-lookup"><span data-stu-id="165f0-145">Supported operations</span></span>

| <span data-ttu-id="165f0-146">كيان الجدولة</span><span class="sxs-lookup"><span data-stu-id="165f0-146">Scheduling entity</span></span> | <span data-ttu-id="165f0-147">‏إنشاء</span><span class="sxs-lookup"><span data-stu-id="165f0-147">Create</span></span> | <span data-ttu-id="165f0-148">تحديث</span><span class="sxs-lookup"><span data-stu-id="165f0-148">Update</span></span> | <span data-ttu-id="165f0-149">حذف </span><span class="sxs-lookup"><span data-stu-id="165f0-149">Delete</span></span> | <span data-ttu-id="165f0-150">اعتبارات هامة</span><span class="sxs-lookup"><span data-stu-id="165f0-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="165f0-151">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="165f0-151">Project task</span></span> | <span data-ttu-id="165f0-152">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-152">Yes</span></span> | <span data-ttu-id="165f0-153">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-153">Yes</span></span> | <span data-ttu-id="165f0-154">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-154">Yes</span></span> | <span data-ttu-id="165f0-155">‏‫بلا</span><span class="sxs-lookup"><span data-stu-id="165f0-155">None</span></span> |
| <span data-ttu-id="165f0-156">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="165f0-156">Project task dependency</span></span> | <span data-ttu-id="165f0-157">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-157">Yes</span></span> | <span data-ttu-id="165f0-158">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-158">Yes</span></span> | | <span data-ttu-id="165f0-159">لا يتم تحديث سجلات تبعية مهمة المشروع.</span><span class="sxs-lookup"><span data-stu-id="165f0-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="165f0-160">بدلاً من ذلك، يمكن حذف سجل قديم ويمكن إنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="165f0-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="165f0-161">تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="165f0-161">Resource assignment</span></span> | <span data-ttu-id="165f0-162">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-162">Yes</span></span> | <span data-ttu-id="165f0-163">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-163">Yes</span></span> | | <span data-ttu-id="165f0-164">العمليات مع الحقول التالية غير مدعومة: **BookableResourceID** و **Effort** و **EffortCompleted** و **EffortRemaining** ة **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="165f0-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="165f0-165">لا يتم تحديث سجلات تعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="165f0-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="165f0-166">بدلاً من ذلك، يمكن حذف السجل القديم ويمكن إنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="165f0-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="165f0-167">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="165f0-167">Project bucket</span></span> | <span data-ttu-id="165f0-168">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="165f0-168">N/A</span></span> | <span data-ttu-id="165f0-169">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="165f0-169">N/A</span></span> | <span data-ttu-id="165f0-170">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="165f0-170">N/A</span></span> | <span data-ttu-id="165f0-171">يتم إنشاء المستودع الافتراضي باستخدام واجهة برمجة التطبيقات **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="165f0-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="165f0-172">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="165f0-172">Project team member</span></span> | <span data-ttu-id="165f0-173">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-173">Yes</span></span> | <span data-ttu-id="165f0-174">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-174">Yes</span></span> | <span data-ttu-id="165f0-175">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-175">Yes</span></span> | <span data-ttu-id="165f0-176">بالنسبة لعملية الإنشاء، استخدم واجهة برمجة التطبيقات **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="165f0-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="165f0-177">Project</span><span class="sxs-lookup"><span data-stu-id="165f0-177">Project</span></span> | <span data-ttu-id="165f0-178">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-178">Yes</span></span> | <span data-ttu-id="165f0-179">نعم </span><span class="sxs-lookup"><span data-stu-id="165f0-179">Yes</span></span> | <span data-ttu-id="165f0-180">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="165f0-180">N/A</span></span> | <span data-ttu-id="165f0-181">العمليات مع الحقول التالية غير مدعومة: **StateCode** و **BulkGenerationStatus** و **GlobalRevisionToken** و **CalendarID** و **Effort** و **EffortCompleted** و **EffortRemaining** و **Progress** و **Finish** و **TaskEarliestStart** و **Duration**.</span><span class="sxs-lookup"><span data-stu-id="165f0-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="165f0-182">يمكن استدعاء واجهات برمجة التطبيقات مع كائنات الكيانات التي تتضمن حقولاً مخصصة.</span><span class="sxs-lookup"><span data-stu-id="165f0-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="165f0-183">خاصية المعرف اختيارية.</span><span class="sxs-lookup"><span data-stu-id="165f0-183">The ID property is optional.</span></span> <span data-ttu-id="165f0-184">إذا تم توفيرها، يحاول النظام استخدامها ويلقي استثناءً إذا لم يكن من الممكن استخدامها.</span><span class="sxs-lookup"><span data-stu-id="165f0-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="165f0-185">إذا لم يتم توفيرها، سيقوم النظام بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="165f0-185">If it isn't provided, the system will generate it.</span></span>

## <a name="limitations-and-known-issues"></a><span data-ttu-id="165f0-186">القيود والمشاكل المعروفة</span><span class="sxs-lookup"><span data-stu-id="165f0-186">Limitations and known issues</span></span>
<span data-ttu-id="165f0-187">فيما يلي قائمة بالقيود والمشاكل المعروفة:</span><span class="sxs-lookup"><span data-stu-id="165f0-187">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="165f0-188">يمكن استخدام واجهات برمجة تطبيقات الجدولة فقط بواسطة **المستخدمين الذين لديهم ترخيص Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="165f0-188">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="165f0-189">لا يمكن استخدامها بواسطة:</span><span class="sxs-lookup"><span data-stu-id="165f0-189">They can't be used by:</span></span>
    - <span data-ttu-id="165f0-190">مستخدمي التطبيق</span><span class="sxs-lookup"><span data-stu-id="165f0-190">Application users</span></span>
    - <span data-ttu-id="165f0-191">مستخدمي النظام</span><span class="sxs-lookup"><span data-stu-id="165f0-191">System users</span></span>
    - <span data-ttu-id="165f0-192">مستخدمي التكامل</span><span class="sxs-lookup"><span data-stu-id="165f0-192">Integration users</span></span>
    - <span data-ttu-id="165f0-193">المستخدمين الآخرين الذين ليس لديهم الترخيص المطلوب</span><span class="sxs-lookup"><span data-stu-id="165f0-193">Other users that don't have the required license</span></span>
- <span data-ttu-id="165f0-194">تتضمن كل **OperationSet** مئة عملية كحدٍ أقصى.</span><span class="sxs-lookup"><span data-stu-id="165f0-194">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="165f0-195">بإمكان كل مستخدم أن يحصل على عشر **OperationSet** مفتوحة كحدٍ أقصى.</span><span class="sxs-lookup"><span data-stu-id="165f0-195">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="165f0-196">يدعم Project Operations في الوقت الحالي 500 مهمة إجمالية كحد أقصى على مشروع.</span><span class="sxs-lookup"><span data-stu-id="165f0-196">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="165f0-197">في الوقت الحالي، لا تتوفر حالة فشل **OperationSet** وسجلات الفشل.</span><span class="sxs-lookup"><span data-stu-id="165f0-197">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="165f0-198">واجهات برمجة تطبيقات الجدولة هي حاليًا في وضع الإصدار الأولي للاستخدام العام.</span><span class="sxs-lookup"><span data-stu-id="165f0-198">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="165f0-199">لا تدعم Microsoft استخدام واجهات برمجة التطبيقات هذه في بيئة الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="165f0-199">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="165f0-200">سيناريو نموذجي</span><span class="sxs-lookup"><span data-stu-id="165f0-200">Sample scenario</span></span>

<span data-ttu-id="165f0-201">في هذا السيناريو، ستقوم بإنشاء مشروع، وعضو فريق، وأربع مهام، وعمليتي تعيين للموارد.</span><span class="sxs-lookup"><span data-stu-id="165f0-201">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="165f0-202">بعد ذلك، عليك تحديث مهمة واحدة وتحديث المشروع وحذف مهمة واحدة وحذف تعيين مورد واحد وإنشاء تبعية مهمة.</span><span class="sxs-lookup"><span data-stu-id="165f0-202">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```C#
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="165f0-203">عينات إضافية</span><span class="sxs-lookup"><span data-stu-id="165f0-203">Additional samples</span></span>

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };
    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
    return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";
    return project;
}

private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
        task["new_amount"] = 591.34m;
        task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }
    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;
    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);
    return taskDependency;
}

#endregion

#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
