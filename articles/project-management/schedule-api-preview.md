---
title: استخدام واجهات برمجة تطبيقات الجدولة لتنفيذ عمليات مع كيانات الجدولة
description: يوفر هذا الموضوع معلومات و عينات لاستخدام واجهات برمجة تطبيقات الجدولة.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4a032dc7bcbdf23fce3c3b2ca63c51d473bd8e26
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116781"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="72baf-103">استخدام واجهات برمجة تطبيقات الجدولة لتنفيذ عمليات مع كيانات الجدولة</span><span class="sxs-lookup"><span data-stu-id="72baf-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="72baf-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="72baf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="72baf-105">تتوفر بعض الوظائف المذكورة في هذا الموضوع أو كلها كجزء من إصدار أولي.</span><span class="sxs-lookup"><span data-stu-id="72baf-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="72baf-106">إن المحتوى والوظائف خاضعة للتغيير.</span><span class="sxs-lookup"><span data-stu-id="72baf-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="72baf-107">كيانات الجدولة</span><span class="sxs-lookup"><span data-stu-id="72baf-107">Scheduling entities</span></span>

<span data-ttu-id="72baf-108">توفر واجهات برمجة تطبيقات جدولة القدرة على تنفيذ عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="72baf-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="72baf-109">تُدار هذه الكيانات من خلال محرك جدولة في المشروع للويب.</span><span class="sxs-lookup"><span data-stu-id="72baf-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="72baf-110">كانت عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة** مقيدة في إصدارات Dynamics 365 Project Operations السابقة.</span><span class="sxs-lookup"><span data-stu-id="72baf-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="72baf-111">يوفر الجدول التالي قائمة كاملة تتضمن **كيانات الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="72baf-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="72baf-112">اسم الكيان</span><span class="sxs-lookup"><span data-stu-id="72baf-112">Entity name</span></span>  | <span data-ttu-id="72baf-113">اسم منطقي للكيان</span><span class="sxs-lookup"><span data-stu-id="72baf-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="72baf-114">Project</span><span class="sxs-lookup"><span data-stu-id="72baf-114">Project</span></span> | <span data-ttu-id="72baf-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="72baf-115">msdyn_project</span></span> |
| <span data-ttu-id="72baf-116">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-116">Project Task</span></span>  | <span data-ttu-id="72baf-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="72baf-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="72baf-118">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-118">Project Task Dependency</span></span>  | <span data-ttu-id="72baf-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="72baf-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="72baf-120">تعيين المورد</span><span class="sxs-lookup"><span data-stu-id="72baf-120">Resource Assignment</span></span> | <span data-ttu-id="72baf-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="72baf-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="72baf-122">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-122">Project Bucket</span></span>  | <span data-ttu-id="72baf-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="72baf-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="72baf-124">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-124">Project Team Member</span></span> | <span data-ttu-id="72baf-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="72baf-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="72baf-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="72baf-126">OperationSet</span></span>

<span data-ttu-id="72baf-127">إن OperationSet عبارة نمط وحدة عمل يمكن استخدامه عندما يكون من الضروري معالجة طلبات متعددة تؤثر على الجدولة ضمن حركة.</span><span class="sxs-lookup"><span data-stu-id="72baf-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="72baf-128">واجهات برمجة تطبيقات الجدولة</span><span class="sxs-lookup"><span data-stu-id="72baf-128">Schedule APIs</span></span>

<span data-ttu-id="72baf-129">فيما يلي قائمة بواجهات برمجة تطبيقات الجدولة الحالية.</span><span class="sxs-lookup"><span data-stu-id="72baf-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="72baf-130">**msdyn_CreateProjectV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء مشروع.</span><span class="sxs-lookup"><span data-stu-id="72baf-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="72baf-131">يتم إنشاء مستودع المشروع والمشروع الافتراضي في الحال.</span><span class="sxs-lookup"><span data-stu-id="72baf-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="72baf-132">**msdyn_CreateTeamMemberV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء عضو فريق مشروع.</span><span class="sxs-lookup"><span data-stu-id="72baf-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="72baf-133">يتم إنشاء سجل عضو الفريق على الفور.</span><span class="sxs-lookup"><span data-stu-id="72baf-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="72baf-134">**msdyn_CreateOperationSetV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لجدولة طلبات متعددة يجب تنفيذها ضمن حركة.</span><span class="sxs-lookup"><span data-stu-id="72baf-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="72baf-135">**msdyn_PSSCreateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء كيان.</span><span class="sxs-lookup"><span data-stu-id="72baf-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="72baf-136">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية الإنشاء.</span><span class="sxs-lookup"><span data-stu-id="72baf-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="72baf-137">**msdyn_PSSUpdateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لتحديث كيان.</span><span class="sxs-lookup"><span data-stu-id="72baf-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="72baf-138">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية التحديث.</span><span class="sxs-lookup"><span data-stu-id="72baf-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="72baf-139">**msdyn_PSSDeleteV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لحذف كيان.</span><span class="sxs-lookup"><span data-stu-id="72baf-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="72baf-140">بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية الحذف.</span><span class="sxs-lookup"><span data-stu-id="72baf-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="72baf-141">**msdyn_ExecuteOperationSetV1**: يتم استخدام واجهة برمجة التطبيقات هذه لتنفيذ جميع العمليات ضمن مجموعة عمليات معينة.</span><span class="sxs-lookup"><span data-stu-id="72baf-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="72baf-142">استخدام واجهات برمجة تطبيقات لجدولة مع OperationSet</span><span class="sxs-lookup"><span data-stu-id="72baf-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="72baf-143">نظرًا لاستخدام السجلات مع كل من **CreateProjectV1** و **CreateTeamMemberV1** على الفور، لا يمكن استخدام واجهات برمجة التطبيقات هذه في **OperationSet** بشكل مباشر.</span><span class="sxs-lookup"><span data-stu-id="72baf-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="72baf-144">ومع ذلك، يمكنك استخدام واجهة برمجة التطبيقات لإنشاء السجلات المطلوبة، وإنشاء  **OperationSet**، ثم استخدام هذه السجلات المنشأة مسبقًا في **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="72baf-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="72baf-145">العمليات المدعومة</span><span class="sxs-lookup"><span data-stu-id="72baf-145">Supported operations</span></span>

