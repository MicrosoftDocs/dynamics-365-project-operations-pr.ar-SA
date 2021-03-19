---
title: إلغاء إدخالات الوقت والمصروفات المعتمدة مسبقا
description: يقدم هذا الموضوع معلومات حول كيفية إلغاء وقت المشروع المعتمد وحركة المصروفات.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 40ac37c1070e1c4da01e96bbc4248977b2b6d284
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290838"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a><span data-ttu-id="8eb73-103">إلغاء إدخالات الوقت أو المصروفات المعتمدة مسبقا</span><span class="sxs-lookup"><span data-stu-id="8eb73-103">Cancel previously approved time or expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8eb73-104">وفي الإصدار الأخير من Dynamics 365 Project Service Automation، يمكن للموافقين إلغاء إدخالات الوقت والمصروفات التي تمت الموافقة عليها مسبقا.</span><span class="sxs-lookup"><span data-stu-id="8eb73-104">In the latest version of Dynamics 365 Project Service Automation, approvers can cancel time or expense entries that they previously approved.</span></span>

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a><span data-ttu-id="8eb73-105">إلغاء إدخال وقت أو مصروفات معتمد مسبقا</span><span class="sxs-lookup"><span data-stu-id="8eb73-105">Cancel a previously approved time or expense entry</span></span>

<span data-ttu-id="8eb73-106">اتبع هذه الخطوات لإلغاء أحد إدخالات الوقت أو المصروفات التي قمت بالموافقة عليها مسبقا.</span><span class="sxs-lookup"><span data-stu-id="8eb73-106">Follow these steps to cancel a time or expense entry that you previously approved.</span></span>

1. <span data-ttu-id="8eb73-107">انتقل إلى **المشاريع** \> **عملي** \> **الموافقات**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-107">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="8eb73-108">في صفحة قائمة **الموافقات**، قم بتغيير طريقة العرض إلى **‏‫الموافقات السابقة الخاصة بي**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-108">On the **Approvals** list page, change the view to **My past approvals**.</span></span> <span data-ttu-id="8eb73-109">يتم عرض قائمة بإدخالات الوقت والمصروفات التي قمت بالموافقة عليها مسبقا.</span><span class="sxs-lookup"><span data-stu-id="8eb73-109">A list of the time and expense entries that you previously approved is shown.</span></span>
3. <span data-ttu-id="8eb73-110">حدد واحدًا أو أكثر من الإدخالات، ثم حدد **إلغاء الموافقة**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-110">Select one or more entries, and then select **Cancel approval**.</span></span> <span data-ttu-id="8eb73-111">تتلقى رسالة تحذير.</span><span class="sxs-lookup"><span data-stu-id="8eb73-111">You receive a warning message.</span></span>
4. <span data-ttu-id="8eb73-112">حدد **موافق** لإلغاء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="8eb73-112">Select **OK** to cancel the approval.</span></span>

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a><span data-ttu-id="8eb73-113">فهم تأثير إلغاء الموافقة على إدخال الوقت أو المصروفات</span><span class="sxs-lookup"><span data-stu-id="8eb73-113">Understand the impact of canceling a time or expense entry approval</span></span>

<span data-ttu-id="8eb73-114">عند إلغاء الموافقة، يحدث هناك تأثير تشغيلي وتأثير مالي.</span><span class="sxs-lookup"><span data-stu-id="8eb73-114">When an approval is canceled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="8eb73-115">التأثير التشغيلي</span><span class="sxs-lookup"><span data-stu-id="8eb73-115">Operational impact</span></span>

<span data-ttu-id="8eb73-116">في جانب العمليات، عند إلغاء موافقة، يتم إعادة تعيين حالة السجل إلى **مسودة**، ولم تعد الموافقة تظهر في طريقة عرض **الموافقات السابقة الخاصة بي**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-116">On the operations side, when an approval is canceled, the status of the record is reset to **Draft**, and the approval no longer appears in the **My past approvals** view.</span></span> <span data-ttu-id="8eb73-117">وبدلا من ذلك، تظهر الموافقة التي تم إلغاؤها في إما طريقة عرض **إدخالات الوقت للموافقة** أو طريقة عرض **إدخالات المصروفات للموافقة**، وذلك استنادا إلى ما إذا كانت إدخال الوقت أم إدخال مصروفات.</span><span class="sxs-lookup"><span data-stu-id="8eb73-117">Instead, the canceled approval appears in either the **Time entries for approval** view or the **Expense entries for approval** view, depending on whether it was a time entry or an expense entry.</span></span> <span data-ttu-id="8eb73-118">بالإضافة إلى ذلك، تتغير حالة إدخال الوقت أو إدخال المصروفات ذي الصلة إلى **تم الإرسال**، بالتالي يكون الإدخال متسقًا مع الموافقات بالحالة **مسودة**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-118">Additionally, the status of the related time or expense entry is changed to **Submitted**, so that the related entry is consistent with approvals that have a status of **Draft**.</span></span>

