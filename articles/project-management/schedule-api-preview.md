---
title: استخدام واجهات برمجة تطبيقات الجدولة لتنفيذ عمليات مع كيانات الجدولة
description: يوفر هذا الموضوع معلومات و عينات لاستخدام واجهات برمجة تطبيقات الجدولة.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950788"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="0e022-103">استخدام واجهات برمجة تطبيقات الجدولة لتنفيذ عمليات مع كيانات الجدولة</span><span class="sxs-lookup"><span data-stu-id="0e022-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="0e022-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="0e022-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="0e022-105">تتوفر بعض الوظائف المذكورة في هذا الموضوع أو كلها كجزء من إصدار أولي.</span><span class="sxs-lookup"><span data-stu-id="0e022-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="0e022-106">إن المحتوى والوظائف خاضعة للتغيير.</span><span class="sxs-lookup"><span data-stu-id="0e022-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="0e022-107">كيانات الجدولة</span><span class="sxs-lookup"><span data-stu-id="0e022-107">Scheduling entities</span></span>

<span data-ttu-id="0e022-108">توفر واجهات برمجة تطبيقات جدولة القدرة على تنفيذ عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="0e022-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="0e022-109">تُدار هذه الكيانات من خلال محرك جدولة في المشروع للويب.</span><span class="sxs-lookup"><span data-stu-id="0e022-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="0e022-110">كانت عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة** مقيدة في إصدارات Dynamics 365 Project Operations السابقة.</span><span class="sxs-lookup"><span data-stu-id="0e022-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="0e022-111">يوفر الجدول التالي قائمة كاملة تتضمن **كيانات الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="0e022-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="0e022-112">اسم الكيان</span><span class="sxs-lookup"><span data-stu-id="0e022-112">Entity name</span></span>  | <span data-ttu-id="0e022-113">اسم منطقي للكيان</span><span class="sxs-lookup"><span data-stu-id="0e022-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="0e022-114">Project</span><span class="sxs-lookup"><span data-stu-id="0e022-114">Project</span></span> | <span data-ttu-id="0e022-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="0e022-115">msdyn_project</span></span> |
| <span data-ttu-id="0e022-116">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-116">Project Task</span></span>  | <span data-ttu-id="0e022-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="0e022-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="0e022-118">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-118">Project Task Dependency</span></span>  | <span data-ttu-id="0e022-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="0e022-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="0e022-120">تعيين المورد</span><span class="sxs-lookup"><span data-stu-id="0e022-120">Resource Assignment</span></span> | <span data-ttu-id="0e022-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="0e022-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="0e022-122">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-122">Project Bucket</span></span>  | <span data-ttu-id="0e022-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="0e022-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="0e022-124">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-124">Project Team Member</span></span> | <span data-ttu-id="0e022-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="0e022-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="0e022-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="0e022-126">OperationSet</span></span>

<span data-ttu-id="0e022-127">إن OperationSet عبارة نمط وحدة عمل يمكن استخدامه عندما يكون من الضروري معالجة طلبات متعددة تؤثر على الجدولة ضمن حركة.</span><span class="sxs-lookup"><span data-stu-id="0e022-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="0e022-128">واجهات برمجة تطبيقات الجدولة</span><span class="sxs-lookup"><span data-stu-id="0e022-128">Schedule APIs</span></span>

<span data-ttu-id="0e022-129">فيما يلي قائمة بواجهات برمجة تطبيقات الجدولة الحالية.</span><span class="sxs-lookup"><span data-stu-id="0e022-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="0e022-130">**msdyn_CreateProjectV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء مشروع.</span><span class="sxs-lookup"><span data-stu-id="0e022-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="0e022-131">يتم إنشاء مستودع المشروع والمشروع الافتراضي في الحال.</span><span class="sxs-lookup"><span data-stu-id="0e022-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="0e022-132">**msdyn_CreateTeamMemberV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء عضو فريق مشروع.</span><span class="sxs-lookup"><span data-stu-id="0e022-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="0e022-133">يتم إنشاء سجل عضو الفريق على الفور.</span><span class="sxs-lookup"><span data-stu-id="0e022-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="0e022-134">**msdyn_CreateOperationSetV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لجدولة طلبات متعددة يجب تنفيذها ضمن حركة.</span><span class="sxs-lookup"><span data-stu-id="0e022-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="0e022-135">**msdyn_PSSCreateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء كيان.</span><span class="sxs-lookup"><span data-stu-id="0e022-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="0e022-136">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية الإنشاء.</span><span class="sxs-lookup"><span data-stu-id="0e022-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="0e022-137">**msdyn_PSSUpdateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لتحديث كيان.</span><span class="sxs-lookup"><span data-stu-id="0e022-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="0e022-138">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية التحديث.</span><span class="sxs-lookup"><span data-stu-id="0e022-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="0e022-139">**msdyn_PSSDeleteV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لحذف كيان.</span><span class="sxs-lookup"><span data-stu-id="0e022-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="0e022-140">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية الحذف.</span><span class="sxs-lookup"><span data-stu-id="0e022-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="0e022-141">**msdyn_ExecuteOperationSetV1**: يتم استخدام واجهة برمجة التطبيقات هذه لتنفيذ جميع العمليات ضمن مجموعة عمليات معينة.</span><span class="sxs-lookup"><span data-stu-id="0e022-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="0e022-142">استخدام واجهات برمجة تطبيقات لجدولة مع OperationSet</span><span class="sxs-lookup"><span data-stu-id="0e022-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="0e022-143">نظرًا لاستخدام السجلات مع كل من **CreateProjectV1** و **CreateTeamMemberV1** على الفور، لا يمكن استخدام واجهات برمجة التطبيقات هذه في **OperationSet** بشكل مباشر.</span><span class="sxs-lookup"><span data-stu-id="0e022-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="0e022-144">ومع ذلك، يمكنك استخدام واجهة برمجة التطبيقات لإنشاء السجلات المطلوبة، وإنشاء  **OperationSet**، ثم استخدام هذه السجلات المنشأة مسبقًا في **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="0e022-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="0e022-145">العمليات المدعومة</span><span class="sxs-lookup"><span data-stu-id="0e022-145">Supported operations</span></span>

