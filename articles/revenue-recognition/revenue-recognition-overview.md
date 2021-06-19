---
title: نظرة عامة على إقرار الإيرادات
description: يوفر هذا الموضوع معلومات حول إقرار الإيرادات في Project Operations.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: f5f962572c6ec0298d2d91d33f83e4120a498a6f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013740"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="8e0ce-103">نظرة عامة على إقرار الإيرادات</span><span class="sxs-lookup"><span data-stu-id="8e0ce-103">Revenue recognition overview</span></span>

<span data-ttu-id="8e0ce-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="8e0ce-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8e0ce-105">في Dynamics 365 Project Operations، تختلف قواعد التعرف علي الإيرادات بناء علي طريقه الفوترة المحددة لأحد المشروعات أو الأجزاء الخاصة بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="8e0ce-106">يوفر هذا الموضوع معلومات حول إقرار الإيرادات في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="8e0ce-107">يتم احتساب المعاملات باستخدام طريقة فوترة الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="8e0ce-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="8e0ce-108">تم ربط إقرار التكلفة والإيرادات.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="8e0ce-109">يتم ترحيل تكلفة المعاملة والمبيعات غير المفوترة باستخدام [دفتر يومية تكامل Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="8e0ce-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="8e0ce-110">يحدد ملف تعريف الإيرادات وتكلفة المشروع ما إذا كان قد تم ترحيل حركات المبيعات غير المفوترة إلى دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="8e0ce-111">في حالة تحديد **إيراد مستحق**، يستخدم النظام **قيمة مبيعات الأعمال تحت التنفيذ** وحسابات **قيمة مبيعات الإيراد المستحق** أثناء الترحيل.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="8e0ce-112">يُمثل التالي مثالاً لهذا الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="8e0ce-113">نوع المعاملة</span><span class="sxs-lookup"><span data-stu-id="8e0ce-113">Transaction type</span></span> | <span data-ttu-id="8e0ce-114">الخصم/الائتمان</span><span class="sxs-lookup"><span data-stu-id="8e0ce-114">Debit/Credit</span></span> | <span data-ttu-id="8e0ce-115">المبلغ</span><span class="sxs-lookup"><span data-stu-id="8e0ce-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8e0ce-116">قيمة مبيعات الأعمال تحت التنفيذ (WIP)</span><span class="sxs-lookup"><span data-stu-id="8e0ce-116">WIP Sales value</span></span> | <span data-ttu-id="8e0ce-117">الخصم</span><span class="sxs-lookup"><span data-stu-id="8e0ce-117">Debit</span></span> | <span data-ttu-id="8e0ce-118">100</span><span class="sxs-lookup"><span data-stu-id="8e0ce-118">100</span></span> |
  | <span data-ttu-id="8e0ce-119">قيمة مبيعات الإيرادات المستحقة</span><span class="sxs-lookup"><span data-stu-id="8e0ce-119">Accrued revenue sales value</span></span> | <span data-ttu-id="8e0ce-120">الائتمان</span><span class="sxs-lookup"><span data-stu-id="8e0ce-120">Credit</span></span> | <span data-ttu-id="8e0ce-121">100</span><span class="sxs-lookup"><span data-stu-id="8e0ce-121">100</span></span> |

- <span data-ttu-id="8e0ce-122">تم التعرف على الإيراد أثناء الفوترة.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="8e0ce-123">يستخدم النظام حساب **الإيراد المفوتر** أثناء الترحيل.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="8e0ce-124">يُمثل التالي مثالاً لهذا الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="8e0ce-125">نوع المعاملة</span><span class="sxs-lookup"><span data-stu-id="8e0ce-125">Transaction type</span></span> | <span data-ttu-id="8e0ce-126">الخصم/الائتمان</span><span class="sxs-lookup"><span data-stu-id="8e0ce-126">Debit/Credit</span></span> | <span data-ttu-id="8e0ce-127">المبلغ</span><span class="sxs-lookup"><span data-stu-id="8e0ce-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8e0ce-128">رصيد العميل</span><span class="sxs-lookup"><span data-stu-id="8e0ce-128">Customer balance</span></span> | <span data-ttu-id="8e0ce-129">الخصم</span><span class="sxs-lookup"><span data-stu-id="8e0ce-129">Debit</span></span> | <span data-ttu-id="8e0ce-130">120</span><span class="sxs-lookup"><span data-stu-id="8e0ce-130">120</span></span> |
  | <span data-ttu-id="8e0ce-131">ضريبة المبيعات المدفوعة</span><span class="sxs-lookup"><span data-stu-id="8e0ce-131">Sales tax payable</span></span> | <span data-ttu-id="8e0ce-132">الائتمان</span><span class="sxs-lookup"><span data-stu-id="8e0ce-132">Credit</span></span> | <span data-ttu-id="8e0ce-133">20</span><span class="sxs-lookup"><span data-stu-id="8e0ce-133">20</span></span> |
  | <span data-ttu-id="8e0ce-134">الإيرادات المفوترة</span><span class="sxs-lookup"><span data-stu-id="8e0ce-134">Invoiced Revenue</span></span> | <span data-ttu-id="8e0ce-135">الائتمان</span><span class="sxs-lookup"><span data-stu-id="8e0ce-135">Credit</span></span> | <span data-ttu-id="8e0ce-136">100</span><span class="sxs-lookup"><span data-stu-id="8e0ce-136">100</span></span> |

- <span data-ttu-id="8e0ce-137">إذا تم استحقاق الإيرادات عند ترحيل المبيعات غير المفوترة ، فسيقوم النظام بعكس الإيرادات المستحقة عند إعداد الفواتير.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="8e0ce-138">نوع المعاملة</span><span class="sxs-lookup"><span data-stu-id="8e0ce-138">Transaction type</span></span> | <span data-ttu-id="8e0ce-139">الخصم/الائتمان</span><span class="sxs-lookup"><span data-stu-id="8e0ce-139">Debit/Credit</span></span> | <span data-ttu-id="8e0ce-140">المبلغ</span><span class="sxs-lookup"><span data-stu-id="8e0ce-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8e0ce-141">قيمة مبيعات الأعمال تحت التنفيذ (WIP)</span><span class="sxs-lookup"><span data-stu-id="8e0ce-141">WIP Sales value</span></span> | <span data-ttu-id="8e0ce-142">الائتمان</span><span class="sxs-lookup"><span data-stu-id="8e0ce-142">Credit</span></span> | <span data-ttu-id="8e0ce-143">100</span><span class="sxs-lookup"><span data-stu-id="8e0ce-143">100</span></span> |
  | <span data-ttu-id="8e0ce-144">قيمة مبيعات الإيرادات المستحقة</span><span class="sxs-lookup"><span data-stu-id="8e0ce-144">Accrued revenue sales value</span></span> | <span data-ttu-id="8e0ce-145">الخصم</span><span class="sxs-lookup"><span data-stu-id="8e0ce-145">Debit</span></span> | <span data-ttu-id="8e0ce-146">100</span><span class="sxs-lookup"><span data-stu-id="8e0ce-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="8e0ce-147">يتم احتساب المعاملات باستخدام طريقة فوترة السعر الثابت</span><span class="sxs-lookup"><span data-stu-id="8e0ce-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="8e0ce-148">إقرار التكلفة والإيرادات منفصلان.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="8e0ce-149">يتم ترحيل تكلفة المعاملة باستخدام [دفتر يومية تكامل Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="8e0ce-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="8e0ce-150">لا يتم إنشاء حركات مبيعات غير مفوترة.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="8e0ce-151">يمكن التعرف علي الإيراد اثناء تحرير الفواتير إذا كانت القاعدة الخاصة بتكلفه المشروع وملف تعريف الإيراد قد تم لها تعيين **القاعدة المستخدمة لعمليات حساب إكمال المشاريع** إلى **لا يوجد أعمال تحت التنفيذ**.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="8e0ce-152">استخدم هذه الطريقة فقط للمشاريع البسيطة قصيرة المدى.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="8e0ce-153">يمكن التعرف علي الإيرادات باستخدام تقديرات إيرادات السعر الثابت، إما طريقة **العقد المكتمل** أو **النسبة المئوية لإقرار إيرادات الإكمال**.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="8e0ce-154">الموارد الإضافية</span><span class="sxs-lookup"><span data-stu-id="8e0ce-154">Additional resources</span></span>
[<span data-ttu-id="8e0ce-155">مقالة تكوين المحاسبة للمشاريع القابلة للفوترة</span><span class="sxs-lookup"><span data-stu-id="8e0ce-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="8e0ce-156">مشاريع تقدير الإيرادات ثابتة السعر</span><span class="sxs-lookup"><span data-stu-id="8e0ce-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="8e0ce-157">إدارة تقديرات الإيرادات</span><span class="sxs-lookup"><span data-stu-id="8e0ce-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="8e0ce-158">أساليب التكلفة للإكمال</span><span class="sxs-lookup"><span data-stu-id="8e0ce-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]