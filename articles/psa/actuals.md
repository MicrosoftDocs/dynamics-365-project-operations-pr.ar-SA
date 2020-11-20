---
title: نظرة عامة على ‏‫القيم الفعلية‬
description: يقدم هذا الموضوع معلومات حول القيم الفعلية للمشروع.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: cf9e36c99790b77f0ed6490f49b4ebeb043bcdf6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129752"
---
# <a name="actuals-overview"></a><span data-ttu-id="d4267-103">نظرة عامة على ‏‫القيم الفعلية‬</span><span class="sxs-lookup"><span data-stu-id="d4267-103">Actuals overview</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="d4267-104">القيم الفعلية هي مقدار العمل الذي تم إكماله في مشروع.</span><span class="sxs-lookup"><span data-stu-id="d4267-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="d4267-105">يمكن تتبع العمل الفعلي للمشروع من خلال المستندات المصدر الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="d4267-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="d4267-106">وتتضمن المستندات المصدر هذه الوقت والمصروفات وإدخالات دفتر اليومية وكذلك الفواتير.</span><span class="sxs-lookup"><span data-stu-id="d4267-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![كيفية تتبع العمل الفعلي للمشروع من خلال مستندات مصدر](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="d4267-108">إرسال إدخال وقت</span><span class="sxs-lookup"><span data-stu-id="d4267-108">Submitting a time entry</span></span>

<span data-ttu-id="d4267-109">في PSA، عند تقديم إدخال وقت لمشروع تم تعيينه إلى بند عقد الوقت والمواد، يتم إنشاء بندي دفتر يومية.</span><span class="sxs-lookup"><span data-stu-id="d4267-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="d4267-110">ويُخصص بند واحد هو للتكلفة، والبند الآخر للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="d4267-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="d4267-111">عند تقديم إدخال وقت لمشروع تم تعيينه إلى بند عقد سعر ثابت، يتم إنشاء بند دفتر يومية للتكلفة فقط.</span><span class="sxs-lookup"><span data-stu-id="d4267-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="d4267-112">يعتمد منطق إدخال الأسعار الافتراضية على سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="d4267-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="d4267-113">يتم نسخ كافة قيم الحقول من إدخال الوقت إلى سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="d4267-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="d4267-114">تتضمن هذه الحقول تاريخ الحركة وبند العقد الذي تم تعيين المشروع له وينتج عن العملة قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="d4267-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="d4267-115">تؤدي الحقول التي تؤثر في الأسعار الافتراضية مثل **الدور** و **"وحدة المؤسسة** إلى إدخال سعر مناسب بشكل افتراضي في سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="d4267-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="d4267-116">إذا قمت باضافة حقل مخصص في إدخال الوقت، وتريد أن يتم نشر قيمة الحقل إلى القيم الفعلية، قم بإنشاء الحقل في الكيان "القيم الفعلية"، واستخدم تعيينات الحقول لنسخ الحقل من إدخال الوقت إلى القيمة الفعلية.</span><span class="sxs-lookup"><span data-stu-id="d4267-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="d4267-117">إرسال إدخال مصروفات</span><span class="sxs-lookup"><span data-stu-id="d4267-117">Submitting an expense entry</span></span>