| <span data-ttu-id="72baf-146">كيان الجدولة</span><span class="sxs-lookup"><span data-stu-id="72baf-146">Scheduling entity</span></span> | <span data-ttu-id="72baf-147">‏إنشاء</span><span class="sxs-lookup"><span data-stu-id="72baf-147">Create</span></span> | <span data-ttu-id="72baf-148">تحديث</span><span class="sxs-lookup"><span data-stu-id="72baf-148">Update</span></span> | <span data-ttu-id="72baf-149">حذف </span><span class="sxs-lookup"><span data-stu-id="72baf-149">Delete</span></span> | <span data-ttu-id="72baf-150">اعتبارات هامة</span><span class="sxs-lookup"><span data-stu-id="72baf-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="72baf-151">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-151">Project task</span></span> | <span data-ttu-id="72baf-152">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-152">Yes</span></span> | <span data-ttu-id="72baf-153">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-153">Yes</span></span> | <span data-ttu-id="72baf-154">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-154">Yes</span></span> | <span data-ttu-id="72baf-155">‏‫بلا</span><span class="sxs-lookup"><span data-stu-id="72baf-155">None</span></span> |
| <span data-ttu-id="72baf-156">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-156">Project task dependency</span></span> | <span data-ttu-id="72baf-157">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-157">Yes</span></span> | <span data-ttu-id="72baf-158">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-158">Yes</span></span> | | <span data-ttu-id="72baf-159">لا يتم تحديث سجلات تبعية مهمة المشروع.</span><span class="sxs-lookup"><span data-stu-id="72baf-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="72baf-160">بدلاً من ذلك، يمكن حذف سجل قديم ويمكن إنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="72baf-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="72baf-161">تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="72baf-161">Resource assignment</span></span> | <span data-ttu-id="72baf-162">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-162">Yes</span></span> | <span data-ttu-id="72baf-163">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-163">Yes</span></span> | | <span data-ttu-id="72baf-164">العمليات مع الحقول التالية غير مدعومة: **BookableResourceID** و **Effort** و **EffortCompleted** و **EffortRemaining** ة **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="72baf-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="72baf-165">لا يتم تحديث سجلات تعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="72baf-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="72baf-166">بدلاً من ذلك، يمكن حذف السجل القديم ويمكن إنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="72baf-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="72baf-167">مستودع المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-167">Project bucket</span></span> | <span data-ttu-id="72baf-168">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="72baf-168">N/A</span></span> | <span data-ttu-id="72baf-169">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="72baf-169">N/A</span></span> | <span data-ttu-id="72baf-170">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="72baf-170">N/A</span></span> | <span data-ttu-id="72baf-171">يتم إنشاء المستودع الافتراضي باستخدام واجهة برمجة التطبيقات **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="72baf-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="72baf-172">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-172">Project team member</span></span> | <span data-ttu-id="72baf-173">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-173">Yes</span></span> | <span data-ttu-id="72baf-174">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-174">Yes</span></span> | <span data-ttu-id="72baf-175">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-175">Yes</span></span> | <span data-ttu-id="72baf-176">بالنسبة لعملية الإنشاء، استخدم واجهة برمجة التطبيقات **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="72baf-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="72baf-177">Project</span><span class="sxs-lookup"><span data-stu-id="72baf-177">Project</span></span> | <span data-ttu-id="72baf-178">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-178">Yes</span></span> | <span data-ttu-id="72baf-179">نعم </span><span class="sxs-lookup"><span data-stu-id="72baf-179">Yes</span></span> | <span data-ttu-id="72baf-180">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="72baf-180">N/A</span></span> | <span data-ttu-id="72baf-181">العمليات مع الحقول التالية غير مدعومة: **StateCode** و **BulkGenerationStatus** و **GlobalRevisionToken** و **CalendarID** و **Effort** و **EffortCompleted** و **EffortRemaining** و **Progress** و **Finish** و **TaskEarliestStart** و **Duration**.</span><span class="sxs-lookup"><span data-stu-id="72baf-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="72baf-182">يمكن استدعاء واجهات برمجة التطبيقات مع كائنات الكيانات التي تتضمن حقولاً مخصصة.</span><span class="sxs-lookup"><span data-stu-id="72baf-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="72baf-183">خاصية المعرف اختيارية.</span><span class="sxs-lookup"><span data-stu-id="72baf-183">The ID property is optional.</span></span> <span data-ttu-id="72baf-184">إذا تم توفيرها، يحاول النظام استخدامها ويلقي استثناءً إذا لم يكن من الممكن استخدامها.</span><span class="sxs-lookup"><span data-stu-id="72baf-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="72baf-185">إذا لم يتم توفيرها، سيقوم النظام بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="72baf-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="72baf-186">الحقول المقيدة</span><span class="sxs-lookup"><span data-stu-id="72baf-186">Restricted fields</span></span>

<span data-ttu-id="72baf-187">يُعرف الجداول التالي الحقول المقيدة من **الإنشاء** و **التحرير.**</span><span class="sxs-lookup"><span data-stu-id="72baf-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="72baf-188">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-188">Project task</span></span>

