---
title: إنشاء سُلفة مؤقتة على عقد - خفيف
description: يقدم هذا الموضوع معلومات حول إنشاء سُلفة على عقد عند الحاجة.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a6bf02c2e2ab2f3c696b1eab1b92a20272187bf5
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181346"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract---lite"></a><span data-ttu-id="bfa97-103">إنشاء سُلفة مؤقتة على عقد - خفيف</span><span class="sxs-lookup"><span data-stu-id="bfa97-103">Creating an ad hoc advance on a contract - lite</span></span>

<span data-ttu-id="bfa97-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="bfa97-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bfa97-105">يدعم Microsoft Dynamics 365 Project Operations سيناريوهات الفوترة التي تشتمل على الدفعات المسبقة والسُلف.</span><span class="sxs-lookup"><span data-stu-id="bfa97-105">Microsoft Dynamics 365 Project Operations supports invoicing scenarios that involve pre-payments and advances.</span></span> <span data-ttu-id="bfa97-106">تعتبر عملية استخدام **السُلف** في **Project Operations** مماثلة لعقود **مقدم الأتعاب**.</span><span class="sxs-lookup"><span data-stu-id="bfa97-106">The process for using **Advances** in **Project Operations** is similar to **Retainer** contracts.</span></span> 

<span data-ttu-id="bfa97-107">أكمل الخطوات التالية لفوترة العميل لسُلفة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-107">Complete the following steps to invoice the customer for an advance.</span></span>

1. <span data-ttu-id="bfa97-108">انتقل إلى صفحة **عقد المشروع**، ثم حدد علامة التبويب **مقدمات الأتعاب والسُلف**.</span><span class="sxs-lookup"><span data-stu-id="bfa97-108">Go to the **Project Contract** page, and then select the **Advances and Retainers** tab.</span></span>
2. <span data-ttu-id="bfa97-109">في الشبكة الفرعية التي تسرد كافة السُلف والدفعات المسبقة التي تم تسجيلها في السابق، حدد **+ مقدم أتعاب مشروع جديد**.</span><span class="sxs-lookup"><span data-stu-id="bfa97-109">In the subgrid that lists all the previously recorded advances and prepayments, select **+ New Project contract retainer**.</span></span> 

    <span data-ttu-id="bfa97-110">عندئذ يفتح نموذج **الإنشاء السريع** لتسجيل دفعة مسبقة أو سُلفة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-110">The **Quick Create** form opens for recording a prepayment or advance.</span></span>
    
3. <span data-ttu-id="bfa97-111">يسرد الجدول التالي الحقول الخاصة بتسجيل سُلفة والاعتبارات التي يجب مراعاتها عند إنشاء سُلفة جديدة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-111">The table below lists the fields for recording an advance and the considerations to keep in mind as you create new ones:</span></span>

    | <span data-ttu-id="bfa97-112">الحقل</span><span class="sxs-lookup"><span data-stu-id="bfa97-112">Field</span></span> | <span data-ttu-id="bfa97-113">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="bfa97-113">Description</span></span> | <span data-ttu-id="bfa97-114">تأثير لاحق</span><span class="sxs-lookup"><span data-stu-id="bfa97-114">Downstream impact</span></span> |
    | --- | --- | --- |
    | <span data-ttu-id="bfa97-115">**عميل عقد المشروع**</span><span class="sxs-lookup"><span data-stu-id="bfa97-115">**Project Contract Customer**</span></span> | <span data-ttu-id="bfa97-116">يشير هذا الحقل إلى العميل على العقد الذي ستتم فوترته لهذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-116">This field indicates which customer on the contract will be invoiced for this advance.</span></span> | <span data-ttu-id="bfa97-117">عند وجود عدد كبير من العملاء في العقد وأردت فوترة كل واحد منهم لمبلغ مقدم أتعاب أو سلفة معينة، أنشئ سلفة لكل عميل على حدة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-117">If you have multiple customers on the contract and want to invoice each of them for a specific retainer or advance amount, create an advance for each customer individually.</span></span> |
    | <span data-ttu-id="bfa97-118">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="bfa97-118">**Description**</span></span> | <span data-ttu-id="bfa97-119">وصف الغرض أو وقت السلفة للمساعدة في تحديد هذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-119">The description of the purpose or timing of the advance to help identify this advance.</span></span> | <span data-ttu-id="bfa97-120">يظهر هذا الوصف على سطر الفاتورة لهذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-120">This description is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="bfa97-121">**المبلغ**</span><span class="sxs-lookup"><span data-stu-id="bfa97-121">**Amount**</span></span> | <span data-ttu-id="bfa97-122">مبلغ الدفعة المسبقة أو السلفة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-122">The amount for the pre-payment or advance.</span></span> | <span data-ttu-id="bfa97-123">يظهر هذا المبلغ على سطر الفاتورة لهذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-123">This amount is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="bfa97-124">**تاريخ الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="bfa97-124">**Invoice Date**</span></span> | <span data-ttu-id="bfa97-125">تاريخ فوترة هذه السلفة على العميل.</span><span class="sxs-lookup"><span data-stu-id="bfa97-125">The date on which this advance is invoiced to the customer.</span></span> | <span data-ttu-id="bfa97-126">هذا هو تاريخ عملية إنشاء الفواتير التلقائية لإنشاء بند فاتورة لهذه السلفة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-126">This is the date for the automated invoice creation process to create an invoice line for this advance.</span></span> |
    | <span data-ttu-id="bfa97-127">**حالة الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="bfa97-127">**Invoice Status**</span></span> | <span data-ttu-id="bfa97-128">هذا إعداد خيار يشير إلى ما إذا تمت إضافة هذه السلفة إلى مسودة فاتورة لهذا العميل.</span><span class="sxs-lookup"><span data-stu-id="bfa97-128">This is an option setting that indicates whether this advance is added to a draft invoice for this customer.</span></span> <span data-ttu-id="bfa97-129">فيما يلي القيم المحتملة:</span><span class="sxs-lookup"><span data-stu-id="bfa97-129">The possible values are:</span></span></br><span data-ttu-id="bfa97-130">- **غير جاهز للفوترة**</span><span class="sxs-lookup"><span data-stu-id="bfa97-130">- **Not ready to invoice**</span></span></br><span data-ttu-id="bfa97-131">- **جاهز للفوترة**</span><span class="sxs-lookup"><span data-stu-id="bfa97-131">- **Ready to invoice**</span></span> | <span data-ttu-id="bfa97-132">عند وضع علامة على سلفة أو دفعة مسبقة على أنها **جاهزة للفوترة**، تتم إضافتها كوقت البند على مسودة الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-132">When an advance or pre-payment is marked as **Ready to invoice**, it is added as a line time on a draft invoice.</span></span> <span data-ttu-id="bfa97-133">يمكن استخدام السلفة المفوتره بالكامل فقط لإجراء التسوية في مقابل تكاليف المشروع لفتره الفاتورة القادمة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-133">Only a fully invoiced advance can be used to reconcile against project costs for the next invoice period.</span></span> |

4. <span data-ttu-id="bfa97-134">حدد **حفظ وإغلاق** في مربع حوار الإنشاء السريع لتسجيل السلفة أو الدفعة المسبقة.</span><span class="sxs-lookup"><span data-stu-id="bfa97-134">Select **Save and close** on the quick create dialog to record the advance or the pre-payment.</span></span>
