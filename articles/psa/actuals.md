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
ms.openlocfilehash: c4a3424bed704243dfb5524fa541c3fcc0899e57
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285602"
---
# <a name="actuals-overview"></a><span data-ttu-id="034b7-103">نظرة عامة على ‏‫القيم الفعلية‬</span><span class="sxs-lookup"><span data-stu-id="034b7-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="034b7-104">القيم الفعلية هي مقدار العمل الذي تم إكماله في مشروع.</span><span class="sxs-lookup"><span data-stu-id="034b7-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="034b7-105">يمكن تتبع العمل الفعلي للمشروع من خلال المستندات المصدر الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="034b7-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="034b7-106">وتتضمن المستندات المصدر هذه الوقت والمصروفات وإدخالات دفتر اليومية وكذلك الفواتير.</span><span class="sxs-lookup"><span data-stu-id="034b7-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![كيفية تتبع العمل الفعلي للمشروع من خلال مستندات مصدر](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="034b7-108">إرسال إدخال وقت</span><span class="sxs-lookup"><span data-stu-id="034b7-108">Submitting a time entry</span></span>

<span data-ttu-id="034b7-109">في PSA، عند تقديم إدخال وقت لمشروع تم تعيينه إلى بند عقد الوقت والمواد، يتم إنشاء بندي دفتر يومية.</span><span class="sxs-lookup"><span data-stu-id="034b7-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="034b7-110">ويُخصص بند واحد هو للتكلفة، والبند الآخر للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="034b7-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="034b7-111">عند تقديم إدخال وقت لمشروع تم تعيينه إلى بند عقد سعر ثابت، يتم إنشاء بند دفتر يومية للتكلفة فقط.</span><span class="sxs-lookup"><span data-stu-id="034b7-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="034b7-112">يعتمد منطق إدخال الأسعار الافتراضية على سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="034b7-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="034b7-113">يتم نسخ كافة قيم الحقول من إدخال الوقت إلى سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="034b7-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="034b7-114">تتضمن هذه الحقول تاريخ الحركة وبند العقد الذي تم تعيين المشروع له وينتج عن العملة قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="034b7-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="034b7-115">تؤدي الحقول التي تؤثر في الأسعار الافتراضية مثل **الدور** و **"وحدة المؤسسة** إلى إدخال سعر مناسب بشكل افتراضي في سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="034b7-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="034b7-116">إذا قمت باضافة حقل مخصص في إدخال الوقت، وتريد أن يتم نشر قيمة الحقل إلى القيم الفعلية، قم بإنشاء الحقل في الكيان "القيم الفعلية"، واستخدم تعيينات الحقول لنسخ الحقل من إدخال الوقت إلى القيمة الفعلية.</span><span class="sxs-lookup"><span data-stu-id="034b7-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="034b7-117">إرسال إدخال مصروفات</span><span class="sxs-lookup"><span data-stu-id="034b7-117">Submitting an expense entry</span></span>

