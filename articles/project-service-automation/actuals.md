---
title: القيم الفعلية
description: يقدم هذا الموضوع معلومات حول القيم الفعلية للمشروع.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748717"
---
# <a name="actuals"></a><span data-ttu-id="d0056-103">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d0056-103">Actuals</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="d0056-104">القيم الفعلية هي مقدار العمل الذي تم إكماله في مشروع.</span><span class="sxs-lookup"><span data-stu-id="d0056-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="d0056-105">يمكن تتبع العمل الفعلي للمشروع من خلال المستندات المصدر الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="d0056-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="d0056-106">وتتضمن المستندات المصدر هذه الوقت والمصروفات وإدخالات دفتر اليومية وكذلك الفواتير.</span><span class="sxs-lookup"><span data-stu-id="d0056-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![كيفية تتبع العمل الفعلي للمشروع من خلال مستندات مصدر](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="d0056-108">إرسال إدخال وقت</span><span class="sxs-lookup"><span data-stu-id="d0056-108">Submitting a time entry</span></span>

<span data-ttu-id="d0056-109">في PSA، عند تقديم إدخال وقت لمشروع تم تعيينه إلى بند عقد الوقت والمواد، يتم إنشاء بندي دفتر يومية.</span><span class="sxs-lookup"><span data-stu-id="d0056-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="d0056-110">ويُخصص بند واحد هو للتكلفة، والبند الآخر للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="d0056-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="d0056-111">عند تقديم إدخال وقت لمشروع تم تعيينه إلى بند عقد سعر ثابت، يتم إنشاء بند دفتر يومية للتكلفة فقط.</span><span class="sxs-lookup"><span data-stu-id="d0056-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="d0056-112">يعتمد منطق إدخال الأسعار الافتراضية على سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="d0056-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="d0056-113">يتم نسخ كافة قيم الحقول من إدخال الوقت إلى سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="d0056-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="d0056-114">تتضمن هذه الحقول تاريخ الحركة وبند العقد الذي تم تعيين المشروع له وينتج عن العملة قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="d0056-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="d0056-115">تؤدي الحقول التي تؤثر في الأسعار الافتراضية مثل **الدور** و **"وحدة المؤسسة** إلى إدخال سعر مناسب بشكل افتراضي في سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="d0056-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="d0056-116">إذا قمت باضافة حقل مخصص في إدخال الوقت، وتريد أن يتم نشر قيمة الحقل إلى القيم الفعلية، قم بإنشاء الحقل في الكيان "القيم الفعلية"، واستخدم تعيينات الحقول لنسخ الحقل من إدخال الوقت إلى القيمة الفعلية.</span><span class="sxs-lookup"><span data-stu-id="d0056-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="d0056-117">إرسال إدخال مصروفات</span><span class="sxs-lookup"><span data-stu-id="d0056-117">Submitting an expense entry</span></span>

<span data-ttu-id="d0056-118">في PSA، عند تقديم إدخال مصروفات لمشروع تم تعيينه إلى بند عقد الوقت والمواد، يتم إنشاء بندي دفتر يومية.</span><span class="sxs-lookup"><span data-stu-id="d0056-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="d0056-119">ويُخصص بند واحد هو للتكلفة، والبند الآخر للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="d0056-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="d0056-120">عند تقديم إدخال مصروفات لمشروع تم تعيينه إلى بند عقد سعر ثابت، يتم إنشاء بند دفتر يومية للتكلفة فقط.</span><span class="sxs-lookup"><span data-stu-id="d0056-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="d0056-121">يستند منطق إدخال الأسعار الافتراضية للمصروفات إلى فئة المصروفات التي تم تحديدها في صفحة **إدخال المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="d0056-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="d0056-122">يتم استخدام تاريخ الحركة وبند العقد الذي تم تعيين المشروع له والعملة جميعًا لتحديد قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="d0056-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="d0056-123">ومع ذلك، بالنسبة للسعر نفسه، يتم تعيين المبلغ الذي ادخله المستخدم مباشرة في بنود دفتر يومية المصروفات المرتبطة بالنسبة للتكلفة والمبيعات بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="d0056-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="d0056-124">في الإصدار الحالي من PSA، لا يتوفر الإدخال المستند إلى الفئة للأسعار الافتراضية لكل وحدة في إدخالات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="d0056-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-journals-to-record-costs"></a><span data-ttu-id="d0056-125">استخدام دفاتر اليومية لتسجيل التكاليف</span><span class="sxs-lookup"><span data-stu-id="d0056-125">Using journals to record costs</span></span>