| <span data-ttu-id="0e022-146">كيان الجدولة</span><span class="sxs-lookup"><span data-stu-id="0e022-146">Scheduling entity</span></span> | <span data-ttu-id="0e022-147">‏إنشاء</span><span class="sxs-lookup"><span data-stu-id="0e022-147">Create</span></span> | <span data-ttu-id="0e022-148">تحديث</span><span class="sxs-lookup"><span data-stu-id="0e022-148">Update</span></span> | <span data-ttu-id="0e022-149">حذف </span><span class="sxs-lookup"><span data-stu-id="0e022-149">Delete</span></span> | <span data-ttu-id="0e022-150">اعتبارات هامة</span><span class="sxs-lookup"><span data-stu-id="0e022-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="0e022-151">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-151">Project task</span></span> | <span data-ttu-id="0e022-152">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-152">Yes</span></span> | <span data-ttu-id="0e022-153">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-153">Yes</span></span> | <span data-ttu-id="0e022-154">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-154">Yes</span></span> | <span data-ttu-id="0e022-155">‏‫بلا</span><span class="sxs-lookup"><span data-stu-id="0e022-155">None</span></span> |
| <span data-ttu-id="0e022-156">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-156">Project task dependency</span></span> | <span data-ttu-id="0e022-157">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-157">Yes</span></span> | <span data-ttu-id="0e022-158">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-158">Yes</span></span> | | <span data-ttu-id="0e022-159">لا يتم تحديث سجلات تبعية مهمة المشروع.</span><span class="sxs-lookup"><span data-stu-id="0e022-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="0e022-160">بدلاً من ذلك، يمكن حذف سجل قديم ويمكن إنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="0e022-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="0e022-161">تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="0e022-161">Resource assignment</span></span> | <span data-ttu-id="0e022-162">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-162">Yes</span></span> | <span data-ttu-id="0e022-163">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-163">Yes</span></span> | | <span data-ttu-id="0e022-164">العمليات مع الحقول التالية غير مدعومة: **BookableResourceID** و **Effort** و **EffortCompleted** و **EffortRemaining** ة **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="0e022-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="0e022-165">لا يتم تحديث سجلات تعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="0e022-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="0e022-166">بدلاً من ذلك، يمكن حذف السجل القديم ويمكن إنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="0e022-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="0e022-167">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-167">Project bucket</span></span> | <span data-ttu-id="0e022-168">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="0e022-168">N/A</span></span> | <span data-ttu-id="0e022-169">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="0e022-169">N/A</span></span> | <span data-ttu-id="0e022-170">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="0e022-170">N/A</span></span> | <span data-ttu-id="0e022-171">يتم إنشاء المستودع الافتراضي باستخدام واجهة برمجة التطبيقات **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="0e022-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="0e022-172">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-172">Project team member</span></span> | <span data-ttu-id="0e022-173">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-173">Yes</span></span> | <span data-ttu-id="0e022-174">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-174">Yes</span></span> | <span data-ttu-id="0e022-175">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-175">Yes</span></span> | <span data-ttu-id="0e022-176">بالنسبة لعملية الإنشاء، استخدم واجهة برمجة التطبيقات **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="0e022-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="0e022-177">Project</span><span class="sxs-lookup"><span data-stu-id="0e022-177">Project</span></span> | <span data-ttu-id="0e022-178">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-178">Yes</span></span> | <span data-ttu-id="0e022-179">نعم </span><span class="sxs-lookup"><span data-stu-id="0e022-179">Yes</span></span> | <span data-ttu-id="0e022-180">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="0e022-180">N/A</span></span> | <span data-ttu-id="0e022-181">العمليات مع الحقول التالية غير مدعومة: **StateCode** و **BulkGenerationStatus** و **GlobalRevisionToken** و **CalendarID** و **Effort** و **EffortCompleted** و **EffortRemaining** و **Progress** و **Finish** و **TaskEarliestStart** و **Duration**.</span><span class="sxs-lookup"><span data-stu-id="0e022-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="0e022-182">يمكن استدعاء واجهات برمجة التطبيقات مع كائنات الكيانات التي تتضمن حقولاً مخصصة.</span><span class="sxs-lookup"><span data-stu-id="0e022-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="0e022-183">خاصية المعرف اختيارية.</span><span class="sxs-lookup"><span data-stu-id="0e022-183">The ID property is optional.</span></span> <span data-ttu-id="0e022-184">إذا تم توفيرها، يحاول النظام استخدامها ويلقي استثناءً إذا لم يكن من الممكن استخدامها.</span><span class="sxs-lookup"><span data-stu-id="0e022-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="0e022-185">إذا لم يتم توفيرها، سيقوم النظام بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="0e022-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="0e022-186">الحقول المقيدة</span><span class="sxs-lookup"><span data-stu-id="0e022-186">Restricted fields</span></span>

<span data-ttu-id="0e022-187">يُعرف الجداول التالي الحقول المقيدة من **الإنشاء** و **التحرير.**</span><span class="sxs-lookup"><span data-stu-id="0e022-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="0e022-188">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-188">Project task</span></span>