<span data-ttu-id="d4267-118">في PSA، عند تقديم إدخال مصروفات لمشروع تم تعيينه إلى بند عقد الوقت والمواد، يتم إنشاء بندي دفتر يومية.</span><span class="sxs-lookup"><span data-stu-id="d4267-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="d4267-119">ويُخصص بند واحد هو للتكلفة، والبند الآخر للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="d4267-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="d4267-120">عند تقديم إدخال مصروفات لمشروع تم تعيينه إلى بند عقد سعر ثابت، يتم إنشاء بند دفتر يومية للتكلفة فقط.</span><span class="sxs-lookup"><span data-stu-id="d4267-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="d4267-121">يستند منطق إدخال الأسعار الافتراضية للمصروفات إلى فئة المصروفات التي تم تحديدها في صفحة **إدخال المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="d4267-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="d4267-122">يتم استخدام تاريخ الحركة وبند العقد الذي تم تعيين المشروع له والعملة جميعًا لتحديد قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="d4267-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="d4267-123">ومع ذلك، بالنسبة للسعر نفسه، يتم تعيين المبلغ الذي ادخله المستخدم مباشرة في بنود دفتر يومية المصروفات المرتبطة بالنسبة للتكلفة والمبيعات بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="d4267-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="d4267-124">في الإصدار الحالي من PSA، لا يتوفر الإدخال المستند إلى الفئة للأسعار الافتراضية لكل وحدة في إدخالات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="d4267-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="d4267-125">استخدام دفاتر يومية الإدخال لتسجيل التكاليف</span><span class="sxs-lookup"><span data-stu-id="d4267-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="d4267-126">في PSA، تتيح لك دفاتر يومية الإدخال تسجيل التكلفة أو العائد في فئات المواد أو الرسوم أو الوقت أو المصروفات أو الحركات الضريبية.</span><span class="sxs-lookup"><span data-stu-id="d4267-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="d4267-127">يحتوي دفتر اليومية على رأس وبنود وإجراء **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="d4267-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="d4267-128">إليك بعض السيناريوهات التي قد تستخدم فيها دفتر اليومية:</span><span class="sxs-lookup"><span data-stu-id="d4267-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="d4267-129">يجب عليك تسجيل التكاليف والمبيعات الفعلية للمواد في أحد المشاريع.</span><span class="sxs-lookup"><span data-stu-id="d4267-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="d4267-130">يجب نقل القيم الفعلية من نظام آخر إلى PSA.</span><span class="sxs-lookup"><span data-stu-id="d4267-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="d4267-131">يجب عليك تسجيل التكاليف التي حدثت في نظام آخ ، مثل تكاليف التدبير أو التقاعد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="d4267-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d4267-132">يجب ألا يتم استخدام دفاتر اليومية لإنشاء القيم الفعلية إلا بواسطة مستخدم على دراية كاملة بالتأثير المحاسبي الذي تحدثه الأعمال الفعلية على المشروع.</span><span class="sxs-lookup"><span data-stu-id="d4267-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="d4267-133">وهذا لأن التطبيق لا يتحقق من نوع بند دفتر اليومية، أو التسعير ذي الصلة الذي تم إدخاله في بند دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="d4267-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="d4267-134">ونظرًا لتأثير هذا النوع من دفاتر اليومية، توخ الحذر الكافي بشأن من يتم منحه حق الوصول لإنشاء دفاتر يومية الإدخال.</span><span class="sxs-lookup"><span data-stu-id="d4267-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="d4267-135">تسجيل القيم الفعلية استنادا إلى أحداث المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-135">Recording actuals based on project events</span></span>

