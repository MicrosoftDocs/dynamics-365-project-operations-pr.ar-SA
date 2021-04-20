---
title: تكوين المكونات الخاضعة للرسوم لشروط التعاقد المستندة إلى المشروع
description: يقدم هذا الموضوع معلومات حول كيفية إضافة مكونات خاضعة للرسوم إلى شروط التعاقد في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ddada2cb412ba7370fb0a750325a84772937d8d0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858457"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="1a998-103">تكوين المكونات الخاضعة للرسوم لشروط التعاقد المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="1a998-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="1a998-104">_**ينطبق على:** نشر خفيف - التعامل مع الفواتير الأولية‬، Project Operations لسيناريوهات الموارد/المنتجات غير المخزنة_</span><span class="sxs-lookup"><span data-stu-id="1a998-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="1a998-105">تتضمن شروط التعاقد المستندة إلى المشروع مكونات *مضمنة* ومكونات *خاضعة للرسوم*.</span><span class="sxs-lookup"><span data-stu-id="1a998-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="1a998-106">المكونات المضمنة هي المكونات التي تخضع لما يلي:</span><span class="sxs-lookup"><span data-stu-id="1a998-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="1a998-107">أسلوب الفوترة وتقسيمات العميل</span><span class="sxs-lookup"><span data-stu-id="1a998-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="1a998-108">حدود يجب عدم تجاوزها</span><span class="sxs-lookup"><span data-stu-id="1a998-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="1a998-109">إعدادات تكرار الفاتورة المحددة في شروط التعاقد المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="1a998-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="1a998-110">يمكن وضع علامة على مجموعة فرعية من المكونات المضمنة باعتبارها خاضعه للرسوم باستخدام حقل **نوع الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="1a998-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="1a998-111">الحقل **نوع الفوترة** هو مجموعة خيارات تسمح بالقيم التالية في سياق شروط التعاقد:</span><span class="sxs-lookup"><span data-stu-id="1a998-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="1a998-112">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-112">Chargeable</span></span>
  - <span data-ttu-id="1a998-113">غير خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-113">Non-chargeable</span></span>