<span data-ttu-id="8eb73-119">وبصفتك القائم على الموافقة، يمكنك تحرير بعض الحقول الخاصة بالموافقة والتي بالحالة **مسودة**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-119">As an approver, you can edit some of the fields of an approval that has a status of **Draft**.</span></span> <span data-ttu-id="8eb73-120">تتضمن هذه الحقول **نوع الفوترة** و **الساعات القابلة للفوترة لإدخالات الوقت**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-120">These fields include **Billing Type** and **Billable Hours for Time Entries**.</span></span> <span data-ttu-id="8eb73-121">بعد إجراء التغييرات، يمكنك الموافقة على السجل مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="8eb73-121">After you make changes, you can approve the record again.</span></span> <span data-ttu-id="8eb73-122">بدلا من ذلك، يمكنك رفض الإدخال.</span><span class="sxs-lookup"><span data-stu-id="8eb73-122">Alternatively, you can reject the entry.</span></span> <span data-ttu-id="8eb73-123">إذا قمت برفض الموافقة على إدخال الوقت، سيتم تغيير حالة الإدخال إلى **تم إرجاعه**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-123">If you reject the approval of a time entry, the status of the entry is changed to **Returned**.</span></span> <span data-ttu-id="8eb73-124">إذا قمت برفض الموافقة على إدخال المصروفات، سيتم تغيير الحالة إلى **تم رفضه**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-124">If you reject the approval of an expense entry, the status is changed to **Rejected**.</span></span> <span data-ttu-id="8eb73-125">من الناحية الوظيفة، تتصرف كل من الإدخالات التي تم إرجاعها ورفضها بنفس الطريقة مثل إدخال بالحالة **مسودة**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-125">Functionally, both returned and rejected entries behave the same as an entry that has a status of **Draft**.</span></span> <span data-ttu-id="8eb73-126">يستطيع عضو فريق المشروع أن يجري أي تغييرات مطلوبة على الإدخال ثم إعادة إرساله للحصول على الموافقة، أو يمكنه حذف الإدخال بالكامل.</span><span class="sxs-lookup"><span data-stu-id="8eb73-126">A project team member can either make any required changes to the entry and then resubmit it for approval, or delete the entry entirely.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="8eb73-127">التأثير المالي</span><span class="sxs-lookup"><span data-stu-id="8eb73-127">Financial impact</span></span>

<span data-ttu-id="8eb73-128">يتأثر المشروع ماليا عند إلغاء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="8eb73-128">A project is also affected financially when an approval is canceled.</span></span> <span data-ttu-id="8eb73-129">أولا، يتم تحديث القيم الفعلية المتعلقة بالتكلفة والمبيعات بالطريقة التالية:</span><span class="sxs-lookup"><span data-stu-id="8eb73-129">First, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="8eb73-130">يتم تعيين حالة التسوية إلى **تم التعديل**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-130">The adjustment status is set to **Adjusted**.</span></span>
- <span data-ttu-id="8eb73-131">يتم تعيين حالة الفوترة إلى **تم الإلغاء**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-131">The billing status is set to **Canceled**.</span></span>

<span data-ttu-id="8eb73-132">بعد ذلك، يتم إنشاء إدخالات إلغاء في جدول القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="8eb73-132">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="8eb73-133">لإنشاء إدخالات إلغاء، ينسخ النظام قيم الحقول من القيم الفعلية الأصلية.</span><span class="sxs-lookup"><span data-stu-id="8eb73-133">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="8eb73-134">والقيم الوحيدة التي لا يتم نسخها هي قيم الكمية.</span><span class="sxs-lookup"><span data-stu-id="8eb73-134">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="8eb73-135">يتم إلغاء هذه القيم بدلا من ذلك.</span><span class="sxs-lookup"><span data-stu-id="8eb73-135">These values are reversed instead.</span></span> <span data-ttu-id="8eb73-136">يتم إنشاء القيم الفعلية المعكوسة لكل من القيم الفعلية لـ **التكلفة** و **المبيعات غير المفوترة**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-136">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="8eb73-137">يتم تعيين حقل **حاله التسوية** للقيم الفعلية الملغاة إلى **غير قابلة للتسوية**، ويتم تعيين حالة الفوترة إلى **تم الإلغاء**.</span><span class="sxs-lookup"><span data-stu-id="8eb73-137">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the billing status is set to **Canceled**.</span></span>

<span data-ttu-id="8eb73-138">بعد إجراء هذه التغييرات، فإن المبلغ الذي تم تسجيله كمصروف في المشروع وكتراكم إيراد في المشروع لن يتم حسبانه ضمن المبالغ التي تمثلها هذه القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="8eb73-138">After these changes are made, the amount that is recorded as spent on the project and the revenue backlog on the project will longer account for the amounts that these actuals represent.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]