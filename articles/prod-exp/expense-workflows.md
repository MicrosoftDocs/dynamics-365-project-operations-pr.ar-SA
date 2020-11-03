---
title: إعداد عمليات سير العمل لإدارة المصروفات
description: يمكنك إعداد عملية سير عمل لمراجعة مستندات المصروفات والنفقات والموافقة عليها.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0af23ed2cf172e4c90de72f5db389c349303c039
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070798"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="4ade1-103">إعداد عمليات سير العمل لإدارة المصروفات</span><span class="sxs-lookup"><span data-stu-id="4ade1-103">Set up Expense management workflows</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="4ade1-104">يمكنك إعداد عملية سير عمل يتم استخدامها لمراجعة مستندات المصروفات والنفقات والموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="4ade1-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="4ade1-105">تتضمن المستندات التي يمكن تعريف عمليات سير العمل لها تقارير المصروفات وطلبات السفر وطلبات السلف النقدية.</span><span class="sxs-lookup"><span data-stu-id="4ade1-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="4ade1-106">يمثل سير العمل عملية أعمال.</span><span class="sxs-lookup"><span data-stu-id="4ade1-106">A workflow represents a business process.</span></span> <span data-ttu-id="4ade1-107">إنه يحدد كيفية تدفق مستند عبر النظام ويشير إلى الشخص الذي يجب عليه إكمال مهمة أو الموافقة على مستند.</span><span class="sxs-lookup"><span data-stu-id="4ade1-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="4ade1-108">هناك العديد من الفوائد التي يمكن من خلالها استخدام نظام سير العمل في مؤسستك:</span><span class="sxs-lookup"><span data-stu-id="4ade1-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="4ade1-109">**العمليات المتسقة** — يمكنك تحديد عملية الموافقة لمستندات معينة، مثل طلبات الشراء وتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="4ade1-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="4ade1-110">يساعد استخدام نظام سير العمل على التأكد من أن المستندات تتم معالجتها والموافقة عليها بطريقة متناسقة وفعالة.</span><span class="sxs-lookup"><span data-stu-id="4ade1-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="4ade1-111">رؤية العملية — يمكنك تعقب الحالة والمحفوظات ومعايير الأداء الخاصة بمثيل سير عمل محدد.</span><span class="sxs-lookup"><span data-stu-id="4ade1-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="4ade1-112">يساعدك ذلك على تحديد ما إذا كان ينبغي إجراء تغييرات على سير العمل لتحسين الكفاءة.</span><span class="sxs-lookup"><span data-stu-id="4ade1-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="4ade1-113">قائمة العمل المركزية — يمكن للمستخدمين عرض قائمة عمل مركزية لعرض مهام سير العمل والموافقة المعينة لها.</span><span class="sxs-lookup"><span data-stu-id="4ade1-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="4ade1-114">**أنواع عمليات سير العمل التي يمكنك إنشاؤها**</span><span class="sxs-lookup"><span data-stu-id="4ade1-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="4ade1-115">يسرد الجدول التالي أنواع عمليات سير العمل التي يمكنك إنشاؤها في **المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="4ade1-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="4ade1-116"><strong>النوع</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="4ade1-117"><strong>استخدم هذا النوع لـ</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="4ade1-118"><strong>تقرير المصروفات</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="4ade1-119">إنشاء عمليات سير عمل لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="4ade1-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="4ade1-120"><strong>نشر تقرير المصروفات تلقائياً</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="4ade1-121">إنشاء نشر عمليات سير عمل لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="4ade1-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="4ade1-122"><strong>عنصر بنود المصروفات</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="4ade1-123">إنشاء عمليات سير عمل لعناصر الأسطر لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="4ade1-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="4ade1-124"><strong>النشر التلقائي لعنصر سطر المصروفات</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="4ade1-125">قم بإنشاء عمليات سير عمل للنشر التلقائي لعناصر الأسطر لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="4ade1-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="4ade1-126"><strong>طلب السفر</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="4ade1-127">قم بإنشاء عمليات سير العمل الموافقة لطلبات السفر.</span><span class="sxs-lookup"><span data-stu-id="4ade1-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="4ade1-128"><strong>طلب السلفة النقدية</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="4ade1-129">إنشاء عمليات سير عمل الموافقة لطلبات السلفة النقدية.</span><span class="sxs-lookup"><span data-stu-id="4ade1-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="4ade1-130"><strong>استرداد ضريبة القيمة المضافة</strong></span><span class="sxs-lookup"><span data-stu-id="4ade1-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="4ade1-131">قم بإنشاء عمليات سير عمل الموافقة لاسترداد ضريبة القيمة المضافة (VAT).</span><span class="sxs-lookup"><span data-stu-id="4ade1-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |

