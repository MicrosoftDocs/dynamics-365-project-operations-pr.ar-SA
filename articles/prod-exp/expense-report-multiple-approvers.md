---
title: موافقون متعددون على تقرير المصروفات
description: يقدم هذا الموضوع معلومات حول تقارير المصروفات التي تتطلب موافقة عدة أشخاص.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0fbe1c93c5359a6be493e3c4e1b27b06dbb48002
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271697"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="39cec-103">موافقون متعددون على تقرير المصروفات</span><span class="sxs-lookup"><span data-stu-id="39cec-103">Multiple approvers on an expense report</span></span>

<span data-ttu-id="39cec-104">بناءً على سياسات الموافقة على المصروفات الخاصة بمؤسستك، قد يتعين على أكثر من شخص الموافقة علي تقرير مصروفات يرسله أحد الموظفين.</span><span class="sxs-lookup"><span data-stu-id="39cec-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="39cec-105">عندما تقوم بإعداد عملية سير العمل للموافقة علي تقرير المصروفات، يمكنك إضافة عناصر سير عمل تتضمن مهام أو خطوات لواحد أو أكثر من القائمين بالموافقة علي تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="39cec-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="39cec-106">على سبيل المثال، قد تحتاج إلى الموافقة على كافة تقارير المصروفات بواسطة شخصين منفصلين أولاً، ومدير الموظف الذي قام بتقديم التقرير ومنسق الحسابات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="39cec-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="39cec-107">إذا قررت طلب العديد من جهات الموافقة علي تقرير المصروفات، يمكنك إضافة عناصر سير العمل بأي من الطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="39cec-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="39cec-108">قم بإضافه عنصر موافقة يحتوي على خطوة واحدة.</span><span class="sxs-lookup"><span data-stu-id="39cec-108">Add one approval element that has one step.</span></span> <span data-ttu-id="39cec-109">على سبيل المثال، قد تتطلب الخطوة تعيين تقرير مصروفات لمجموعة مستخدمين، والموافقة عليه بواسطة 50% من أعضاء مجموعة المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="39cec-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="39cec-110">قم بإضافة عنصر موافقة يحتوي على العديد من الخطوات.</span><span class="sxs-lookup"><span data-stu-id="39cec-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="39cec-111">على سبيل المثال، قد يحتوي عنصر الموافقة على الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="39cec-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="39cec-112">يوافق مدير الموظف الذي أرسل تقرير المصروفات عليه.</span><span class="sxs-lookup"><span data-stu-id="39cec-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="39cec-113">يتحقق موظف الحسابات الدائنة من الإيصالات وعناصر تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="39cec-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="39cec-114">يوافق مالك الموازنة على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="39cec-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="39cec-115">قم بإضافة عناصر موافقة متعددة، يشتمل كل منها على خطوة واحدة.</span><span class="sxs-lookup"><span data-stu-id="39cec-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="39cec-116">على سبيل المثال، قد تقوم بإضافة عنصر موافقة منفصل لكل من الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="39cec-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="39cec-117">يوافق مدير الموظف على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="39cec-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="39cec-118">يوافق مالك الموازنة على تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="39cec-118">The budget owner approves the expense report.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]