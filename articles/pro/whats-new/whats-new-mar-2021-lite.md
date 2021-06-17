---
title: الجديد في مارس 2021 - النشر الخفيف لـ Project Operations
description: يوفر هذا الموضوع معلومات حول التحديثات الإصلاحية المتوفرة في إصدار مارس 2021 من النشر الخفيف لـ Project Operations.
author: sigitac
ms.date: 03/03/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: efddb96b2cb428b9dc0488c32eb5670d01322bcb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993850"
---
# <a name="whats-new-march-2021---project-operations-lite-deployment"></a><span data-ttu-id="60a34-103">الجديد في مارس 2021 - النشر الخفيف لـ Project Operations</span><span class="sxs-lookup"><span data-stu-id="60a34-103">What's new March 2021 - Project Operations lite deployment</span></span>

<span data-ttu-id="60a34-104">_ينطبق على: النشر الخفيف – من الصفقة إلى الفوترة الأولية_</span><span class="sxs-lookup"><span data-stu-id="60a34-104">_Applies To: Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="60a34-105">ينطبق هذه الموضوع على مكونات وإصدارات Dynamics 365 Project Operations التالية:</span><span class="sxs-lookup"><span data-stu-id="60a34-105">This topic applies to the following Dynamics 365 Project Operations components and versions:</span></span>

- <span data-ttu-id="60a34-106">Project Operations على بيئة Dataverse الإصدار 4.8.0.91</span><span class="sxs-lookup"><span data-stu-id="60a34-106">Project Operations on Dataverse environment version 4.8.0.91</span></span> 

## <a name="quality-updates"></a><span data-ttu-id="60a34-107">التحديثات الإصلاحية</span><span class="sxs-lookup"><span data-stu-id="60a34-107">Quality updates</span></span>