| <span data-ttu-id="72baf-189">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="72baf-189">**Logical name**</span></span>                       | <span data-ttu-id="72baf-190">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="72baf-190">**Can create**</span></span> | <span data-ttu-id="72baf-191">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="72baf-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="72baf-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="72baf-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="72baf-193">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-193">no</span></span>             | <span data-ttu-id="72baf-194">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-194">no</span></span>               |
| <span data-ttu-id="72baf-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="72baf-196">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-196">no</span></span>             | <span data-ttu-id="72baf-197">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-197">no</span></span>               |
| <span data-ttu-id="72baf-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="72baf-198">msdyn_actualend</span></span>                        | <span data-ttu-id="72baf-199">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-199">no</span></span>             | <span data-ttu-id="72baf-200">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-200">no</span></span>               |
| <span data-ttu-id="72baf-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="72baf-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="72baf-202">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-202">no</span></span>             | <span data-ttu-id="72baf-203">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-203">no</span></span>               |
| <span data-ttu-id="72baf-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="72baf-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="72baf-205">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-205">no</span></span>             | <span data-ttu-id="72baf-206">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-206">no</span></span>               |
| <span data-ttu-id="72baf-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="72baf-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="72baf-208">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-208">no</span></span>             | <span data-ttu-id="72baf-209">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-209">no</span></span>               |
| <span data-ttu-id="72baf-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="72baf-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="72baf-211">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-211">no</span></span>             | <span data-ttu-id="72baf-212">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-212">no</span></span>               |
| <span data-ttu-id="72baf-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="72baf-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="72baf-214">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-214">no</span></span>             | <span data-ttu-id="72baf-215">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-215">no</span></span>               |
| <span data-ttu-id="72baf-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="72baf-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="72baf-217">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-217">no</span></span>             | <span data-ttu-id="72baf-218">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-218">no</span></span>               |
| <span data-ttu-id="72baf-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="72baf-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="72baf-220">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-220">no</span></span>             | <span data-ttu-id="72baf-221">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-221">no</span></span>               |
| <span data-ttu-id="72baf-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="72baf-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="72baf-223">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-223">no</span></span>             | <span data-ttu-id="72baf-224">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-224">no</span></span>               |
| <span data-ttu-id="72baf-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="72baf-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="72baf-226">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-226">no</span></span>             | <span data-ttu-id="72baf-227">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-227">no</span></span>               |
| <span data-ttu-id="72baf-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="72baf-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="72baf-229">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-229">no</span></span>             | <span data-ttu-id="72baf-230">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-230">no</span></span>               |
| <span data-ttu-id="72baf-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="72baf-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="72baf-232">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-232">no</span></span>             | <span data-ttu-id="72baf-233">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-233">no</span></span>               |
| <span data-ttu-id="72baf-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="72baf-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="72baf-235">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-235">no</span></span>             | <span data-ttu-id="72baf-236">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-236">no</span></span>               |
| <span data-ttu-id="72baf-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="72baf-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="72baf-238">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-238">no</span></span>             | <span data-ttu-id="72baf-239">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-239">no</span></span>               |
| <span data-ttu-id="72baf-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="72baf-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="72baf-241">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-241">no</span></span>             | <span data-ttu-id="72baf-242">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-242">no</span></span>               |
| <span data-ttu-id="72baf-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="72baf-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="72baf-244">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-244">no</span></span>             | <span data-ttu-id="72baf-245">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-245">no</span></span>               |
| <span data-ttu-id="72baf-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="72baf-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="72baf-247">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-247">no</span></span>             | <span data-ttu-id="72baf-248">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-248">no</span></span>               |
| <span data-ttu-id="72baf-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="72baf-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="72baf-250">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-250">no</span></span>             | <span data-ttu-id="72baf-251">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-251">no</span></span>               |
| <span data-ttu-id="72baf-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="72baf-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="72baf-253">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-253">no</span></span>             | <span data-ttu-id="72baf-254">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-254">no</span></span>               |
| <span data-ttu-id="72baf-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="72baf-256">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-256">no</span></span>             | <span data-ttu-id="72baf-257">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-257">no</span></span>               |
| <span data-ttu-id="72baf-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="72baf-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="72baf-259">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-259">no</span></span>             | <span data-ttu-id="72baf-260">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-260">no</span></span>               |
| <span data-ttu-id="72baf-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="72baf-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="72baf-262">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-262">no</span></span>             | <span data-ttu-id="72baf-263">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-263">no</span></span>               |
| <span data-ttu-id="72baf-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="72baf-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="72baf-265">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-265">no</span></span>             | <span data-ttu-id="72baf-266">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-266">no</span></span>               |
| <span data-ttu-id="72baf-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="72baf-267">msdyn_progress</span></span>                         | <span data-ttu-id="72baf-268">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-268">no</span></span>             | <span data-ttu-id="72baf-269">لا (نعم لـ P4W)</span><span class="sxs-lookup"><span data-stu-id="72baf-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="72baf-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="72baf-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="72baf-271">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-271">no</span></span>             | <span data-ttu-id="72baf-272">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-272">no</span></span>               |
| <span data-ttu-id="72baf-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="72baf-274">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-274">no</span></span>             | <span data-ttu-id="72baf-275">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-275">no</span></span>               |
| <span data-ttu-id="72baf-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="72baf-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="72baf-277">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-277">no</span></span>             | <span data-ttu-id="72baf-278">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-278">no</span></span>               |
| <span data-ttu-id="72baf-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="72baf-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="72baf-280">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-280">no</span></span>             | <span data-ttu-id="72baf-281">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-281">no</span></span>               |
| <span data-ttu-id="72baf-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="72baf-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="72baf-283">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-283">no</span></span>             | <span data-ttu-id="72baf-284">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-284">no</span></span>               |
| <span data-ttu-id="72baf-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="72baf-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="72baf-286">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-286">no</span></span>             | <span data-ttu-id="72baf-287">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-287">no</span></span>               |
| <span data-ttu-id="72baf-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="72baf-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="72baf-289">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-289">no</span></span>             | <span data-ttu-id="72baf-290">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-290">no</span></span>               |
| <span data-ttu-id="72baf-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="72baf-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="72baf-292">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-292">no</span></span>             | <span data-ttu-id="72baf-293">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-293">no</span></span>               |
| <span data-ttu-id="72baf-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="72baf-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="72baf-295">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-295">no</span></span>             | <span data-ttu-id="72baf-296">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-296">no</span></span>               |
| <span data-ttu-id="72baf-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="72baf-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="72baf-298">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-298">no</span></span>             | <span data-ttu-id="72baf-299">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-299">no</span></span>               |
| <span data-ttu-id="72baf-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="72baf-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="72baf-301">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-301">no</span></span>             | <span data-ttu-id="72baf-302">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-302">no</span></span>               |
| <span data-ttu-id="72baf-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="72baf-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="72baf-304">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-304">no</span></span>             | <span data-ttu-id="72baf-305">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-305">no</span></span>               |
| <span data-ttu-id="72baf-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="72baf-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="72baf-307">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-307">no</span></span>             | <span data-ttu-id="72baf-308">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-308">no</span></span>               |
| <span data-ttu-id="72baf-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="72baf-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="72baf-310">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-310">no</span></span>             | <span data-ttu-id="72baf-311">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-311">no</span></span>               |
| <span data-ttu-id="72baf-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="72baf-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="72baf-313">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-313">no</span></span>             | <span data-ttu-id="72baf-314">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-314">no</span></span>               |
| <span data-ttu-id="72baf-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="72baf-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="72baf-316">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-316">no</span></span>             | <span data-ttu-id="72baf-317">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-317">no</span></span>               |
| <span data-ttu-id="72baf-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="72baf-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="72baf-319">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-319">no</span></span>             | <span data-ttu-id="72baf-320">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-320">no</span></span>               |
| <span data-ttu-id="72baf-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="72baf-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="72baf-322">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-322">no</span></span>             | <span data-ttu-id="72baf-323">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-323">no</span></span>               |
| <span data-ttu-id="72baf-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="72baf-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="72baf-325">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-325">no</span></span>             | <span data-ttu-id="72baf-326">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-326">no</span></span>               |
| <span data-ttu-id="72baf-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="72baf-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="72baf-328">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-328">no</span></span>             | <span data-ttu-id="72baf-329">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-329">no</span></span>               |
| <span data-ttu-id="72baf-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="72baf-330">msdyn_summary</span></span>                          | <span data-ttu-id="72baf-331">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-331">no</span></span>             | <span data-ttu-id="72baf-332">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-332">no</span></span>               |
| <span data-ttu-id="72baf-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="72baf-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="72baf-334">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-334">no</span></span>             | <span data-ttu-id="72baf-335">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-335">no</span></span>               |
| <span data-ttu-id="72baf-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="72baf-337">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-337">no</span></span>             | <span data-ttu-id="72baf-338">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="72baf-339">تبعية مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-339">Project task dependency</span></span>