<span data-ttu-id="034b7-118">في PSA، عند تقديم إدخال مصروفات لمشروع تم تعيينه إلى بند عقد الوقت والمواد، يتم إنشاء بندي دفتر يومية.</span><span class="sxs-lookup"><span data-stu-id="034b7-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="034b7-119">ويُخصص بند واحد هو للتكلفة، والبند الآخر للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="034b7-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="034b7-120">عند تقديم إدخال مصروفات لمشروع تم تعيينه إلى بند عقد سعر ثابت، يتم إنشاء بند دفتر يومية للتكلفة فقط.</span><span class="sxs-lookup"><span data-stu-id="034b7-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="034b7-121">يستند منطق إدخال الأسعار الافتراضية للمصروفات إلى فئة المصروفات التي تم تحديدها في صفحة **إدخال المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="034b7-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="034b7-122">يتم استخدام تاريخ الحركة وبند العقد الذي تم تعيين المشروع له والعملة جميعًا لتحديد قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="034b7-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="034b7-123">ومع ذلك، بالنسبة للسعر نفسه، يتم تعيين المبلغ الذي ادخله المستخدم مباشرة في بنود دفتر يومية المصروفات المرتبطة بالنسبة للتكلفة والمبيعات بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="034b7-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="034b7-124">في الإصدار الحالي من PSA، لا يتوفر الإدخال المستند إلى الفئة للأسعار الافتراضية لكل وحدة في إدخالات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="034b7-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="034b7-125">استخدام دفاتر يومية الإدخال لتسجيل التكاليف</span><span class="sxs-lookup"><span data-stu-id="034b7-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="034b7-126">في PSA، تتيح لك دفاتر يومية الإدخال تسجيل التكلفة أو العائد في فئات المواد أو الرسوم أو الوقت أو المصروفات أو الحركات الضريبية.</span><span class="sxs-lookup"><span data-stu-id="034b7-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="034b7-127">يحتوي دفتر اليومية على رأس وبنود وإجراء **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="034b7-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="034b7-128">إليك بعض السيناريوهات التي قد تستخدم فيها دفتر اليومية:</span><span class="sxs-lookup"><span data-stu-id="034b7-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="034b7-129">يجب عليك تسجيل التكاليف والمبيعات الفعلية للمواد في أحد المشاريع.</span><span class="sxs-lookup"><span data-stu-id="034b7-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="034b7-130">يجب نقل القيم الفعلية من نظام آخر إلى PSA.</span><span class="sxs-lookup"><span data-stu-id="034b7-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="034b7-131">يجب عليك تسجيل التكاليف التي حدثت في نظام آخ ، مثل تكاليف التدبير أو التقاعد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="034b7-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="034b7-132">يجب ألا يتم استخدام دفاتر اليومية لإنشاء القيم الفعلية إلا بواسطة مستخدم على دراية كاملة بالتأثير المحاسبي الذي تحدثه الأعمال الفعلية على المشروع.</span><span class="sxs-lookup"><span data-stu-id="034b7-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="034b7-133">وهذا لأن التطبيق لا يتحقق من نوع بند دفتر اليومية، أو التسعير ذي الصلة الذي تم إدخاله في بند دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="034b7-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="034b7-134">ونظرًا لتأثير هذا النوع من دفاتر اليومية، توخ الحذر الكافي بشأن من يتم منحه حق الوصول لإنشاء دفاتر يومية الإدخال.</span><span class="sxs-lookup"><span data-stu-id="034b7-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="034b7-135">تسجيل القيم الفعلية استنادا إلى أحداث المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-135">Recording actuals based on project events</span></span>

