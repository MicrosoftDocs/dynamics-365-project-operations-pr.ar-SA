---
title: فواتير المشروع التصحيحية
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء الفواتير التصحيحية وتأكيدها في Project Operations.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: dfa5535597ee6e144259c9246b33075f3492285e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004065"
---
# <a name="corrective-project-invoices"></a><span data-ttu-id="47872-103">فواتير المشروع التصحيحية</span><span class="sxs-lookup"><span data-stu-id="47872-103">Corrective project invoices</span></span>

<span data-ttu-id="47872-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="47872-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="47872-105">يمكن تصحيح فاتورة مشروع مؤكدة لمعالجة التغييرات أو الأرصدة نتيجة التفاوض مع العميل ومدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="47872-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="47872-106">لإجراء عمليات تحرير على فاتورة مؤكدة، افتح الفاتورة المؤكدة وحدد **تصحيح هذه الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="47872-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="47872-107">لا يتوفر هذا التحديد ما لم يتم تأكيد فاتورة المشروع.</span><span class="sxs-lookup"><span data-stu-id="47872-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="47872-108">يتم إنشاء فاتورة مسودة جديدة من الفاتورة المؤكدة.</span><span class="sxs-lookup"><span data-stu-id="47872-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="47872-109">يتم نسخ كافة تفاصيل بنود الفاتورة من الفاتورة المؤكدة في السابق إلى المسودة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="47872-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="47872-110">فيما يلي بعض النقاط الأساسية للتعرف على تفاصيل البنود في الفاتورة الجديدة التي تم تصحيحها:</span><span class="sxs-lookup"><span data-stu-id="47872-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="47872-111">يتم تحديث جميع الكميات إلى صفر.</span><span class="sxs-lookup"><span data-stu-id="47872-111">All quantities are updated to zero.</span></span> <span data-ttu-id="47872-112">يفترض التطبيق أن جميع الأصناف المفوترة مقيدة في الحساب بشكل كامل.</span><span class="sxs-lookup"><span data-stu-id="47872-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="47872-113">عند الضرورة، يمكنك تحديث هذه الكميات يدويًا لتعكس الكمية التي تجري فوترتها، وليس الكمية التي يجري تقييدها في الحساب.</span><span class="sxs-lookup"><span data-stu-id="47872-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="47872-114">استنادًا إلى الكمية التي تقوم بإدخالها، يحتسب التطبيق الكمية المقيدة في الحساب.</span><span class="sxs-lookup"><span data-stu-id="47872-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="47872-115">ويظهر هذا المبلغ في القيم الفعلية التي يتم إنشاؤها عند تأكيد الفاتورة المصححة.</span><span class="sxs-lookup"><span data-stu-id="47872-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="47872-116">إذا كنت تجري تغييرات على مبلغ الضريبة، فيجب عليك إدخال مبلغ الضريبة الصحيح وليس مبلغ الضريبة الذي يجري تقييده في الحساب.</span><span class="sxs-lookup"><span data-stu-id="47872-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="47872-117">لا يتم نسخ شروط التعاقد التي تستند إلى المنتج والتي تم تأكيدها في السابق.</span><span class="sxs-lookup"><span data-stu-id="47872-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="47872-118">لا يتم دعم معالجة التصحيحات على فاتورة مشروع تستند إلى منتج.</span><span class="sxs-lookup"><span data-stu-id="47872-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="47872-119">تتم دائمًا معالجه تصحيحات المراحل الرئيسية كأرصدة كاملة.</span><span class="sxs-lookup"><span data-stu-id="47872-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="47872-120">يمكن تصحيح مقدم الأتعاب أو السلفة إذا تمت فوترة العميل بمبلغ غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="47872-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="47872-121">يمكن تصحيح تسويات مقدم الأتعاب والسلف إذا تم استخدام مبلغ غير صحيح للتسوية في مقابل الرسوم في فاتورة مؤكدة سابقًا.</span><span class="sxs-lookup"><span data-stu-id="47872-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="47872-122">تم تعيين حقل **التصحيح** إلى **نعم** في تفاصيل بنود الفواتير التي تعتبر تصحيحات لرسوم تمت فوترها في السابق.</span><span class="sxs-lookup"><span data-stu-id="47872-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="47872-123">تتضمن الفواتير ذات تفاصيل بنود فواتير مصححة حقلاً يسمى **لديه تصحيحات** معينًا أيضًا إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="47872-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="47872-124">القيم الفعلية التي يتم إنشاؤها عند تأكيد فاتورة تصحيحية</span><span class="sxs-lookup"><span data-stu-id="47872-124">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="47872-125">يسرد الجدول التالي القيم الفعلية التي يتم إنشاؤها عند تأكيد فاتورة تصحيحية.</span><span class="sxs-lookup"><span data-stu-id="47872-125">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="47872-126">
                    <strong>السيناريو</strong>
                </span><span class="sxs-lookup"><span data-stu-id="47872-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="47872-127">
                    <strong>القيم الفعلية المنشأة عند التأكيد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="47872-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="47872-128">تأكيد تصحيح سلفة أو مقدم أتعاب مفوترة.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="47872-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-129">إلغاء مبيعات غير مفوترة لمقدم الأتعاب أو السلفة التي تم إنشاؤها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="47872-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="47872-130">يكون هذا المبلغ موجبًا لأنه معد لإلغاء المبلغ السالب الذي تم إنشاؤه عند فوترة السلف أو مقدم الأتعاب.</span><span class="sxs-lookup"><span data-stu-id="47872-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-131">يتم إنشاء قيمة فعلية لإلغاء المبيعات المفوترة للمبلغ على السلفة أو مقدم الأتعاب لإلغاء المبيعات الأصلية المفوترة.</span><span class="sxs-lookup"><span data-stu-id="47872-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-132">يتم إنشاء قيمة فعلية جديدة للمبيعات المفوترة للمبلغ المصحح على مقدم الأتعاب أو بنود الفاتورة المصححة القائمة على السلفة.</span><span class="sxs-lookup"><span data-stu-id="47872-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-133">قيمة فعلية للمبيعات غير المفوترة للمبلغ السالب لمقدم الأتعاب أو بنود الفاتورة المصححة القائمة على السلفة، التي سيتم استخدامها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="47872-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="47872-134">تأكيد تصحيح سلفة أو مقدم أتعاب تمت تسويته في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-135">إلغاء مبيعات غير مفوترة لمقدم الأتعاب أو السلفة التي تم إنشاؤها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="47872-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="47872-136">يكون هذا المبلغ موجبًا وهو معد لإلغاء المبلغ السالب الذي تم إنشاؤه عند حدوث التسوية السابقة.</span><span class="sxs-lookup"><span data-stu-id="47872-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-137">القيمة الفعلية لإلغاء مبيعات مفوترة للمبلغ على الفاتورة السابقة.</span><span class="sxs-lookup"><span data-stu-id="47872-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-138">قيمة فعلية جديدة للمبيعات المفوترة للمبلغ المصحح على مقدم الأتعاب المطبق على الفاتورة المصححة.</span><span class="sxs-lookup"><span data-stu-id="47872-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-139">قيمة فعلية للمبيعات غير المفوترة مع مبلغ سالب من السلفة أو مقدم الأتعاب المتبقية والمصححة، التي سيتم استخدامها للتسوية على الفواتير اللاحقة.</span><span class="sxs-lookup"><span data-stu-id="47872-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="47872-140">فوترة الرصيد الكامل لحركة وقت تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-141">إلغاء مبيعات مفوترة للساعات والمبلغ في تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="47872-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-142">قيمة فعلية جديدة للمبيعات غير المفوترة للساعات والمبلغ في تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="47872-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="47872-143">فوترة الرصيد الجزئي على حركة الوقت.</span><span class="sxs-lookup"><span data-stu-id="47872-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-144">إلغاء مبيعات مفوترة للساعات والمبلغ المفوترة على تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="47872-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-145">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="47872-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-146">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والساعات المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="47872-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="47872-147">فوترة الرصيد الكامل لحركة مصروفات تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-148">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="47872-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-149">قيمة فعلية جديدة للمبيعات غير المفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="47872-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="47872-150">فوترة الرصيد الجزئي لحركة مصروفات تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-151">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="47872-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-152">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة المصححة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="47872-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-153">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والكمية المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="47872-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="47872-154">فوترة الرصيد الكامل لحركة مواد مفوترة في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-154">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-155">عكس مبيعات مفوترة للكمية والمبلغ في تفاصيل بند الفاتورة الأصلية للمواد.</span><span class="sxs-lookup"><span data-stu-id="47872-155">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-156">قيمة مبيعات فعلية جديدة غير مفوترة للكمية والمبلغ في تفاصيل بند الفاتورة الأصلية للمواد.</span><span class="sxs-lookup"><span data-stu-id="47872-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="47872-157">فوترة الرصيد الجزئي في حركة مواد.</span><span class="sxs-lookup"><span data-stu-id="47872-157">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-158">عكس مبيعات مفوترة للكمية والمبلغ المفوتر على بند الفاتورة الأصلية للمواد.</span><span class="sxs-lookup"><span data-stu-id="47872-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-159">قيمة مبيعات فعلية جديدة غير مفوترة خاضعة للرسوم للكمية والمبلغ في تفاصيل بند الفاتورة المعدّلة، وعكس هذه القيمة، وقيمة مبيعات فعلية مكافئة مفوترة.</span><span class="sxs-lookup"><span data-stu-id="47872-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-160">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والكمية المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="47872-160">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="47872-161">فوترة الرصيد الكامل لحركة رسوم تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-161">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-162">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="47872-162">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-163">قيمة فعلية جديدة للمبيعات غير المفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="47872-163">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="47872-164">فوترة الرصيد الجزئي لحركة رسوم تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-164">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-165">إلغاء مبيعات مفوترة للكمية والمبلغ المفوتر على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="47872-165">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-166">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة التصحيحية المعدلة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="47872-166">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="47872-167">فوترة الرصيد الكامل لمرحلة رئيسية تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-167">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-168">إلغاء مبيعات مفوترة للمبلغ في تفاصيل بند الفاتورة الأصلية للمرحلة الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="47872-168">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="47872-169">يتم تحديث حالة الفاتورة للمرحلة الرئيسية من <b>فاتورة عميل مرحَّلة‬</b> إلى <b>جاهز للفوترة</b>.</span><span class="sxs-lookup"><span data-stu-id="47872-169">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="47872-170">فوترة الرصيد الجزئي لمرحلة رئيسية تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-170">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-171">غير مدعوم</span><span class="sxs-lookup"><span data-stu-id="47872-171">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="47872-172">الأرصدة والتصحيحات لشروط تعاقد مستندة إلى مشروع تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="47872-172">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="47872-173">غير مدعوم</span><span class="sxs-lookup"><span data-stu-id="47872-173">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
