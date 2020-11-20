---
title: تأكيد فاتورة أولية - خفيف
description: يوفر هذا الموضوع معلومات حول تأكيد الفواتير الأولية في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 02b671e4ad327b2448529d7119211613f3a9cb27
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176505"
---
# <a name="confirm-a-proforma-invoice---lite"></a><span data-ttu-id="b9bd9-103">تأكيد فاتورة أولية - خفيف</span><span class="sxs-lookup"><span data-stu-id="b9bd9-103">Confirm a proforma invoice - lite</span></span>

<span data-ttu-id="b9bd9-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="b9bd9-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="b9bd9-105">بعد تأكيد فاتورة أولية، يتم تحديث حالة فاتورة المشروع إلى **مؤكدة**.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="b9bd9-106">عندما يتم تأكيد الفاتورة، تصبح للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="b9bd9-107">بعد ذلك، يمكن تصحيح الفاتورة فقط في حال وجود أي تصحيحات أو اعتمادات بدأها العميل أو عند تمييز الفاتورة كمدفوعة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, of if the invoice is marked as paid.</span></span>

<span data-ttu-id="b9bd9-108">يسرد الجدول التالي القيم الفعلية التي أنشأها النظام.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="b9bd9-109">يتم إنشاء هذه القيم الفعلية عند تنفيذ عمليات معينة على مسودة فاتورة المشروع قبل تأكيدها.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="b9bd9-110">
                    <strong>السيناريو</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b9bd9-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="b9bd9-111">
                    <strong>القيم الفعلية المنشأة عند التأكيد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b9bd9-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9bd9-112">فوترة سلفة أو مقدم الأتعاب</span><span class="sxs-lookup"><span data-stu-id="b9bd9-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-113">يتم إنشاء قيمة فعلية لمبيعات مفوترة من النوع <strong>مقدم الأتعاب</strong> بالمبلغ على السلفة أو مقدم الأتعاب.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-114">قيمة فعلية للمبيعات غير المفوترة للمبلغ السالب لمقدم الأتعاب أو السلفة التي سيتم استخدامها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9bd9-115">بعد إجراء تسوية كاملة لمقدم أتعاب أو سلفة على فاتورة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-116">إلغاء مبيعات غير مفوترة لمقدم الأتعاب أو السلفة التي تم إنشاؤها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="b9bd9-117">يكون هذا المبلغ موجبًا لأنه معد لإلغاء المبلغ السالب الذي تم إنشاؤه عند فوترة السلف أو مقدم الأتعاب.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-118">القيمة الفعلية للمبيعات المفوترة للمبلغ على هذه الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="b9bd9-119">بعد إجراء تسوية جزئية لمقدم أتعاب أو سلفة على فاتورة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-120">إلغاء مبيعات غير مفوترة لمقدم الأتعاب أو السلفة التي تم إنشاؤها للتسوية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="b9bd9-121">يكون هذا المبلغ موجبًا لأنه معد لإلغاء المبلغ السالب الذي تم إنشاؤه عند فوترة السلف أو مقدم الأتعاب.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-122">القيمة الفعلية للمبيعات المفوترة للمبلغ على هذه الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-123">قيمة فعلية سالبة للمبيعات غير المفوترة للمبلغ المتبقي للسلفة أو مقدم الأتعاب الذي سيتم استخدامه على الفواتير المستقبلية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9bd9-124">فوترة حركة وقت دون أي عمليات تحرير على مسودة الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-125">إلغاء مبيعات غير مفوترة للساعات والمبلغ في الموافقة على الوقت الأصلي.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-126">قيمة فعلية للمبيعات المفوترة للساعات والمبلغ في الموافقة على الوقت الأصلي.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="b9bd9-127">فوترة حركة وقت تم تحريرها لتقليل الكمية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-128">إلغاء مبيعات غير مفوترة للساعات والمبلغ في الموافقة على الوقت الأصلي.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-129">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-130">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات المتبقية والمبلغ المتبقي بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9bd9-131">فوترة حركة وقت تم تحريرها لزيادة الكمية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-132">إلغاء مبيعات غير مفوترة للساعات والمبلغ في الموافقة على الوقت الأصلي.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-133">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9bd9-134">فوترة حركة مصروفات دون أي عمليات تحرير على مسودة الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-135">إلغاء مبيعات غير مفوترة للكمية والمبلغ في الموافقة على المصروفات الأصلية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-136">القيمة الفعلية للمبيعات المفوترة للكمية والمبلغ في الموافقة على المصروفات الأصلية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="b9bd9-137">فوترة حركة مصروفات تم تحريرها لتقليل الكمية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-138">إلغاء مبيعات غير مفوترة للكمية والمبلغ في الموافقة على المصروفات الأصلية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-139">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-140">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع للكمية المتبقية والمبلغ المتبقي بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9bd9-141">فوترة حركة مصروفات تم تحريرها لزيادة الكمية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-142">إلغاء مبيعات غير مفوترة للكمية والمبلغ في الموافقة على المصروفات الأصلية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-143">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9bd9-144">فوترة الرسوم.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-144">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-145">إلغاء مبيعات غير مفوترة لمبلغ الرسوم في سطر دفتر اليومية الأصلي.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-145">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-146">القيمة الفعلية للمبيعات المفوترة للكمية والمبلغ على سطر دفتر يومية الرسوم الأصلي.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-146">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="b9bd9-147">فوترة مرحلة رئيسية.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-147">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-148">قيمة فعلية لمبيعات مفوترة لمبلغ المرحلة الرئيسية في المرحلة الرئيسية الأصلية على شروط تعاقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-148">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="b9bd9-149">فوترة شروط التعاقد المستندة إلى المنتج</span><span class="sxs-lookup"><span data-stu-id="b9bd9-149">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9bd9-150">القيمة الفعلية للمبيعات المفوترة لبند المنتج مع الكمية والمبلغ من شروط التعاقد المستندة إلى المنتج.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-150">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