| <span data-ttu-id="0e022-189">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="0e022-189">**Logical name**</span></span>                       | <span data-ttu-id="0e022-190">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="0e022-190">**Can create**</span></span> | <span data-ttu-id="0e022-191">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="0e022-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="0e022-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="0e022-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="0e022-193">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-193">no</span></span>             | <span data-ttu-id="0e022-194">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-194">no</span></span>               |
| <span data-ttu-id="0e022-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="0e022-196">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-196">no</span></span>             | <span data-ttu-id="0e022-197">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-197">no</span></span>               |
| <span data-ttu-id="0e022-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="0e022-198">msdyn_actualend</span></span>                        | <span data-ttu-id="0e022-199">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-199">no</span></span>             | <span data-ttu-id="0e022-200">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-200">no</span></span>               |
| <span data-ttu-id="0e022-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="0e022-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="0e022-202">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-202">no</span></span>             | <span data-ttu-id="0e022-203">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-203">no</span></span>               |
| <span data-ttu-id="0e022-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="0e022-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="0e022-205">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-205">no</span></span>             | <span data-ttu-id="0e022-206">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-206">no</span></span>               |
| <span data-ttu-id="0e022-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="0e022-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="0e022-208">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-208">no</span></span>             | <span data-ttu-id="0e022-209">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-209">no</span></span>               |
| <span data-ttu-id="0e022-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="0e022-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="0e022-211">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-211">no</span></span>             | <span data-ttu-id="0e022-212">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-212">no</span></span>               |
| <span data-ttu-id="0e022-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="0e022-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="0e022-214">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-214">no</span></span>             | <span data-ttu-id="0e022-215">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-215">no</span></span>               |
| <span data-ttu-id="0e022-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="0e022-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="0e022-217">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-217">no</span></span>             | <span data-ttu-id="0e022-218">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-218">no</span></span>               |
| <span data-ttu-id="0e022-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="0e022-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="0e022-220">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-220">no</span></span>             | <span data-ttu-id="0e022-221">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-221">no</span></span>               |
| <span data-ttu-id="0e022-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="0e022-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="0e022-223">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-223">no</span></span>             | <span data-ttu-id="0e022-224">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-224">no</span></span>               |
| <span data-ttu-id="0e022-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="0e022-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="0e022-226">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-226">no</span></span>             | <span data-ttu-id="0e022-227">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-227">no</span></span>               |
| <span data-ttu-id="0e022-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="0e022-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="0e022-229">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-229">no</span></span>             | <span data-ttu-id="0e022-230">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-230">no</span></span>               |
| <span data-ttu-id="0e022-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="0e022-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="0e022-232">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-232">no</span></span>             | <span data-ttu-id="0e022-233">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-233">no</span></span>               |
| <span data-ttu-id="0e022-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="0e022-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="0e022-235">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-235">no</span></span>             | <span data-ttu-id="0e022-236">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-236">no</span></span>               |
| <span data-ttu-id="0e022-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="0e022-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="0e022-238">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-238">no</span></span>             | <span data-ttu-id="0e022-239">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-239">no</span></span>               |
| <span data-ttu-id="0e022-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="0e022-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="0e022-241">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-241">no</span></span>             | <span data-ttu-id="0e022-242">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-242">no</span></span>               |
| <span data-ttu-id="0e022-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="0e022-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="0e022-244">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-244">no</span></span>             | <span data-ttu-id="0e022-245">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-245">no</span></span>               |
| <span data-ttu-id="0e022-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="0e022-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="0e022-247">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-247">no</span></span>             | <span data-ttu-id="0e022-248">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-248">no</span></span>               |
| <span data-ttu-id="0e022-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="0e022-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="0e022-250">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-250">no</span></span>             | <span data-ttu-id="0e022-251">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-251">no</span></span>               |
| <span data-ttu-id="0e022-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="0e022-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="0e022-253">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-253">no</span></span>             | <span data-ttu-id="0e022-254">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-254">no</span></span>               |
| <span data-ttu-id="0e022-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="0e022-256">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-256">no</span></span>             | <span data-ttu-id="0e022-257">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-257">no</span></span>               |
| <span data-ttu-id="0e022-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="0e022-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="0e022-259">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-259">no</span></span>             | <span data-ttu-id="0e022-260">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-260">no</span></span>               |
| <span data-ttu-id="0e022-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="0e022-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="0e022-262">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-262">no</span></span>             | <span data-ttu-id="0e022-263">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-263">no</span></span>               |
| <span data-ttu-id="0e022-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="0e022-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="0e022-265">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-265">no</span></span>             | <span data-ttu-id="0e022-266">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-266">no</span></span>               |
| <span data-ttu-id="0e022-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="0e022-267">msdyn_progress</span></span>                         | <span data-ttu-id="0e022-268">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-268">no</span></span>             | <span data-ttu-id="0e022-269">لا (نعم لـ P4W)</span><span class="sxs-lookup"><span data-stu-id="0e022-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="0e022-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="0e022-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="0e022-271">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-271">no</span></span>             | <span data-ttu-id="0e022-272">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-272">no</span></span>               |
| <span data-ttu-id="0e022-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="0e022-274">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-274">no</span></span>             | <span data-ttu-id="0e022-275">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-275">no</span></span>               |
| <span data-ttu-id="0e022-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="0e022-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="0e022-277">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-277">no</span></span>             | <span data-ttu-id="0e022-278">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-278">no</span></span>               |
| <span data-ttu-id="0e022-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="0e022-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="0e022-280">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-280">no</span></span>             | <span data-ttu-id="0e022-281">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-281">no</span></span>               |
| <span data-ttu-id="0e022-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="0e022-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="0e022-283">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-283">no</span></span>             | <span data-ttu-id="0e022-284">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-284">no</span></span>               |
| <span data-ttu-id="0e022-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="0e022-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="0e022-286">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-286">no</span></span>             | <span data-ttu-id="0e022-287">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-287">no</span></span>               |
| <span data-ttu-id="0e022-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="0e022-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="0e022-289">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-289">no</span></span>             | <span data-ttu-id="0e022-290">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-290">no</span></span>               |
| <span data-ttu-id="0e022-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="0e022-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="0e022-292">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-292">no</span></span>             | <span data-ttu-id="0e022-293">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-293">no</span></span>               |
| <span data-ttu-id="0e022-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="0e022-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="0e022-295">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-295">no</span></span>             | <span data-ttu-id="0e022-296">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-296">no</span></span>               |
| <span data-ttu-id="0e022-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="0e022-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="0e022-298">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-298">no</span></span>             | <span data-ttu-id="0e022-299">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-299">no</span></span>               |
| <span data-ttu-id="0e022-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="0e022-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="0e022-301">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-301">no</span></span>             | <span data-ttu-id="0e022-302">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-302">no</span></span>               |
| <span data-ttu-id="0e022-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="0e022-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="0e022-304">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-304">no</span></span>             | <span data-ttu-id="0e022-305">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-305">no</span></span>               |
| <span data-ttu-id="0e022-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="0e022-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="0e022-307">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-307">no</span></span>             | <span data-ttu-id="0e022-308">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-308">no</span></span>               |
| <span data-ttu-id="0e022-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="0e022-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="0e022-310">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-310">no</span></span>             | <span data-ttu-id="0e022-311">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-311">no</span></span>               |
| <span data-ttu-id="0e022-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="0e022-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="0e022-313">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-313">no</span></span>             | <span data-ttu-id="0e022-314">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-314">no</span></span>               |
| <span data-ttu-id="0e022-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="0e022-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="0e022-316">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-316">no</span></span>             | <span data-ttu-id="0e022-317">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-317">no</span></span>               |
| <span data-ttu-id="0e022-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="0e022-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="0e022-319">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-319">no</span></span>             | <span data-ttu-id="0e022-320">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-320">no</span></span>               |
| <span data-ttu-id="0e022-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="0e022-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="0e022-322">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-322">no</span></span>             | <span data-ttu-id="0e022-323">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-323">no</span></span>               |
| <span data-ttu-id="0e022-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="0e022-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="0e022-325">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-325">no</span></span>             | <span data-ttu-id="0e022-326">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-326">no</span></span>               |
| <span data-ttu-id="0e022-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="0e022-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="0e022-328">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-328">no</span></span>             | <span data-ttu-id="0e022-329">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-329">no</span></span>               |
| <span data-ttu-id="0e022-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="0e022-330">msdyn_summary</span></span>                          | <span data-ttu-id="0e022-331">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-331">no</span></span>             | <span data-ttu-id="0e022-332">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-332">no</span></span>               |
| <span data-ttu-id="0e022-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="0e022-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="0e022-334">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-334">no</span></span>             | <span data-ttu-id="0e022-335">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-335">no</span></span>               |
| <span data-ttu-id="0e022-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="0e022-337">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-337">no</span></span>             | <span data-ttu-id="0e022-338">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="0e022-339">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-339">Project task dependency</span></span>

