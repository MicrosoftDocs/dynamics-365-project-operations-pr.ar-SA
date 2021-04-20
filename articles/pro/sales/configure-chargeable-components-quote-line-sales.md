---
title: تكوين المكونات الخاضعة للرسوم الخاصة ببند عرض أسعار
description: يقدم هذا الموضوع معلومات حول إعداد المكونات الخاضعة وغير الخاضعة للرسوم في بند عرض أسعار مستند إلى مشروع.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a9e1851bd8c5a4070df2774c945d1f3eabaaa8a
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858277"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="d7646-103">تكوين المكونات الخاضعة للرسوم لبند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="d7646-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="d7646-104">_**ينطبق على:** نشر خفيف - التعامل مع الفواتير الأولية‬، Project Operations لسيناريوهات الموارد/المنتجات غير المخزنة_</span><span class="sxs-lookup"><span data-stu-id="d7646-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d7646-105">يتضمن بند عرض أسعار مستند إلى المشروع مكونات *مضمنة* ومكونات *خاضعة للرسوم*.</span><span class="sxs-lookup"><span data-stu-id="d7646-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="d7646-106">تخضع المكونات المضمنة لما يلي:</span><span class="sxs-lookup"><span data-stu-id="d7646-106">Included components are subject to:</span></span>

  - <span data-ttu-id="d7646-107">أسلوب الفوترة وتقسيمات العميل</span><span class="sxs-lookup"><span data-stu-id="d7646-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="d7646-108">حدود يجب عدم تجاوزها</span><span class="sxs-lookup"><span data-stu-id="d7646-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="d7646-109">إعدادات تكرار الفاتورة المحددة في بند عرض الأسعار المستند إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="d7646-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="d7646-110">يمكن وضع علامة على مجموعة فرعية من المكونات المضمنة باعتبارها خاضعه للرسوم باستخدام حقل **نوع الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="d7646-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="d7646-111">الحقل **نوع الفوترة** هو مجموعة خيارات تسمح بالقيم التالية في سياق بند عرض الأسعار:</span><span class="sxs-lookup"><span data-stu-id="d7646-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="d7646-112">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-112">Chargeable</span></span>
  - <span data-ttu-id="d7646-113">غير خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-113">Non-chargeable</span></span>

