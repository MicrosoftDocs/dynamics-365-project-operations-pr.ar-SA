---
title: إنشاء سُلفة مؤقتة في عقد
description: يقدم هذا الموضوع معلومات حول إنشاء سُلفة على عقد عند الحاجة.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 51e3b0ac8e111be70fe6ad0f9c162dfaec3339ad
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003480"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract"></a><span data-ttu-id="a6344-103">إنشاء سُلفة مؤقتة في عقد</span><span class="sxs-lookup"><span data-stu-id="a6344-103">Creating an ad hoc advance on a contract</span></span>

<span data-ttu-id="a6344-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="a6344-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a6344-105">يدعم Microsoft Dynamics 365 Project Operations سيناريوهات الفوترة التي تشتمل على الدفعات المسبقة والسُلف.</span><span class="sxs-lookup"><span data-stu-id="a6344-105">Microsoft Dynamics 365 Project Operations supports invoicing scenarios that involve pre-payments and advances.</span></span> <span data-ttu-id="a6344-106">تعتبر عملية استخدام **السُلف** في **Project Operations** مماثلة لعقود **مقدم الأتعاب**.</span><span class="sxs-lookup"><span data-stu-id="a6344-106">The process for using **Advances** in **Project Operations** is similar to **Retainer** contracts.</span></span> 

<span data-ttu-id="a6344-107">أكمل الخطوات التالية لفوترة العميل لسُلفة.</span><span class="sxs-lookup"><span data-stu-id="a6344-107">Complete the following steps to invoice the customer for an advance.</span></span>

1. <span data-ttu-id="a6344-108">انتقل إلى صفحة **عقد المشروع**، ثم حدد علامة التبويب **مقدمات الأتعاب والسُلف**.</span><span class="sxs-lookup"><span data-stu-id="a6344-108">Go to the **Project Contract** page, and then select the **Advances and Retainers** tab.</span></span>
2. <span data-ttu-id="a6344-109">في الشبكة الفرعية التي تسرد كافة السُلف والدفعات المسبقة التي تم تسجيلها في السابق، حدد **+ مقدم أتعاب مشروع جديد**.</span><span class="sxs-lookup"><span data-stu-id="a6344-109">In the subgrid that lists all the previously recorded advances and prepayments, select **+ New Project contract retainer**.</span></span> 

    <span data-ttu-id="a6344-110">عندئذ يفتح نموذج **الإنشاء السريع** لتسجيل دفعة مسبقة أو سُلفة.</span><span class="sxs-lookup"><span data-stu-id="a6344-110">The **Quick Create** form opens for recording a prepayment or advance.</span></span>
    