| <span data-ttu-id="72baf-340">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="72baf-340">**Logical name**</span></span>              | <span data-ttu-id="72baf-341">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="72baf-341">**Can create**</span></span> | <span data-ttu-id="72baf-342">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="72baf-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="72baf-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="72baf-343">msdyn_linktype</span></span>                | <span data-ttu-id="72baf-344">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-344">no</span></span>             | <span data-ttu-id="72baf-345">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-345">no</span></span>           |
| <span data-ttu-id="72baf-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="72baf-346">msdyn_linktypename</span></span>            | <span data-ttu-id="72baf-347">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-347">no</span></span>             | <span data-ttu-id="72baf-348">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-348">no</span></span>           |
| <span data-ttu-id="72baf-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="72baf-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="72baf-350">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-350">yes</span></span>            | <span data-ttu-id="72baf-351">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-351">no</span></span>           |
| <span data-ttu-id="72baf-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="72baf-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="72baf-353">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-353">yes</span></span>            | <span data-ttu-id="72baf-354">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-354">no</span></span>           |
| <span data-ttu-id="72baf-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="72baf-355">msdyn_project</span></span>                 | <span data-ttu-id="72baf-356">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-356">yes</span></span>            | <span data-ttu-id="72baf-357">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-357">no</span></span>           |
| <span data-ttu-id="72baf-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="72baf-358">msdyn_projectname</span></span>             | <span data-ttu-id="72baf-359">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-359">yes</span></span>            | <span data-ttu-id="72baf-360">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-360">no</span></span>           |
| <span data-ttu-id="72baf-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="72baf-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="72baf-362">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-362">yes</span></span>            | <span data-ttu-id="72baf-363">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-363">no</span></span>           |
| <span data-ttu-id="72baf-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="72baf-364">msdyn_successortask</span></span>           | <span data-ttu-id="72baf-365">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-365">yes</span></span>            | <span data-ttu-id="72baf-366">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-366">no</span></span>           |
| <span data-ttu-id="72baf-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="72baf-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="72baf-368">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-368">yes</span></span>            | <span data-ttu-id="72baf-369">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="72baf-370">تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="72baf-370">Resource assignment</span></span>

