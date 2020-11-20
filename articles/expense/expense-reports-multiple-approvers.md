---
title: تقارير المصروفات والموافقون المتعددون
description: يقدم هذا الموضوع معلومات حول تقارير المصروفات التي تتطلب موافقة أكثر من شخص.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: cfa8677f38e9468aa3236f587d2e9bd5af839054
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120977"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="49ca0-103">تقارير المصروفات والموافقون المتعددون</span><span class="sxs-lookup"><span data-stu-id="49ca0-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="49ca0-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="49ca0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="49ca0-105">بناءً على سياسات الموافقة على المصروفات الخاصة بمؤسستك، قد يتعين على أكثر من شخص الموافقة على تقرير مصروفات مُرسل.</span><span class="sxs-lookup"><span data-stu-id="49ca0-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="49ca0-106">عندما تقوم بإعداد عملية سير العمل للموافقة على تقرير المصروفات، يمكنك إضافة عناصر سير عمل تتضمن مهام أو خطوات لواحد أو أكثر من القائمين بالموافقة على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="49ca0-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="49ca0-107">على سبيل المثال، قد تحتاج إلى الموافقة على كافة تقارير المصروفات بواسطة شخصين منفصلين، ومدير الموظف الذي قام بتقديم التقرير ومنسق الحسابات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="49ca0-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="49ca0-108">إذا قررت طلب العديد من جهات الموافقة على تقرير المصروفات، يمكنك إضافة عناصر سير العمل بأي من الطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="49ca0-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="49ca0-109">قم بإضافه عنصر موافقة يحتوي على خطوة واحدة.</span><span class="sxs-lookup"><span data-stu-id="49ca0-109">Add one approval element that has one step.</span></span> <span data-ttu-id="49ca0-110">على سبيل المثال، قد تتطلب الخطوة تعيين تقرير مصروفات لمجموعة مستخدمين، والموافقة عليه بواسطة 50% من أعضاء مجموعة المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="49ca0-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="49ca0-111">قم بإضافة عنصر موافقة يحتوي على العديد من الخطوات.</span><span class="sxs-lookup"><span data-stu-id="49ca0-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="49ca0-112">على سبيل المثال، قد يحتوي عنصر الموافقة على الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="49ca0-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="49ca0-113">يوافق مدير الموظف الذي أرسل تقرير المصروفات عليه.</span><span class="sxs-lookup"><span data-stu-id="49ca0-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="49ca0-114">يتحقق موظف الحسابات الدائنة من الإيصالات وعناصر تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="49ca0-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="49ca0-115">يوافق مالك الموازنة على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="49ca0-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="49ca0-116">قم بإضافة عناصر موافقة متعددة، يشتمل كل منها على خطوة واحدة.</span><span class="sxs-lookup"><span data-stu-id="49ca0-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="49ca0-117">على سبيل المثال، قد تقوم بإضافة عنصر موافقة منفصل لكل من الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="49ca0-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="49ca0-118">يوافق مدير الموظف على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="49ca0-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="49ca0-119">يوافق مالك الموازنة على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="49ca0-119">The budget owner approves the expense report.</span></span>
