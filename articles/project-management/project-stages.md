---
title: مراحل المشروع
description: يقدم هذا الموضوع معلومات حول مراحل المشروع المتوفرة في Microsoft Dynamics Project Operations.
author: ruhercul
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 079c3d2d16cf802d2b9ecc779577e6e390d92ddc
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996910"
---
# <a name="project-stages"></a><span data-ttu-id="90ab6-103">مراحل المشروع</span><span class="sxs-lookup"><span data-stu-id="90ab6-103">Project stages</span></span>

<span data-ttu-id="90ab6-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="90ab6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="90ab6-105">يتم تصميم مراحل المشروع لتعكس حالة المشروع أثناء تقدمه.</span><span class="sxs-lookup"><span data-stu-id="90ab6-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="90ab6-106">يمكن استخدام التخصيصات لتحديث المراحل تلقائيًا باستخدام عمليات سير عمل الأعمال أو Power Automate أو ملحقات المكونات الإضافية.</span><span class="sxs-lookup"><span data-stu-id="90ab6-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="90ab6-107">يتم تعريف المراحل التالية في سير إجراءات العمل‬ الافتراضي:</span><span class="sxs-lookup"><span data-stu-id="90ab6-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="90ab6-108">جديدة</span><span class="sxs-lookup"><span data-stu-id="90ab6-108">New</span></span>
- <span data-ttu-id="90ab6-109">اقتباس</span><span class="sxs-lookup"><span data-stu-id="90ab6-109">Quote</span></span>
- <span data-ttu-id="90ab6-110">الخطة</span><span class="sxs-lookup"><span data-stu-id="90ab6-110">Plan</span></span>
- <span data-ttu-id="90ab6-111">تسليم</span><span class="sxs-lookup"><span data-stu-id="90ab6-111">Deliver</span></span>
- <span data-ttu-id="90ab6-112">تم</span><span class="sxs-lookup"><span data-stu-id="90ab6-112">Complete</span></span>
- <span data-ttu-id="90ab6-113">إقفال</span><span class="sxs-lookup"><span data-stu-id="90ab6-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="90ab6-114">جديدة</span><span class="sxs-lookup"><span data-stu-id="90ab6-114">New</span></span>

<span data-ttu-id="90ab6-115">عند إنشاء مشروع، يتم تعيين مرحلة المشروع إلى **جديد**.</span><span class="sxs-lookup"><span data-stu-id="90ab6-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="90ab6-116">إذا تم إنشاء المشروع من قالب، فقد يحتوي على جدول وتقدير وبيانات الفريق.</span><span class="sxs-lookup"><span data-stu-id="90ab6-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="90ab6-117">وبخلاف ذلك، فهو مخطط للمشروع، ويجب إدخال المكونات المتبقية.</span><span class="sxs-lookup"><span data-stu-id="90ab6-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="90ab6-118">عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="90ab6-118">Quote</span></span>

<span data-ttu-id="90ab6-119">عند ربط مشروع بعرض أسعار أو عند قيامك بإنشاء مشروع من عرض أسعار، فإنه يتم تعيين مرحلة المشروع إلى **عرض أسعار**، ويتم تحديث تواريخ البدء والانتهاء المقدرة.</span><span class="sxs-lookup"><span data-stu-id="90ab6-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="90ab6-120">عندما يكون المشروع في مرحلة **عرض الأسعار**، تعرض علامة التبويب **المبيعات** في **كيان المشروع** تفاصيل عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="90ab6-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="90ab6-121">الخطة</span><span class="sxs-lookup"><span data-stu-id="90ab6-121">Plan</span></span>

<span data-ttu-id="90ab6-122">عندما تفوز بعرض أسعار مقترن بمشروع، ويتم نقل الشروع إلى مرحلة **العقد**، فإنه يتم تحديث مرحلة المشروع إلى **الخطة**.</span><span class="sxs-lookup"><span data-stu-id="90ab6-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="90ab6-123">عندما يكون المشروع في مرحلة **الخطة**، تعرض صفحة **كيان المشروع** تفاصيل العقد.</span><span class="sxs-lookup"><span data-stu-id="90ab6-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="90ab6-124">تسليم</span><span class="sxs-lookup"><span data-stu-id="90ab6-124">Deliver</span></span>

<span data-ttu-id="90ab6-125">عند اكتمال خطة المشروع، وتكون مستعدًا لبدء المشروع، يتعين على مدير المشروع تحديث مرحلة المشروع إلى **التسليم** لإظهار أن المشروع قد بدأ.</span><span class="sxs-lookup"><span data-stu-id="90ab6-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="90ab6-126">‏‫مكتمل‬</span><span class="sxs-lookup"><span data-stu-id="90ab6-126">Complete</span></span> 

<span data-ttu-id="90ab6-127">عند اكتمال العمل الخاص بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **مكتمل**.</span><span class="sxs-lookup"><span data-stu-id="90ab6-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="90ab6-128">ومن خلال تحديث مرحلة المشروع إلى **مكتمل**، يشير مدير المشروع إلى أن العمل قد تم بنسبة 100 بالمائة، ولكنه تم فتح المشروع بحيث يمكن تسجيل أي إدخالات زمنية أو مصروفات معلقة.</span><span class="sxs-lookup"><span data-stu-id="90ab6-128">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="90ab6-129">إغلاق</span><span class="sxs-lookup"><span data-stu-id="90ab6-129">Close</span></span>

<span data-ttu-id="90ab6-130">عندما يتم تسجيل جميع الحركات الخاصة بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **الإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="90ab6-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="90ab6-131">وعند هذه النقطة، لا يمكن تسجيل أي حركات، ويتم تعيين المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="90ab6-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]