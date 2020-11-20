---
title: القيم الفعلية
description: يقدم هذا الموضوع معلومات حول كيفية العمل مع القيم الفعلية في Microsoft Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 13c429763fa805fae5324e4dcf1bf7669e842281
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126287"
---
# <a name="actuals"></a><span data-ttu-id="9a9bc-103">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-103">Actuals</span></span> 

<span data-ttu-id="9a9bc-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="9a9bc-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="9a9bc-105">القيم الفعلية هي مقدار العمل الذي تم إكماله في مشروع.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="9a9bc-106">يتم إنشاؤها كنتيجة لإدخالات الوقت والمصروفات وإدخالات دفتر اليومية والفواتير.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="9a9bc-107">إرسال بنود دفتر اليومية والوقت</span><span class="sxs-lookup"><span data-stu-id="9a9bc-107">Journal lines and time submission</span></span>

<span data-ttu-id="9a9bc-108">لمزيد من المعلومات حول إدخال الوقت، راجع [نظرة عامة حول إدخال الوقت](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9a9bc-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="9a9bc-109">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="9a9bc-109">Time and materials</span></span>

<span data-ttu-id="9a9bc-110">عندما يكون إدخال الوقت المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد الوقت والمواد، يقوم النظام بإنشاء بندين لدفتر اليومية، بند للتكلفة وبند للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="9a9bc-111">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="9a9bc-111">Fixed price</span></span>

<span data-ttu-id="9a9bc-112">عندما يكون إدخال الوقت المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد بسعر ثابت، يُنشئ النظام بند دفتر يومية للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="9a9bc-113">التسعير الافتراضي</span><span class="sxs-lookup"><span data-stu-id="9a9bc-113">Default pricing</span></span>

<span data-ttu-id="9a9bc-114">يكمن منطق إنشاء الأسعار الافتراضية في دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="9a9bc-115">يتم نسخ قيم الحقول من إدخال الوقت إلى دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="9a9bc-116">تتضمن هذه القيم تاريخ الحركة وشروط التعاقد التي تم تعيين المشروع لهاـ وينتج عن العملة قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="9a9bc-117">تُستخدم الحقول التي تؤثر في التسعير الافتراضي مثل **الدور** و **وحدة المؤسسة** لتحديد السعر المناسب في دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="9a9bc-118">يمكنك إضافة حقل مخصص في إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="9a9bc-119">إذا أردت أن يتم نشر قيمة الحقل على القيم الفعلية، فأنشئ الحقل في كيان القيم الفعلية، واستخدم تعيينات الحقول لنسخ الحقل من إدخال الوقت إلى القيمة الفعلية.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="9a9bc-120">إرسال أسطر دفتر اليومية والمصروفات الأساسية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="9a9bc-121">لمزيد من المعلومات حول إدخال المصروفات، راجع [نظرة عامة حول المصروفات](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9a9bc-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="9a9bc-122">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="9a9bc-122">Time and materials</span></span>

<span data-ttu-id="9a9bc-123">عندما يكون إدخال المصروفات الأساسية المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد الوقت والمواد، يقوم النظام بإنشاء بندين لدفتر اليومية، بند للتكلفة وبند للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="9a9bc-124">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="9a9bc-124">Fixed price</span></span>

<span data-ttu-id="9a9bc-125">عندما يكون إدخال المصروفات الأساسية المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد بسعر ثابت، يُنشئ النظام بند دفتر يومية للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="9a9bc-126">التسعير الافتراضي</span><span class="sxs-lookup"><span data-stu-id="9a9bc-126">Default pricing</span></span>

<span data-ttu-id="9a9bc-127">يستند منطق إدخال الأسعار الافتراضية للمصروفات إلى فئة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="9a9bc-128">يتم استخدام تاريخ الحركة وبند العقد الذي تم تعيين المشروع له والعملة جميعًا لتحديد قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="9a9bc-129">ومع ذلك، بشكل افتراضي، يتم تعيين المبلغ الذي تم إدخاله للسعر بحد ذاته بشكل مباشر على أسطر دفتر يومية المصروفات للتكلفة والمبيعات.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="9a9bc-130">لا يتوفر الإدخال المستند إلى الفئة للأسعار الافتراضية لكل وحدة في إدخالات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="9a9bc-131">استخدام دفاتر يومية الإدخالات لتسجيل التكاليف</span><span class="sxs-lookup"><span data-stu-id="9a9bc-131">Use entry journals to record costs</span></span>

<span data-ttu-id="9a9bc-132">يمكنك استخدام دفاتر يومية الإدخالات لتسجيل التكلفة أو الإيرادات في فئات المواد أو الرسوم أو الوقت أو المصروفات أو الحركات الضريبية.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="9a9bc-133">يمكن استخدام دفاتر اليومية للأغراض التالية:</span><span class="sxs-lookup"><span data-stu-id="9a9bc-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="9a9bc-134">تسجيل التكلفة الفعلية للموارد والمبيعات في أحد المشاريع.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="9a9bc-135">نقل القيم الفعلية للحركات من نظام آخر إلى Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="9a9bc-136">تسجيل التكاليف التي حدثت في نظام آخر.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="9a9bc-137">يمكن أن تتضمن هذه التكاليف تكاليف التدبير أو التعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9a9bc-138">لا يتحقق التطبيق من نوع أسطر دفتر اليومية أو التسعير ذي الصلة الذي تم إدخاله على سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="9a9bc-139">وبالتالي، فإن المستخدم الذي يكون على دراية بالتأثير المحاسبي للقيم الفعلية على المشروع وهو وحده الذي يجب عليه أن يستخدم دفاتر يومية الإدخالات لإنشاء القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="9a9bc-140">بسبب تأثير نوع دفتر اليومية هذا، يجب عليك اختيار من يمكنه الوصول إلى إنشاء دفاتر يومية الإدخال بعناية.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="9a9bc-141">تسجيل القيم الفعلية استنادًا إلى أحداث المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-141">Record actuals based on project events</span></span>

<span data-ttu-id="9a9bc-142">يسجل Project Operations الحركات المالية التي تحدث أثناء المشروع.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="9a9bc-143">تم تسجيل هذه الحركات على أنها قيم فعليه.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="9a9bc-144">توضح الجداول التالية الأنواع المختلفة من القيم الفعلية التي يتم إنشاؤها، وذلك استنادا إلى ما إذا كان المشروع هو مشروع الوقت والمواد أو أحد المشاريع ثابتة السعر، أو في مرحلة المبيعات الأولية، أو أنه مشروع داخلي.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="9a9bc-145">ينتمي المورد إلى نفس الوحدة التنظيمية باعتباره وحدة التعاقد الخاصة بالمشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="9a9bc-146">حدث</span><span class="sxs-lookup"><span data-stu-id="9a9bc-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="9a9bc-147">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="9a9bc-148">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="9a9bc-149">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="9a9bc-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="9a9bc-150">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="9a9bc-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="9a9bc-151">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="9a9bc-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="9a9bc-152">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-152">Actuals</span></span></th>
<th><span data-ttu-id="9a9bc-153">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="9a9bc-153">Transaction currency</span></span></th>
<th><span data-ttu-id="9a9bc-154">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="9a9bc-154">Fixed price</span></span></th>
<th><span data-ttu-id="9a9bc-155">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="9a9bc-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="9a9bc-156">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="9a9bc-157">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-158">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="9a9bc-159">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9a9bc-160">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="9a9bc-161">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-161">Cost actual</span></span></td>
<td><span data-ttu-id="9a9bc-162">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-163">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-164">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="9a9bc-165">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-166">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-167">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="9a9bc-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="9a9bc-168">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9a9bc-169">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="9a9bc-170">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-170">Cost actual</span></span></td>
<td><span data-ttu-id="9a9bc-171">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-172">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-173">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-174">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-175">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-176">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="9a9bc-177">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-178">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="9a9bc-179">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9a9bc-180">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="9a9bc-181">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="9a9bc-182">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-183">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="9a9bc-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-184">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-185">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-186">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-187">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-187">Billed sales</span></span></td>
<td><span data-ttu-id="9a9bc-188">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9a9bc-189">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="9a9bc-190">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="9a9bc-191">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-192">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-193">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-194">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-195">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-196">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="9a9bc-197">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-198">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="9a9bc-199">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9a9bc-200">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="9a9bc-201">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="9a9bc-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="9a9bc-202">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="9a9bc-203">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="9a9bc-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="9a9bc-204">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="9a9bc-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="9a9bc-205">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="9a9bc-206">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="9a9bc-207">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-208">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-208">Billed sales</span></span></td>
<td><span data-ttu-id="9a9bc-209">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9a9bc-210">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="9a9bc-211">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="9a9bc-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="9a9bc-212">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-213">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="9a9bc-214">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-215">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="9a9bc-216">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="9a9bc-217">ينتمي المورد إلى وحدة تنظيمية تختلف عن وحدة التعاقد الخاصة بالمشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="9a9bc-218">حدث</span><span class="sxs-lookup"><span data-stu-id="9a9bc-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="9a9bc-219">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="9a9bc-220">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="9a9bc-221">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="9a9bc-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="9a9bc-222">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="9a9bc-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="9a9bc-223">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="9a9bc-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="9a9bc-224">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-224">Actuals</span></span></th>
<th><span data-ttu-id="9a9bc-225">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="9a9bc-225">Transaction currency</span></span></th>
<th><span data-ttu-id="9a9bc-226">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="9a9bc-226">Fixed price</span></span></th>
<th><span data-ttu-id="9a9bc-227">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="9a9bc-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="9a9bc-228">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="9a9bc-229">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-230">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="9a9bc-231">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="9a9bc-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="9a9bc-232">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="9a9bc-233">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-233">Cost actual</span></span></td>
<td><span data-ttu-id="9a9bc-234">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="9a9bc-235">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="9a9bc-236">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="9a9bc-237">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="9a9bc-238">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-239">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="9a9bc-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="9a9bc-240">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-241">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="9a9bc-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="9a9bc-242">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="9a9bc-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-243">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="9a9bc-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="9a9bc-244">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="9a9bc-245">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="9a9bc-246">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-246">Cost actual</span></span></td>
<td><span data-ttu-id="9a9bc-247">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="9a9bc-248">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="9a9bc-249">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="9a9bc-250">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="9a9bc-251">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-252">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="9a9bc-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="9a9bc-253">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="9a9bc-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-254">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="9a9bc-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="9a9bc-255">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-256">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="9a9bc-257">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-258">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="9a9bc-259">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9a9bc-260">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="9a9bc-261">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="9a9bc-262">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-263">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="9a9bc-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-264">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-265">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="9a9bc-266">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-267">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-267">Billed sales</span></span></td>
<td><span data-ttu-id="9a9bc-268">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9a9bc-269">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="9a9bc-270">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="9a9bc-271">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-272">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-273">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-274">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9a9bc-275">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-276">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="9a9bc-277">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-278">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="9a9bc-279">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9a9bc-280">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="9a9bc-281">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="9a9bc-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="9a9bc-282">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="9a9bc-283">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="9a9bc-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="9a9bc-284">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="9a9bc-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="9a9bc-285">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="9a9bc-286">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="9a9bc-287">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-288">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-288">Billed sales</span></span></td>
<td><span data-ttu-id="9a9bc-289">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9a9bc-290">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="9a9bc-291">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="9a9bc-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="9a9bc-292">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-293">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="9a9bc-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="9a9bc-294">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9a9bc-295">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="9a9bc-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="9a9bc-296">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="9a9bc-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