<span data-ttu-id="d7646-114">يمكن تحديد المكونات الخاضعة للرسوم في فئات المهام والأدوار والحركات.</span><span class="sxs-lookup"><span data-stu-id="d7646-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="d7646-115">يتم تحديد الخضوع للرسوم على المهام لبند عرض أسعار وينطبق على كافة فئات الحركات المضمنة في هذا البند.</span><span class="sxs-lookup"><span data-stu-id="d7646-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="d7646-116">إذا كان حقل **تضمين المهام** معينّا إلى **المشروع بأكمله** أو إذا ترك فارغًا، فلن تكون علامة تبويب **المهام الخاضعة للرسوم** متوفرة.</span><span class="sxs-lookup"><span data-stu-id="d7646-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="d7646-117">يتم تحديد الخضوع للرسوم المحدد على بند عرض الأسعار وينطبق فقط فئة الحركة **الوقت**.</span><span class="sxs-lookup"><span data-stu-id="d7646-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="d7646-118">إذا كان حقل **تضمين الوقت** معينّا إلى **لا** على بند عرض أسعار المشروع، فلن تكون علامة تبويب **الأدوار الخاضعة للرسوم** متوفرة.</span><span class="sxs-lookup"><span data-stu-id="d7646-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="d7646-119">يتم تحديد الخضوع للرسوم على فئات الحركة لبند عرض أسعار وينطبق فقط على فئة الحركة **المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="d7646-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="d7646-120">إذا كان حقل **تضمين المصروفات** معينّا إلى **لا** على بند عرض أسعار المشروع، فلن تكون علامة تبويب **الأدوار الخاضعة للرسوم** متوفرة.</span><span class="sxs-lookup"><span data-stu-id="d7646-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="d7646-121">تحديث مهمة مشروع كي تكون خاضعة أو غير خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="d7646-122">بإمكان مهمة مشروع أن تكون خاضعة أو غير خاضعة للرسوم في سياق بند عرض أسعار قائم على مشروع معين، مما يؤدي إلى جعل الإعداد التالي ممكنًا.</span><span class="sxs-lookup"><span data-stu-id="d7646-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="d7646-123">إذا تضمن بند عرض الأسعار الذي يستند إلى المشروع **الوقت** والمهمة **T1**، يتم ربط المهمة ببند عرض الأسعار على أنها خاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d7646-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="d7646-124">عند وجود بند عرض أسعار آخر يتضمن **المصروفات**، فيمكنك ربط المهمة **T1** على بند عرض الأسعار كغير خاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d7646-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="d7646-125">ونتيجة لذلك سيكون كل الوقت المسجل في المهمة خاضعًا للرسوم وستكون جميع المصروفات المسجلة على المهمة غير قابلة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d7646-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="d7646-126">يمكن تكوين نوع فوترة المهمة على علامة تبويب **المهام الخاضعة للرسوم** في بند عرض الأسعار القائم على المشروع من خلال تحديث حقل **نوع الفوترة** على الشبكة الفرعية **مهام بند عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="d7646-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="d7646-127">أو، يمكنك تحديث نوع الفوترة لمهمة مشروع في الحقل **نوع الفوترة** على الشبكة الفرعية في إعداد فوترة مهمة المشروع الذي يعرض بنود عرض الأسعار المقترنة بمهمة.</span><span class="sxs-lookup"><span data-stu-id="d7646-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="d7646-128">تحديث دور كي يكون خاضعًا أو غير خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="d7646-129">بإمكان الدور أن يكون خاضعًا أو غير خاضع للرسوم في سياق بند عرض أسعار معين يستند إلى مشروع.</span><span class="sxs-lookup"><span data-stu-id="d7646-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="d7646-130">يمكن تكوين نوع فوترة الدور على علامة تبويب **الأدوار الخاضعة للرسوم** في بند عرض الأسعار من خلال تحديث حقل **نوع الفوترة** على الشبكة الفرعية **الأدوار الخاضعة للرسوم**.</span><span class="sxs-lookup"><span data-stu-id="d7646-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="d7646-131">تحديث فئة حركة كي تكون خاضعة أو غير خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="d7646-132">بإمكان فئة الحركة أن تكون خاضعة أو غير خاضعة للرسوم في بند عرض أسعار محدد.</span><span class="sxs-lookup"><span data-stu-id="d7646-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="d7646-133">يمكن تكوين نوع فوترة الحركة على علامة تبويب **الفئات الخاضعة للرسوم** في بند عرض الأسعار من خلال تحديث حقل **نوع الفوترة** على الشبكة الفرعية **الفئات الخاضعة للرسوم**.</span><span class="sxs-lookup"><span data-stu-id="d7646-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="d7646-134">حل الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-134">Resolve chargeability</span></span>
<span data-ttu-id="d7646-135">يعتبر تقدير أو قيمة فعلية تم إنشاؤها للوقت خاضعة للرسوم فقط في الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="d7646-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="d7646-136">تم تضمين **الوقت** في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d7646-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="d7646-137">تم تكوين **الدور** كخاضع للرسوم في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d7646-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="d7646-138">تم تعيين **المهام المضمنة** إلى **مهام محددة** في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d7646-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="d7646-139">إذا كانت هذه الأشياء الثلاثة صحيحة، فيتم تكوين **المهمة** كخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d7646-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="d7646-140">يعتبر تقدير أو قيمة فعلية تم إنشاؤها للمصروفات خاضعة للرسوم فقط في الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="d7646-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="d7646-141">تم تضمين **المصروفات** في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d7646-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="d7646-142">تم تكوين **فئة الحركة** كخاضعة للرسوم في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d7646-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="d7646-143">تم تعيين **المهام المضمنة** إلى **مهام محددة** في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d7646-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="d7646-144">إذا كانت هذه الأشياء الثلاثة صحيحة، فيتم تكوين **المهمة** كخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d7646-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="d7646-145">يعتبر تقدير أو قيمة فعلية تم إنشاؤها للمواد خاضعة للرسوم فقط في الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="d7646-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="d7646-146">تم تضمين **المواد** في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d7646-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="d7646-147">تم تعيين **المهام المضمنة** إلى **مهام محددة** في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d7646-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="d7646-148">إذا كان هذان الشيئان صحيحين، فيجب أيضًا تكوين **المهمة** كخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d7646-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="d7646-149">
                    <strong>يتضمن الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="d7646-150">
                    <strong>يتضمن المصروفات</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="d7646-151">
                    <strong>يتضمن المواد</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="d7646-152">
                    <strong>المهام المضمنة</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-153">
                    <strong>الدور</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d7646-154">
                    <strong>الفئة</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-155">
                    <strong>مهمة</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="d7646-156">
                    <strong>تأثير الخضوع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-157">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-158">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-159">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-160">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="d7646-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-161">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-162">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-163">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-164">الفوترة على قيمة الوقت الفعلية: خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-165">نوع الفوترة على القيمة الفعلية للمصروفات: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-166">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-167">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-168">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-169">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-170">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="d7646-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-171">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-172">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-173">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-174">الفوترة على قيمة الوقت الفعلية: خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-175">نوع الفوترة على القيمة الفعلية للمصروفات: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-176">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-177">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-178">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-179">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-180">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="d7646-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-181">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-182">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-183">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-184">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-185">نوع الفوترة على القيمة الفعلية للمصروفات: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-186">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-187">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-188">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-189">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-190">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="d7646-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-191">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-192">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-193">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-194">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-195">نوع الفوترة على القيمة الفعلية للمصروفات: <strong>غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-196">نوع الفوترة على القيمة الفعلية للمواد: <strong>غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-197">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-198">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-199">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-200">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="d7646-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-201">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-202">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-203">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-204">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-205">نوع الفوترة على القيمة الفعلية للمصروفات: <strong>غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-206">نوع الفوترة على القيمة الفعلية للمواد: <strong> غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-207">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-208">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-209">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-210">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="d7646-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-211">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d7646-212">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-213">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-214">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-215">نوع الفوترة على القيمة الفعلية للمصروفات: <strong>غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-216">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="d7646-217">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-218">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-219">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-220">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="d7646-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-221">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d7646-222">
                    <strong>خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-223">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-224">الفوترة على قيمة الوقت الفعلية: <strong>غير متوفرة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-225">نوع الفوترة على القيمة الفعلية للمصروفات: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-226">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="d7646-227">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-228">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-229">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-230">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="d7646-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-231">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d7646-232">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-233">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-234">الفوترة على قيمة الوقت الفعلية: <strong>غير متوفرة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-235">نوع الفوترة على القيمة الفعلية للمصروفات: <strong> غير خاضع للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-236">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-237">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="d7646-238">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-239">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-240">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="d7646-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-241">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-242">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-243">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-244">الفوترة على قيمة الوقت الفعلية: خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-245">نوع الفوترة على القيمة الفعلية للمصروفات:<strong> غير متوفر</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-246">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-247">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="d7646-248">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d7646-249">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-250">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="d7646-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-251">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-252">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-253">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-254">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-255">نوع الفوترة على القيمة الفعلية للمصروفات:<strong> غير متوفر</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-256">نوع الفوترة على القيمة الفعلية للمواد: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-257">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-258">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="d7646-259">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-260">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="d7646-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-261">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-262">خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-263">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-264">الفوترة على قيمة الوقت الفعلية: خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-265">نوع الفوترة على القيمة الفعلية للمصروفات: خاضع للرسوم</span><span class="sxs-lookup"><span data-stu-id="d7646-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d7646-266">نوع الفوترة على القيمة الفعلية للمواد: <strong> غير متوفر</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d7646-267">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d7646-268">نعم </span><span class="sxs-lookup"><span data-stu-id="d7646-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="d7646-269">
                    <strong>لا </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d7646-270">المشروع بكامله</span><span class="sxs-lookup"><span data-stu-id="d7646-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d7646-271">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d7646-272">
                    <strong>غير خاضعة للرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d7646-273">يتعذر تعيين</span><span class="sxs-lookup"><span data-stu-id="d7646-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d7646-274">الفوترة على قيمة الوقت الفعلية: <strong>غير خاضعة للرسوم </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-275">نوع الفوترة على القيمة الفعلية للمصروفات:<strong> غير خاضع للرسوم </strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="d7646-276">نوع الفوترة على القيمة الفعلية للمواد:<strong> غير متوفر</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7646-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