| <span data-ttu-id="0e022-340">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="0e022-340">**Logical name**</span></span>              | <span data-ttu-id="0e022-341">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="0e022-341">**Can create**</span></span> | <span data-ttu-id="0e022-342">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="0e022-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="0e022-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="0e022-343">msdyn_linktype</span></span>                | <span data-ttu-id="0e022-344">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-344">no</span></span>             | <span data-ttu-id="0e022-345">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-345">no</span></span>           |
| <span data-ttu-id="0e022-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="0e022-346">msdyn_linktypename</span></span>            | <span data-ttu-id="0e022-347">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-347">no</span></span>             | <span data-ttu-id="0e022-348">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-348">no</span></span>           |
| <span data-ttu-id="0e022-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="0e022-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="0e022-350">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-350">yes</span></span>            | <span data-ttu-id="0e022-351">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-351">no</span></span>           |
| <span data-ttu-id="0e022-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="0e022-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="0e022-353">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-353">yes</span></span>            | <span data-ttu-id="0e022-354">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-354">no</span></span>           |
| <span data-ttu-id="0e022-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="0e022-355">msdyn_project</span></span>                 | <span data-ttu-id="0e022-356">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-356">yes</span></span>            | <span data-ttu-id="0e022-357">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-357">no</span></span>           |
| <span data-ttu-id="0e022-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="0e022-358">msdyn_projectname</span></span>             | <span data-ttu-id="0e022-359">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-359">yes</span></span>            | <span data-ttu-id="0e022-360">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-360">no</span></span>           |
| <span data-ttu-id="0e022-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="0e022-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="0e022-362">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-362">yes</span></span>            | <span data-ttu-id="0e022-363">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-363">no</span></span>           |
| <span data-ttu-id="0e022-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="0e022-364">msdyn_successortask</span></span>           | <span data-ttu-id="0e022-365">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-365">yes</span></span>            | <span data-ttu-id="0e022-366">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-366">no</span></span>           |
| <span data-ttu-id="0e022-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="0e022-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="0e022-368">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-368">yes</span></span>            | <span data-ttu-id="0e022-369">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="0e022-370">تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="0e022-370">Resource assignment</span></span>