<span data-ttu-id="1a998-114">يمكن تحديد المكونات الخاضعة للرسوم في فئات المهام والأدوار والحركات.</span><span class="sxs-lookup"><span data-stu-id="1a998-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="1a998-115">يتم تحديد الخضوع للرسوم في المهام الخاصة بشروط تعاقد المشروع وينطبق على كافة فئات الحركات المضمنة في شروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="1a998-116">إذا كان حقل **تضمين المهام** على شروط التعاقد فارغًا أو معينّا إلى **المشروع بأكمله**، فلن تكون علامة تبويب **المهام الخاضعة للرسوم** متوفرة.</span><span class="sxs-lookup"><span data-stu-id="1a998-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="1a998-117">ينطبق الخضوع للرسوم المحدد على أدوار شروط تعاقد المشروع فقط على فئة الحركة **الوقت**.</span><span class="sxs-lookup"><span data-stu-id="1a998-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="1a998-118">إذا كان حقل **تضمين الوقت** على شروط التعاقد معينّا إلى **لا**، فلن تكون علامة تبويب **الأدوار الخاضعة للرسوم** متوفرة.</span><span class="sxs-lookup"><span data-stu-id="1a998-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="1a998-119">ينطبق الخضوع للرسوم المحدد على فئات الحركة لشروط تعاقد المشروع فقط على فئة الحركة **المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="1a998-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="1a998-120">إذا كان حقل **تضمين المصروفات** معينّا إلى **لا**، فلن تكون علامة تبويب **الفئات الخاضعة للرسوم** متوفرة.</span><span class="sxs-lookup"><span data-stu-id="1a998-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1a998-121">تحديث مهمة مشروع باعتبارها خاضعة أو غير خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="1a998-122">بإمكان مهمة مشروع أن تكون خاضعة أو غير خاضعة للرسوم على شرط تعاقد معين، مما يؤدي إلى جعل الإعداد التالي ممكنًا:</span><span class="sxs-lookup"><span data-stu-id="1a998-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="1a998-123">إذا تضمنت شروط تعاقد المشروع **الوقت** ومهمة معينة، فسيتم ربط **T1** بها كخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="1a998-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="1a998-124">عند وجود شرط تعاقد آخر يتضمن **المصروفات**، فيمكنك ربط المهمة T1 على شروط التعاقد كغير خاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="1a998-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="1a998-125">ونتيجة لذلك سيكون كل الوقت المسجل في المهمة خاضعًا للرسوم وستكون جميع المصروفات غير خاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="1a998-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="1a998-126">يمكن تكوين نوع فوترة المهمة على علامة تبويب **المهام الخاضعة للرسوم** في شرط التعاقد من خلال تحديث حقل **نوع الفوترة** على الشبكة الفرعية لمهام شروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="1a998-127">أو، يمكنك تحديث حقل **نوع الفوترة** على الشبكة الفرعية في إعداد فوترة مهمة المشروع الذي يعرض بنود شروط التعاقد المقترنة بمهمة.</span><span class="sxs-lookup"><span data-stu-id="1a998-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1a998-128">تحديث دور باعتباره خاضع أو غير خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="1a998-129">بإمكان الدور أن يكون خاضعًا أو غير خاضع للرسوم في شرط تعاقد محدد.</span><span class="sxs-lookup"><span data-stu-id="1a998-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="1a998-130">يمكن تكوين نوع فوترة الدور على علامة تبويب **الأدوار الخاضعة للرسوم** في شروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="1a998-131">للقيام بذلك، يمكنك تحديث حقل **نوع الفوترة** على الشبكة الفرعية **الأدوار الخاضعة للرسوم**.</span><span class="sxs-lookup"><span data-stu-id="1a998-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1a998-132">تحديث فئة حركة كخاضعة غير خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="1a998-133">بإمكان فئة الحركة أن تكون خاضعة أو غير خاضعة للرسوم في شرط تعاقد محدد.</span><span class="sxs-lookup"><span data-stu-id="1a998-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="1a998-134">يمكن تكوين نوع فوترة الحركة على علامة تبويب **الفئات الخاضعة للرسوم** في شروط التعاقد المستندة إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="1a998-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="1a998-135">للقيام بذلك، يمكنك تحديث حقل **نوع الفوترة** على الشبكة الفرعية **الفئات الخاضعة للرسوم**.</span><span class="sxs-lookup"><span data-stu-id="1a998-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="1a998-136">حل الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-136">Resolve chargeability</span></span>