<span data-ttu-id="d4267-136">تسجل PSA الحركات المالية التي تحدث أثناء المشروع.</span><span class="sxs-lookup"><span data-stu-id="d4267-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="d4267-137">تم تسجيل هذه الحركات على أنها **قيم فعليه**.</span><span class="sxs-lookup"><span data-stu-id="d4267-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="d4267-138">توضح الجداول التالية الأنواع المختلفة من القيم الفعلية التي يتم إنشاؤها، وذلك استنادا إلى ما إذا كان المشروع هو مشروع الوقت والمواد أو أحد المشاريع ثابتة السعر، أو في مرحلة المبيعات الأولية، أو أنه مشروع داخلي.</span><span class="sxs-lookup"><span data-stu-id="d4267-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="d4267-139">**ينتمي المورد إلى نفس الوحدة التنظيمية باعتباره وحدة التعاقد الخاصة بالمشروع**</span><span class="sxs-lookup"><span data-stu-id="d4267-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="d4267-140">حدث</span><span class="sxs-lookup"><span data-stu-id="d4267-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="d4267-141">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="d4267-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="d4267-142">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="d4267-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="d4267-143">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="d4267-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="d4267-144">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="d4267-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="d4267-145">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="d4267-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="d4267-146">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d4267-146">Actuals</span></span></th>
<th><span data-ttu-id="d4267-147">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="d4267-147">Transaction currency</span></span></th>
<th><span data-ttu-id="d4267-148">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="d4267-148">Fixed price</span></span></th>
<th><span data-ttu-id="d4267-149">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="d4267-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="d4267-150">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="d4267-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="d4267-151">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d4267-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-152">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="d4267-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="d4267-153">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d4267-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d4267-154">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d4267-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d4267-155">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-155">Cost actual</span></span></td>
<td><span data-ttu-id="d4267-156">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-157">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-158">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="d4267-159">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-160">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-161">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d4267-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="d4267-162">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d4267-163">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d4267-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d4267-164">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-164">Cost actual</span></span></td>
<td><span data-ttu-id="d4267-165">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-166">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-167">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-168">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-169">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-170">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d4267-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d4267-171">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-172">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d4267-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d4267-173">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d4267-174">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="d4267-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d4267-175">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="d4267-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d4267-176">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-177">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="d4267-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-178">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-179">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-180">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-181">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="d4267-181">Billed sales</span></span></td>
<td><span data-ttu-id="d4267-182">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d4267-183">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="d4267-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d4267-184">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="d4267-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d4267-185">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-186">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-187">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-188">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-189">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-190">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d4267-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d4267-191">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-192">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d4267-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d4267-193">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d4267-194">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d4267-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d4267-195">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="d4267-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d4267-196">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="d4267-197">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="d4267-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="d4267-198">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="d4267-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="d4267-199">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d4267-200">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="d4267-201">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-202">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="d4267-202">Billed sales</span></span></td>
<td><span data-ttu-id="d4267-203">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d4267-204">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d4267-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d4267-205">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="d4267-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d4267-206">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-207">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d4267-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="d4267-208">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-209">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d4267-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="d4267-210">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="d4267-211">**ينتمي المورد إلى وحدة تنظيمية تختلف عن وحدة التعاقد الخاصة بالمشروع**</span><span class="sxs-lookup"><span data-stu-id="d4267-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="d4267-212">حدث</span><span class="sxs-lookup"><span data-stu-id="d4267-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="d4267-213">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="d4267-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="d4267-214">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="d4267-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="d4267-215">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="d4267-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="d4267-216">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="d4267-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="d4267-217">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="d4267-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="d4267-218">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d4267-218">Actuals</span></span></th>
<th><span data-ttu-id="d4267-219">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="d4267-219">Transaction currency</span></span></th>
<th><span data-ttu-id="d4267-220">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="d4267-220">Fixed price</span></span></th>
<th><span data-ttu-id="d4267-221">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="d4267-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="d4267-222">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="d4267-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="d4267-223">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d4267-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-224">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="d4267-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="d4267-225">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="d4267-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="d4267-226">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d4267-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d4267-227">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-227">Cost actual</span></span></td>
<td><span data-ttu-id="d4267-228">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="d4267-229">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="d4267-230">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="d4267-231">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="d4267-232">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-233">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="d4267-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="d4267-234">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-235">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="d4267-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="d4267-236">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="d4267-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-237">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="d4267-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="d4267-238">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="d4267-239">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d4267-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d4267-240">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-240">Cost actual</span></span></td>
<td><span data-ttu-id="d4267-241">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d4267-242">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="d4267-243">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d4267-244">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="d4267-245">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="d4267-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-246">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="d4267-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="d4267-247">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="d4267-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-248">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="d4267-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="d4267-249">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d4267-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-250">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d4267-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d4267-251">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-252">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d4267-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d4267-253">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d4267-254">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="d4267-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d4267-255">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="d4267-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d4267-256">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-257">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="d4267-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-258">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-259">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="d4267-260">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-261">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="d4267-261">Billed sales</span></span></td>
<td><span data-ttu-id="d4267-262">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d4267-263">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="d4267-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d4267-264">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="d4267-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d4267-265">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-266">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-267">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-268">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d4267-269">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-270">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d4267-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d4267-271">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-272">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d4267-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d4267-273">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d4267-274">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d4267-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d4267-275">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="d4267-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d4267-276">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="d4267-277">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="d4267-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="d4267-278">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="d4267-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="d4267-279">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d4267-280">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="d4267-281">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="d4267-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-282">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="d4267-282">Billed sales</span></span></td>
<td><span data-ttu-id="d4267-283">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d4267-284">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="d4267-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d4267-285">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="d4267-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d4267-286">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-287">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="d4267-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="d4267-288">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d4267-289">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="d4267-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="d4267-290">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="d4267-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
