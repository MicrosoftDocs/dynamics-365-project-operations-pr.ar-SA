---
title: استخدام واجهات برمجة التطبيقات لجدولة المشروع لتنفيذ عمليات مع كيانات الجدولة
description: يوفر هذا الموضوع معلومات ونماذج لاستخدام واجهات برمجة التطبيقات لجدولة المشروع.
author: sigitac
ms.date: 06/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4915261c08a3271a919e04084e92a14b297c1b35
ms.sourcegitcommit: 2f16c2bc7c8350676a6a380c61fffa9958db6a0b
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/22/2021
ms.locfileid: "6293211"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="171f4-103">استخدام واجهات برمجة التطبيقات لجدولة المشروع لتنفيذ عمليات مع كيانات الجدولة</span><span class="sxs-lookup"><span data-stu-id="171f4-103">Use Project schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="171f4-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="171f4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="171f4-105">تتوفر بعض الوظائف المذكورة في هذا الموضوع أو كلها كجزء من إصدار أولي.</span><span class="sxs-lookup"><span data-stu-id="171f4-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="171f4-106">إن المحتوى والوظائف خاضعة للتغيير.</span><span class="sxs-lookup"><span data-stu-id="171f4-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="171f4-107">كيانات الجدولة</span><span class="sxs-lookup"><span data-stu-id="171f4-107">Scheduling entities</span></span>

<span data-ttu-id="171f4-108">توفر واجهات برمجة التطبيقات لجدولة المشروع القدرة على تنفيذ عمليات إنشاء وتحديث وحذف باستخدام **كيانات الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="171f4-108">Project schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="171f4-109">تُدار هذه الكيانات من خلال محرك جدولة في المشروع للويب.</span><span class="sxs-lookup"><span data-stu-id="171f4-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="171f4-110">كانت عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة** مقيدة في إصدارات Dynamics 365 Project Operations السابقة.</span><span class="sxs-lookup"><span data-stu-id="171f4-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="171f4-111">يوفر الجدول التالي قائمة كاملة بكيانات جدولة المشروع.</span><span class="sxs-lookup"><span data-stu-id="171f4-111">The following table provides a full list of the Project schedule entities.</span></span>

| <span data-ttu-id="171f4-112">اسم الكيان</span><span class="sxs-lookup"><span data-stu-id="171f4-112">Entity name</span></span>  | <span data-ttu-id="171f4-113">اسم منطقي للكيان</span><span class="sxs-lookup"><span data-stu-id="171f4-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="171f4-114">Project</span><span class="sxs-lookup"><span data-stu-id="171f4-114">Project</span></span> | <span data-ttu-id="171f4-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="171f4-115">msdyn_project</span></span> |
| <span data-ttu-id="171f4-116">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-116">Project Task</span></span>  | <span data-ttu-id="171f4-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="171f4-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="171f4-118">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-118">Project Task Dependency</span></span>  | <span data-ttu-id="171f4-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="171f4-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="171f4-120">تعيين المورد</span><span class="sxs-lookup"><span data-stu-id="171f4-120">Resource Assignment</span></span> | <span data-ttu-id="171f4-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="171f4-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="171f4-122">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-122">Project Bucket</span></span>  | <span data-ttu-id="171f4-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="171f4-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="171f4-124">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-124">Project Team Member</span></span> | <span data-ttu-id="171f4-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="171f4-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="171f4-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="171f4-126">OperationSet</span></span>

<span data-ttu-id="171f4-127">إن OperationSet عبارة نمط وحدة عمل يمكن استخدامه عندما يكون من الضروري معالجة طلبات متعددة تؤثر على الجدولة ضمن حركة.</span><span class="sxs-lookup"><span data-stu-id="171f4-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="project-schedule-apis"></a><span data-ttu-id="171f4-128">واجهات برمجة التطبيقات لجدولة المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-128">Project schedule APIs</span></span>

<span data-ttu-id="171f4-129">وفيما يلي قائمة بواجهات برمجة التطبيقات لجدولة المشروع.</span><span class="sxs-lookup"><span data-stu-id="171f4-129">The following is a list of current Project schedule APIs.</span></span>

- <span data-ttu-id="171f4-130">**msdyn_CreateProjectV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء مشروع.</span><span class="sxs-lookup"><span data-stu-id="171f4-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="171f4-131">يتم إنشاء مستودع المشروع والمشروع الافتراضي في الحال.</span><span class="sxs-lookup"><span data-stu-id="171f4-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="171f4-132">**msdyn_CreateTeamMemberV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء عضو فريق مشروع.</span><span class="sxs-lookup"><span data-stu-id="171f4-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="171f4-133">يتم إنشاء سجل عضو الفريق على الفور.</span><span class="sxs-lookup"><span data-stu-id="171f4-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="171f4-134">**msdyn_CreateOperationSetV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لجدولة طلبات متعددة يجب تنفيذها ضمن حركة.</span><span class="sxs-lookup"><span data-stu-id="171f4-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="171f4-135">**msdyn_PSSCreateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء كيان.</span><span class="sxs-lookup"><span data-stu-id="171f4-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="171f4-136">يمكن أن يكون الكيان أيًا من كيانات جدولة المشروع التي تدعم عملية الإنشاء.</span><span class="sxs-lookup"><span data-stu-id="171f4-136">The entity can be any of the Project scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="171f4-137">**msdyn_PSSUpdateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لتحديث كيان.</span><span class="sxs-lookup"><span data-stu-id="171f4-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="171f4-138">يمكن أن يكون الكيان أيًا من كيانات جدولة المشروع التي تدعم عملية التحديث.</span><span class="sxs-lookup"><span data-stu-id="171f4-138">The entity can be any of the Project scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="171f4-139">**msdyn_PSSDeleteV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لحذف كيان.</span><span class="sxs-lookup"><span data-stu-id="171f4-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="171f4-140">يمكن أن يكون الكيان أيًا من كيانات جدولة المشروع التي تدعم عملية الحذف.</span><span class="sxs-lookup"><span data-stu-id="171f4-140">The entity can be any of the Project scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="171f4-141">**msdyn_ExecuteOperationSetV1**: يتم استخدام واجهة برمجة التطبيقات هذه لتنفيذ جميع العمليات ضمن مجموعة عمليات معينة.</span><span class="sxs-lookup"><span data-stu-id="171f4-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-project-schedule-apis-with-operationset"></a><span data-ttu-id="171f4-142">استخدام واجهات برمجة التطبيقات لجدولة المشروع مع OperationSet</span><span class="sxs-lookup"><span data-stu-id="171f4-142">Using Project schedule APIs with OperationSet</span></span>

