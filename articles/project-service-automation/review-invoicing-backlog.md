---
title: مراجعة تراكم الفوترة في المشاريع وعقود المشاريع
description: يقدم هذا الموضوع معلومات حول كيفية مراجعة الوقت والمصروفات وتراكم المنتجات وكيفية وضع علامة جاهز للفوترة عليها.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 03/11/2019
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 2.x and 3.x
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: db15ea136b9939c0a0631936bcadab538bf2dd4a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748704"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a><span data-ttu-id="b4b09-103">مراجعة تراكم الفوترة في المشاريع وعقود المشاريع</span><span class="sxs-lookup"><span data-stu-id="b4b09-103">Review the invoicing backlog on projects and project contracts</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b4b09-104">عندما تكون إحدى الحركات جاهزة لكي يتم إنشاء فاتورة لها ومعالجتها، فيجب وضع علامة **جاهزة للفوترة** عليها.</span><span class="sxs-lookup"><span data-stu-id="b4b09-104">When a transaction is ready to have an invoice created and processed, the transaction should be marked **Ready to invoice**.</span></span> <span data-ttu-id="b4b09-105">يوضح هذا الموضوع أنواع الحركات التي يمكن إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="b4b09-105">This topic describes the types of transactions that can be created.</span></span>

## <a name="review-the-time-and-material-billing-backlog"></a><span data-ttu-id="b4b09-106">مراجعة تراكم فوترة المواد والوقت</span><span class="sxs-lookup"><span data-stu-id="b4b09-106">Review the time and material billing backlog</span></span>

<span data-ttu-id="b4b09-107">عندما يتم تقديم إدخال الوقت أو المصروفات والموافقة عليهما لمشروع، فإن PSA يقوم بإنشاء مشروع فعلي.</span><span class="sxs-lookup"><span data-stu-id="b4b09-107">When a time or expense entry is submitted and approved for a project, PSA creates a project actual.</span></span> <span data-ttu-id="b4b09-108">إذا تم تعيين مجموعة فئات المشروع وفئة الحركة إلى بند عقد لمشروع الوقت والمواد، فسيتم إنشاء قيمتين فعليتين عند الموافقة على الإدخال:</span><span class="sxs-lookup"><span data-stu-id="b4b09-108">If the combination of the project and the transaction class are mapped to a contract line for a time-and-materials project, two actuals are created when the entry is approved:</span></span>

- <span data-ttu-id="b4b09-109">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="b4b09-109">Cost actual</span></span> 
- <span data-ttu-id="b4b09-110">المبيعات الفعلية غير المفوترة</span><span class="sxs-lookup"><span data-stu-id="b4b09-110">Unbilled sales actual</span></span>

<span data-ttu-id="b4b09-111">تمثل القيم الفعلية للمبيعات غير المفوترة تراكم الفوترة، ويجب تعيين حالة فوترتها إلى **جاهزة للفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-111">Unbilled sales actuals represent the billing backlog, and their billing status must be set to **Ready to Invoice**.</span></span> <span data-ttu-id="b4b09-112">عندما يتم إنشاء فاتورة مشروع، يتم نسخ القيم الفعلية للمبيعات غير المفوترة والتي تم تمييزها بعلامة **جاهزة للفوترة** على أنها تفاصيل بند الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="b4b09-112">When a project invoice is created, unbilled sales actuals that are marked **Ready to Invoice** are copied over as invoice line details.</span></span>

<span data-ttu-id="b4b09-113">لمراجعة تراكم الفوترة الخاص بالوقت والمواد، انتقل إلى **المبيعات**\> **الفوترة** \> **تراكم فوترة الوقت والمواد**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-113">To review the billing backlog for time and materials, go to **Sales** \> **Billing** \> **Time and Material Billing Backlog**.</span></span> <span data-ttu-id="b4b09-114">حدد كافة القيم الفعلية للمبيعات غير المفوترة والتي تكون جاهزة للفوترة، ثم حدد **جاهزة للفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-114">Select all the unbilled sales actuals that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="b4b09-115">تم تغيير حالة الفوترة لهذه القيم الفعلية إلى **جاهزة للفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-115">The billing status of these actuals is changed to **Ready to Invoice**.</span></span>

![تراكم فوترة الوقت والمواد](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a><span data-ttu-id="b4b09-117">مراجعة تراكم فوترة المنتجات</span><span class="sxs-lookup"><span data-stu-id="b4b09-117">Review the product billing backlog</span></span>

<span data-ttu-id="b4b09-118">في PSA، عندما يكون لعقد مشروع بنود عقد مستندة إلى المنتج، تتم مراعاة هذه البنود للفوترة عندما يتم إنشاء فاتورة لعقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="b4b09-118">In PSA, when a project contract has product-based contract lines, those lines are considered for invoicing whenever an invoice is created for the project contract.</span></span> <span data-ttu-id="b4b09-119">يتم نسخ أي منتج له بنود عقد تم تمييزه بعلامة **جاهز للفوترة** إلى فاتورة المشروع مثل بنود فاتورة المشروع.</span><span class="sxs-lookup"><span data-stu-id="b4b09-119">Any product that has contract lines that are marked **Ready to Invoice** is copied over to the project invoice as project invoice lines.</span></span>

<span data-ttu-id="b4b09-120">لمراجعة تراكم الفوترة للمنتجات، انتقل إلى **المبيعات** \>**فوترة**\> **تراكم فوترة المنتج**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-120">To review the billing backlog for products, go to **Sales** \> **Billing** \> **Product Billing Backlog**.</span></span> <span data-ttu-id="b4b09-121">حدد جميع بنود العقد المستندة إلى المنتج والتي تكون جاهزة للفوترة، ثم حدد **جاهزة للفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-121">Select all the product-based contract lines that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="b4b09-122">تم تغيير حالة الفوترة لهذه البنود إلى **جاهزة للفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-122">The billing status of these lines is changed to **Ready to Invoice**.</span></span>

![تراكم فوترة المنتجات](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a><span data-ttu-id="b4b09-124">مراجعة المراحل الرئيسية للفوترة في عقود السعر الثابت</span><span class="sxs-lookup"><span data-stu-id="b4b09-124">Review billing milestones on fixed-price contracts</span></span>

<span data-ttu-id="b4b09-125">يجب أن يحدد كل بند عقد مشروع له أسلوب فوترة ثابت السعر المراحل الرئيسية للعقد.</span><span class="sxs-lookup"><span data-stu-id="b4b09-125">Each project contract line that has a fixed-price billing method must define contract milestones.</span></span> <span data-ttu-id="b4b09-126">ويمكن فوترة المراحل الرئيسية للعقد هذه فقط إذا تم تمييزها بعلامة **جاهزة للفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-126">These contract milestones can be invoiced only if they are marked **Ready to Invoice**.</span></span> 

<span data-ttu-id="b4b09-127">لمراجعة المراحل الرئيسية للفوترة، انتقل إلى **المبيعات**\> **الفوترة**\> **المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-127">To review billing milestones, go to **Sales** \> **Billing** \> **Fixed Price Milestones**.</span></span> <span data-ttu-id="b4b09-128">حدد المراحل الرئيسية الجاهزة للفوترة، ثم حدد **جاهزة للفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-128">Select the milestones that are ready to be invoiced, and then select **Ready to invoice**.</span></span> <span data-ttu-id="b4b09-129">تم تغيير حالة الفوترة لهذه المراحل الرئيسية إلى **جاهزة للفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b4b09-129">The billing status of these milestones is changed to **Ready to Invoice**.</span></span>

![المراحل الرئيسية للأسعار الثابتة](media/FPBacklog.png)
