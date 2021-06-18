---
title: فواتير تصحيحية قائمة على المشروع
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء الفواتير التصحيحية القائمة على المشروع وتأكيدها في Project Operations.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6b6670f823577bf7f784443f97f0b77e1e9a6aa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012255"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="e6829-103">فواتير تصحيحية قائمة على المشروع</span><span class="sxs-lookup"><span data-stu-id="e6829-103">Corrective project-based invoices</span></span>

<span data-ttu-id="e6829-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="e6829-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e6829-105">يمكن تصحيح فاتورة مشروع مؤكدة لمعالجة التغييرات أو الأرصدة نتيجة التفاوض مع العميل ومدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="e6829-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="e6829-106">لإجراء عمليات تحرير على فاتورة مؤكدة، افتح الفاتورة المؤكدة وحدد **تصحيح هذه الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="e6829-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="e6829-107">لا يتوفر هذا التحديد ما لم يتم تأكيد فاتورة المشروع أو إذا كانت الفاتورة التي تستند إلى المشروع تتضمن مقدمات الأتعاب أو السُلف أو تسويات مقدمات الأتعاب أو السُلف.</span><span class="sxs-lookup"><span data-stu-id="e6829-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="e6829-108">يتم إنشاء فاتورة مسودة جديدة من الفاتورة المؤكدة.</span><span class="sxs-lookup"><span data-stu-id="e6829-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="e6829-109">يتم نسخ كافة تفاصيل بنود الفاتورة من الفاتورة المؤكدة في السابق إلى المسودة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="e6829-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="e6829-110">فيما يلي بعض النقاط الأساسية للتعرف على تفاصيل البنود في الفاتورة الجديدة التي تم تصحيحها:</span><span class="sxs-lookup"><span data-stu-id="e6829-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="e6829-111">يتم تحديث جميع الكميات إلى صفر.</span><span class="sxs-lookup"><span data-stu-id="e6829-111">All quantities are updated to zero.</span></span> <span data-ttu-id="e6829-112">يفترض Dynamics 365 Project Operations أن جميع العناصر المفوترة تم تقييدها للحساب بالكامل.</span><span class="sxs-lookup"><span data-stu-id="e6829-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="e6829-113">عند الضرورة، يمكنك تحديث هذه الكميات يدويًا لتعكس الكمية التي تجري فوترتها، وليس الكمية التي يجري تقييدها في الحساب.</span><span class="sxs-lookup"><span data-stu-id="e6829-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="e6829-114">استنادًا إلى الكمية التي تقوم بإدخالها، يحتسب التطبيق الكمية المقيدة في الحساب.</span><span class="sxs-lookup"><span data-stu-id="e6829-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="e6829-115">ويظهر هذا المبلغ في القيم الفعلية التي يتم إنشاؤها عند تأكيد الفاتورة المصححة.</span><span class="sxs-lookup"><span data-stu-id="e6829-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="e6829-116">إذا كنت تجري تغييرات على مبلغ الضريبة، فيجب عليك إدخال مبلغ الضريبة الصحيح وليس مبلغ الضريبة الذي يجري تقييده في الحساب.</span><span class="sxs-lookup"><span data-stu-id="e6829-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="e6829-117">تتم دائمًا معالجه تصحيحات المراحل الرئيسية كأرصدة كاملة.</span><span class="sxs-lookup"><span data-stu-id="e6829-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="e6829-118">بالنسبة إلى تفاصيل بنود الفاتورة التي تُعد تصحيحات لمصاريف أخرى مفوترة، يتم تعيين حقل **التصحيح** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e6829-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="e6829-119">بالنسبة إلى الفواتير التي تتضمن تفاصيل بنود تصحيحية، يتم تعيين حقل **له تصحيحات‬** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e6829-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="e6829-120">القيم الفعلية التي يتم إنشاؤها عند تأكيد فاتورة تصحيحية</span><span class="sxs-lookup"><span data-stu-id="e6829-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="e6829-121">يسرد الجدول التالي القيم الفعلية التي يتم إنشاؤها عند تأكيد فاتورة تصحيحية.</span><span class="sxs-lookup"><span data-stu-id="e6829-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="e6829-122">
                    <strong>السيناريو</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e6829-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="e6829-123">
                    <strong>القيم الفعلية المنشأة عند التأكيد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e6829-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e6829-124">فوترة الرصيد الكامل لحركة وقت تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e6829-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-125">إلغاء مبيعات مفوترة للساعات والمبلغ في تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="e6829-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-126">قيمة فعلية جديدة للمبيعات غير المفوترة للساعات والمبلغ في تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="e6829-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="e6829-127">فوترة الرصيد الجزئي على حركة الوقت.</span><span class="sxs-lookup"><span data-stu-id="e6829-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-128">إلغاء مبيعات مفوترة للساعات والمبلغ المفوترة على تفاصيل بند الفاتورة الأصلية للوقت.</span><span class="sxs-lookup"><span data-stu-id="e6829-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-129">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="e6829-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-130">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والساعات المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="e6829-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e6829-131">فوترة الرصيد الكامل لحركة مصروفات تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e6829-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-132">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="e6829-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-133">قيمة فعلية جديدة للمبيعات غير المفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="e6829-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="e6829-134">فوترة الرصيد الجزئي لحركة مصروفات تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e6829-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-135">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="e6829-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-136">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة المصححة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="e6829-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-137">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والكمية المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="e6829-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e6829-138">فوترة الرصيد الكامل لحركة مواد مفوترة في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e6829-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-139">عكس مبيعات مفوترة للكمية والمبلغ في تفاصيل بند الفاتورة الأصلية للمواد.</span><span class="sxs-lookup"><span data-stu-id="e6829-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-140">قيمة مبيعات فعلية جديدة غير مفوترة للكمية والمبلغ في تفاصيل بند الفاتورة الأصلية للمواد.</span><span class="sxs-lookup"><span data-stu-id="e6829-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="e6829-141">فوترة الرصيد الجزئي في حركة مواد.</span><span class="sxs-lookup"><span data-stu-id="e6829-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-142">عكس مبيعات مفوترة للكمية والمبلغ المفوتر على بند الفاتورة الأصلية للمواد.</span><span class="sxs-lookup"><span data-stu-id="e6829-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-143">قيمة مبيعات فعلية جديدة غير مفوترة خاضعة للرسوم للكمية والمبلغ في تفاصيل بند الفاتورة المعدّلة، وعكس هذه القيمة، وقيمة مبيعات فعلية مكافئة مفوترة.</span><span class="sxs-lookup"><span data-stu-id="e6829-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-144">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والكمية المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="e6829-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e6829-145">فوترة الرصيد الكامل لحركة رسوم تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e6829-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-146">إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="e6829-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-147">قيمة فعلية جديدة للمبيعات غير المفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="e6829-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e6829-148">فوترة الرصيد الجزئي لحركة رسوم تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e6829-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-149">إلغاء مبيعات مفوترة للكمية والمبلغ المفوتر على تفاصيل بند الفاتورة الأصلية للرسوم.</span><span class="sxs-lookup"><span data-stu-id="e6829-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-150">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة التصحيحية المعدلة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="e6829-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="e6829-151">فوترة الرصيد الكامل لمرحلة رئيسية تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e6829-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-152">إلغاء مبيعات مفوترة للمبلغ في تفاصيل بند الفاتورة الأصلية للمرحلة الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="e6829-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="e6829-153">يتم تحديث حالة الفاتورة للمرحلة الرئيسية من <b>فاتورة عميل مرحَّلة‬</b> إلى <b>جاهز للفوترة</b>.</span><span class="sxs-lookup"><span data-stu-id="e6829-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="e6829-154">فوترة الرصيد الجزئي لمرحلة رئيسية تمت فوترتها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e6829-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e6829-155">هذا السيناريو غير مدعوم.</span><span class="sxs-lookup"><span data-stu-id="e6829-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