<span data-ttu-id="171f4-143">نظرًا لاستخدام السجلات مع كل من **CreateProjectV1** و **CreateTeamMemberV1** على الفور، لا يمكن استخدام واجهات برمجة التطبيقات هذه في **OperationSet** بشكل مباشر.</span><span class="sxs-lookup"><span data-stu-id="171f4-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="171f4-144">ومع ذلك، يمكنك استخدام واجهة برمجة التطبيقات لإنشاء السجلات المطلوبة، وإنشاء  **OperationSet**، ثم استخدام هذه السجلات المنشأة مسبقًا في **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="171f4-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="171f4-145">العمليات المدعومة</span><span class="sxs-lookup"><span data-stu-id="171f4-145">Supported operations</span></span>

| <span data-ttu-id="171f4-146">كيان الجدولة</span><span class="sxs-lookup"><span data-stu-id="171f4-146">Scheduling entity</span></span> | <span data-ttu-id="171f4-147">‏إنشاء</span><span class="sxs-lookup"><span data-stu-id="171f4-147">Create</span></span> | <span data-ttu-id="171f4-148">تحديث</span><span class="sxs-lookup"><span data-stu-id="171f4-148">Update</span></span> | <span data-ttu-id="171f4-149">حذف </span><span class="sxs-lookup"><span data-stu-id="171f4-149">Delete</span></span> | <span data-ttu-id="171f4-150">اعتبارات هامة</span><span class="sxs-lookup"><span data-stu-id="171f4-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="171f4-151">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-151">Project task</span></span> | <span data-ttu-id="171f4-152">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-152">Yes</span></span> | <span data-ttu-id="171f4-153">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-153">Yes</span></span> | <span data-ttu-id="171f4-154">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-154">Yes</span></span> | <span data-ttu-id="171f4-155">‏‫بلا</span><span class="sxs-lookup"><span data-stu-id="171f4-155">None</span></span> |
| <span data-ttu-id="171f4-156">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-156">Project task dependency</span></span> | <span data-ttu-id="171f4-157">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-157">Yes</span></span> | <span data-ttu-id="171f4-158">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-158">Yes</span></span> | | <span data-ttu-id="171f4-159">لا يتم تحديث سجلات تبعية مهمة المشروع.</span><span class="sxs-lookup"><span data-stu-id="171f4-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="171f4-160">بدلاً من ذلك، يمكن حذف سجل قديم ويمكن إنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="171f4-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="171f4-161">تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="171f4-161">Resource assignment</span></span> | <span data-ttu-id="171f4-162">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-162">Yes</span></span> | <span data-ttu-id="171f4-163">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-163">Yes</span></span> | | <span data-ttu-id="171f4-164">العمليات مع الحقول التالية غير مدعومة: **BookableResourceID** و **Effort** و **EffortCompleted** و **EffortRemaining** ة **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="171f4-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="171f4-165">لا يتم تحديث سجلات تعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="171f4-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="171f4-166">بدلاً من ذلك، يمكن حذف السجل القديم ويمكن إنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="171f4-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="171f4-167">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-167">Project bucket</span></span> | <span data-ttu-id="171f4-168">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="171f4-168">N/A</span></span> | <span data-ttu-id="171f4-169">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="171f4-169">N/A</span></span> | <span data-ttu-id="171f4-170">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="171f4-170">N/A</span></span> | <span data-ttu-id="171f4-171">يتم إنشاء المستودع الافتراضي باستخدام واجهة برمجة التطبيقات **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="171f4-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="171f4-172">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-172">Project team member</span></span> | <span data-ttu-id="171f4-173">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-173">Yes</span></span> | <span data-ttu-id="171f4-174">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-174">Yes</span></span> | <span data-ttu-id="171f4-175">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-175">Yes</span></span> | <span data-ttu-id="171f4-176">بالنسبة لعملية الإنشاء، استخدم واجهة برمجة التطبيقات **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="171f4-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="171f4-177">Project</span><span class="sxs-lookup"><span data-stu-id="171f4-177">Project</span></span> | <span data-ttu-id="171f4-178">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-178">Yes</span></span> | <span data-ttu-id="171f4-179">نعم </span><span class="sxs-lookup"><span data-stu-id="171f4-179">Yes</span></span> | <span data-ttu-id="171f4-180">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="171f4-180">N/A</span></span> | <span data-ttu-id="171f4-181">العمليات مع الحقول التالية غير مدعومة: **StateCode** و **BulkGenerationStatus** و **GlobalRevisionToken** و **CalendarID** و **Effort** و **EffortCompleted** و **EffortRemaining** و **Progress** و **Finish** و **TaskEarliestStart** و **Duration**.</span><span class="sxs-lookup"><span data-stu-id="171f4-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="171f4-182">يمكن استدعاء واجهات برمجة التطبيقات مع كائنات الكيانات التي تتضمن حقولاً مخصصة.</span><span class="sxs-lookup"><span data-stu-id="171f4-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="171f4-183">خاصية المعرف اختيارية.</span><span class="sxs-lookup"><span data-stu-id="171f4-183">The ID property is optional.</span></span> <span data-ttu-id="171f4-184">إذا تم توفيرها، يحاول النظام استخدامها ويلقي استثناءً إذا لم يكن من الممكن استخدامها.</span><span class="sxs-lookup"><span data-stu-id="171f4-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="171f4-185">إذا لم يتم توفيرها، سيقوم النظام بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="171f4-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="171f4-186">الحقول المقيدة</span><span class="sxs-lookup"><span data-stu-id="171f4-186">Restricted fields</span></span>