3. <span data-ttu-id="a6344-111">يسرد الجدول التالي الحقول الخاصة بتسجيل سُلفة والاعتبارات التي يجب مراعاتها عند إنشاء سُلفة جديدة.</span><span class="sxs-lookup"><span data-stu-id="a6344-111">The table below lists the fields for recording an advance and the considerations to keep in mind as you create new ones:</span></span>

    | <span data-ttu-id="a6344-112">الحقل</span><span class="sxs-lookup"><span data-stu-id="a6344-112">Field</span></span> | <span data-ttu-id="a6344-113">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="a6344-113">Description</span></span> | <span data-ttu-id="a6344-114">تأثير لاحق</span><span class="sxs-lookup"><span data-stu-id="a6344-114">Downstream impact</span></span> |
    | --- | --- | --- |
    | <span data-ttu-id="a6344-115">**عميل عقد المشروع**</span><span class="sxs-lookup"><span data-stu-id="a6344-115">**Project Contract Customer**</span></span> | <span data-ttu-id="a6344-116">يشير هذا الحقل إلى العميل على العقد الذي ستتم فوترته لهذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="a6344-116">This field indicates which customer on the contract will be invoiced for this advance.</span></span> | <span data-ttu-id="a6344-117">عند وجود عدد كبير من العملاء في العقد وأردت فوترة كل واحد منهم لمبلغ مقدم أتعاب أو سلفة معينة، أنشئ سلفة لكل عميل على حدة.</span><span class="sxs-lookup"><span data-stu-id="a6344-117">If you have multiple customers on the contract and want to invoice each of them for a specific retainer or advance amount, create an advance for each customer individually.</span></span> |
    | <span data-ttu-id="a6344-118">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="a6344-118">**Description**</span></span> | <span data-ttu-id="a6344-119">وصف الغرض أو وقت السلفة للمساعدة في تحديد هذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="a6344-119">The description of the purpose or timing of the advance to help identify this advance.</span></span> | <span data-ttu-id="a6344-120">يظهر هذا الوصف على سطر الفاتورة لهذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="a6344-120">This description is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="a6344-121">**المبلغ**</span><span class="sxs-lookup"><span data-stu-id="a6344-121">**Amount**</span></span> | <span data-ttu-id="a6344-122">مبلغ الدفعة المسبقة أو السلفة.</span><span class="sxs-lookup"><span data-stu-id="a6344-122">The amount for the pre-payment or advance.</span></span> | <span data-ttu-id="a6344-123">يظهر هذا المبلغ على سطر الفاتورة لهذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="a6344-123">This amount is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="a6344-124">**تاريخ الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="a6344-124">**Invoice Date**</span></span> | <span data-ttu-id="a6344-125">تاريخ فوترة هذه السلفة على العميل.</span><span class="sxs-lookup"><span data-stu-id="a6344-125">The date on which this advance is invoiced to the customer.</span></span> | <span data-ttu-id="a6344-126">هذا هو تاريخ عملية إنشاء الفواتير التلقائية لإنشاء بند فاتورة لهذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="a6344-126">This is the date for the automated invoice creation process to create an invoice line for this advance.</span></span> |
    | <span data-ttu-id="a6344-127">**حالة الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="a6344-127">**Invoice Status**</span></span> | <span data-ttu-id="a6344-128">هذا إعداد خيار يشير إلى ما إذا تمت إضافة هذه السلفة إلى مسودة فاتورة لهذا العميل.</span><span class="sxs-lookup"><span data-stu-id="a6344-128">This is an option setting that indicates whether this advance is added to a draft invoice for this customer.</span></span> <span data-ttu-id="a6344-129">فيما يلي القيم المحتملة:</span><span class="sxs-lookup"><span data-stu-id="a6344-129">The possible values are:</span></span></br><span data-ttu-id="a6344-130">- **غير جاهز للفوترة**</span><span class="sxs-lookup"><span data-stu-id="a6344-130">- **Not ready to invoice**</span></span></br><span data-ttu-id="a6344-131">- **جاهز للفوترة**</span><span class="sxs-lookup"><span data-stu-id="a6344-131">- **Ready to invoice**</span></span> | <span data-ttu-id="a6344-132">عند وضع علامة على سلفة أو دفعة مسبقة على أنها **جاهزة للفوترة**، تتم إضافتها كوقت البند على مسودة الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="a6344-132">When an advance or pre-payment is marked as **Ready to invoice**, it is added as a line time on a draft invoice.</span></span> <span data-ttu-id="a6344-133">يمكن استخدام السلفة المفوتره بالكامل فقط لإجراء التسوية في مقابل تكاليف المشروع لفتره الفاتورة القادمة.</span><span class="sxs-lookup"><span data-stu-id="a6344-133">Only a fully invoiced advance can be used to reconcile against project costs for the next invoice period.</span></span> |

4. <span data-ttu-id="a6344-134">حدد **حفظ وإغلاق** في مربع حوار الإنشاء السريع لتسجيل السلفة أو الدفعة المسبقة.</span><span class="sxs-lookup"><span data-stu-id="a6344-134">Select **Save and close** on the quick create dialog to record the advance or the pre-payment.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]