| <span data-ttu-id="72baf-371">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="72baf-371">**Logical name**</span></span>             | <span data-ttu-id="72baf-372">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="72baf-372">**Can create**</span></span> | <span data-ttu-id="72baf-373">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="72baf-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="72baf-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="72baf-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="72baf-375">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-375">yes</span></span>            | <span data-ttu-id="72baf-376">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-376">no</span></span>           |
| <span data-ttu-id="72baf-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="72baf-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="72baf-378">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-378">yes</span></span>            | <span data-ttu-id="72baf-379">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-379">no</span></span>           |
| <span data-ttu-id="72baf-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="72baf-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="72baf-381">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-381">no</span></span>             | <span data-ttu-id="72baf-382">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-382">no</span></span>           |
| <span data-ttu-id="72baf-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="72baf-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="72baf-384">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-384">no</span></span>             | <span data-ttu-id="72baf-385">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-385">no</span></span>           |
| <span data-ttu-id="72baf-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="72baf-386">msdyn_committype</span></span>             | <span data-ttu-id="72baf-387">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-387">no</span></span>             | <span data-ttu-id="72baf-388">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-388">no</span></span>           |
| <span data-ttu-id="72baf-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="72baf-389">msdyn_committypename</span></span>         | <span data-ttu-id="72baf-390">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-390">no</span></span>             | <span data-ttu-id="72baf-391">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-391">no</span></span>           |
| <span data-ttu-id="72baf-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="72baf-392">msdyn_effort</span></span>                 | <span data-ttu-id="72baf-393">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-393">no</span></span>             | <span data-ttu-id="72baf-394">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-394">no</span></span>           |
| <span data-ttu-id="72baf-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="72baf-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="72baf-396">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-396">no</span></span>             | <span data-ttu-id="72baf-397">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-397">no</span></span>           |
| <span data-ttu-id="72baf-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="72baf-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="72baf-399">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-399">no</span></span>             | <span data-ttu-id="72baf-400">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-400">no</span></span>           |
| <span data-ttu-id="72baf-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="72baf-401">msdyn_finish</span></span>                 | <span data-ttu-id="72baf-402">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-402">no</span></span>             | <span data-ttu-id="72baf-403">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-403">no</span></span>           |
| <span data-ttu-id="72baf-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="72baf-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="72baf-405">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-405">no</span></span>             | <span data-ttu-id="72baf-406">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-406">no</span></span>           |
| <span data-ttu-id="72baf-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="72baf-408">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-408">no</span></span>             | <span data-ttu-id="72baf-409">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-409">no</span></span>           |
| <span data-ttu-id="72baf-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="72baf-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="72baf-411">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-411">no</span></span>             | <span data-ttu-id="72baf-412">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-412">no</span></span>           |
| <span data-ttu-id="72baf-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="72baf-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="72baf-414">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-414">no</span></span>             | <span data-ttu-id="72baf-415">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-415">no</span></span>           |
| <span data-ttu-id="72baf-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="72baf-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="72baf-417">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-417">no</span></span>             | <span data-ttu-id="72baf-418">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-418">no</span></span>           |
| <span data-ttu-id="72baf-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="72baf-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="72baf-420">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-420">no</span></span>             | <span data-ttu-id="72baf-421">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-421">no</span></span>           |
| <span data-ttu-id="72baf-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="72baf-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="72baf-423">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-423">no</span></span>             | <span data-ttu-id="72baf-424">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-424">no</span></span>           |
| <span data-ttu-id="72baf-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="72baf-425">msdyn_projectid</span></span>              | <span data-ttu-id="72baf-426">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-426">yes</span></span>            | <span data-ttu-id="72baf-427">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-427">no</span></span>           |
| <span data-ttu-id="72baf-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="72baf-428">msdyn_projectidname</span></span>          | <span data-ttu-id="72baf-429">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-429">no</span></span>             | <span data-ttu-id="72baf-430">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-430">no</span></span>           |
| <span data-ttu-id="72baf-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="72baf-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="72baf-432">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-432">no</span></span>             | <span data-ttu-id="72baf-433">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-433">no</span></span>           |
| <span data-ttu-id="72baf-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="72baf-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="72baf-435">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-435">no</span></span>             | <span data-ttu-id="72baf-436">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-436">no</span></span>           |
| <span data-ttu-id="72baf-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="72baf-437">msdyn_start</span></span>                  | <span data-ttu-id="72baf-438">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-438">no</span></span>             | <span data-ttu-id="72baf-439">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-439">no</span></span>           |
| <span data-ttu-id="72baf-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="72baf-440">msdyn_taskid</span></span>                 | <span data-ttu-id="72baf-441">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-441">no</span></span>             | <span data-ttu-id="72baf-442">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-442">no</span></span>           |
| <span data-ttu-id="72baf-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="72baf-443">msdyn_taskidname</span></span>             | <span data-ttu-id="72baf-444">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-444">no</span></span>             | <span data-ttu-id="72baf-445">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-445">no</span></span>           |
| <span data-ttu-id="72baf-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="72baf-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="72baf-447">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-447">no</span></span>             | <span data-ttu-id="72baf-448">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="72baf-449">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="72baf-449">Project team member</span></span>