<span data-ttu-id="171f4-187">يُعرف الجداول التالي الحقول المقيدة من **الإنشاء** و **التحرير.**</span><span class="sxs-lookup"><span data-stu-id="171f4-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="171f4-188">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-188">Project task</span></span>

| <span data-ttu-id="171f4-189">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="171f4-189">**Logical name**</span></span>                       | <span data-ttu-id="171f4-190">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="171f4-190">**Can create**</span></span> | <span data-ttu-id="171f4-191">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="171f4-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="171f4-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="171f4-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="171f4-193">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-193">no</span></span>             | <span data-ttu-id="171f4-194">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-194">no</span></span>               |
| <span data-ttu-id="171f4-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="171f4-196">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-196">no</span></span>             | <span data-ttu-id="171f4-197">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-197">no</span></span>               |
| <span data-ttu-id="171f4-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="171f4-198">msdyn_actualend</span></span>                        | <span data-ttu-id="171f4-199">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-199">no</span></span>             | <span data-ttu-id="171f4-200">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-200">no</span></span>               |
| <span data-ttu-id="171f4-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="171f4-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="171f4-202">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-202">no</span></span>             | <span data-ttu-id="171f4-203">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-203">no</span></span>               |
| <span data-ttu-id="171f4-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="171f4-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="171f4-205">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-205">no</span></span>             | <span data-ttu-id="171f4-206">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-206">no</span></span>               |
| <span data-ttu-id="171f4-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="171f4-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="171f4-208">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-208">no</span></span>             | <span data-ttu-id="171f4-209">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-209">no</span></span>               |
| <span data-ttu-id="171f4-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="171f4-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="171f4-211">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-211">no</span></span>             | <span data-ttu-id="171f4-212">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-212">no</span></span>               |
| <span data-ttu-id="171f4-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="171f4-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="171f4-214">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-214">no</span></span>             | <span data-ttu-id="171f4-215">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-215">no</span></span>               |
| <span data-ttu-id="171f4-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="171f4-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="171f4-217">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-217">no</span></span>             | <span data-ttu-id="171f4-218">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-218">no</span></span>               |
| <span data-ttu-id="171f4-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="171f4-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="171f4-220">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-220">no</span></span>             | <span data-ttu-id="171f4-221">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-221">no</span></span>               |
| <span data-ttu-id="171f4-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="171f4-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="171f4-223">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-223">no</span></span>             | <span data-ttu-id="171f4-224">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-224">no</span></span>               |
| <span data-ttu-id="171f4-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="171f4-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="171f4-226">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-226">no</span></span>             | <span data-ttu-id="171f4-227">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-227">no</span></span>               |
| <span data-ttu-id="171f4-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="171f4-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="171f4-229">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-229">no</span></span>             | <span data-ttu-id="171f4-230">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-230">no</span></span>               |
| <span data-ttu-id="171f4-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="171f4-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="171f4-232">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-232">no</span></span>             | <span data-ttu-id="171f4-233">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-233">no</span></span>               |
| <span data-ttu-id="171f4-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="171f4-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="171f4-235">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-235">no</span></span>             | <span data-ttu-id="171f4-236">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-236">no</span></span>               |
| <span data-ttu-id="171f4-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="171f4-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="171f4-238">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-238">no</span></span>             | <span data-ttu-id="171f4-239">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-239">no</span></span>               |
| <span data-ttu-id="171f4-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="171f4-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="171f4-241">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-241">no</span></span>             | <span data-ttu-id="171f4-242">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-242">no</span></span>               |
| <span data-ttu-id="171f4-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="171f4-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="171f4-244">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-244">no</span></span>             | <span data-ttu-id="171f4-245">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-245">no</span></span>               |
| <span data-ttu-id="171f4-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="171f4-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="171f4-247">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-247">no</span></span>             | <span data-ttu-id="171f4-248">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-248">no</span></span>               |
| <span data-ttu-id="171f4-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="171f4-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="171f4-250">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-250">no</span></span>             | <span data-ttu-id="171f4-251">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-251">no</span></span>               |
| <span data-ttu-id="171f4-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="171f4-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="171f4-253">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-253">no</span></span>             | <span data-ttu-id="171f4-254">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-254">no</span></span>               |
| <span data-ttu-id="171f4-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="171f4-256">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-256">no</span></span>             | <span data-ttu-id="171f4-257">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-257">no</span></span>               |
| <span data-ttu-id="171f4-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="171f4-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="171f4-259">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-259">no</span></span>             | <span data-ttu-id="171f4-260">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-260">no</span></span>               |
| <span data-ttu-id="171f4-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="171f4-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="171f4-262">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-262">no</span></span>             | <span data-ttu-id="171f4-263">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-263">no</span></span>               |
| <span data-ttu-id="171f4-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="171f4-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="171f4-265">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-265">no</span></span>             | <span data-ttu-id="171f4-266">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-266">no</span></span>               |
| <span data-ttu-id="171f4-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="171f4-267">msdyn_progress</span></span>                         | <span data-ttu-id="171f4-268">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-268">no</span></span>             | <span data-ttu-id="171f4-269">لا (نعم لـ P4W)</span><span class="sxs-lookup"><span data-stu-id="171f4-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="171f4-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="171f4-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="171f4-271">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-271">no</span></span>             | <span data-ttu-id="171f4-272">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-272">no</span></span>               |
| <span data-ttu-id="171f4-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="171f4-274">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-274">no</span></span>             | <span data-ttu-id="171f4-275">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-275">no</span></span>               |
| <span data-ttu-id="171f4-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="171f4-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="171f4-277">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-277">no</span></span>             | <span data-ttu-id="171f4-278">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-278">no</span></span>               |
| <span data-ttu-id="171f4-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="171f4-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="171f4-280">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-280">no</span></span>             | <span data-ttu-id="171f4-281">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-281">no</span></span>               |
| <span data-ttu-id="171f4-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="171f4-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="171f4-283">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-283">no</span></span>             | <span data-ttu-id="171f4-284">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-284">no</span></span>               |
| <span data-ttu-id="171f4-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="171f4-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="171f4-286">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-286">no</span></span>             | <span data-ttu-id="171f4-287">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-287">no</span></span>               |
| <span data-ttu-id="171f4-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="171f4-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="171f4-289">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-289">no</span></span>             | <span data-ttu-id="171f4-290">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-290">no</span></span>               |
| <span data-ttu-id="171f4-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="171f4-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="171f4-292">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-292">no</span></span>             | <span data-ttu-id="171f4-293">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-293">no</span></span>               |
| <span data-ttu-id="171f4-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="171f4-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="171f4-295">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-295">no</span></span>             | <span data-ttu-id="171f4-296">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-296">no</span></span>               |
| <span data-ttu-id="171f4-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="171f4-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="171f4-298">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-298">no</span></span>             | <span data-ttu-id="171f4-299">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-299">no</span></span>               |
| <span data-ttu-id="171f4-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="171f4-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="171f4-301">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-301">no</span></span>             | <span data-ttu-id="171f4-302">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-302">no</span></span>               |
| <span data-ttu-id="171f4-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="171f4-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="171f4-304">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-304">no</span></span>             | <span data-ttu-id="171f4-305">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-305">no</span></span>               |
| <span data-ttu-id="171f4-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="171f4-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="171f4-307">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-307">no</span></span>             | <span data-ttu-id="171f4-308">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-308">no</span></span>               |
| <span data-ttu-id="171f4-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="171f4-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="171f4-310">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-310">no</span></span>             | <span data-ttu-id="171f4-311">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-311">no</span></span>               |
| <span data-ttu-id="171f4-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="171f4-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="171f4-313">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-313">no</span></span>             | <span data-ttu-id="171f4-314">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-314">no</span></span>               |
| <span data-ttu-id="171f4-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="171f4-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="171f4-316">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-316">no</span></span>             | <span data-ttu-id="171f4-317">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-317">no</span></span>               |
| <span data-ttu-id="171f4-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="171f4-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="171f4-319">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-319">no</span></span>             | <span data-ttu-id="171f4-320">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-320">no</span></span>               |
| <span data-ttu-id="171f4-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="171f4-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="171f4-322">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-322">no</span></span>             | <span data-ttu-id="171f4-323">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-323">no</span></span>               |
| <span data-ttu-id="171f4-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="171f4-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="171f4-325">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-325">no</span></span>             | <span data-ttu-id="171f4-326">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-326">no</span></span>               |
| <span data-ttu-id="171f4-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="171f4-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="171f4-328">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-328">no</span></span>             | <span data-ttu-id="171f4-329">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-329">no</span></span>               |
| <span data-ttu-id="171f4-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="171f4-330">msdyn_summary</span></span>                          | <span data-ttu-id="171f4-331">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-331">no</span></span>             | <span data-ttu-id="171f4-332">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-332">no</span></span>               |
| <span data-ttu-id="171f4-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="171f4-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="171f4-334">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-334">no</span></span>             | <span data-ttu-id="171f4-335">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-335">no</span></span>               |
| <span data-ttu-id="171f4-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="171f4-337">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-337">no</span></span>             | <span data-ttu-id="171f4-338">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="171f4-339">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-339">Project task dependency</span></span>

