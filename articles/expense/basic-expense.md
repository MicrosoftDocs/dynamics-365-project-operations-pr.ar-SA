---
title: إدخال المصروفات (خفيفة)
description: يقدم هذا الموضوع معلومات حول كيفية العمل مع إدخال المصروفات في عملية نشر خفيفة.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 746d5d9ff56222e7d6b9b6e264db75d5814365c7
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965713"
---
# <a name="expense-entry-lite"></a><span data-ttu-id="5e734-103">إدخال المصروفات (خفيفة)</span><span class="sxs-lookup"><span data-stu-id="5e734-103">Expense entry (lite)</span></span>

<span data-ttu-id="5e734-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="5e734-104">_**Applies to:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5e734-105">إدارة المصروفات الأساسية، أو الخفيفة، هي القدرة على تسجيل المصروفات البسيطة.</span><span class="sxs-lookup"><span data-stu-id="5e734-105">Basic, or lite, expense management is the capability to record simple expenses.</span></span> <span data-ttu-id="5e734-106">يمكنك تسجيل المصروفات في مقابل مشروع، ومن ثم يقوم الموافق على المشروع بمراجعتها والموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="5e734-106">You can record expenses against a project, and then the project approver will review and approve them.</span></span>

<span data-ttu-id="5e734-107">لمزيد من المعلومات حول قدرات المصروفات في Dynamics 365 Project Operations، راجع [نظرة عامة حول المصروفات](expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="5e734-107">For more information about expense capabilities in Dynamics 365 Project Operations, see [Expense overview](expense-overview.md).</span></span>

## <a name="capture-a-basic-expense"></a><span data-ttu-id="5e734-108">تسجيل مصروفات أساسية</span><span class="sxs-lookup"><span data-stu-id="5e734-108">Capture a basic expense</span></span>

<span data-ttu-id="5e734-109">يمكنك تسجيل المصروفات بحيث يمكنك إرسالها إلى الموافق.</span><span class="sxs-lookup"><span data-stu-id="5e734-109">You can capture your expenses so that you can submit them to the approver.</span></span>

1. <span data-ttu-id="5e734-110">انتقل إلى **المصروفات**، وحدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="5e734-110">Go to **Expenses**, and select **New**.</span></span>
2. <span data-ttu-id="5e734-111">في صفحة **المصروفات الجديدة**، أدخل معلومات المصروفات المطلوبة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5e734-111">On the **New Expense** page, enter the required expense information, and then select **Save**.</span></span>

## <a name="submit-a-basic-expense"></a><span data-ttu-id="5e734-112">إرسال مصروفات أساسية</span><span class="sxs-lookup"><span data-stu-id="5e734-112">Submit a basic expense</span></span>

<span data-ttu-id="5e734-113">بعد أن تنتهي من تسجيل كافة المصروفات، يجب عليك إرسالها للموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="5e734-113">After you've finished capturing all your expenses, and you're ready to have them approved, you must submit them.</span></span>

1. <span data-ttu-id="5e734-114">انتقل إلى **المصروفات**، وحدد أحدها.</span><span class="sxs-lookup"><span data-stu-id="5e734-114">Go to **Expenses**, and select an expense.</span></span> <span data-ttu-id="5e734-115">أو حدد كافة المصروفات باستخدام خانة الاختيار الموجودة في الرأس.</span><span class="sxs-lookup"><span data-stu-id="5e734-115">Or, select all the expenses by using the check box on the header.</span></span>
2. <span data-ttu-id="5e734-116">حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="5e734-116">Select **Submit**.</span></span> <span data-ttu-id="5e734-117">يعالج النظام الإدخالات المحددة ثم ينشئ طلبات الموافقة على المصروفات.</span><span class="sxs-lookup"><span data-stu-id="5e734-117">The system processes the selected entries and then creates expense approval requests.</span></span>

## <a name="recall-a-basic-expense"></a><span data-ttu-id="5e734-118">استدعاء مصروفات أساسية</span><span class="sxs-lookup"><span data-stu-id="5e734-118">Recall a basic expense</span></span>

<span data-ttu-id="5e734-119">عند إرسال مصروفات عن طريق الخطأ، يمكنك استدعاؤها.</span><span class="sxs-lookup"><span data-stu-id="5e734-119">When you submit an expense by mistake, you can recall it.</span></span> <span data-ttu-id="5e734-120">يتوقف الوقت المطلوب لاستدعاء إدخال المصروفات على مرحلة الموافقة عليه.</span><span class="sxs-lookup"><span data-stu-id="5e734-120">The time that is required to recall an expense entry depends on its approval stage.</span></span>  <span data-ttu-id="5e734-121">إذا لم يكن الموافق قد وافق بعد على الإدخال، فيمكن أن يحدث الاستدعاء على الفور.</span><span class="sxs-lookup"><span data-stu-id="5e734-121">If the approver hasn't yet approved the entry, the recall can occur immediately.</span></span> <span data-ttu-id="5e734-122">ومع ذلك، إذا كانت قد تمت الموافقة على الإدخال، فيجب على الموافق الموافقة على الاستدعاء وإلغاء الحركات.</span><span class="sxs-lookup"><span data-stu-id="5e734-122">However, if the entry has already been approved, the approver is asked to approve the recall and reverse the transactions.</span></span>

1. <span data-ttu-id="5e734-123">انتقل إلى **المصروفات**، ثم في قائمة المصروفات، حدد إدخال المصروفات الذي ترغب استدعائه.</span><span class="sxs-lookup"><span data-stu-id="5e734-123">Go to **Expenses**, and then, in the list of expenses, select the expense to recall.</span></span>
2. <span data-ttu-id="5e734-124">حدد **استرجاع**.</span><span class="sxs-lookup"><span data-stu-id="5e734-124">Select **Recall**.</span></span> <span data-ttu-id="5e734-125">إذا لم تكن الموافقة على إدخال المصروفات قد حدثت بعد، فسيقوم النظام باستدعائه على الفور.</span><span class="sxs-lookup"><span data-stu-id="5e734-125">If the expense entry hasn't yet been approved, the system immediately recalls it.</span></span> <span data-ttu-id="5e734-126">إذا كانت قد تمت الموافقة على إدخال المصروفات، فسيتم إنشاء طلب استدعاء لإعلام الموافق برغبتك في إلغاء إدخال المصروفات.</span><span class="sxs-lookup"><span data-stu-id="5e734-126">If the expense entry has already been approved, a recall request is created to notify the approver that you want to reverse the expense.</span></span> <span data-ttu-id="5e734-127">سيؤكد الموافق عندئذٍ أنه يمكن تنفيذ الإلغاء، وسيتم إرجاع الإدخال.</span><span class="sxs-lookup"><span data-stu-id="5e734-127">The approver will then confirm that the reversal can be done, and the entry will be returned.</span></span>

## <a name="delete-a-basic-expense"></a><span data-ttu-id="5e734-128">حذف مصروفات أساسية</span><span class="sxs-lookup"><span data-stu-id="5e734-128">Delete a basic expense</span></span>

<span data-ttu-id="5e734-129">يمكن حذف المصروفات التي لم يتم إرسالها بعد.</span><span class="sxs-lookup"><span data-stu-id="5e734-129">Expenses that haven't yet been submitted can be deleted.</span></span> <span data-ttu-id="5e734-130">لحذف إدخال مصروفات تم إرساله، يجب أولاً استدعاؤه.</span><span class="sxs-lookup"><span data-stu-id="5e734-130">To delete an expense that has already been submitted, you must first recall it.</span></span>

## <a name="see-also"></a><span data-ttu-id="5e734-131">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="5e734-131">See also</span></span>

- [<span data-ttu-id="5e734-132">نظرة عامة على الموافقات</span><span class="sxs-lookup"><span data-stu-id="5e734-132">Approvals overview</span></span>](../approvals/approvals-overview.md)
