---
title: الصفحة الرئيسية للقيم الفعلية
description: يقدم هذا الموضوع معلومات حول كيفية العمل مع القيم الفعلية في Microsoft Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 75ad336a995aba3505325466433a5c5e2bb3e776
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907302"
---
# <a name="actuals"></a><span data-ttu-id="8f530-103">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="8f530-103">Actuals</span></span>

<span data-ttu-id="8f530-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="8f530-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8f530-105">القيم الفعلية هي مقدار العمل الذي تم إكماله في مشروع.</span><span class="sxs-lookup"><span data-stu-id="8f530-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="8f530-106">يتم إنشاؤها كنتيجة لإدخالات الوقت والمصروفات وإدخالات دفتر اليومية والفواتير.</span><span class="sxs-lookup"><span data-stu-id="8f530-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="8f530-107">إرسال بنود دفتر اليومية والوقت</span><span class="sxs-lookup"><span data-stu-id="8f530-107">Journal lines and time submission</span></span>

<span data-ttu-id="8f530-108">لمزيد من المعلومات حول إدخال الوقت، راجع [نظرة عامة حول إدخال الوقت](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8f530-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="8f530-109">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="8f530-109">Time and materials</span></span>

<span data-ttu-id="8f530-110">عندما يكون إدخال الوقت المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد الوقت والمواد، يقوم النظام بإنشاء بندين لدفتر اليومية، بند للتكلفة وبند للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="8f530-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="8f530-111">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="8f530-111">Fixed price</span></span>

<span data-ttu-id="8f530-112">عندما يكون إدخال الوقت المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد بسعر ثابت، يُنشئ النظام بند دفتر يومية للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="8f530-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="8f530-113">التسعير الافتراضي</span><span class="sxs-lookup"><span data-stu-id="8f530-113">Default pricing</span></span>

<span data-ttu-id="8f530-114">يكمن منطق إنشاء الأسعار الافتراضية في دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="8f530-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="8f530-115">يتم نسخ قيم الحقول من إدخال الوقت إلى دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="8f530-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="8f530-116">تتضمن هذه القيم تاريخ الحركة وشروط التعاقد التي تم تعيين المشروع لهاـ وينتج عن العملة قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="8f530-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="8f530-117">تُستخدم الحقول التي تؤثر في التسعير الافتراضي مثل **الدور** و**وحدة المؤسسة** لتحديد السعر المناسب في دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="8f530-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="8f530-118">يمكنك إضافة حقل مخصص في إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="8f530-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="8f530-119">إذا أردت أن يتم نشر قيمة الحقل على القيم الفعلية، فأنشئ الحقل في كيان القيم الفعلية، واستخدم تعيينات الحقول لنسخ الحقل من إدخال الوقت إلى القيمة الفعلية.</span><span class="sxs-lookup"><span data-stu-id="8f530-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="8f530-120">إرسال أسطر دفتر اليومية والمصروفات الأساسية</span><span class="sxs-lookup"><span data-stu-id="8f530-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="8f530-121">لمزيد من المعلومات حول إدخال المصروفات، راجع [نظرة عامة حول المصروفات](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8f530-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="8f530-122">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="8f530-122">Time and materials</span></span>

<span data-ttu-id="8f530-123">عندما يكون إدخال المصروفات الأساسية المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد الوقت والمواد، يقوم النظام بإنشاء بندين لدفتر اليومية، بند للتكلفة وبند للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="8f530-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="8f530-124">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="8f530-124">Fixed price</span></span>

<span data-ttu-id="8f530-125">عندما يكون إدخال المصروفات الأساسية المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد بسعر ثابت، يُنشئ النظام بند دفتر يومية للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="8f530-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="8f530-126">التسعير الافتراضي</span><span class="sxs-lookup"><span data-stu-id="8f530-126">Default pricing</span></span>

<span data-ttu-id="8f530-127">يستند منطق إدخال الأسعار الافتراضية للمصروفات إلى فئة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="8f530-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="8f530-128">يتم استخدام تاريخ الحركة وبند العقد الذي تم تعيين المشروع له والعملة جميعًا لتحديد قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="8f530-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="8f530-129">ومع ذلك، بشكل افتراضي، يتم تعيين المبلغ الذي تم إدخاله للسعر بحد ذاته بشكل مباشر على أسطر دفتر يومية المصروفات للتكلفة والمبيعات.</span><span class="sxs-lookup"><span data-stu-id="8f530-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="8f530-130">لا يتوفر الإدخال المستند إلى الفئة للأسعار الافتراضية لكل وحدة في إدخالات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="8f530-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="8f530-131">استخدام دفاتر يومية الإدخالات لتسجيل التكاليف</span><span class="sxs-lookup"><span data-stu-id="8f530-131">Use entry journals to record costs</span></span>

<span data-ttu-id="8f530-132">يمكنك استخدام دفاتر يومية الإدخالات لتسجيل التكلفة أو الإيرادات في فئات المواد أو الرسوم أو الوقت أو المصروفات أو الحركات الضريبية.</span><span class="sxs-lookup"><span data-stu-id="8f530-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="8f530-133">يمكن استخدام دفاتر اليومية للأغراض التالية:</span><span class="sxs-lookup"><span data-stu-id="8f530-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="8f530-134">تسجيل التكلفة الفعلية للموارد والمبيعات في أحد المشاريع.</span><span class="sxs-lookup"><span data-stu-id="8f530-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="8f530-135">نقل القيم الفعلية للحركات من نظام آخر إلى Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="8f530-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="8f530-136">تسجيل التكاليف التي حدثت في نظام آخر.</span><span class="sxs-lookup"><span data-stu-id="8f530-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="8f530-137">يمكن أن تتضمن هذه التكاليف تكاليف التدبير أو التعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="8f530-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8f530-138">لا يتحقق التطبيق من نوع أسطر دفتر اليومية أو التسعير ذي الصلة الذي تم إدخاله على سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="8f530-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="8f530-139">وبالتالي، فإن المستخدم الذي يكون على دراية بالتأثير المحاسبي للقيم الفعلية على المشروع وهو وحده الذي يجب عليه أن يستخدم دفاتر يومية الإدخالات لإنشاء القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="8f530-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="8f530-140">بسبب تأثير نوع دفتر اليومية هذا، يجب عليك اختيار من يمكنه الوصول إلى إنشاء دفاتر يومية الإدخال بعناية.</span><span class="sxs-lookup"><span data-stu-id="8f530-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="8f530-141">تسجيل القيم الفعلية استنادًا إلى أحداث المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-141">Record actuals based on project events</span></span>

<span data-ttu-id="8f530-142">يسجل Project Operations الحركات المالية التي تحدث أثناء المشروع.</span><span class="sxs-lookup"><span data-stu-id="8f530-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="8f530-143">تم تسجيل هذه الحركات على أنها قيم فعليه.</span><span class="sxs-lookup"><span data-stu-id="8f530-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="8f530-144">توضح الجداول التالية الأنواع المختلفة من القيم الفعلية التي يتم إنشاؤها، وذلك استنادا إلى ما إذا كان المشروع هو مشروع الوقت والمواد أو أحد المشاريع ثابتة السعر، أو في مرحلة المبيعات الأولية، أو أنه مشروع داخلي.</span><span class="sxs-lookup"><span data-stu-id="8f530-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="8f530-145">ينتمي المورد إلى نفس الوحدة التنظيمية باعتباره وحدة التعاقد الخاصة بالمشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="8f530-146">حدث</span><span class="sxs-lookup"><span data-stu-id="8f530-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="8f530-147">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="8f530-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="8f530-148">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="8f530-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="8f530-149">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="8f530-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="8f530-150">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="8f530-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="8f530-151">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="8f530-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="8f530-152">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="8f530-152">Actuals</span></span></th>
<th><span data-ttu-id="8f530-153">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="8f530-153">Transaction currency</span></span></th>
<th><span data-ttu-id="8f530-154">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="8f530-154">Fixed price</span></span></th>
<th><span data-ttu-id="8f530-155">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="8f530-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="8f530-156">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="8f530-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="8f530-157">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="8f530-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-158">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="8f530-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="8f530-159">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="8f530-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="8f530-160">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="8f530-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="8f530-161">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-161">Cost actual</span></span></td>
<td><span data-ttu-id="8f530-162">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-163">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-164">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="8f530-165">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-166">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-167">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="8f530-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="8f530-168">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="8f530-169">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="8f530-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="8f530-170">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-170">Cost actual</span></span></td>
<td><span data-ttu-id="8f530-171">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-172">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-173">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-174">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-175">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-176">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="8f530-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="8f530-177">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-178">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="8f530-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="8f530-179">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="8f530-180">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="8f530-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="8f530-181">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="8f530-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="8f530-182">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-183">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="8f530-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-184">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-185">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-186">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-187">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="8f530-187">Billed sales</span></span></td>
<td><span data-ttu-id="8f530-188">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="8f530-189">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="8f530-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="8f530-190">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="8f530-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="8f530-191">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-192">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-193">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-194">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-195">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-196">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="8f530-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="8f530-197">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-198">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="8f530-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="8f530-199">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="8f530-200">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="8f530-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="8f530-201">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="8f530-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="8f530-202">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="8f530-203">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="8f530-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="8f530-204">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="8f530-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="8f530-205">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="8f530-206">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="8f530-207">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-208">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="8f530-208">Billed sales</span></span></td>
<td><span data-ttu-id="8f530-209">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="8f530-210">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="8f530-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="8f530-211">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="8f530-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="8f530-212">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-213">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="8f530-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="8f530-214">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-215">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="8f530-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="8f530-216">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="8f530-217">ينتمي المورد إلى وحدة تنظيمية تختلف عن وحدة التعاقد الخاصة بالمشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="8f530-218">حدث</span><span class="sxs-lookup"><span data-stu-id="8f530-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="8f530-219">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="8f530-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="8f530-220">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="8f530-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="8f530-221">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="8f530-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="8f530-222">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="8f530-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="8f530-223">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="8f530-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="8f530-224">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="8f530-224">Actuals</span></span></th>
<th><span data-ttu-id="8f530-225">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="8f530-225">Transaction currency</span></span></th>
<th><span data-ttu-id="8f530-226">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="8f530-226">Fixed price</span></span></th>
<th><span data-ttu-id="8f530-227">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="8f530-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="8f530-228">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="8f530-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="8f530-229">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="8f530-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-230">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="8f530-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="8f530-231">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="8f530-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="8f530-232">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="8f530-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="8f530-233">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-233">Cost actual</span></span></td>
<td><span data-ttu-id="8f530-234">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="8f530-235">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="8f530-236">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="8f530-237">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="8f530-238">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-239">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="8f530-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="8f530-240">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-241">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="8f530-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="8f530-242">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="8f530-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-243">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="8f530-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="8f530-244">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="8f530-245">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="8f530-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="8f530-246">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-246">Cost actual</span></span></td>
<td><span data-ttu-id="8f530-247">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="8f530-248">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="8f530-249">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="8f530-250">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="8f530-251">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="8f530-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-252">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="8f530-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="8f530-253">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="8f530-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-254">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="8f530-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="8f530-255">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="8f530-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-256">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="8f530-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="8f530-257">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-258">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="8f530-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="8f530-259">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="8f530-260">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="8f530-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="8f530-261">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="8f530-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="8f530-262">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-263">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="8f530-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-264">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-265">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="8f530-266">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-267">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="8f530-267">Billed sales</span></span></td>
<td><span data-ttu-id="8f530-268">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="8f530-269">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="8f530-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="8f530-270">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="8f530-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="8f530-271">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-272">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-273">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-274">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="8f530-275">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-276">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="8f530-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="8f530-277">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-278">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="8f530-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="8f530-279">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="8f530-280">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="8f530-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="8f530-281">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="8f530-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="8f530-282">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="8f530-283">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="8f530-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="8f530-284">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="8f530-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="8f530-285">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="8f530-286">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="8f530-287">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="8f530-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-288">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="8f530-288">Billed sales</span></span></td>
<td><span data-ttu-id="8f530-289">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="8f530-290">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="8f530-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="8f530-291">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="8f530-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="8f530-292">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-293">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="8f530-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="8f530-294">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="8f530-295">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="8f530-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="8f530-296">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8f530-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