| <span data-ttu-id="171f4-340">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="171f4-340">**Logical name**</span></span>              | <span data-ttu-id="171f4-341">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="171f4-341">**Can create**</span></span> | <span data-ttu-id="171f4-342">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="171f4-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="171f4-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="171f4-343">msdyn_linktype</span></span>                | <span data-ttu-id="171f4-344">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-344">no</span></span>             | <span data-ttu-id="171f4-345">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-345">no</span></span>           |
| <span data-ttu-id="171f4-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="171f4-346">msdyn_linktypename</span></span>            | <span data-ttu-id="171f4-347">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-347">no</span></span>             | <span data-ttu-id="171f4-348">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-348">no</span></span>           |
| <span data-ttu-id="171f4-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="171f4-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="171f4-350">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-350">yes</span></span>            | <span data-ttu-id="171f4-351">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-351">no</span></span>           |
| <span data-ttu-id="171f4-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="171f4-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="171f4-353">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-353">yes</span></span>            | <span data-ttu-id="171f4-354">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-354">no</span></span>           |
| <span data-ttu-id="171f4-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="171f4-355">msdyn_project</span></span>                 | <span data-ttu-id="171f4-356">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-356">yes</span></span>            | <span data-ttu-id="171f4-357">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-357">no</span></span>           |
| <span data-ttu-id="171f4-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="171f4-358">msdyn_projectname</span></span>             | <span data-ttu-id="171f4-359">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-359">yes</span></span>            | <span data-ttu-id="171f4-360">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-360">no</span></span>           |
| <span data-ttu-id="171f4-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="171f4-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="171f4-362">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-362">yes</span></span>            | <span data-ttu-id="171f4-363">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-363">no</span></span>           |
| <span data-ttu-id="171f4-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="171f4-364">msdyn_successortask</span></span>           | <span data-ttu-id="171f4-365">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-365">yes</span></span>            | <span data-ttu-id="171f4-366">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-366">no</span></span>           |
| <span data-ttu-id="171f4-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="171f4-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="171f4-368">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-368">yes</span></span>            | <span data-ttu-id="171f4-369">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="171f4-370">تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="171f4-370">Resource assignment</span></span>