| <span data-ttu-id="0e022-371">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="0e022-371">**Logical name**</span></span>             | <span data-ttu-id="0e022-372">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="0e022-372">**Can create**</span></span> | <span data-ttu-id="0e022-373">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="0e022-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="0e022-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="0e022-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="0e022-375">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-375">yes</span></span>            | <span data-ttu-id="0e022-376">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-376">no</span></span>           |
| <span data-ttu-id="0e022-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="0e022-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="0e022-378">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-378">yes</span></span>            | <span data-ttu-id="0e022-379">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-379">no</span></span>           |
| <span data-ttu-id="0e022-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="0e022-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="0e022-381">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-381">no</span></span>             | <span data-ttu-id="0e022-382">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-382">no</span></span>           |
| <span data-ttu-id="0e022-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="0e022-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="0e022-384">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-384">no</span></span>             | <span data-ttu-id="0e022-385">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-385">no</span></span>           |
| <span data-ttu-id="0e022-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="0e022-386">msdyn_committype</span></span>             | <span data-ttu-id="0e022-387">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-387">no</span></span>             | <span data-ttu-id="0e022-388">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-388">no</span></span>           |
| <span data-ttu-id="0e022-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="0e022-389">msdyn_committypename</span></span>         | <span data-ttu-id="0e022-390">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-390">no</span></span>             | <span data-ttu-id="0e022-391">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-391">no</span></span>           |
| <span data-ttu-id="0e022-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="0e022-392">msdyn_effort</span></span>                 | <span data-ttu-id="0e022-393">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-393">no</span></span>             | <span data-ttu-id="0e022-394">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-394">no</span></span>           |
| <span data-ttu-id="0e022-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="0e022-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="0e022-396">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-396">no</span></span>             | <span data-ttu-id="0e022-397">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-397">no</span></span>           |
| <span data-ttu-id="0e022-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="0e022-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="0e022-399">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-399">no</span></span>             | <span data-ttu-id="0e022-400">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-400">no</span></span>           |
| <span data-ttu-id="0e022-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="0e022-401">msdyn_finish</span></span>                 | <span data-ttu-id="0e022-402">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-402">no</span></span>             | <span data-ttu-id="0e022-403">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-403">no</span></span>           |
| <span data-ttu-id="0e022-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="0e022-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="0e022-405">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-405">no</span></span>             | <span data-ttu-id="0e022-406">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-406">no</span></span>           |
| <span data-ttu-id="0e022-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="0e022-408">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-408">no</span></span>             | <span data-ttu-id="0e022-409">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-409">no</span></span>           |
| <span data-ttu-id="0e022-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="0e022-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="0e022-411">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-411">no</span></span>             | <span data-ttu-id="0e022-412">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-412">no</span></span>           |
| <span data-ttu-id="0e022-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="0e022-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="0e022-414">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-414">no</span></span>             | <span data-ttu-id="0e022-415">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-415">no</span></span>           |
| <span data-ttu-id="0e022-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="0e022-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="0e022-417">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-417">no</span></span>             | <span data-ttu-id="0e022-418">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-418">no</span></span>           |
| <span data-ttu-id="0e022-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="0e022-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="0e022-420">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-420">no</span></span>             | <span data-ttu-id="0e022-421">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-421">no</span></span>           |
| <span data-ttu-id="0e022-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="0e022-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="0e022-423">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-423">no</span></span>             | <span data-ttu-id="0e022-424">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-424">no</span></span>           |
| <span data-ttu-id="0e022-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="0e022-425">msdyn_projectid</span></span>              | <span data-ttu-id="0e022-426">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-426">yes</span></span>            | <span data-ttu-id="0e022-427">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-427">no</span></span>           |
| <span data-ttu-id="0e022-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="0e022-428">msdyn_projectidname</span></span>          | <span data-ttu-id="0e022-429">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-429">no</span></span>             | <span data-ttu-id="0e022-430">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-430">no</span></span>           |
| <span data-ttu-id="0e022-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="0e022-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="0e022-432">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-432">no</span></span>             | <span data-ttu-id="0e022-433">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-433">no</span></span>           |
| <span data-ttu-id="0e022-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="0e022-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="0e022-435">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-435">no</span></span>             | <span data-ttu-id="0e022-436">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-436">no</span></span>           |
| <span data-ttu-id="0e022-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="0e022-437">msdyn_start</span></span>                  | <span data-ttu-id="0e022-438">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-438">no</span></span>             | <span data-ttu-id="0e022-439">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-439">no</span></span>           |
| <span data-ttu-id="0e022-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="0e022-440">msdyn_taskid</span></span>                 | <span data-ttu-id="0e022-441">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-441">no</span></span>             | <span data-ttu-id="0e022-442">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-442">no</span></span>           |
| <span data-ttu-id="0e022-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="0e022-443">msdyn_taskidname</span></span>             | <span data-ttu-id="0e022-444">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-444">no</span></span>             | <span data-ttu-id="0e022-445">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-445">no</span></span>           |
| <span data-ttu-id="0e022-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="0e022-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="0e022-447">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-447">no</span></span>             | <span data-ttu-id="0e022-448">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="0e022-449">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="0e022-449">Project team member</span></span>