| <span data-ttu-id="60a34-108">**منطقة الميزات**</span><span class="sxs-lookup"><span data-stu-id="60a34-108">**Feature area**</span></span> | <span data-ttu-id="60a34-109">**رقم المرجع**</span><span class="sxs-lookup"><span data-stu-id="60a34-109">**Reference number**</span></span> | <span data-ttu-id="60a34-110">**تحديث إصلاحي**</span><span class="sxs-lookup"><span data-stu-id="60a34-110">**Quality update**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="60a34-111">الفوترة والتسعير</span><span class="sxs-lookup"><span data-stu-id="60a34-111">Billing and pricing</span></span> | <span data-ttu-id="60a34-112">2133873 </span><span class="sxs-lookup"><span data-stu-id="60a34-112">2133873</span></span> | <span data-ttu-id="60a34-113">تم إصلاح عرض رمز عملة **سعر مبيعات الوحدة** في شبكة **تقديرات المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="60a34-113">Fixed the display of **Unit Sales Price** currency symbol in the **Expense Estimates** grid.</span></span> |
| <span data-ttu-id="60a34-114">الفوترة والتسعير</span><span class="sxs-lookup"><span data-stu-id="60a34-114">Billing and pricing</span></span> | <span data-ttu-id="60a34-115">2174616 </span><span class="sxs-lookup"><span data-stu-id="60a34-115">2174616</span></span> | <span data-ttu-id="60a34-116">عندما يفوز أحد عروض الأسعار، يُشار إلى قائمة أسعار العرض المخصصة على تفاصيل شروط التعاقد المنسوخة من عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="60a34-116">When a quote is won, the contract custom pricelist is referenced on contract line details that are copied from the quote.</span></span> |
| <span data-ttu-id="60a34-117">إدارة الفرص</span><span class="sxs-lookup"><span data-stu-id="60a34-117">Opportunity Management</span></span> | <span data-ttu-id="60a34-118">2167475 </span><span class="sxs-lookup"><span data-stu-id="60a34-118">2167475</span></span> | <span data-ttu-id="60a34-119">تم إصلاح مبلغ الضريبة في فاتورة التصحيح التي أنشأت إدخالاً فعليًا غير مفوتر.</span><span class="sxs-lookup"><span data-stu-id="60a34-119">Fixed tax amount in the correction invoice that originated an unbilled actual entry.</span></span> |
| <span data-ttu-id="60a34-120">إدارة الفرص</span><span class="sxs-lookup"><span data-stu-id="60a34-120">Opportunity Management</span></span> | <span data-ttu-id="60a34-121">2176285 </span><span class="sxs-lookup"><span data-stu-id="60a34-121">2176285</span></span> | <span data-ttu-id="60a34-122">يجب عدم نسخ مبلغ الضريبة من تفاصيل بنود عقد المبيعات/عرض الأسعار إلى تفاصيل بنود عقد التكلفة/عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="60a34-122">Tax amount must not be copied from sales contract/quote line details to cost contract/quote line details.</span></span> |
| <span data-ttu-id="60a34-123">إدارة الفرص</span><span class="sxs-lookup"><span data-stu-id="60a34-123">Opportunity Management</span></span> | <span data-ttu-id="60a34-124">2188079 </span><span class="sxs-lookup"><span data-stu-id="60a34-124">2188079</span></span> | <span data-ttu-id="60a34-125">يجب عدم إنشاء قاعدة تقسيم الفوترة في العقود غير المستندة إلى العمل.</span><span class="sxs-lookup"><span data-stu-id="60a34-125">Split billing rule must not be created for contracts that are not work-based.</span></span> |
| <span data-ttu-id="60a34-126">التخطيط والتعقب</span><span class="sxs-lookup"><span data-stu-id="60a34-126">Planning and Tracking</span></span> | <span data-ttu-id="60a34-127">2138853 </span><span class="sxs-lookup"><span data-stu-id="60a34-127">2138853</span></span> | <span data-ttu-id="60a34-128">تم تحديث وظيفة نسخ المشروع لضمان نسخ بنود تقدير المصروفات التي تشير إلى المهام إلى المشروع الوجهة.</span><span class="sxs-lookup"><span data-stu-id="60a34-128">Project copy function updated to ensure expense estimate lines that reference tasks are copied to the destination project.</span></span> |
| <span data-ttu-id="60a34-129">التخطيط والتعقب</span><span class="sxs-lookup"><span data-stu-id="60a34-129">Planning and Tracking</span></span> | <span data-ttu-id="60a34-130">2173259 </span><span class="sxs-lookup"><span data-stu-id="60a34-130">2173259</span></span> | <span data-ttu-id="60a34-131">تم تحديث وظيفة نسخ المشروع لضمان أنها لا تعرض رسالة الخطأ **جارٍ نسخ WBS‎‬** في سيناريوهات معينة.</span><span class="sxs-lookup"><span data-stu-id="60a34-131">Project copy function updated to ensure it doesn't display the **Copying WBS** error message in certain scenarios.</span></span> |
| <span data-ttu-id="60a34-132">الوقت والمصروفات</span><span class="sxs-lookup"><span data-stu-id="60a34-132">Time and Expense</span></span> | <span data-ttu-id="60a34-133">2148910 </span><span class="sxs-lookup"><span data-stu-id="60a34-133">2148910</span></span> | <span data-ttu-id="60a34-134">تم إصلاح مشكلة عرض في صفحة **تحرير الإدخال** في شبكة **إدخال الوقت**.</span><span class="sxs-lookup"><span data-stu-id="60a34-134">Fixed display issue with the **Edit Entry** page in the **Time Entry** grid.</span></span> |
| <span data-ttu-id="60a34-135">الوقت والمصروفات</span><span class="sxs-lookup"><span data-stu-id="60a34-135">Time and Expense</span></span> | <span data-ttu-id="60a34-136">2159798 </span><span class="sxs-lookup"><span data-stu-id="60a34-136">2159798</span></span> | <span data-ttu-id="60a34-137">تم تشديد عناصر التحكم لضمان عدم تحرير إدخالات المصروفات الموافق عليها.</span><span class="sxs-lookup"><span data-stu-id="60a34-137">Tightened controls to ensure approved expense entries can't be edited.</span></span> |