| <span data-ttu-id="171f4-371">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="171f4-371">**Logical name**</span></span>             | <span data-ttu-id="171f4-372">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="171f4-372">**Can create**</span></span> | <span data-ttu-id="171f4-373">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="171f4-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="171f4-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="171f4-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="171f4-375">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-375">yes</span></span>            | <span data-ttu-id="171f4-376">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-376">no</span></span>           |
| <span data-ttu-id="171f4-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="171f4-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="171f4-378">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-378">yes</span></span>            | <span data-ttu-id="171f4-379">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-379">no</span></span>           |
| <span data-ttu-id="171f4-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="171f4-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="171f4-381">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-381">no</span></span>             | <span data-ttu-id="171f4-382">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-382">no</span></span>           |
| <span data-ttu-id="171f4-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="171f4-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="171f4-384">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-384">no</span></span>             | <span data-ttu-id="171f4-385">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-385">no</span></span>           |
| <span data-ttu-id="171f4-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="171f4-386">msdyn_committype</span></span>             | <span data-ttu-id="171f4-387">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-387">no</span></span>             | <span data-ttu-id="171f4-388">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-388">no</span></span>           |
| <span data-ttu-id="171f4-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="171f4-389">msdyn_committypename</span></span>         | <span data-ttu-id="171f4-390">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-390">no</span></span>             | <span data-ttu-id="171f4-391">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-391">no</span></span>           |
| <span data-ttu-id="171f4-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="171f4-392">msdyn_effort</span></span>                 | <span data-ttu-id="171f4-393">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-393">no</span></span>             | <span data-ttu-id="171f4-394">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-394">no</span></span>           |
| <span data-ttu-id="171f4-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="171f4-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="171f4-396">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-396">no</span></span>             | <span data-ttu-id="171f4-397">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-397">no</span></span>           |
| <span data-ttu-id="171f4-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="171f4-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="171f4-399">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-399">no</span></span>             | <span data-ttu-id="171f4-400">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-400">no</span></span>           |
| <span data-ttu-id="171f4-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="171f4-401">msdyn_finish</span></span>                 | <span data-ttu-id="171f4-402">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-402">no</span></span>             | <span data-ttu-id="171f4-403">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-403">no</span></span>           |
| <span data-ttu-id="171f4-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="171f4-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="171f4-405">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-405">no</span></span>             | <span data-ttu-id="171f4-406">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-406">no</span></span>           |
| <span data-ttu-id="171f4-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="171f4-408">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-408">no</span></span>             | <span data-ttu-id="171f4-409">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-409">no</span></span>           |
| <span data-ttu-id="171f4-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="171f4-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="171f4-411">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-411">no</span></span>             | <span data-ttu-id="171f4-412">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-412">no</span></span>           |
| <span data-ttu-id="171f4-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="171f4-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="171f4-414">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-414">no</span></span>             | <span data-ttu-id="171f4-415">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-415">no</span></span>           |
| <span data-ttu-id="171f4-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="171f4-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="171f4-417">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-417">no</span></span>             | <span data-ttu-id="171f4-418">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-418">no</span></span>           |
| <span data-ttu-id="171f4-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="171f4-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="171f4-420">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-420">no</span></span>             | <span data-ttu-id="171f4-421">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-421">no</span></span>           |
| <span data-ttu-id="171f4-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="171f4-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="171f4-423">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-423">no</span></span>             | <span data-ttu-id="171f4-424">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-424">no</span></span>           |
| <span data-ttu-id="171f4-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="171f4-425">msdyn_projectid</span></span>              | <span data-ttu-id="171f4-426">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-426">yes</span></span>            | <span data-ttu-id="171f4-427">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-427">no</span></span>           |
| <span data-ttu-id="171f4-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="171f4-428">msdyn_projectidname</span></span>          | <span data-ttu-id="171f4-429">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-429">no</span></span>             | <span data-ttu-id="171f4-430">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-430">no</span></span>           |
| <span data-ttu-id="171f4-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="171f4-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="171f4-432">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-432">no</span></span>             | <span data-ttu-id="171f4-433">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-433">no</span></span>           |
| <span data-ttu-id="171f4-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="171f4-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="171f4-435">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-435">no</span></span>             | <span data-ttu-id="171f4-436">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-436">no</span></span>           |
| <span data-ttu-id="171f4-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="171f4-437">msdyn_start</span></span>                  | <span data-ttu-id="171f4-438">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-438">no</span></span>             | <span data-ttu-id="171f4-439">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-439">no</span></span>           |
| <span data-ttu-id="171f4-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="171f4-440">msdyn_taskid</span></span>                 | <span data-ttu-id="171f4-441">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-441">no</span></span>             | <span data-ttu-id="171f4-442">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-442">no</span></span>           |
| <span data-ttu-id="171f4-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="171f4-443">msdyn_taskidname</span></span>             | <span data-ttu-id="171f4-444">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-444">no</span></span>             | <span data-ttu-id="171f4-445">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-445">no</span></span>           |
| <span data-ttu-id="171f4-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="171f4-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="171f4-447">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-447">no</span></span>             | <span data-ttu-id="171f4-448">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="171f4-449">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="171f4-449">Project team member</span></span>