| <span data-ttu-id="72baf-450">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="72baf-450">**Logical name**</span></span>                                 | <span data-ttu-id="72baf-451">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="72baf-451">**Can create**</span></span> | <span data-ttu-id="72baf-452">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="72baf-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="72baf-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="72baf-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="72baf-454">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-454">no</span></span>             | <span data-ttu-id="72baf-455">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-455">no</span></span>           |
| <span data-ttu-id="72baf-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="72baf-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="72baf-457">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-457">no</span></span>             | <span data-ttu-id="72baf-458">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-458">no</span></span>           |
| <span data-ttu-id="72baf-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="72baf-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="72baf-460">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-460">no</span></span>             | <span data-ttu-id="72baf-461">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-461">no</span></span>           |
| <span data-ttu-id="72baf-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="72baf-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="72baf-463">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-463">no</span></span>             | <span data-ttu-id="72baf-464">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-464">no</span></span>           |
| <span data-ttu-id="72baf-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="72baf-465">msdyn_effort</span></span>                                     | <span data-ttu-id="72baf-466">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-466">no</span></span>             | <span data-ttu-id="72baf-467">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-467">no</span></span>           |
| <span data-ttu-id="72baf-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="72baf-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="72baf-469">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-469">no</span></span>             | <span data-ttu-id="72baf-470">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-470">no</span></span>           |
| <span data-ttu-id="72baf-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="72baf-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="72baf-472">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-472">no</span></span>             | <span data-ttu-id="72baf-473">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-473">no</span></span>           |
| <span data-ttu-id="72baf-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="72baf-474">msdyn_finish</span></span>                                     | <span data-ttu-id="72baf-475">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-475">no</span></span>             | <span data-ttu-id="72baf-476">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-476">no</span></span>           |
| <span data-ttu-id="72baf-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="72baf-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="72baf-478">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-478">no</span></span>             | <span data-ttu-id="72baf-479">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-479">no</span></span>           |
| <span data-ttu-id="72baf-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="72baf-480">msdyn_hours</span></span>                                      | <span data-ttu-id="72baf-481">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-481">no</span></span>             | <span data-ttu-id="72baf-482">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-482">no</span></span>           |
| <span data-ttu-id="72baf-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="72baf-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="72baf-484">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-484">no</span></span>             | <span data-ttu-id="72baf-485">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-485">no</span></span>           |
| <span data-ttu-id="72baf-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="72baf-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="72baf-487">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-487">no</span></span>             | <span data-ttu-id="72baf-488">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-488">no</span></span>           |
| <span data-ttu-id="72baf-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="72baf-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="72baf-490">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-490">no</span></span>             | <span data-ttu-id="72baf-491">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-491">no</span></span>           |
| <span data-ttu-id="72baf-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="72baf-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="72baf-493">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-493">no</span></span>             | <span data-ttu-id="72baf-494">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-494">no</span></span>           |
| <span data-ttu-id="72baf-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="72baf-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="72baf-496">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-496">no</span></span>             | <span data-ttu-id="72baf-497">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-497">no</span></span>           |
| <span data-ttu-id="72baf-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="72baf-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="72baf-499">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-499">no</span></span>             | <span data-ttu-id="72baf-500">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-500">no</span></span>           |
| <span data-ttu-id="72baf-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="72baf-501">msdyn_start</span></span>                                      | <span data-ttu-id="72baf-502">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-502">no</span></span>             | <span data-ttu-id="72baf-503">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="72baf-504">Project</span><span class="sxs-lookup"><span data-stu-id="72baf-504">Project</span></span>