| <span data-ttu-id="0e022-450">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="0e022-450">**Logical name**</span></span>                                 | <span data-ttu-id="0e022-451">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="0e022-451">**Can create**</span></span> | <span data-ttu-id="0e022-452">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="0e022-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="0e022-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="0e022-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="0e022-454">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-454">no</span></span>             | <span data-ttu-id="0e022-455">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-455">no</span></span>           |
| <span data-ttu-id="0e022-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="0e022-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="0e022-457">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-457">no</span></span>             | <span data-ttu-id="0e022-458">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-458">no</span></span>           |
| <span data-ttu-id="0e022-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="0e022-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="0e022-460">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-460">no</span></span>             | <span data-ttu-id="0e022-461">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-461">no</span></span>           |
| <span data-ttu-id="0e022-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="0e022-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="0e022-463">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-463">no</span></span>             | <span data-ttu-id="0e022-464">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-464">no</span></span>           |
| <span data-ttu-id="0e022-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="0e022-465">msdyn_effort</span></span>                                     | <span data-ttu-id="0e022-466">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-466">no</span></span>             | <span data-ttu-id="0e022-467">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-467">no</span></span>           |
| <span data-ttu-id="0e022-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="0e022-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="0e022-469">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-469">no</span></span>             | <span data-ttu-id="0e022-470">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-470">no</span></span>           |
| <span data-ttu-id="0e022-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="0e022-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="0e022-472">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-472">no</span></span>             | <span data-ttu-id="0e022-473">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-473">no</span></span>           |
| <span data-ttu-id="0e022-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="0e022-474">msdyn_finish</span></span>                                     | <span data-ttu-id="0e022-475">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-475">no</span></span>             | <span data-ttu-id="0e022-476">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-476">no</span></span>           |
| <span data-ttu-id="0e022-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="0e022-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="0e022-478">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-478">no</span></span>             | <span data-ttu-id="0e022-479">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-479">no</span></span>           |
| <span data-ttu-id="0e022-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="0e022-480">msdyn_hours</span></span>                                      | <span data-ttu-id="0e022-481">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-481">no</span></span>             | <span data-ttu-id="0e022-482">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-482">no</span></span>           |
| <span data-ttu-id="0e022-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="0e022-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="0e022-484">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-484">no</span></span>             | <span data-ttu-id="0e022-485">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-485">no</span></span>           |
| <span data-ttu-id="0e022-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="0e022-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="0e022-487">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-487">no</span></span>             | <span data-ttu-id="0e022-488">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-488">no</span></span>           |
| <span data-ttu-id="0e022-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="0e022-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="0e022-490">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-490">no</span></span>             | <span data-ttu-id="0e022-491">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-491">no</span></span>           |
| <span data-ttu-id="0e022-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="0e022-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="0e022-493">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-493">no</span></span>             | <span data-ttu-id="0e022-494">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-494">no</span></span>           |
| <span data-ttu-id="0e022-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="0e022-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="0e022-496">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-496">no</span></span>             | <span data-ttu-id="0e022-497">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-497">no</span></span>           |
| <span data-ttu-id="0e022-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="0e022-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="0e022-499">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-499">no</span></span>             | <span data-ttu-id="0e022-500">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-500">no</span></span>           |
| <span data-ttu-id="0e022-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="0e022-501">msdyn_start</span></span>                                      | <span data-ttu-id="0e022-502">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-502">no</span></span>             | <span data-ttu-id="0e022-503">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="0e022-504">Project</span><span class="sxs-lookup"><span data-stu-id="0e022-504">Project</span></span>

