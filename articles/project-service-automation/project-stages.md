---
title: مراحل المشروع
description: يقدم هذا الموضوع معلومات حول مراحل المشروع.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 983c25a0-ed21-4151-a109-b385a88285fa
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 70aa057e127df7ba925e84f5d056a06a4cc8833e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748629"
---
# <a name="project-stages"></a><span data-ttu-id="9fbcc-103">مراحل المشروع</span><span class="sxs-lookup"><span data-stu-id="9fbcc-103">Project stages</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="9fbcc-104">يتم تحديث مراحل المشروع لعكس حالة المشروع أثناء تقدمه.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-104">Project stages are updated to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="9fbcc-105">يعمل سير إجراءات العمل الافتراضي على تحديث بعش مراحل المشروع تلقائيًا بينما يتم تحديث مراحل أخرى يدويًا بواسطة مدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-105">The default business process flow automatically updates some stages of the project while others are manually updated by the project manager.</span></span> 

<span data-ttu-id="9fbcc-106">يتم تعريف المراحل التالية في سير إجراءات العمل‬ الافتراضي:</span><span class="sxs-lookup"><span data-stu-id="9fbcc-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="9fbcc-107">جديد</span><span class="sxs-lookup"><span data-stu-id="9fbcc-107">New</span></span>
- <span data-ttu-id="9fbcc-108">عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="9fbcc-108">Quote</span></span>
- <span data-ttu-id="9fbcc-109">الخطة</span><span class="sxs-lookup"><span data-stu-id="9fbcc-109">Plan</span></span>
- <span data-ttu-id="9fbcc-110">تسليم</span><span class="sxs-lookup"><span data-stu-id="9fbcc-110">Deliver</span></span>
- <span data-ttu-id="9fbcc-111">‏‫مكتمل‬</span><span class="sxs-lookup"><span data-stu-id="9fbcc-111">Complete</span></span>
- <span data-ttu-id="9fbcc-112">إغلاق</span><span class="sxs-lookup"><span data-stu-id="9fbcc-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="9fbcc-113">جديد</span><span class="sxs-lookup"><span data-stu-id="9fbcc-113">New</span></span>

<span data-ttu-id="9fbcc-114">عند إنشاء مشروع، يتم تعيين مرحلة المشروع إلى **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="9fbcc-115">إذا تم إنشاء المشروع من قالب، فقد يحتوي على جدول وتقدير وبيانات الفريق.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="9fbcc-116">وبخلاف ذلك، فهو مجرد مخطط للمشروع، ويجب إدخال المكونات المتبقية.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="9fbcc-117">عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="9fbcc-117">Quote</span></span>

<span data-ttu-id="9fbcc-118">عند ربط مشروع بعرض أسعار أو عند قيامك بإنشاء مشروع من عرض أسعار، فإنه يتم تعيين مرحلة المشروع إلى **عرض أسعار**، ويتم تحديث تواريخ البدء والانتهاء المقدرة.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="9fbcc-119">عندما يكون المشروع في مرحلة **عرض الأسعار**، تعرض علامة التبويب **المبيعات** في **كيان المشروع** تفاصيل عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="9fbcc-120">الخطة</span><span class="sxs-lookup"><span data-stu-id="9fbcc-120">Plan</span></span>

<span data-ttu-id="9fbcc-121">عندما تفوز بعرض أسعار مقترن بمشروع، ويتم نقل الشروع إلى مرحلة **العقد**، فإنه يتم تحديث مرحلة المشروع إلى **الخطة**.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="9fbcc-122">عندما يكون المشروع في مرحلة **الخطة**، تعرض صفحة **كيان المشروع** تفاصيل العقد.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="9fbcc-123">تسليم</span><span class="sxs-lookup"><span data-stu-id="9fbcc-123">Deliver</span></span>

<span data-ttu-id="9fbcc-124">عند اكتمال خطة المشروع، وتكون مستعدًا لبدء المشروع، يتعين علي مدير المشروع تحديث مرحلة المشروع إلى **التسليم** لإظهار أن المشروع قد بدأ.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="9fbcc-125">‏‫مكتمل‬</span><span class="sxs-lookup"><span data-stu-id="9fbcc-125">Complete</span></span> 

<span data-ttu-id="9fbcc-126">عند اكتمال العمل الخاص بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **مكتمل**.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="9fbcc-127">ومن خلال تحديث مرحلة المشروع إلى **مكتمل**، يشير مدير المشروع إلى أن العمل قد تم بنسبة 100 بالمائة، ولكنه تم فتح المشروع بحيث يمكن تسجيل أي إدخالات زمنية أو مصروفات معلقة.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="9fbcc-128">إغلاق</span><span class="sxs-lookup"><span data-stu-id="9fbcc-128">Close</span></span>

<span data-ttu-id="9fbcc-129">عندما يتم تسجيل جميع الحركات الخاصة بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **الإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="9fbcc-130">وعند هذه النقطة، لا يمكن تسجيل أي حركات، ويتم تعيين المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="9fbcc-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>
