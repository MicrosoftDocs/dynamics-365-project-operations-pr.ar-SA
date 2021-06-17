---
title: إنشاء فواتير تصحيحية قائمة على المشروع
description: يوفر هذا الموضوع معلومات حول الفواتير التصحيحية في Project Operations.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f0423fe9895b91431b2a83a8fff81118205b0736
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001590"
---
# <a name="create-corrective-project-based-invoices"></a><span data-ttu-id="f735f-103">إنشاء فواتير تصحيحية قائمة على المشروع</span><span class="sxs-lookup"><span data-stu-id="f735f-103">Create corrective project-based invoices</span></span> 

<span data-ttu-id="f735f-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="f735f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f735f-105">يمكن تصحيح فاتورة مشروع مؤكدة لمعالجة التغييرات أو الأرصدة نتيجة التفاوض مع العميل ومدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="f735f-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="f735f-106">لإجراء عمليات تحرير على فاتورة مؤكدة، افتح الفاتورة المؤكدة وحدد **تصحيح هذه الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="f735f-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="f735f-107">لا يتوفر هذا التحديد ما لم يتم تأكيد فاتورة المشروع.</span><span class="sxs-lookup"><span data-stu-id="f735f-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="f735f-108">يتم إنشاء فاتورة مسودة جديدة من الفاتورة المؤكدة.</span><span class="sxs-lookup"><span data-stu-id="f735f-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="f735f-109">يتم نسخ كافة تفاصيل بنود الفاتورة من الفاتورة المؤكدة في السابق إلى المسودة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="f735f-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="f735f-110">فيما يلي بعض النقاط الأساسية لمساعدتك في فهم المزيد حول تفاصيل البنود في الفاتورة الجديدة التي تم تصحيحها:</span><span class="sxs-lookup"><span data-stu-id="f735f-110">The following are some key points to help you understand more about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="f735f-111">يتم تحديث جميع الكميات إلى صفر.</span><span class="sxs-lookup"><span data-stu-id="f735f-111">All quantities are updated to zero.</span></span> <span data-ttu-id="f735f-112">يفترض ذلك أن جميع العناصر المفوترة تم تقييدها للحساب بالكامل.</span><span class="sxs-lookup"><span data-stu-id="f735f-112">This assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="f735f-113">عند الضرورة، يمكنك تحديث هذه الكميات يدويًا لتعكس الكمية التي تجري فوترتها، وليس الكمية التي يجري تقييدها في الحساب.</span><span class="sxs-lookup"><span data-stu-id="f735f-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="f735f-114">استنادًا إلى الكمية التي تقوم بإدخالها، يحتسب التطبيق الكمية المقيدة في الحساب.</span><span class="sxs-lookup"><span data-stu-id="f735f-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="f735f-115">ويظهر هذا المبلغ في القيم الفعلية التي يتم إنشاؤها عند تأكيد الفاتورة المصححة.</span><span class="sxs-lookup"><span data-stu-id="f735f-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="f735f-116">إذا كنت تجري تغييرات على مبلغ الضريبة، فيجب عليك إدخال مبلغ الضريبة الصحيح وليس مبلغ الضريبة الذي يجري تقييده في الحساب.</span><span class="sxs-lookup"><span data-stu-id="f735f-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="f735f-117">تتم دائمًا معالجه تصحيحات المراحل الرئيسية كأرصدة كاملة.</span><span class="sxs-lookup"><span data-stu-id="f735f-117">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="f735f-118">يمكن تصحيح مقدم الأتعاب أو السلفة إذا تمت فوترة العميل بمبلغ غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="f735f-118">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="f735f-119">يمكن تصحيح تسويات مقدم الأتعاب والسلف إذا تم استخدام مبلغ غير صحيح للتسوية في مقابل الرسوم في فاتورة مؤكدة سابقًا.</span><span class="sxs-lookup"><span data-stu-id="f735f-119">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f735f-120">تفاصيل بنود الفاتورة التي تُعد تصحيحات لمصاريف أخرى مفوترة لديه حقل **التصحيح** معين إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="f735f-120">Invoice line details that are corrections to other already invoiced charges have the **Correction** field set to **Yes**.</span></span> <span data-ttu-id="f735f-121">تتضمن الفواتير ذات تفاصيل بنود فواتير مصححة حقلاً يسمى **لديه تصحيحات** معينًا أيضًا إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="f735f-121">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="f735f-122">القيم الفعلية التي تم إنشاؤها عند تأكيد فاتورة تصحيحية</span><span class="sxs-lookup"><span data-stu-id="f735f-122">Actuals created on confirmation of a corrective invoice</span></span>