| <span data-ttu-id="0e022-505">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="0e022-505">**Logical name**</span></span>                       | <span data-ttu-id="0e022-506">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="0e022-506">**Can create**</span></span> | <span data-ttu-id="0e022-507">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="0e022-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="0e022-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="0e022-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="0e022-509">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-509">no</span></span>             | <span data-ttu-id="0e022-510">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-510">no</span></span>           |
| <span data-ttu-id="0e022-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="0e022-512">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-512">no</span></span>             | <span data-ttu-id="0e022-513">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-513">no</span></span>           |
| <span data-ttu-id="0e022-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="0e022-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="0e022-515">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-515">no</span></span>             | <span data-ttu-id="0e022-516">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-516">no</span></span>           |
| <span data-ttu-id="0e022-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="0e022-518">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-518">no</span></span>             | <span data-ttu-id="0e022-519">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-519">no</span></span>           |
| <span data-ttu-id="0e022-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="0e022-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="0e022-521">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-521">no</span></span>             | <span data-ttu-id="0e022-522">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-522">no</span></span>           |
| <span data-ttu-id="0e022-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="0e022-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="0e022-524">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-524">no</span></span>             | <span data-ttu-id="0e022-525">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-525">no</span></span>           |
| <span data-ttu-id="0e022-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="0e022-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="0e022-527">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-527">yes</span></span>            | <span data-ttu-id="0e022-528">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-528">no</span></span>           |
| <span data-ttu-id="0e022-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="0e022-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="0e022-530">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-530">yes</span></span>            | <span data-ttu-id="0e022-531">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-531">no</span></span>           |
| <span data-ttu-id="0e022-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="0e022-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="0e022-533">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-533">yes</span></span>            | <span data-ttu-id="0e022-534">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-534">no</span></span>           |
| <span data-ttu-id="0e022-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="0e022-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="0e022-536">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-536">no</span></span>             | <span data-ttu-id="0e022-537">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-537">no</span></span>           |
| <span data-ttu-id="0e022-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="0e022-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="0e022-539">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-539">no</span></span>             | <span data-ttu-id="0e022-540">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-540">no</span></span>           |
| <span data-ttu-id="0e022-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="0e022-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="0e022-542">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-542">no</span></span>             | <span data-ttu-id="0e022-543">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-543">no</span></span>           |
| <span data-ttu-id="0e022-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="0e022-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="0e022-545">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-545">no</span></span>             | <span data-ttu-id="0e022-546">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-546">no</span></span>           |
| <span data-ttu-id="0e022-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="0e022-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="0e022-548">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-548">no</span></span>             | <span data-ttu-id="0e022-549">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-549">no</span></span>           |
| <span data-ttu-id="0e022-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="0e022-550">msdyn_duration</span></span>                         | <span data-ttu-id="0e022-551">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-551">no</span></span>             | <span data-ttu-id="0e022-552">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-552">no</span></span>           |
| <span data-ttu-id="0e022-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="0e022-553">msdyn_effort</span></span>                           | <span data-ttu-id="0e022-554">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-554">no</span></span>             | <span data-ttu-id="0e022-555">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-555">no</span></span>           |
| <span data-ttu-id="0e022-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="0e022-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="0e022-557">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-557">no</span></span>             | <span data-ttu-id="0e022-558">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-558">no</span></span>           |
| <span data-ttu-id="0e022-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="0e022-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="0e022-560">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-560">no</span></span>             | <span data-ttu-id="0e022-561">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-561">no</span></span>           |
| <span data-ttu-id="0e022-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="0e022-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="0e022-563">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-563">no</span></span>             | <span data-ttu-id="0e022-564">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-564">no</span></span>           |
| <span data-ttu-id="0e022-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="0e022-565">msdyn_finish</span></span>                           | <span data-ttu-id="0e022-566">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-566">yes</span></span>            | <span data-ttu-id="0e022-567">نعم</span><span class="sxs-lookup"><span data-stu-id="0e022-567">yes</span></span>          |
| <span data-ttu-id="0e022-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="0e022-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="0e022-569">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-569">no</span></span>             | <span data-ttu-id="0e022-570">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-570">no</span></span>           |
| <span data-ttu-id="0e022-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="0e022-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="0e022-572">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-572">no</span></span>             | <span data-ttu-id="0e022-573">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-573">no</span></span>           |
| <span data-ttu-id="0e022-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="0e022-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="0e022-575">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-575">no</span></span>             | <span data-ttu-id="0e022-576">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-576">no</span></span>           |
| <span data-ttu-id="0e022-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="0e022-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="0e022-578">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-578">no</span></span>             | <span data-ttu-id="0e022-579">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-579">no</span></span>           |
| <span data-ttu-id="0e022-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="0e022-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="0e022-581">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-581">no</span></span>             | <span data-ttu-id="0e022-582">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-582">no</span></span>           |
| <span data-ttu-id="0e022-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="0e022-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="0e022-584">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-584">no</span></span>             | <span data-ttu-id="0e022-585">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-585">no</span></span>           |
| <span data-ttu-id="0e022-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="0e022-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="0e022-587">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-587">no</span></span>             | <span data-ttu-id="0e022-588">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-588">no</span></span>           |
| <span data-ttu-id="0e022-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="0e022-590">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-590">no</span></span>             | <span data-ttu-id="0e022-591">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-591">no</span></span>           |
| <span data-ttu-id="0e022-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="0e022-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="0e022-593">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-593">no</span></span>             | <span data-ttu-id="0e022-594">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-594">no</span></span>           |
| <span data-ttu-id="0e022-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="0e022-596">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-596">no</span></span>             | <span data-ttu-id="0e022-597">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-597">no</span></span>           |
| <span data-ttu-id="0e022-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="0e022-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="0e022-599">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-599">no</span></span>             | <span data-ttu-id="0e022-600">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-600">no</span></span>           |
| <span data-ttu-id="0e022-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="0e022-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="0e022-602">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-602">no</span></span>             | <span data-ttu-id="0e022-603">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-603">no</span></span>           |
| <span data-ttu-id="0e022-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="0e022-604">msdyn_progress</span></span>                         | <span data-ttu-id="0e022-605">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-605">no</span></span>             | <span data-ttu-id="0e022-606">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-606">no</span></span>           |
| <span data-ttu-id="0e022-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="0e022-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="0e022-608">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-608">no</span></span>             | <span data-ttu-id="0e022-609">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-609">no</span></span>           |
| <span data-ttu-id="0e022-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="0e022-611">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-611">no</span></span>             | <span data-ttu-id="0e022-612">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-612">no</span></span>           |
| <span data-ttu-id="0e022-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="0e022-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="0e022-614">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-614">no</span></span>             | <span data-ttu-id="0e022-615">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-615">no</span></span>           |
| <span data-ttu-id="0e022-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="0e022-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="0e022-617">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-617">no</span></span>             | <span data-ttu-id="0e022-618">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-618">no</span></span>           |
| <span data-ttu-id="0e022-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="0e022-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="0e022-620">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-620">no</span></span>             | <span data-ttu-id="0e022-621">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-621">no</span></span>           |
| <span data-ttu-id="0e022-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="0e022-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="0e022-623">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-623">no</span></span>             | <span data-ttu-id="0e022-624">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-624">no</span></span>           |
| <span data-ttu-id="0e022-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="0e022-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="0e022-626">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-626">no</span></span>             | <span data-ttu-id="0e022-627">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-627">no</span></span>           |
| <span data-ttu-id="0e022-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="0e022-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="0e022-629">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-629">no</span></span>             | <span data-ttu-id="0e022-630">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-630">no</span></span>           |
| <span data-ttu-id="0e022-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="0e022-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="0e022-632">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-632">no</span></span>             | <span data-ttu-id="0e022-633">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-633">no</span></span>           |
| <span data-ttu-id="0e022-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="0e022-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="0e022-635">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-635">no</span></span>             | <span data-ttu-id="0e022-636">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-636">no</span></span>           |
| <span data-ttu-id="0e022-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="0e022-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="0e022-638">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-638">no</span></span>             | <span data-ttu-id="0e022-639">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-639">no</span></span>           |
| <span data-ttu-id="0e022-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="0e022-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="0e022-641">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-641">no</span></span>             | <span data-ttu-id="0e022-642">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-642">no</span></span>           |
| <span data-ttu-id="0e022-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="0e022-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="0e022-644">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-644">no</span></span>             | <span data-ttu-id="0e022-645">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-645">no</span></span>           |
| <span data-ttu-id="0e022-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="0e022-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="0e022-647">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-647">no</span></span>             | <span data-ttu-id="0e022-648">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-648">no</span></span>           |
| <span data-ttu-id="0e022-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="0e022-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="0e022-650">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-650">no</span></span>             | <span data-ttu-id="0e022-651">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-651">no</span></span>           |
| <span data-ttu-id="0e022-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="0e022-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="0e022-653">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-653">no</span></span>             | <span data-ttu-id="0e022-654">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-654">no</span></span>           |
| <span data-ttu-id="0e022-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="0e022-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="0e022-656">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-656">no</span></span>             | <span data-ttu-id="0e022-657">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-657">no</span></span>           |
| <span data-ttu-id="0e022-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="0e022-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="0e022-659">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-659">no</span></span>             | <span data-ttu-id="0e022-660">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-660">no</span></span>           |
| <span data-ttu-id="0e022-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="0e022-662">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-662">no</span></span>             | <span data-ttu-id="0e022-663">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-663">no</span></span>           |
| <span data-ttu-id="0e022-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="0e022-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="0e022-665">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-665">no</span></span>             | <span data-ttu-id="0e022-666">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-666">no</span></span>           |
| <span data-ttu-id="0e022-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="0e022-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="0e022-668">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-668">no</span></span>             | <span data-ttu-id="0e022-669">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="0e022-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="0e022-670">القيود والمشاكل المعروفة</span><span class="sxs-lookup"><span data-stu-id="0e022-670">Limitations and known issues</span></span>
<span data-ttu-id="0e022-671">فيما يلي قائمة بالقيود والمشاكل المعروفة:</span><span class="sxs-lookup"><span data-stu-id="0e022-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="0e022-672">يمكن استخدام واجهات برمجة تطبيقات الجدولة فقط بواسطة **المستخدمين الذين لديهم ترخيص Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="0e022-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="0e022-673">لا يمكن استخدامها بواسطة:</span><span class="sxs-lookup"><span data-stu-id="0e022-673">They can't be used by:</span></span>
    - <span data-ttu-id="0e022-674">مستخدمي التطبيق</span><span class="sxs-lookup"><span data-stu-id="0e022-674">Application users</span></span>
    - <span data-ttu-id="0e022-675">مستخدمي النظام</span><span class="sxs-lookup"><span data-stu-id="0e022-675">System users</span></span>
    - <span data-ttu-id="0e022-676">مستخدمي التكامل</span><span class="sxs-lookup"><span data-stu-id="0e022-676">Integration users</span></span>
    - <span data-ttu-id="0e022-677">المستخدمين الآخرين الذين ليس لديهم الترخيص المطلوب</span><span class="sxs-lookup"><span data-stu-id="0e022-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="0e022-678">تتضمن كل **OperationSet** مئة عملية كحدٍ أقصى.</span><span class="sxs-lookup"><span data-stu-id="0e022-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="0e022-679">بإمكان كل مستخدم أن يحصل على عشر **OperationSet** مفتوحة كحدٍ أقصى.</span><span class="sxs-lookup"><span data-stu-id="0e022-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="0e022-680">يدعم Project Operations في الوقت الحالي 500 مهمة إجمالية كحد أقصى على مشروع.</span><span class="sxs-lookup"><span data-stu-id="0e022-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="0e022-681">في الوقت الحالي، لا تتوفر حالة فشل **OperationSet** وسجلات الفشل.</span><span class="sxs-lookup"><span data-stu-id="0e022-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="0e022-682">واجهات برمجة تطبيقات الجدولة هي حاليًا في وضع الإصدار الأولي للاستخدام العام.</span><span class="sxs-lookup"><span data-stu-id="0e022-682">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="0e022-683">لا تدعم Microsoft استخدام واجهات برمجة التطبيقات هذه في بيئة الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="0e022-683">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>
