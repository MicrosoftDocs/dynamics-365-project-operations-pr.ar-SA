---
title: إعداد عمليات سير العمل لإدارة المصروفات
description: يمكنك إعداد عملية سير عمل يتم استخدامها لمراجعة مستندات المصروفات والنفقات والموافقة عليها.
author: suvaidya
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: aab6e18d1ddcffa57cf7cd4cb09eec5a4b89c0fd
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001005"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="298dc-103">إعداد عمليات سير العمل لإدارة المصروفات</span><span class="sxs-lookup"><span data-stu-id="298dc-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="298dc-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="298dc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="298dc-105">يمكنك إعداد عملية سير عمل لمراجعة مستندات المصروفات والنفقات والموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="298dc-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="298dc-106">يمكنك تحديد مهام سير العمل لتقارير المصروفات وطلبات السفر وطلبات السلف النقدية.</span><span class="sxs-lookup"><span data-stu-id="298dc-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="298dc-107">يمثل سير العمل عملية تجارية ويحدد كيفية تدفق مستند من خلال النظام.</span><span class="sxs-lookup"><span data-stu-id="298dc-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="298dc-108">كما يشير سير العمل أيضا إلى من يجب عليه إكمال مهمة أو الموافقة على مستند.</span><span class="sxs-lookup"><span data-stu-id="298dc-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="298dc-109">هناك العديد من الفوائد التي يمكن من خلالها استخدام نظام سير العمل في مؤسستك:</span><span class="sxs-lookup"><span data-stu-id="298dc-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="298dc-110">**العمليات المتسقة**: يمكنك تحديد عملية الموافقة لمستندات معينة، مثل طلبات الشراء وتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="298dc-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="298dc-111">يساعد استخدام نظام سير العمل على التأكد من أن المستندات تتم معالجتها واعتمادها بطريقة متناسقة وفعالة.</span><span class="sxs-lookup"><span data-stu-id="298dc-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="298dc-112">**رؤية العملية**: يمكنك تعقب الحالة والمحفوظات ومعايير الأداء الخاصة بمثيل سير عمل محدد.</span><span class="sxs-lookup"><span data-stu-id="298dc-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="298dc-113">يساعدك ذلك على تحديد ما إذا كان ينبغي إجراء تغييرات على سير العمل لتحسين الكفاءة.</span><span class="sxs-lookup"><span data-stu-id="298dc-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="298dc-114">**قائمة العمل المركزية** : يمكن للمستخدمين عرض قائمة عمل مركزية لعرض مهام سير العمل والاعتمادات المعينة اليهم.</span><span class="sxs-lookup"><span data-stu-id="298dc-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="298dc-115">أنواع سير العمل</span><span class="sxs-lookup"><span data-stu-id="298dc-115">Workflow types</span></span>

<span data-ttu-id="298dc-116">يسرد الجدول التالي أنواع عمليات السير التي يمكنك إنشاؤها في **إدارة المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="298dc-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="298dc-117"><strong>النوع</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="298dc-118"><strong>استخدم هذا النوع لـ</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="298dc-119"><strong>الموافقة على تقرير المصروفات تلقائياً</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="298dc-120">إنشاء عمليات سير عمل لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="298dc-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="298dc-121"><strong>نشر تقرير المصروفات تلقائياً</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="298dc-122">إنشاء نشر عمليات سير عمل لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="298dc-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="298dc-123"><strong>عنصر بنود المصروفات</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="298dc-124">إنشاء عمليات سير عمل لعناصر الأسطر لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="298dc-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="298dc-125"><strong>النشر التلقائي لعنصر سطر المصروفات</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="298dc-126">قم بإنشاء عمليات سير عمل للنشر التلقائي لعناصر الأسطر لتقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="298dc-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="298dc-127"><strong>طلب السفر</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="298dc-128">قم بإنشاء عمليات سير العمل الموافقة لطلبات السفر.</span><span class="sxs-lookup"><span data-stu-id="298dc-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="298dc-129"><strong>طلب السلفة النقدية</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="298dc-130">إنشاء عمليات سير عمل الموافقة لطلبات السلفة النقدية.</span><span class="sxs-lookup"><span data-stu-id="298dc-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="298dc-131"><strong>استرداد ضريبة القيمة المضافة</strong></span><span class="sxs-lookup"><span data-stu-id="298dc-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="298dc-132">قم بإنشاء عمليات سير عمل الموافقة لاسترداد ضريبة القيمة المضافة (VAT).</span><span class="sxs-lookup"><span data-stu-id="298dc-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |


[!INCLUDE[footer-include](../includes/footer-banner.md)]