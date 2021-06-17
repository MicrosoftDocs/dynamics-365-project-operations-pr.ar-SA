---
title: إعداد عمليات سير العمل لإدارة المصروفات
description: يمكنك إعداد عملية سير عمل لمراجعة مستندات المصروفات والنفقات والموافقة عليها.
author: ShylaThompson
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 4070b4fb5109464abdabbce971688fb881dfcf2c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005100"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="02248-103">إعداد عمليات سير العمل لإدارة المصروفات</span><span class="sxs-lookup"><span data-stu-id="02248-103">Set up Expense management workflows</span></span>

<span data-ttu-id="02248-104">يمكنك إعداد عملية سير عمل يتم استخدامها لمراجعة مستندات المصروفات والنفقات والموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="02248-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="02248-105">تتضمن المستندات التي يمكن تعريف عمليات سير العمل لها تقارير المصروفات وطلبات السفر وطلبات السلف النقدية.</span><span class="sxs-lookup"><span data-stu-id="02248-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="02248-106">يمثل سير العمل عملية أعمال.</span><span class="sxs-lookup"><span data-stu-id="02248-106">A workflow represents a business process.</span></span> <span data-ttu-id="02248-107">إنه يحدد كيفية تدفق مستند عبر النظام ويشير إلى الشخص الذي يجب عليه إكمال مهمة أو الموافقة على مستند.</span><span class="sxs-lookup"><span data-stu-id="02248-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="02248-108">هناك العديد من الفوائد التي يمكن من خلالها استخدام نظام سير العمل في مؤسستك:</span><span class="sxs-lookup"><span data-stu-id="02248-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="02248-109">**العمليات المتسقة** — يمكنك تحديد عملية الموافقة لمستندات معينة، مثل طلبات الشراء وتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="02248-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="02248-110">يساعد استخدام نظام سير العمل على التأكد من أن المستندات تتم معالجتها والموافقة عليها بطريقة متناسقة وفعالة.</span><span class="sxs-lookup"><span data-stu-id="02248-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="02248-111">رؤية العملية — يمكنك تعقب الحالة والمحفوظات ومعايير الأداء الخاصة بمثيل سير عمل محدد.</span><span class="sxs-lookup"><span data-stu-id="02248-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="02248-112">يساعدك ذلك على تحديد ما إذا كان ينبغي إجراء تغييرات على سير العمل لتحسين الكفاءة.</span><span class="sxs-lookup"><span data-stu-id="02248-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="02248-113">قائمة العمل المركزية — يمكن للمستخدمين عرض قائمة عمل مركزية لعرض مهام سير العمل والموافقة المعينة لها.</span><span class="sxs-lookup"><span data-stu-id="02248-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="02248-114">**أنواع عمليات سير العمل التي يمكنك إنشاؤها**</span><span class="sxs-lookup"><span data-stu-id="02248-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="02248-115">يسرد الجدول التالي أنواع عمليات سير العمل التي يمكنك إنشاؤها في **المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="02248-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="02248-116"><strong>النوع</strong></span><span class="sxs-lookup"><span data-stu-id="02248-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="02248-117"><strong>استخدم هذا النوع لـ</strong></span><span class="sxs-lookup"><span data-stu-id="02248-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="02248-118"><strong>تقرير المصروفات</strong></span><span class="sxs-lookup"><span data-stu-id="02248-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="02248-119">إنشاء عمليات سير عمل لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="02248-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="02248-120"><strong>نشر تقرير المصروفات تلقائياً</strong></span><span class="sxs-lookup"><span data-stu-id="02248-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="02248-121">إنشاء نشر عمليات سير عمل لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="02248-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="02248-122"><strong>عنصر بنود المصروفات</strong></span><span class="sxs-lookup"><span data-stu-id="02248-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="02248-123">إنشاء عمليات سير عمل لعناصر الأسطر لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="02248-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="02248-124"><strong>النشر التلقائي لعنصر سطر المصروفات</strong></span><span class="sxs-lookup"><span data-stu-id="02248-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="02248-125">قم بإنشاء عمليات سير عمل للنشر التلقائي لعناصر الأسطر لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="02248-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="02248-126"><strong>طلب السفر</strong></span><span class="sxs-lookup"><span data-stu-id="02248-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="02248-127">قم بإنشاء عمليات سير العمل الموافقة لطلبات السفر.</span><span class="sxs-lookup"><span data-stu-id="02248-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="02248-128"><strong>طلب السلفة النقدية</strong></span><span class="sxs-lookup"><span data-stu-id="02248-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="02248-129">إنشاء عمليات سير عمل الموافقة لطلبات السلفة النقدية.</span><span class="sxs-lookup"><span data-stu-id="02248-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="02248-130"><strong>استرداد ضريبة القيمة المضافة</strong></span><span class="sxs-lookup"><span data-stu-id="02248-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="02248-131">قم بإنشاء عمليات سير عمل الموافقة لاسترداد ضريبة القيمة المضافة (VAT).</span><span class="sxs-lookup"><span data-stu-id="02248-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |



[!INCLUDE[footer-include](../includes/footer-banner.md)]