<span data-ttu-id="f735f-123">يسرد الجدول التالي القيم الفعلية التي يتم إنشاؤها عند تأكيد فاتورة تصحيحية.</span><span class="sxs-lookup"><span data-stu-id="f735f-123">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="f735f-124">
                    <strong>السيناريو</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f735f-124">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="f735f-125">
                    <strong>القيم الفعلية المنشأة عند التأكيد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f735f-125">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="f735f-126">تأكيد تصحيح سلفة أو مقدم أتعاب مفوترة.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="f735f-126">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-127">إلغاء مبيعات غير مفوترة لمقدم الأتعاب أو السلفة التي تم إنشاؤها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="f735f-127">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="f735f-128">يكون هذا المبلغ موجبًا لأنه معد لإلغاء المبلغ السالب الذي تم إنشاؤه عند فوترة السلف أو مقدم الأتعاب.</span><span class="sxs-lookup"><span data-stu-id="f735f-128">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-129">يتم إنشاء قيمة فعلية لإلغاء المبيعات المفوترة للمبلغ على السلفة أو مقدم الأتعاب لإلغاء المبيعات الأصلية المفوترة.</span><span class="sxs-lookup"><span data-stu-id="f735f-129">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-130">يتم إنشاء قيمة فعلية جديدة للمبيعات المفوترة للمبلغ المصحح على مقدم الأتعاب أو بنود الفاتورة المصححة القائمة على السلفة.</span><span class="sxs-lookup"><span data-stu-id="f735f-130">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-131">قيمة فعلية للمبيعات غير المفوترة للمبلغ السالب لمقدم الأتعاب أو بنود الفاتورة المصححة القائمة على السلفة، التي سيتم استخدامها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="f735f-131">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="f735f-132">تأكيد تصحيح سلفة أو مقدم أتعاب تمت تسويته في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="f735f-132">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-133">إلغاء مبيعات غير مفوترة لمقدم الأتعاب أو السلفة التي تم إنشاؤها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="f735f-133">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="f735f-134">يكون هذا المبلغ موجبًا وهو معد لإلغاء المبلغ السالب الذي تم إنشاؤه عند حدوث التسوية السابقة.</span><span class="sxs-lookup"><span data-stu-id="f735f-134">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-135">القيمة الفعلية لإلغاء مبيعات مفوترة للمبلغ على الفاتورة السابقة.</span><span class="sxs-lookup"><span data-stu-id="f735f-135">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-136">قيمة فعلية جديدة للمبيعات المفوترة للمبلغ المصحح على مقدم الأتعاب المطبق على الفاتورة المصححة.</span><span class="sxs-lookup"><span data-stu-id="f735f-136">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-137">قيمة فعلية للمبيعات غير المفوترة مع مبلغ سالب من السلفة أو مقدم الأتعاب المتبقية والمصححة، التي سيتم استخدامها للتسوية على الفواتير اللاحقة.</span><span class="sxs-lookup"><span data-stu-id="f735f-137">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f735f-138">فوترة الرصيد الكامل لحركة وقت تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="f735f-138">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-139">إلغاء مبيعات مفوترة للساعات والمبلغ في تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="f735f-139">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-140">قيمة فعلية جديدة للمبيعات غير المفوترة للساعات والمبلغ في تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="f735f-140">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="f735f-141">فوترة الرصيد الجزئي على حركة الوقت.</span><span class="sxs-lookup"><span data-stu-id="f735f-141">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-142">إلغاء مبيعات مفوترة للساعات والمبلغ المفوترة على تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="f735f-142">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-143">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="f735f-143">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-144">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والساعات المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="f735f-144">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f735f-145">فوترة الرصيد الكامل لحركة مصروفات تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="f735f-145">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-146">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="f735f-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-147">قيمة فعلية جديدة للمبيعات غير المفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="f735f-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="f735f-148">فوترة الرصيد الجزئي لحركة مصروفات تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="f735f-148">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-149">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="f735f-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-150">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة المصححة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="f735f-150">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-151">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والكمية المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="f735f-151">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f735f-152">فوترة الرصيد الكامل لحركة رسوم تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="f735f-152">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-153">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="f735f-153">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-154">قيمة فعلية جديدة للمبيعات غير المفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="f735f-154">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f735f-155">فوترة الرصيد الجزئي لحركة رسوم تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="f735f-155">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-156">إلغاء مبيعات مفوترة للكمية والمبلغ المفوتر على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="f735f-156">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-157">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة التصحيحية المعدلة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="f735f-157">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="f735f-158">فوترة الرصيد الكامل لمرحلة رئيسية تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="f735f-158">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-159">إلغاء مبيعات مفوترة للمبلغ في تفاصيل بند الفاتورة الأصلية للمرحلة الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="f735f-159">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="f735f-160">يتم تحديث حالة الفاتورة للمرحلة الرئيسية من <b>فاتورة عميل مرحَّلة‬</b> إلى <b>جاهز للفوترة</b>.</span><span class="sxs-lookup"><span data-stu-id="f735f-160">The invoice status on the milestone is updated from <b>Customer invoice posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="f735f-161">فوترة الرصيد الجزئي لمرحلة رئيسية تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="f735f-161">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f735f-162">غير مدعوم</span><span class="sxs-lookup"><span data-stu-id="f735f-162">Unsupported</span></span> </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