<span data-ttu-id="1a998-137">يعتبر تقدير أو قيمة فعلية تم إنشاؤها للوقت خاضعة للرسوم فقط في الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="1a998-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="1a998-138">تم تضمين **الوقت** في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="1a998-139">تم تكوين **الدور** كخاضع للرسوم في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="1a998-140">تم تعيين **المهام المضمنة** إلى **مهام محددة** في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="1a998-141">إذا كانت هذه الأشياء الثلاثة صحيحة، فيتم تكوين المهمة كخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="1a998-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="1a998-142">يعتبر تقدير أو قيمة فعلية تم إنشاؤها للمصروفات خاضعة للرسوم فقط في الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="1a998-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="1a998-143">تم تضمين **المصروفات** في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="1a998-144">تم تكوين **فئة الحركة** كخاضعة للرسوم في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="1a998-145">تم تعيين **المهام المضمنة** إلى **مهمة محددة** في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="1a998-146">إذا كانت هذه الأشياء الثلاثة صحيحة، فيتم تكوين **المهمة** كخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="1a998-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="1a998-147">يعتبر تقدير أو قيمة فعلية تم إنشاؤها للمواد خاضعة للرسوم فقط في الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="1a998-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="1a998-148">تم تضمين **المواد** في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="1a998-149">تم تعيين **المهام المضمنة** إلى **مهام محددة** في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="1a998-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="1a998-150">إذا كان هذان الشيئان صحيحين، فيتم تكوين **المهمة** كخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="1a998-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1a998-151">
                    <strong>يتضمن الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1a998-152">
                    <strong>يتضمن المصروفات</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1a998-153">
                    <strong>يتضمن المواد</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="1a998-154">
                    <strong>المهام المضمنة</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-155">
                    <strong>الدور</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1a998-156">
                    <strong>الفئة</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-157">
                    <strong>مهمة</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="1a998-158">
                    <strong>تأثير الخضوع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-159">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-160">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-161">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-162">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="1a998-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-163">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-164">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-165">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-166">الفوترة على قيمة الوقت الفعلية: <strong>خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-167">نوع الفوترة على القيمة الفعلية للمصروفات: <strong>خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-168">نوع الفوترة على القيمة الفعلية للمواد: <strong>خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-169">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-170">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-171">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-172">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="1a998-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-173">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-174">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-175">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-176">الفوترة على قيمة الوقت الفعلية: <strong>خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-177">نوع الفوترة على القيمة الفعلية للمصروفات: <strong>خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-178">نوع الفوترة على القيمة الفعلية للمواد: <strong>خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-179">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-180">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-181">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-182">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="1a998-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-183">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-184">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-185">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-186">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-187">نوع الفوترة على القيمة الفعلية للمصروفات: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1a998-188">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-189">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-190">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-191">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-192">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="1a998-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-193">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-194">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-195">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-196">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-197">نوع الفوترة على القيمة الفعلية للمصروفات: <strong>غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-198">نوع الفوترة على القيمة الفعلية للمواد: <strong>غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-199">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-200">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-201">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-202">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="1a998-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-203">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-204">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-205">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-206">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-207">نوع الفوترة على القيمة الفعلية للمصروفات: <strong>غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-208">نوع الفوترة على القيمة الفعلية للمواد: <strong> غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-209">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-210">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-211">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-212">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="1a998-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-213">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1a998-214">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-215">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-216">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-217">نوع الفوترة على القيمة الفعلية للمصروفات: <strong>غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-218">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1a998-219">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-220">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-221">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-222">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="1a998-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-223">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1a998-224">
                    <strong>خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-225">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-226">الفوترة على قيمة الوقت الفعلية: <strong>غير متوفرة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-227">نوع الفوترة على القيمة الفعلية للمصروفات: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1a998-228">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1a998-229">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-230">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-231">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-232">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="1a998-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-233">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1a998-234">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-235">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-236">الفوترة على قيمة الوقت الفعلية: <strong>غير متوفرة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-237">نوع الفوترة على القيمة الفعلية للمصروفات: <strong> غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-238">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-239">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1a998-240">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-241">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-242">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="1a998-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-243">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-244">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-245">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-246">الفوترة على قيمة الوقت الفعلية: خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1a998-247">نوع الفوترة على القيمة الفعلية للمصروفات:<strong> غير متوفر</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-248">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-249">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1a998-250">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1a998-251">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-252">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="1a998-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-253">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-254">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-255">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-256">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-257">نوع الفوترة على القيمة الفعلية للمصروفات:<strong> غير متوفر</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-258">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-259">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-260">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1a998-261">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-262">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="1a998-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-263">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-264">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-265">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-266">الفوترة على قيمة الوقت الفعلية: خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1a998-267">نوع الفوترة على القيمة الفعلية للمصروفات: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="1a998-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1a998-268">نوع الفوترة على القيمة الفعلية للمواد: <strong> غير متوفر</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1a998-269">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1a998-270">نعم </span><span class="sxs-lookup"><span data-stu-id="1a998-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1a998-271">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1a998-272">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="1a998-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1a998-273">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1a998-274">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1a998-275">لا يمكن تعيينه</span><span class="sxs-lookup"><span data-stu-id="1a998-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1a998-276">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-277">نوع الفوترة على القيمة الفعلية للمصروفات:<strong> غير خاضع للرسوم </strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1a998-278">نوع الفوترة على القيمة الفعلية للمواد:<strong> غير متوفر</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1a998-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