- [<span data-ttu-id="0e022-684">القيود والحدود على المشروعات والمهام</span><span class="sxs-lookup"><span data-stu-id="0e022-684">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="0e022-685">معالجة الخطأ</span><span class="sxs-lookup"><span data-stu-id="0e022-685">Error handling</span></span>

   - <span data-ttu-id="0e022-686">لمراجعة الأخطاء التي تم إنشاؤها من مجموعات العمليات، انتقل إلى **الإعدادات** \> **تكامل الجدول** \> **مجموعات العمليات**.</span><span class="sxs-lookup"><span data-stu-id="0e022-686">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="0e022-687">لمراجعة الأخطاء التي تم إنشاؤها من خدمة جدولة المشروع، انتقل إلى **الإعدادات** \> **تكامل الجدول** \> **سجلات أخطاء PSS**.</span><span class="sxs-lookup"><span data-stu-id="0e022-687">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="0e022-688">سيناريو نموذجي</span><span class="sxs-lookup"><span data-stu-id="0e022-688">Sample scenario</span></span>

<span data-ttu-id="0e022-689">في هذا السيناريو، ستقوم بإنشاء مشروع، وعضو فريق، وأربع مهام، وعمليتي تعيين للموارد.</span><span class="sxs-lookup"><span data-stu-id="0e022-689">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="0e022-690">بعد ذلك، عليك تحديث مهمة واحدة وتحديث المشروع وحذف مهمة واحدة وحذف تعيين مورد واحد وإنشاء تبعية مهمة.</span><span class="sxs-lookup"><span data-stu-id="0e022-690">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="0e022-691">عينات إضافية</span><span class="sxs-lookup"><span data-stu-id="0e022-691">Additional samples</span></span>

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