| <span data-ttu-id="171f4-450">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="171f4-450">**Logical name**</span></span>                                 | <span data-ttu-id="171f4-451">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="171f4-451">**Can create**</span></span> | <span data-ttu-id="171f4-452">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="171f4-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="171f4-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="171f4-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="171f4-454">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-454">no</span></span>             | <span data-ttu-id="171f4-455">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-455">no</span></span>           |
| <span data-ttu-id="171f4-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="171f4-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="171f4-457">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-457">no</span></span>             | <span data-ttu-id="171f4-458">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-458">no</span></span>           |
| <span data-ttu-id="171f4-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="171f4-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="171f4-460">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-460">no</span></span>             | <span data-ttu-id="171f4-461">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-461">no</span></span>           |
| <span data-ttu-id="171f4-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="171f4-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="171f4-463">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-463">no</span></span>             | <span data-ttu-id="171f4-464">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-464">no</span></span>           |
| <span data-ttu-id="171f4-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="171f4-465">msdyn_effort</span></span>                                     | <span data-ttu-id="171f4-466">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-466">no</span></span>             | <span data-ttu-id="171f4-467">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-467">no</span></span>           |
| <span data-ttu-id="171f4-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="171f4-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="171f4-469">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-469">no</span></span>             | <span data-ttu-id="171f4-470">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-470">no</span></span>           |
| <span data-ttu-id="171f4-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="171f4-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="171f4-472">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-472">no</span></span>             | <span data-ttu-id="171f4-473">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-473">no</span></span>           |
| <span data-ttu-id="171f4-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="171f4-474">msdyn_finish</span></span>                                     | <span data-ttu-id="171f4-475">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-475">no</span></span>             | <span data-ttu-id="171f4-476">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-476">no</span></span>           |
| <span data-ttu-id="171f4-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="171f4-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="171f4-478">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-478">no</span></span>             | <span data-ttu-id="171f4-479">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-479">no</span></span>           |
| <span data-ttu-id="171f4-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="171f4-480">msdyn_hours</span></span>                                      | <span data-ttu-id="171f4-481">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-481">no</span></span>             | <span data-ttu-id="171f4-482">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-482">no</span></span>           |
| <span data-ttu-id="171f4-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="171f4-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="171f4-484">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-484">no</span></span>             | <span data-ttu-id="171f4-485">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-485">no</span></span>           |
| <span data-ttu-id="171f4-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="171f4-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="171f4-487">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-487">no</span></span>             | <span data-ttu-id="171f4-488">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-488">no</span></span>           |
| <span data-ttu-id="171f4-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="171f4-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="171f4-490">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-490">no</span></span>             | <span data-ttu-id="171f4-491">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-491">no</span></span>           |
| <span data-ttu-id="171f4-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="171f4-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="171f4-493">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-493">no</span></span>             | <span data-ttu-id="171f4-494">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-494">no</span></span>           |
| <span data-ttu-id="171f4-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="171f4-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="171f4-496">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-496">no</span></span>             | <span data-ttu-id="171f4-497">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-497">no</span></span>           |
| <span data-ttu-id="171f4-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="171f4-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="171f4-499">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-499">no</span></span>             | <span data-ttu-id="171f4-500">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-500">no</span></span>           |
| <span data-ttu-id="171f4-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="171f4-501">msdyn_start</span></span>                                      | <span data-ttu-id="171f4-502">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-502">no</span></span>             | <span data-ttu-id="171f4-503">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="171f4-504">Project</span><span class="sxs-lookup"><span data-stu-id="171f4-504">Project</span></span>

