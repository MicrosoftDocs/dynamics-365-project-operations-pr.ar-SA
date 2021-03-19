---
title: مراحل المشروع
description: يقدم هذا الموضوع معلومات حول مراحل المشروع المتوفرة في Microsoft Dynamics Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: a5c695e0cd39f8a222e719cc6c9ffe984fe80b07
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286772"
---
# <a name="project-stages"></a><span data-ttu-id="56ff7-103">مراحل المشروع</span><span class="sxs-lookup"><span data-stu-id="56ff7-103">Project stages</span></span>

<span data-ttu-id="56ff7-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="56ff7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="56ff7-105">يتم تصميم مراحل المشروع لتعكس حالة المشروع أثناء تقدمه.</span><span class="sxs-lookup"><span data-stu-id="56ff7-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="56ff7-106">يمكن استخدام التخصيصات لتحديث المراحل تلقائيًا باستخدام عمليات سير عمل الأعمال أو Power Automate أو ملحقات المكونات الإضافية.</span><span class="sxs-lookup"><span data-stu-id="56ff7-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="56ff7-107">يتم تعريف المراحل التالية في سير إجراءات العمل‬ الافتراضي:</span><span class="sxs-lookup"><span data-stu-id="56ff7-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="56ff7-108">جديدة</span><span class="sxs-lookup"><span data-stu-id="56ff7-108">New</span></span>
- <span data-ttu-id="56ff7-109">اقتباس</span><span class="sxs-lookup"><span data-stu-id="56ff7-109">Quote</span></span>
- <span data-ttu-id="56ff7-110">الخطة</span><span class="sxs-lookup"><span data-stu-id="56ff7-110">Plan</span></span>
- <span data-ttu-id="56ff7-111">تسليم</span><span class="sxs-lookup"><span data-stu-id="56ff7-111">Deliver</span></span>
- <span data-ttu-id="56ff7-112">تم</span><span class="sxs-lookup"><span data-stu-id="56ff7-112">Complete</span></span>
- <span data-ttu-id="56ff7-113">إقفال</span><span class="sxs-lookup"><span data-stu-id="56ff7-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="56ff7-114">جديدة</span><span class="sxs-lookup"><span data-stu-id="56ff7-114">New</span></span>

<span data-ttu-id="56ff7-115">عند إنشاء مشروع، يتم تعيين مرحلة المشروع إلى **جديد**.</span><span class="sxs-lookup"><span data-stu-id="56ff7-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="56ff7-116">إذا تم إنشاء المشروع من قالب، فقد يحتوي على جدول وتقدير وبيانات الفريق.</span><span class="sxs-lookup"><span data-stu-id="56ff7-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="56ff7-117">وبخلاف ذلك، فهو مخطط للمشروع، ويجب إدخال المكونات المتبقية.</span><span class="sxs-lookup"><span data-stu-id="56ff7-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="56ff7-118">عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="56ff7-118">Quote</span></span>

<span data-ttu-id="56ff7-119">عند ربط مشروع بعرض أسعار أو عند قيامك بإنشاء مشروع من عرض أسعار، فإنه يتم تعيين مرحلة المشروع إلى **عرض أسعار**، ويتم تحديث تواريخ البدء والانتهاء المقدرة.</span><span class="sxs-lookup"><span data-stu-id="56ff7-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="56ff7-120">عندما يكون المشروع في مرحلة **عرض الأسعار**، تعرض علامة التبويب **المبيعات** في **كيان المشروع** تفاصيل عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="56ff7-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="56ff7-121">الخطة</span><span class="sxs-lookup"><span data-stu-id="56ff7-121">Plan</span></span>

<span data-ttu-id="56ff7-122">عندما تفوز بعرض أسعار مقترن بمشروع، ويتم نقل الشروع إلى مرحلة **العقد**، فإنه يتم تحديث مرحلة المشروع إلى **الخطة**.</span><span class="sxs-lookup"><span data-stu-id="56ff7-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="56ff7-123">عندما يكون المشروع في مرحلة **الخطة**، تعرض صفحة **كيان المشروع** تفاصيل العقد.</span><span class="sxs-lookup"><span data-stu-id="56ff7-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="56ff7-124">تسليم</span><span class="sxs-lookup"><span data-stu-id="56ff7-124">Deliver</span></span>

<span data-ttu-id="56ff7-125">عند اكتمال خطة المشروع، وتكون مستعدًا لبدء المشروع، يتعين على مدير المشروع تحديث مرحلة المشروع إلى **التسليم** لإظهار أن المشروع قد بدأ.</span><span class="sxs-lookup"><span data-stu-id="56ff7-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="56ff7-126">‏‫مكتمل‬</span><span class="sxs-lookup"><span data-stu-id="56ff7-126">Complete</span></span> 

<span data-ttu-id="56ff7-127">عند اكتمال العمل الخاص بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **مكتمل**.</span><span class="sxs-lookup"><span data-stu-id="56ff7-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="56ff7-128">ومن خلال تحديث مرحلة المشروع إلى **مكتمل**، يشير مدير المشروع إلى أن العمل قد تم بنسبة 100 بالمائة، ولكنه تم فتح المشروع بحيث يمكن تسجيل أي إدخالات زمنية أو مصروفات معلقة.</span><span class="sxs-lookup"><span data-stu-id="56ff7-128">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="56ff7-129">إغلاق</span><span class="sxs-lookup"><span data-stu-id="56ff7-129">Close</span></span>

<span data-ttu-id="56ff7-130">عندما يتم تسجيل جميع الحركات الخاصة بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **الإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="56ff7-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="56ff7-131">وعند هذه النقطة، لا يمكن تسجيل أي حركات، ويتم تعيين المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="56ff7-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]