| <span data-ttu-id="72baf-505">**الاسم المنطقي**</span><span class="sxs-lookup"><span data-stu-id="72baf-505">**Logical name**</span></span>                       | <span data-ttu-id="72baf-506">**يمكن الإنشاء**</span><span class="sxs-lookup"><span data-stu-id="72baf-506">**Can create**</span></span> | <span data-ttu-id="72baf-507">**يمكنه التحرير**</span><span class="sxs-lookup"><span data-stu-id="72baf-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="72baf-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="72baf-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="72baf-509">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-509">no</span></span>             | <span data-ttu-id="72baf-510">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-510">no</span></span>           |
| <span data-ttu-id="72baf-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="72baf-512">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-512">no</span></span>             | <span data-ttu-id="72baf-513">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-513">no</span></span>           |
| <span data-ttu-id="72baf-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="72baf-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="72baf-515">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-515">no</span></span>             | <span data-ttu-id="72baf-516">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-516">no</span></span>           |
| <span data-ttu-id="72baf-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="72baf-518">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-518">no</span></span>             | <span data-ttu-id="72baf-519">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-519">no</span></span>           |
| <span data-ttu-id="72baf-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="72baf-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="72baf-521">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-521">no</span></span>             | <span data-ttu-id="72baf-522">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-522">no</span></span>           |
| <span data-ttu-id="72baf-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="72baf-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="72baf-524">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-524">no</span></span>             | <span data-ttu-id="72baf-525">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-525">no</span></span>           |
| <span data-ttu-id="72baf-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="72baf-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="72baf-527">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-527">yes</span></span>            | <span data-ttu-id="72baf-528">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-528">no</span></span>           |
| <span data-ttu-id="72baf-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="72baf-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="72baf-530">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-530">yes</span></span>            | <span data-ttu-id="72baf-531">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-531">no</span></span>           |
| <span data-ttu-id="72baf-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="72baf-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="72baf-533">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-533">yes</span></span>            | <span data-ttu-id="72baf-534">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-534">no</span></span>           |
| <span data-ttu-id="72baf-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="72baf-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="72baf-536">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-536">no</span></span>             | <span data-ttu-id="72baf-537">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-537">no</span></span>           |
| <span data-ttu-id="72baf-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="72baf-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="72baf-539">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-539">no</span></span>             | <span data-ttu-id="72baf-540">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-540">no</span></span>           |
| <span data-ttu-id="72baf-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="72baf-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="72baf-542">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-542">no</span></span>             | <span data-ttu-id="72baf-543">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-543">no</span></span>           |
| <span data-ttu-id="72baf-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="72baf-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="72baf-545">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-545">no</span></span>             | <span data-ttu-id="72baf-546">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-546">no</span></span>           |
| <span data-ttu-id="72baf-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="72baf-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="72baf-548">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-548">no</span></span>             | <span data-ttu-id="72baf-549">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-549">no</span></span>           |
| <span data-ttu-id="72baf-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="72baf-550">msdyn_duration</span></span>                         | <span data-ttu-id="72baf-551">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-551">no</span></span>             | <span data-ttu-id="72baf-552">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-552">no</span></span>           |
| <span data-ttu-id="72baf-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="72baf-553">msdyn_effort</span></span>                           | <span data-ttu-id="72baf-554">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-554">no</span></span>             | <span data-ttu-id="72baf-555">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-555">no</span></span>           |
| <span data-ttu-id="72baf-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="72baf-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="72baf-557">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-557">no</span></span>             | <span data-ttu-id="72baf-558">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-558">no</span></span>           |
| <span data-ttu-id="72baf-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="72baf-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="72baf-560">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-560">no</span></span>             | <span data-ttu-id="72baf-561">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-561">no</span></span>           |
| <span data-ttu-id="72baf-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="72baf-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="72baf-563">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-563">no</span></span>             | <span data-ttu-id="72baf-564">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-564">no</span></span>           |
| <span data-ttu-id="72baf-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="72baf-565">msdyn_finish</span></span>                           | <span data-ttu-id="72baf-566">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-566">yes</span></span>            | <span data-ttu-id="72baf-567">نعم</span><span class="sxs-lookup"><span data-stu-id="72baf-567">yes</span></span>          |
| <span data-ttu-id="72baf-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="72baf-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="72baf-569">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-569">no</span></span>             | <span data-ttu-id="72baf-570">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-570">no</span></span>           |
| <span data-ttu-id="72baf-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="72baf-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="72baf-572">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-572">no</span></span>             | <span data-ttu-id="72baf-573">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-573">no</span></span>           |
| <span data-ttu-id="72baf-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="72baf-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="72baf-575">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-575">no</span></span>             | <span data-ttu-id="72baf-576">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-576">no</span></span>           |
| <span data-ttu-id="72baf-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="72baf-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="72baf-578">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-578">no</span></span>             | <span data-ttu-id="72baf-579">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-579">no</span></span>           |
| <span data-ttu-id="72baf-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="72baf-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="72baf-581">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-581">no</span></span>             | <span data-ttu-id="72baf-582">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-582">no</span></span>           |
| <span data-ttu-id="72baf-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="72baf-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="72baf-584">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-584">no</span></span>             | <span data-ttu-id="72baf-585">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-585">no</span></span>           |
| <span data-ttu-id="72baf-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="72baf-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="72baf-587">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-587">no</span></span>             | <span data-ttu-id="72baf-588">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-588">no</span></span>           |
| <span data-ttu-id="72baf-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="72baf-590">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-590">no</span></span>             | <span data-ttu-id="72baf-591">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-591">no</span></span>           |
| <span data-ttu-id="72baf-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="72baf-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="72baf-593">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-593">no</span></span>             | <span data-ttu-id="72baf-594">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-594">no</span></span>           |
| <span data-ttu-id="72baf-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="72baf-596">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-596">no</span></span>             | <span data-ttu-id="72baf-597">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-597">no</span></span>           |
| <span data-ttu-id="72baf-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="72baf-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="72baf-599">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-599">no</span></span>             | <span data-ttu-id="72baf-600">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-600">no</span></span>           |
| <span data-ttu-id="72baf-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="72baf-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="72baf-602">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-602">no</span></span>             | <span data-ttu-id="72baf-603">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-603">no</span></span>           |
| <span data-ttu-id="72baf-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="72baf-604">msdyn_progress</span></span>                         | <span data-ttu-id="72baf-605">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-605">no</span></span>             | <span data-ttu-id="72baf-606">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-606">no</span></span>           |
| <span data-ttu-id="72baf-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="72baf-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="72baf-608">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-608">no</span></span>             | <span data-ttu-id="72baf-609">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-609">no</span></span>           |
| <span data-ttu-id="72baf-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="72baf-611">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-611">no</span></span>             | <span data-ttu-id="72baf-612">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-612">no</span></span>           |
| <span data-ttu-id="72baf-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="72baf-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="72baf-614">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-614">no</span></span>             | <span data-ttu-id="72baf-615">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-615">no</span></span>           |
| <span data-ttu-id="72baf-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="72baf-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="72baf-617">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-617">no</span></span>             | <span data-ttu-id="72baf-618">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-618">no</span></span>           |
| <span data-ttu-id="72baf-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="72baf-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="72baf-620">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-620">no</span></span>             | <span data-ttu-id="72baf-621">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-621">no</span></span>           |
| <span data-ttu-id="72baf-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="72baf-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="72baf-623">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-623">no</span></span>             | <span data-ttu-id="72baf-624">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-624">no</span></span>           |
| <span data-ttu-id="72baf-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="72baf-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="72baf-626">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-626">no</span></span>             | <span data-ttu-id="72baf-627">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-627">no</span></span>           |
| <span data-ttu-id="72baf-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="72baf-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="72baf-629">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-629">no</span></span>             | <span data-ttu-id="72baf-630">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-630">no</span></span>           |
| <span data-ttu-id="72baf-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="72baf-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="72baf-632">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-632">no</span></span>             | <span data-ttu-id="72baf-633">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-633">no</span></span>           |
| <span data-ttu-id="72baf-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="72baf-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="72baf-635">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-635">no</span></span>             | <span data-ttu-id="72baf-636">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-636">no</span></span>           |
| <span data-ttu-id="72baf-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="72baf-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="72baf-638">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-638">no</span></span>             | <span data-ttu-id="72baf-639">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-639">no</span></span>           |
| <span data-ttu-id="72baf-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="72baf-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="72baf-641">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-641">no</span></span>             | <span data-ttu-id="72baf-642">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-642">no</span></span>           |
| <span data-ttu-id="72baf-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="72baf-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="72baf-644">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-644">no</span></span>             | <span data-ttu-id="72baf-645">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-645">no</span></span>           |
| <span data-ttu-id="72baf-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="72baf-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="72baf-647">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-647">no</span></span>             | <span data-ttu-id="72baf-648">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-648">no</span></span>           |
| <span data-ttu-id="72baf-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="72baf-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="72baf-650">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-650">no</span></span>             | <span data-ttu-id="72baf-651">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-651">no</span></span>           |
| <span data-ttu-id="72baf-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="72baf-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="72baf-653">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-653">no</span></span>             | <span data-ttu-id="72baf-654">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-654">no</span></span>           |
| <span data-ttu-id="72baf-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="72baf-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="72baf-656">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-656">no</span></span>             | <span data-ttu-id="72baf-657">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-657">no</span></span>           |
| <span data-ttu-id="72baf-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="72baf-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="72baf-659">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-659">no</span></span>             | <span data-ttu-id="72baf-660">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-660">no</span></span>           |
| <span data-ttu-id="72baf-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="72baf-662">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-662">no</span></span>             | <span data-ttu-id="72baf-663">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-663">no</span></span>           |
| <span data-ttu-id="72baf-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="72baf-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="72baf-665">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-665">no</span></span>             | <span data-ttu-id="72baf-666">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-666">no</span></span>           |
| <span data-ttu-id="72baf-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="72baf-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="72baf-668">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-668">no</span></span>             | <span data-ttu-id="72baf-669">‏‏لا</span><span class="sxs-lookup"><span data-stu-id="72baf-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="72baf-670">القيود والمشاكل المعروفة</span><span class="sxs-lookup"><span data-stu-id="72baf-670">Limitations and known issues</span></span>
<span data-ttu-id="72baf-671">فيما يلي قائمة بالقيود والمشاكل المعروفة:</span><span class="sxs-lookup"><span data-stu-id="72baf-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="72baf-672">يمكن استخدام واجهات برمجة تطبيقات الجدولة فقط بواسطة **المستخدمين الذين لديهم ترخيص Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="72baf-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="72baf-673">لا يمكن استخدامها بواسطة:</span><span class="sxs-lookup"><span data-stu-id="72baf-673">They can't be used by:</span></span>
    - <span data-ttu-id="72baf-674">مستخدمي التطبيق</span><span class="sxs-lookup"><span data-stu-id="72baf-674">Application users</span></span>
    - <span data-ttu-id="72baf-675">مستخدمي النظام</span><span class="sxs-lookup"><span data-stu-id="72baf-675">System users</span></span>
    - <span data-ttu-id="72baf-676">مستخدمي التكامل</span><span class="sxs-lookup"><span data-stu-id="72baf-676">Integration users</span></span>
    - <span data-ttu-id="72baf-677">المستخدمين الآخرين الذين ليس لديهم الترخيص المطلوب</span><span class="sxs-lookup"><span data-stu-id="72baf-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="72baf-678">تتضمن كل **OperationSet** مئة عملية كحدٍ أقصى.</span><span class="sxs-lookup"><span data-stu-id="72baf-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="72baf-679">بإمكان كل مستخدم أن يحصل على عشر **OperationSet** مفتوحة كحدٍ أقصى.</span><span class="sxs-lookup"><span data-stu-id="72baf-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="72baf-680">يدعم Project Operations في الوقت الحالي 500 مهمة إجمالية كحد أقصى على مشروع.</span><span class="sxs-lookup"><span data-stu-id="72baf-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="72baf-681">في الوقت الحالي، لا تتوفر حالة فشل **OperationSet** وسجلات الفشل.</span><span class="sxs-lookup"><span data-stu-id="72baf-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="72baf-682">القيود والحدود على المشروعات والمهام</span><span class="sxs-lookup"><span data-stu-id="72baf-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="72baf-683">معالجة الخطأ</span><span class="sxs-lookup"><span data-stu-id="72baf-683">Error handling</span></span>

   - <span data-ttu-id="72baf-684">لمراجعة الأخطاء التي تم إنشاؤها من مجموعات العمليات، انتقل إلى **الإعدادات** \> **تكامل الجدول** \> **مجموعات العمليات**.</span><span class="sxs-lookup"><span data-stu-id="72baf-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="72baf-685">لمراجعة الأخطاء التي تم إنشاؤها من خدمة جدولة المشروع، انتقل إلى **الإعدادات** \> **تكامل الجدول** \> **سجلات أخطاء PSS**.</span><span class="sxs-lookup"><span data-stu-id="72baf-685">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="72baf-686">سيناريو نموذجي</span><span class="sxs-lookup"><span data-stu-id="72baf-686">Sample scenario</span></span>

<span data-ttu-id="72baf-687">في هذا السيناريو، ستقوم بإنشاء مشروع، وعضو فريق، وأربع مهام، وعمليتي تعيين للموارد.</span><span class="sxs-lookup"><span data-stu-id="72baf-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="72baf-688">بعد ذلك، عليك تحديث مهمة واحدة وتحديث المشروع وحذف مهمة واحدة وحذف تعيين مورد واحد وإنشاء تبعية مهمة.</span><span class="sxs-lookup"><span data-stu-id="72baf-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="72baf-689">عينات إضافية</span><span class="sxs-lookup"><span data-stu-id="72baf-689">Additional samples</span></span>

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
