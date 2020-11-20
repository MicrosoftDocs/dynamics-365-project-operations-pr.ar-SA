---
title: تأكيد فاتورة أولية
description: يقدم هذا الموضوع معلومات حول تأكيد الفاتورة الأولية.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fa1e6c17fbda76a283c2ec68760a00e846decf83
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128087"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="3fddf-103">تأكيد فاتورة أولية</span><span class="sxs-lookup"><span data-stu-id="3fddf-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="3fddf-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="3fddf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="3fddf-105">بعد تأكيد فاتورة أولية، يتم تحديث حالة فاتورة المشروع إلى **مؤكدة**.</span><span class="sxs-lookup"><span data-stu-id="3fddf-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="3fddf-106">عندما يتم تأكيد الفاتورة، تصبح للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="3fddf-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="3fddf-107">بعد ذلك، يمكن تصحيح الفاتورة فقط في حال وجود أي تصحيحات أو اعتمادات بدأها العميل أو عند تمييزها كمدفوعة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="3fddf-108">يسرد الجدول التالي القيم الفعلية التي أنشأها النظام.</span><span class="sxs-lookup"><span data-stu-id="3fddf-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="3fddf-109">يتم إنشاء هذه القيم الفعلية عند تنفيذ عمليات معينة على مسودة فاتورة المشروع قبل تأكيدها.</span><span class="sxs-lookup"><span data-stu-id="3fddf-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="3fddf-110">
                    <strong>السيناريو</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3fddf-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="3fddf-111">
                    <strong>القيم الفعلية المنشأة عند التأكيد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3fddf-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3fddf-112">فوترة حركة وقت دون أي عمليات تحرير على مسودة الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-113">إلغاء مبيعات غير مفوترة للساعات والمبلغ في الموافقة على الوقت الأصلي.</span><span class="sxs-lookup"><span data-stu-id="3fddf-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-114">قيمة فعلية للمبيعات المفوترة للساعات والمبلغ في الموافقة على الوقت الأصلي.</span><span class="sxs-lookup"><span data-stu-id="3fddf-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="3fddf-115">فوترة حركة وقت تم تحريرها لتقليل الكمية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-116">إلغاء مبيعات غير مفوترة للساعات والمبلغ في الموافقة على الوقت الأصلي.</span><span class="sxs-lookup"><span data-stu-id="3fddf-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-117">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-118">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات المتبقية والمبلغ المتبقي بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3fddf-119">فوترة حركة وقت تم تحريرها لزيادة الكمية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-120">إلغاء مبيعات غير مفوترة للساعات والمبلغ في الموافقة على الوقت الأصلي.</span><span class="sxs-lookup"><span data-stu-id="3fddf-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-121">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3fddf-122">فوترة حركة مصروفات دون أي عمليات تحرير على مسودة الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-123">إلغاء مبيعات غير مفوترة للكمية والمبلغ في الموافقة على المصروفات الأصلية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-124">القيمة الفعلية للمبيعات المفوترة للكمية والمبلغ في الموافقة على المصروفات الأصلية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="3fddf-125">فوترة حركة مصروفات تم تحريرها لتقليل الكمية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-126">إلغاء مبيعات غير مفوترة للكمية والمبلغ في الموافقة على المصروفات الأصلية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-127">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-128">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع للكمية المتبقية والمبلغ المتبقي بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3fddf-129">فوترة حركة مصروفات تم تحريرها لزيادة الكمية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-130">إلغاء مبيعات غير مفوترة للكمية والمبلغ في الموافقة على المصروفات الأصلية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-131">قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء للقيمة الفعلية للمبيعات غير المفوترة، وقيمة فعلية مكافئة للمبيعات المفوترة.</span><span class="sxs-lookup"><span data-stu-id="3fddf-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3fddf-132">فوترة الرسوم.</span><span class="sxs-lookup"><span data-stu-id="3fddf-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-133">إلغاء مبيعات غير مفوترة لمبلغ الرسوم في سطر دفتر اليومية الأصلي.</span><span class="sxs-lookup"><span data-stu-id="3fddf-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-134">القيمة الفعلية للمبيعات المفوترة للكمية والمبلغ على سطر دفتر يومية الرسوم الأصلي.</span><span class="sxs-lookup"><span data-stu-id="3fddf-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="3fddf-135">فوترة مرحلة رئيسية.</span><span class="sxs-lookup"><span data-stu-id="3fddf-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="3fddf-136">قيمة فعلية لمبيعات مفوترة لمبلغ المرحلة الرئيسية في المرحلة الرئيسية الأصلية على شروط تعاقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="3fddf-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
