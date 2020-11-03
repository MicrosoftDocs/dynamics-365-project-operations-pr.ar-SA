---
title: التوزيعات في تقرير المصروفات
description: عندما تقوم بإدخال المصروفات في تقرير مصروفات، يمكنك توزيعها عبر العديد من المشروعات أو الكيانات القانونية أو الحسابات في مؤسستك.
author: suvaidya
manager: AnnBe
ms.date: 10/10/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: a1fa7383e7715fe57380de0a006ccc4e020bb5a5
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070525"
---
# <a name="distributions-on-an-expense-report"></a><span data-ttu-id="4fc64-103">التوزيعات في تقرير المصروفات</span><span class="sxs-lookup"><span data-stu-id="4fc64-103">Distributions on an expense report</span></span>

<span data-ttu-id="4fc64-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="4fc64-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="4fc64-105">عندما تقوم بإدخال المصروفات في تقرير مصروفات، يمكنك توزيعها عبر العديد من المشروعات أو الأبعاد المالية أو الحسابات في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="4fc64-105">When you enter expenses on an expense report, you can distribute them across multiple projects, financial dimensions, or accounts in your organization.</span></span>

<span data-ttu-id="4fc64-106">على سبيل المثال، سافرت نانسي، وهي مندوبة مبيعات لشركة Fabrikam، من كوبنهاغن إلى فرانكفورت.</span><span class="sxs-lookup"><span data-stu-id="4fc64-106">For example, Nancy, a Fabrikam sales representative, traveled from Copenhagen to Frankfurt.</span></span> <span data-ttu-id="4fc64-107">في فرانكفورت، التقت نانسي بمؤسستين لمناقشة مشروعات منفصلة لكل مؤسسة.</span><span class="sxs-lookup"><span data-stu-id="4fc64-107">In Frankfurt, Nancy met with two organizations to discuss separate projects for each organization.</span></span> <span data-ttu-id="4fc64-108">أمضت نانسي سبعة أيام في العمل مع المؤسسة A على المشروع A، وثلاثة أيام في العمل مع المؤسسة B على المشروع B.</span><span class="sxs-lookup"><span data-stu-id="4fc64-108">Nancy spent seven business days working with organization A on project A, and three business days working with organization B on project B.</span></span>

<span data-ttu-id="4fc64-109">بسبب قيام نانسي بالعمل على مشروعين منفصلين أثناء وجودها في فرانكفورت، قامت بتوزيع المصروفات على كل مشروع بالطريقة المناسبة وذلك عند إدخالها تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="4fc64-109">Because Nancy worked on two separate projects while was in Frankfurt, when she enters the expense report, Nancy distributes the expenses as appropriate for each project.</span></span> <span data-ttu-id="4fc64-110">يوضح الجدول التالي كيف وزعت نانسي المصروفات.</span><span class="sxs-lookup"><span data-stu-id="4fc64-110">The following table shows how Nancy distributed the expenses.</span></span>

| <span data-ttu-id="4fc64-111">نوع المصروفات</span><span class="sxs-lookup"><span data-stu-id="4fc64-111">Expense type</span></span> | <span data-ttu-id="4fc64-112">إجمالي مبلغ المصروفات</span><span class="sxs-lookup"><span data-stu-id="4fc64-112">Total expense amount</span></span> | <span data-ttu-id="4fc64-113">المبلغ الموزع على المشروع A</span><span class="sxs-lookup"><span data-stu-id="4fc64-113">Amount distributed to project A</span></span> | <span data-ttu-id="4fc64-114">المبلغ الموزع على المشروع B</span><span class="sxs-lookup"><span data-stu-id="4fc64-114">Amount distributed to project B</span></span> |
|--------------|----------------------|---------------------------------|---------------------------------|
| <span data-ttu-id="4fc64-115">سعر القطار</span><span class="sxs-lookup"><span data-stu-id="4fc64-115">Train fare</span></span>   | <span data-ttu-id="4fc64-116">DKK 578</span><span class="sxs-lookup"><span data-stu-id="4fc64-116">DKK 578</span></span>              | <span data-ttu-id="4fc64-117">DKK 405</span><span class="sxs-lookup"><span data-stu-id="4fc64-117">DKK 405</span></span>                         | <span data-ttu-id="4fc64-118">DKK 173</span><span class="sxs-lookup"><span data-stu-id="4fc64-118">DKK 173</span></span>                         |
| <span data-ttu-id="4fc64-119">فندق</span><span class="sxs-lookup"><span data-stu-id="4fc64-119">Hotel</span></span>        | <span data-ttu-id="4fc64-120">725 يورو</span><span class="sxs-lookup"><span data-stu-id="4fc64-120">EUR 725</span></span>              | <span data-ttu-id="4fc64-121">557 يورو</span><span class="sxs-lookup"><span data-stu-id="4fc64-121">EUR 557</span></span>                         | <span data-ttu-id="4fc64-122">168 يورو</span><span class="sxs-lookup"><span data-stu-id="4fc64-122">EUR 168</span></span>                         |
| <span data-ttu-id="4fc64-123">الوجبات</span><span class="sxs-lookup"><span data-stu-id="4fc64-123">Meals</span></span>        | <span data-ttu-id="4fc64-124">346 يورو</span><span class="sxs-lookup"><span data-stu-id="4fc64-124">EUR 346</span></span>              | <span data-ttu-id="4fc64-125">284 يورو</span><span class="sxs-lookup"><span data-stu-id="4fc64-125">EUR 284</span></span>                         | <span data-ttu-id="4fc64-126">62 يورو</span><span class="sxs-lookup"><span data-stu-id="4fc64-126">EUR 62</span></span>                          |