<span data-ttu-id="034b7-136">تسجل PSA الحركات المالية التي تحدث أثناء المشروع.</span><span class="sxs-lookup"><span data-stu-id="034b7-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="034b7-137">تم تسجيل هذه الحركات على أنها **قيم فعليه**.</span><span class="sxs-lookup"><span data-stu-id="034b7-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="034b7-138">توضح الجداول التالية الأنواع المختلفة من القيم الفعلية التي يتم إنشاؤها، وذلك استنادا إلى ما إذا كان المشروع هو مشروع الوقت والمواد أو أحد المشاريع ثابتة السعر، أو في مرحلة المبيعات الأولية، أو أنه مشروع داخلي.</span><span class="sxs-lookup"><span data-stu-id="034b7-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="034b7-139">**ينتمي المورد إلى نفس الوحدة التنظيمية باعتباره وحدة التعاقد الخاصة بالمشروع**</span><span class="sxs-lookup"><span data-stu-id="034b7-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="034b7-140">حدث</span><span class="sxs-lookup"><span data-stu-id="034b7-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="034b7-141">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="034b7-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="034b7-142">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="034b7-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="034b7-143">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="034b7-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="034b7-144">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="034b7-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="034b7-145">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="034b7-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="034b7-146">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="034b7-146">Actuals</span></span></th>
<th><span data-ttu-id="034b7-147">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="034b7-147">Transaction currency</span></span></th>
<th><span data-ttu-id="034b7-148">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="034b7-148">Fixed price</span></span></th>
<th><span data-ttu-id="034b7-149">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="034b7-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="034b7-150">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="034b7-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="034b7-151">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="034b7-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-152">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="034b7-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="034b7-153">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="034b7-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="034b7-154">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="034b7-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="034b7-155">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-155">Cost actual</span></span></td>
<td><span data-ttu-id="034b7-156">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-157">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-158">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="034b7-159">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-160">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-161">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="034b7-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="034b7-162">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="034b7-163">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="034b7-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="034b7-164">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-164">Cost actual</span></span></td>
<td><span data-ttu-id="034b7-165">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-166">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-167">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-168">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-169">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-170">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="034b7-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="034b7-171">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-172">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="034b7-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="034b7-173">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="034b7-174">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="034b7-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="034b7-175">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="034b7-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="034b7-176">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-177">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="034b7-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-178">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-179">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-180">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-181">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="034b7-181">Billed sales</span></span></td>
<td><span data-ttu-id="034b7-182">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="034b7-183">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="034b7-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="034b7-184">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="034b7-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="034b7-185">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-186">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-187">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-188">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-189">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-190">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="034b7-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="034b7-191">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-192">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="034b7-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="034b7-193">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="034b7-194">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="034b7-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="034b7-195">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="034b7-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="034b7-196">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="034b7-197">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="034b7-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="034b7-198">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="034b7-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="034b7-199">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="034b7-200">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="034b7-201">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-202">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="034b7-202">Billed sales</span></span></td>
<td><span data-ttu-id="034b7-203">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="034b7-204">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="034b7-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="034b7-205">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="034b7-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="034b7-206">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-207">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="034b7-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="034b7-208">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-209">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="034b7-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="034b7-210">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="034b7-211">**ينتمي المورد إلى وحدة تنظيمية تختلف عن وحدة التعاقد الخاصة بالمشروع**</span><span class="sxs-lookup"><span data-stu-id="034b7-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="034b7-212">حدث</span><span class="sxs-lookup"><span data-stu-id="034b7-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="034b7-213">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="034b7-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="034b7-214">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="034b7-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="034b7-215">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="034b7-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="034b7-216">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="034b7-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="034b7-217">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="034b7-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="034b7-218">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="034b7-218">Actuals</span></span></th>
<th><span data-ttu-id="034b7-219">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="034b7-219">Transaction currency</span></span></th>
<th><span data-ttu-id="034b7-220">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="034b7-220">Fixed price</span></span></th>
<th><span data-ttu-id="034b7-221">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="034b7-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="034b7-222">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="034b7-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="034b7-223">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="034b7-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-224">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="034b7-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="034b7-225">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="034b7-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="034b7-226">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="034b7-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="034b7-227">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-227">Cost actual</span></span></td>
<td><span data-ttu-id="034b7-228">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="034b7-229">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="034b7-230">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="034b7-231">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="034b7-232">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-233">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="034b7-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="034b7-234">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-235">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="034b7-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="034b7-236">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="034b7-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-237">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="034b7-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="034b7-238">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="034b7-239">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="034b7-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="034b7-240">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-240">Cost actual</span></span></td>
<td><span data-ttu-id="034b7-241">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="034b7-242">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="034b7-243">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="034b7-244">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="034b7-245">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="034b7-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-246">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="034b7-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="034b7-247">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="034b7-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-248">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="034b7-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="034b7-249">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="034b7-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-250">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="034b7-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="034b7-251">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-252">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="034b7-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="034b7-253">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="034b7-254">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="034b7-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="034b7-255">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="034b7-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="034b7-256">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-257">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="034b7-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-258">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-259">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="034b7-260">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-261">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="034b7-261">Billed sales</span></span></td>
<td><span data-ttu-id="034b7-262">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="034b7-263">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="034b7-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="034b7-264">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="034b7-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="034b7-265">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-266">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-267">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-268">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="034b7-269">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-270">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="034b7-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="034b7-271">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-272">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="034b7-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="034b7-273">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="034b7-274">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="034b7-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="034b7-275">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="034b7-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="034b7-276">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="034b7-277">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="034b7-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="034b7-278">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="034b7-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="034b7-279">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="034b7-280">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="034b7-281">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="034b7-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-282">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="034b7-282">Billed sales</span></span></td>
<td><span data-ttu-id="034b7-283">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="034b7-284">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="034b7-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="034b7-285">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="034b7-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="034b7-286">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-287">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="034b7-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="034b7-288">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="034b7-289">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="034b7-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="034b7-290">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="034b7-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]