| <span data-ttu-id="171f4-505">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="171f4-505">**Logical name**</span></span>                       | <span data-ttu-id="171f4-506">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="171f4-506">**Can create**</span></span> | <span data-ttu-id="171f4-507">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="171f4-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="171f4-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="171f4-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="171f4-509">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-509">no</span></span>             | <span data-ttu-id="171f4-510">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-510">no</span></span>           |
| <span data-ttu-id="171f4-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="171f4-512">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-512">no</span></span>             | <span data-ttu-id="171f4-513">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-513">no</span></span>           |
| <span data-ttu-id="171f4-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="171f4-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="171f4-515">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-515">no</span></span>             | <span data-ttu-id="171f4-516">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-516">no</span></span>           |
| <span data-ttu-id="171f4-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="171f4-518">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-518">no</span></span>             | <span data-ttu-id="171f4-519">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-519">no</span></span>           |
| <span data-ttu-id="171f4-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="171f4-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="171f4-521">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-521">no</span></span>             | <span data-ttu-id="171f4-522">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-522">no</span></span>           |
| <span data-ttu-id="171f4-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="171f4-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="171f4-524">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-524">no</span></span>             | <span data-ttu-id="171f4-525">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-525">no</span></span>           |
| <span data-ttu-id="171f4-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="171f4-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="171f4-527">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-527">yes</span></span>            | <span data-ttu-id="171f4-528">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-528">no</span></span>           |
| <span data-ttu-id="171f4-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="171f4-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="171f4-530">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-530">yes</span></span>            | <span data-ttu-id="171f4-531">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-531">no</span></span>           |
| <span data-ttu-id="171f4-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="171f4-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="171f4-533">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-533">yes</span></span>            | <span data-ttu-id="171f4-534">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-534">no</span></span>           |
| <span data-ttu-id="171f4-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="171f4-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="171f4-536">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-536">no</span></span>             | <span data-ttu-id="171f4-537">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-537">no</span></span>           |
| <span data-ttu-id="171f4-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="171f4-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="171f4-539">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-539">no</span></span>             | <span data-ttu-id="171f4-540">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-540">no</span></span>           |
| <span data-ttu-id="171f4-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="171f4-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="171f4-542">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-542">no</span></span>             | <span data-ttu-id="171f4-543">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-543">no</span></span>           |
| <span data-ttu-id="171f4-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="171f4-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="171f4-545">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-545">no</span></span>             | <span data-ttu-id="171f4-546">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-546">no</span></span>           |
| <span data-ttu-id="171f4-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="171f4-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="171f4-548">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-548">no</span></span>             | <span data-ttu-id="171f4-549">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-549">no</span></span>           |
| <span data-ttu-id="171f4-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="171f4-550">msdyn_duration</span></span>                         | <span data-ttu-id="171f4-551">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-551">no</span></span>             | <span data-ttu-id="171f4-552">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-552">no</span></span>           |
| <span data-ttu-id="171f4-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="171f4-553">msdyn_effort</span></span>                           | <span data-ttu-id="171f4-554">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-554">no</span></span>             | <span data-ttu-id="171f4-555">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-555">no</span></span>           |
| <span data-ttu-id="171f4-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="171f4-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="171f4-557">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-557">no</span></span>             | <span data-ttu-id="171f4-558">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-558">no</span></span>           |
| <span data-ttu-id="171f4-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="171f4-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="171f4-560">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-560">no</span></span>             | <span data-ttu-id="171f4-561">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-561">no</span></span>           |
| <span data-ttu-id="171f4-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="171f4-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="171f4-563">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-563">no</span></span>             | <span data-ttu-id="171f4-564">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-564">no</span></span>           |
| <span data-ttu-id="171f4-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="171f4-565">msdyn_finish</span></span>                           | <span data-ttu-id="171f4-566">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-566">yes</span></span>            | <span data-ttu-id="171f4-567">نعم</span><span class="sxs-lookup"><span data-stu-id="171f4-567">yes</span></span>          |
| <span data-ttu-id="171f4-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="171f4-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="171f4-569">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-569">no</span></span>             | <span data-ttu-id="171f4-570">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-570">no</span></span>           |
| <span data-ttu-id="171f4-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="171f4-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="171f4-572">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-572">no</span></span>             | <span data-ttu-id="171f4-573">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-573">no</span></span>           |
| <span data-ttu-id="171f4-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="171f4-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="171f4-575">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-575">no</span></span>             | <span data-ttu-id="171f4-576">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-576">no</span></span>           |
| <span data-ttu-id="171f4-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="171f4-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="171f4-578">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-578">no</span></span>             | <span data-ttu-id="171f4-579">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-579">no</span></span>           |
| <span data-ttu-id="171f4-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="171f4-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="171f4-581">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-581">no</span></span>             | <span data-ttu-id="171f4-582">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-582">no</span></span>           |
| <span data-ttu-id="171f4-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="171f4-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="171f4-584">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-584">no</span></span>             | <span data-ttu-id="171f4-585">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-585">no</span></span>           |
| <span data-ttu-id="171f4-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="171f4-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="171f4-587">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-587">no</span></span>             | <span data-ttu-id="171f4-588">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-588">no</span></span>           |
| <span data-ttu-id="171f4-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="171f4-590">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-590">no</span></span>             | <span data-ttu-id="171f4-591">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-591">no</span></span>           |
| <span data-ttu-id="171f4-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="171f4-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="171f4-593">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-593">no</span></span>             | <span data-ttu-id="171f4-594">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-594">no</span></span>           |
| <span data-ttu-id="171f4-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="171f4-596">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-596">no</span></span>             | <span data-ttu-id="171f4-597">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-597">no</span></span>           |
| <span data-ttu-id="171f4-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="171f4-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="171f4-599">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-599">no</span></span>             | <span data-ttu-id="171f4-600">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-600">no</span></span>           |
| <span data-ttu-id="171f4-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="171f4-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="171f4-602">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-602">no</span></span>             | <span data-ttu-id="171f4-603">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-603">no</span></span>           |
| <span data-ttu-id="171f4-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="171f4-604">msdyn_progress</span></span>                         | <span data-ttu-id="171f4-605">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-605">no</span></span>             | <span data-ttu-id="171f4-606">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-606">no</span></span>           |
| <span data-ttu-id="171f4-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="171f4-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="171f4-608">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-608">no</span></span>             | <span data-ttu-id="171f4-609">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-609">no</span></span>           |
| <span data-ttu-id="171f4-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="171f4-611">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-611">no</span></span>             | <span data-ttu-id="171f4-612">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-612">no</span></span>           |
| <span data-ttu-id="171f4-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="171f4-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="171f4-614">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-614">no</span></span>             | <span data-ttu-id="171f4-615">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-615">no</span></span>           |
| <span data-ttu-id="171f4-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="171f4-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="171f4-617">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-617">no</span></span>             | <span data-ttu-id="171f4-618">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-618">no</span></span>           |
| <span data-ttu-id="171f4-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="171f4-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="171f4-620">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-620">no</span></span>             | <span data-ttu-id="171f4-621">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-621">no</span></span>           |
| <span data-ttu-id="171f4-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="171f4-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="171f4-623">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-623">no</span></span>             | <span data-ttu-id="171f4-624">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-624">no</span></span>           |
| <span data-ttu-id="171f4-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="171f4-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="171f4-626">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-626">no</span></span>             | <span data-ttu-id="171f4-627">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-627">no</span></span>           |
| <span data-ttu-id="171f4-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="171f4-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="171f4-629">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-629">no</span></span>             | <span data-ttu-id="171f4-630">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-630">no</span></span>           |
| <span data-ttu-id="171f4-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="171f4-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="171f4-632">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-632">no</span></span>             | <span data-ttu-id="171f4-633">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-633">no</span></span>           |
| <span data-ttu-id="171f4-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="171f4-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="171f4-635">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-635">no</span></span>             | <span data-ttu-id="171f4-636">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-636">no</span></span>           |
| <span data-ttu-id="171f4-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="171f4-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="171f4-638">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-638">no</span></span>             | <span data-ttu-id="171f4-639">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-639">no</span></span>           |
| <span data-ttu-id="171f4-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="171f4-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="171f4-641">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-641">no</span></span>             | <span data-ttu-id="171f4-642">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-642">no</span></span>           |
| <span data-ttu-id="171f4-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="171f4-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="171f4-644">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-644">no</span></span>             | <span data-ttu-id="171f4-645">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-645">no</span></span>           |
| <span data-ttu-id="171f4-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="171f4-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="171f4-647">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-647">no</span></span>             | <span data-ttu-id="171f4-648">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-648">no</span></span>           |
| <span data-ttu-id="171f4-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="171f4-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="171f4-650">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-650">no</span></span>             | <span data-ttu-id="171f4-651">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-651">no</span></span>           |
| <span data-ttu-id="171f4-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="171f4-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="171f4-653">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-653">no</span></span>             | <span data-ttu-id="171f4-654">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-654">no</span></span>           |
| <span data-ttu-id="171f4-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="171f4-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="171f4-656">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-656">no</span></span>             | <span data-ttu-id="171f4-657">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-657">no</span></span>           |
| <span data-ttu-id="171f4-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="171f4-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="171f4-659">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-659">no</span></span>             | <span data-ttu-id="171f4-660">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-660">no</span></span>           |
| <span data-ttu-id="171f4-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="171f4-662">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-662">no</span></span>             | <span data-ttu-id="171f4-663">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-663">no</span></span>           |
| <span data-ttu-id="171f4-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="171f4-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="171f4-665">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-665">no</span></span>             | <span data-ttu-id="171f4-666">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-666">no</span></span>           |
| <span data-ttu-id="171f4-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="171f4-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="171f4-668">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-668">no</span></span>             | <span data-ttu-id="171f4-669">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="171f4-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="171f4-670">القيود والمشاكل المعروفة</span><span class="sxs-lookup"><span data-stu-id="171f4-670">Limitations and known issues</span></span>
<span data-ttu-id="171f4-671">فيما يلي قائمة بالقيود والمشاكل المعروفة:</span><span class="sxs-lookup"><span data-stu-id="171f4-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="171f4-672">لا يمكن استخدام واجهات برمجة تطبيقات جدولة المشروع إلا بواسطة **المستخدمين الذين لديهم ترخيص Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="171f4-672">Project Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="171f4-673">لا يمكن استخدامها بواسطة:</span><span class="sxs-lookup"><span data-stu-id="171f4-673">They can't be used by:</span></span>
    - <span data-ttu-id="171f4-674">مستخدمي التطبيق</span><span class="sxs-lookup"><span data-stu-id="171f4-674">Application users</span></span>
    - <span data-ttu-id="171f4-675">مستخدمي النظام</span><span class="sxs-lookup"><span data-stu-id="171f4-675">System users</span></span>
    - <span data-ttu-id="171f4-676">مستخدمي التكامل</span><span class="sxs-lookup"><span data-stu-id="171f4-676">Integration users</span></span>
    - <span data-ttu-id="171f4-677">المستخدمين الآخرين الذين ليس لديهم الترخيص المطلوب</span><span class="sxs-lookup"><span data-stu-id="171f4-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="171f4-678">تتضمن كل **OperationSet** مئة عملية كحدٍ أقصى.</span><span class="sxs-lookup"><span data-stu-id="171f4-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="171f4-679">بإمكان كل مستخدم أن يحصل على عشر **OperationSet** مفتوحة كحدٍ أقصى.</span><span class="sxs-lookup"><span data-stu-id="171f4-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="171f4-680">يدعم Project Operations في الوقت الحالي 500 مهمة إجمالية كحد أقصى على مشروع.</span><span class="sxs-lookup"><span data-stu-id="171f4-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="171f4-681">في الوقت الحالي، لا تتوفر حالة فشل **OperationSet** وسجلات الفشل.</span><span class="sxs-lookup"><span data-stu-id="171f4-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="171f4-682">القيود والحدود على المشروعات والمهام</span><span class="sxs-lookup"><span data-stu-id="171f4-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="171f4-683">معالجة الخطأ</span><span class="sxs-lookup"><span data-stu-id="171f4-683">Error handling</span></span>

   - <span data-ttu-id="171f4-684">لمراجعة الأخطاء التي تم إنشاؤها من مجموعات العمليات، انتقل إلى **الإعدادات** \> **تكامل الجدول** \> **مجموعات العمليات**.</span><span class="sxs-lookup"><span data-stu-id="171f4-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="171f4-685">لمراجعة الأخطاء التي تم إنشاؤها من خدمة جدولة المشروع، انتقل إلى **إعدادات** \> **‏‫تكامل الجدولة** \> **سجلات أخطاء PSS**.</span><span class="sxs-lookup"><span data-stu-id="171f4-685">To review errors generated from the Project schedule Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="171f4-686">سيناريو نموذجي</span><span class="sxs-lookup"><span data-stu-id="171f4-686">Sample scenario</span></span>

<span data-ttu-id="171f4-687">في هذا السيناريو، ستقوم بإنشاء مشروع، وعضو فريق، وأربع مهام، وعمليتي تعيين للموارد.</span><span class="sxs-lookup"><span data-stu-id="171f4-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="171f4-688">بعد ذلك، عليك تحديث مهمة واحدة وتحديث المشروع وحذف مهمة واحدة وحذف تعيين مورد واحد وإنشاء تبعية مهمة.</span><span class="sxs-lookup"><span data-stu-id="171f4-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```csharp
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
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="171f4-689">عينات إضافية</span><span class="sxs-lookup"><span data-stu-id="171f4-689">Additional samples</span></span>

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
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
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
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
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
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
/// </summary>
/// <param name="operationSetId">operationSet id</param>
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
/// <param name="operationSetId">operationSet id</param>
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
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
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
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
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
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
