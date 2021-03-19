---
title: سير عمل إدارة المصروفات
description: يشرح الموضوع كيف يمكنك استخدام نظام سير العمل في Microsoft Dynamics 365 Finance، لإعداد عملية مراجعة لتقارير المصروفات في إدارة المصروفات.
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
ms.openlocfilehash: fde336f53d72e9ddf38c5123d9e774a4c3a22a28
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271652"
---
# <a name="expense-management-workflow"></a><span data-ttu-id="c5df9-103">سير عمل إدارة المصروفات</span><span class="sxs-lookup"><span data-stu-id="c5df9-103">Expense management workflow</span></span>

<span data-ttu-id="c5df9-104">يمكنك استخدام نظام سير العمل لإعداد عملية مراجعة لتقارير المصروفات في إدارة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-104">You can use the workflow system to set up a review process for expense reports in Expense management.</span></span> <span data-ttu-id="c5df9-105">يمكنك إعداد سير عمل يستخدم المعايير التالية لتحديد الجهة التي توافق على تقارير المصروفات:</span><span class="sxs-lookup"><span data-stu-id="c5df9-105">You can set up a workflow that uses the following criteria to determine who approves expense reports:</span></span>

- <span data-ttu-id="c5df9-106">التدرج الهرمي للمرؤوسين وحدود الموافقة المحددة مسبقًا</span><span class="sxs-lookup"><span data-stu-id="c5df9-106">The employee reporting hierarchy and predefined approval limits</span></span>
- <span data-ttu-id="c5df9-107">موافقة متعددة المستويات تدعم الموافقين المؤقتين والموافق النهائي</span><span class="sxs-lookup"><span data-stu-id="c5df9-107">Multi-level approval that supports interim approvers and a final approver</span></span>
- <span data-ttu-id="c5df9-108">الأبعاد المالية ومسؤولية المشروع</span><span class="sxs-lookup"><span data-stu-id="c5df9-108">Financial dimensions and project responsibility</span></span>
- <span data-ttu-id="c5df9-109">تعيين إلى مستخدمين معينين أو مجموعات مستخدمين معينة</span><span class="sxs-lookup"><span data-stu-id="c5df9-109">Assignment to specific users or user groups</span></span>

<span data-ttu-id="c5df9-110">يمكن إنشاء الموافقات على سير العمل لتقارير المصروفات وطلبات السفر والسلف النقدية واسترداد ضريبة القيمة المضافة (VAT).</span><span class="sxs-lookup"><span data-stu-id="c5df9-110">Workflow approvals can be created for expense reports, travel requisitions, cash advances, and value-added tax (VAT) recovery.</span></span>

<span data-ttu-id="c5df9-111">**مثال**</span><span class="sxs-lookup"><span data-stu-id="c5df9-111">**Example**</span></span>

<span data-ttu-id="c5df9-112">تعتبر العملية التالية مثالاً عن سير عمل إدارة المصروفات لتقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-112">The following process is an example of the expense management workflow for an expense report.</span></span>

1. <span data-ttu-id="c5df9-113">يقوم موظف بإنشاء تقرير مصروفات ويحفظه.</span><span class="sxs-lookup"><span data-stu-id="c5df9-113">An employee creates and saves an expense report.</span></span>
2. <span data-ttu-id="c5df9-114">يقدم الموظف تقرير المصروفات كي تتم الموافقة عليه.</span><span class="sxs-lookup"><span data-stu-id="c5df9-114">The employee submits the expense report for approval.</span></span> <span data-ttu-id="c5df9-115">يتم تحديد الموافق استنادًا إلى القواعد التي تم تعريفها عندما تم إعداد سير العمل.</span><span class="sxs-lookup"><span data-stu-id="c5df9-115">The approver is identified based on the rules that were defined when the workflow was set up.</span></span>
3. <span data-ttu-id="c5df9-116">يتلقى الموافق إعلامًا يشير إلى أن تقرير المصروفات أصبح جاهزًا للموافقة عليه.</span><span class="sxs-lookup"><span data-stu-id="c5df9-116">The approver receives a notification that an expense report is ready for approval.</span></span> <span data-ttu-id="c5df9-117">يراجع الموافق تقرير المصروفات ويتحقق من استيفاء الشروط التالية:</span><span class="sxs-lookup"><span data-stu-id="c5df9-117">The approver reviews the expense report and verifies that the following conditions are met:</span></span>

    - <span data-ttu-id="c5df9-118">المصروفات لا تنتهك سياسات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-118">The expenses don't violate any expense policies.</span></span> <span data-ttu-id="c5df9-119">إذا انتهك أحد بنود المصروفات إحدى السياسات، يتحقق الموافق من أن تقرير المصروفات يتضمن مبرر عمل صالحًا.</span><span class="sxs-lookup"><span data-stu-id="c5df9-119">If an expense violates a policy, the approver verifies that the expense report includes a valid business justification.</span></span>
    - <span data-ttu-id="c5df9-120">يتم إرفاق الإيصالات الإلكترونية بتقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-120">Electronic receipts are attached to the expense report.</span></span>

4. <span data-ttu-id="c5df9-121">يقوم الموافق بالموافقة على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-121">The approver approves the expense report.</span></span>
5. <span data-ttu-id="c5df9-122">يتم تعيين تقرير المصروفات إلى منسق الحسابات الدائنة لترحيله.</span><span class="sxs-lookup"><span data-stu-id="c5df9-122">The expense report is assigned to the Accounts payable coordinator for posting.</span></span>
6. <span data-ttu-id="c5df9-123">تحدث إحدى الخطوات التالية، استنادًا إلى ما إذا تم تكوين الترحيل التلقائي:</span><span class="sxs-lookup"><span data-stu-id="c5df9-123">One of the following steps occurs, depending on whether automatic posting is configured:</span></span>

    - <span data-ttu-id="c5df9-124">إذا تم تكوين الترحيل التلقائي، تتم معالجة تقرير المصروفات للدفع، ويتم تحديث حالة تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-124">If automatic posting is configured, the expense report is processed for payment, and the status of the expense report is updated.</span></span>
    - <span data-ttu-id="c5df9-125">إذا لم يتم تكوين الترحيل التلقائي، سيتحقق منسق الحسابات الدائنة من إرسال جميع الإيصالات الأصلية، ومن أن الإيصالات تتلاءم مع المصروفات على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-125">If automatic posting isn't configured, the Accounts payable coordinator verifies that all original receipts have been submitted, and that the receipts are aligned with the expenses on the expense report.</span></span> <span data-ttu-id="c5df9-126">يجب أيضًأ التحقق من صحة كافة أكواد الضريبة التي تم إدخالها في تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-126">All tax codes that are entered on the expense report must also be verified as correct.</span></span>

<span data-ttu-id="c5df9-127">وبعد التحقق من هذه المتطلبات، يتم ترحيل تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c5df9-127">After these requirements are verified, the expense report is posted.</span></span>

<span data-ttu-id="c5df9-128">بعد ترحيل تقرير المصروفات، يتم تخويل الدفع لتقرير المصروفات، ويتم تعويض الموظف.</span><span class="sxs-lookup"><span data-stu-id="c5df9-128">After the expense report is posted, payment is authorized for the expense report, and the employee is reimbursed.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]