<span data-ttu-id="d0056-126">في PSA، تتيح لك دفاتر اليومية تسجيل التكلفة أو العائد في فئات المواد أو الرسوم أو الوقت أو المصروفات أو الحركات الضريبية.</span><span class="sxs-lookup"><span data-stu-id="d0056-126">In PSA, journals let you record cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="d0056-127">يحتوي دفتر اليومية علي رأس وبنود واجراء **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="d0056-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="d0056-128">إليك بعض السيناريوهات التي قد تستخدم فيها دفتر اليومية:</span><span class="sxs-lookup"><span data-stu-id="d0056-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="d0056-129">يجب عليك تسجيل التكاليف والمبيعات الفعلية للمواد في أحد المشاريع.</span><span class="sxs-lookup"><span data-stu-id="d0056-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="d0056-130">يجب نقل القيم الفعلية من نظام آخر إلى PSA.</span><span class="sxs-lookup"><span data-stu-id="d0056-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="d0056-131">يجب عليك تسجيل التكاليف التي حدثت في نظام آخ ، مثل تكاليف التدبير أو التقاعد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="d0056-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="d0056-132">تسجيل القيم الفعلية استنادا إلى أحداث المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-132">Recording actuals based on project events</span></span>

<span data-ttu-id="d0056-133">تسجل PSA الحركات المالية التي تحدث أثناء المشروع.</span><span class="sxs-lookup"><span data-stu-id="d0056-133">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="d0056-134">تم تسجيل هذه الحركات على أنها **قيم فعليه**.</span><span class="sxs-lookup"><span data-stu-id="d0056-134">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="d0056-135">توضح الجداول التالية الأنواع المختلفة من القيم الفعلية التي يتم إنشاؤها، وذلك استنادا إلى ما إذا كان المشروع هو مشروع الوقت والمواد أو أحد المشاريع ثابتة السعر، أو في مرحلة المبيعات الأولية، أو أنه مشروع داخلي.</span><span class="sxs-lookup"><span data-stu-id="d0056-135">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="d0056-136">**ينتمي المورد إلى نفس الوحدة التنظيمية باعتباره وحدة التعاقد الخاصة بالمشروع**</span><span class="sxs-lookup"><span data-stu-id="d0056-136">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="d0056-137">حدث</span><span class="sxs-lookup"><span data-stu-id="d0056-137">Event</span></span></th>
<th colspan="4"><span data-ttu-id="d0056-138">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="d0056-138">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="d0056-139">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="d0056-139">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="d0056-140">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="d0056-140">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="d0056-141">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="d0056-141">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="d0056-142">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="d0056-142">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="d0056-143">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d0056-143">Actuals</span></span></th>
<th><span data-ttu-id="d0056-144">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="d0056-144">Transaction currency</span></span></th>
<th><span data-ttu-id="d0056-145">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="d0056-145">Fixed price</span></span></th>
<th><span data-ttu-id="d0056-146">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="d0056-146">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="d0056-147">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="d0056-147">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="d0056-148">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d0056-148">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-149">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="d0056-149">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="d0056-150">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d0056-150">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d0056-151">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d0056-151">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d0056-152">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-152">Cost actual</span></span></td>
<td><span data-ttu-id="d0056-153">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-153">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-154">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-154">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-155">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-155">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="d0056-156">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-156">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-157">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-157">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-158">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d0056-158">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="d0056-159">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-159">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d0056-160">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d0056-160">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d0056-161">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-161">Cost actual</span></span></td>
<td><span data-ttu-id="d0056-162">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-162">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-163">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-163">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-164">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-164">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-165">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-165">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-166">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-167">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d0056-167">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d0056-168">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-168">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-169">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d0056-169">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d0056-170">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-170">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d0056-171">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="d0056-171">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d0056-172">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="d0056-172">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d0056-173">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-173">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-174">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="d0056-174">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-175">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-175">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-176">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-176">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-177">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-177">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-178">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="d0056-178">Billed sales</span></span></td>
<td><span data-ttu-id="d0056-179">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d0056-180">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="d0056-180">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d0056-181">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="d0056-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d0056-182">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-182">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-183">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-183">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-184">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-184">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-185">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-185">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-186">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-187">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d0056-187">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d0056-188">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-188">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-189">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d0056-189">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d0056-190">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d0056-191">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d0056-191">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d0056-192">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="d0056-192">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d0056-193">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-193">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="d0056-194">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="d0056-194">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="d0056-195">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="d0056-195">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="d0056-196">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-196">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d0056-197">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-197">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="d0056-198">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-198">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-199">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="d0056-199">Billed sales</span></span></td>
<td><span data-ttu-id="d0056-200">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-200">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d0056-201">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d0056-201">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d0056-202">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="d0056-202">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d0056-203">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-203">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-204">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d0056-204">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="d0056-205">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-205">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-206">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d0056-206">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="d0056-207">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-207">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="d0056-208">**ينتمي المورد إلى وحدة تنظيمية تختلف عن وحدة التعاقد الخاصة بالمشروع**</span><span class="sxs-lookup"><span data-stu-id="d0056-208">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="d0056-209">حدث</span><span class="sxs-lookup"><span data-stu-id="d0056-209">Event</span></span></th>
<th colspan="4"><span data-ttu-id="d0056-210">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="d0056-210">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="d0056-211">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="d0056-211">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="d0056-212">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="d0056-212">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="d0056-213">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="d0056-213">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="d0056-214">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="d0056-214">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="d0056-215">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d0056-215">Actuals</span></span></th>
<th><span data-ttu-id="d0056-216">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="d0056-216">Transaction currency</span></span></th>
<th><span data-ttu-id="d0056-217">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="d0056-217">Fixed price</span></span></th>
<th><span data-ttu-id="d0056-218">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="d0056-218">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="d0056-219">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="d0056-219">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="d0056-220">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d0056-220">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-221">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="d0056-221">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="d0056-222">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d0056-222">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="d0056-223">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d0056-223">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d0056-224">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-224">Cost actual</span></span></td>
<td><span data-ttu-id="d0056-225">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-225">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="d0056-226">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-226">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="d0056-227">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-227">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="d0056-228">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-228">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="d0056-229">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-229">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-230">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d0056-230">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="d0056-231">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-231">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-232">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="d0056-232">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="d0056-233">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="d0056-233">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-234">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="d0056-234">Interorganizational sales</span></span></td>
<td><span data-ttu-id="d0056-235">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-235">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="d0056-236">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d0056-236">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d0056-237">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-237">Cost actual</span></span></td>
<td><span data-ttu-id="d0056-238">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-238">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d0056-239">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-239">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="d0056-240">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-240">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d0056-241">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-241">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="d0056-242">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d0056-242">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-243">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="d0056-243">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="d0056-244">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="d0056-244">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-245">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="d0056-245">Interorganizational sales</span></span></td>
<td><span data-ttu-id="d0056-246">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d0056-246">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-247">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d0056-247">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d0056-248">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-248">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-249">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d0056-249">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d0056-250">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-250">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d0056-251">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="d0056-251">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d0056-252">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="d0056-252">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d0056-253">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-253">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-254">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="d0056-254">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-255">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-255">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-256">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-256">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="d0056-257">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-257">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-258">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="d0056-258">Billed sales</span></span></td>
<td><span data-ttu-id="d0056-259">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d0056-260">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="d0056-260">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d0056-261">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="d0056-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d0056-262">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-262">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-263">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-263">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-264">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-264">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-265">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-265">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d0056-266">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-267">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d0056-267">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d0056-268">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-268">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-269">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d0056-269">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d0056-270">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-270">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d0056-271">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d0056-271">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d0056-272">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="d0056-272">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d0056-273">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-273">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="d0056-274">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="d0056-274">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="d0056-275">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="d0056-275">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="d0056-276">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-276">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d0056-277">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-277">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="d0056-278">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d0056-278">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-279">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="d0056-279">Billed sales</span></span></td>
<td><span data-ttu-id="d0056-280">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-280">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d0056-281">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d0056-281">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d0056-282">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="d0056-282">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d0056-283">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-283">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-284">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d0056-284">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="d0056-285">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-285">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d0056-286">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d0056-286">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="d0056-287">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d0056-287">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
