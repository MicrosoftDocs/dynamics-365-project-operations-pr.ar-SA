---
title: أنواع مراحل المشروع
description: يقدم هذا الموضوع معلومات حول مراحل المشروع.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 06/19/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: ed725d8ea2f671c45a7a19bb017bbb08c41f42db
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6008970"
---
# <a name="project-stage-types"></a><span data-ttu-id="e31e2-103">أنواع مراحل المشروع</span><span class="sxs-lookup"><span data-stu-id="e31e2-103">Project stage types</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e31e2-104">يتم تصميم مراحل المشروع لتعكس حالة المشروع أثناء تقدمه.</span><span class="sxs-lookup"><span data-stu-id="e31e2-104">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="e31e2-105">يمكن استخدام التخصيصات لتحديث المراحل تلقائيًا باستخدام عمليات سير عمل الأعمال أو Power Automate أو ملحقات المكونات الإضافية.</span><span class="sxs-lookup"><span data-stu-id="e31e2-105">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="e31e2-106">يتم تعريف المراحل التالية في سير إجراءات العمل‬ الافتراضي:</span><span class="sxs-lookup"><span data-stu-id="e31e2-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="e31e2-107">جديد</span><span class="sxs-lookup"><span data-stu-id="e31e2-107">New</span></span>
- <span data-ttu-id="e31e2-108">اقتباس</span><span class="sxs-lookup"><span data-stu-id="e31e2-108">Quote</span></span>
- <span data-ttu-id="e31e2-109">الخطة</span><span class="sxs-lookup"><span data-stu-id="e31e2-109">Plan</span></span>
- <span data-ttu-id="e31e2-110">تسليم</span><span class="sxs-lookup"><span data-stu-id="e31e2-110">Deliver</span></span>
- <span data-ttu-id="e31e2-111">‏‫مكتمل‬</span><span class="sxs-lookup"><span data-stu-id="e31e2-111">Complete</span></span>
- <span data-ttu-id="e31e2-112">إغلاق</span><span class="sxs-lookup"><span data-stu-id="e31e2-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="e31e2-113">جديد</span><span class="sxs-lookup"><span data-stu-id="e31e2-113">New</span></span>

<span data-ttu-id="e31e2-114">عند إنشاء مشروع، يتم تعيين مرحلة المشروع إلى **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e31e2-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="e31e2-115">إذا تم إنشاء المشروع من قالب، فقد يحتوي على جدول وتقدير وبيانات الفريق.</span><span class="sxs-lookup"><span data-stu-id="e31e2-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="e31e2-116">وبخلاف ذلك، فهو مجرد مخطط للمشروع، ويجب إدخال المكونات المتبقية.</span><span class="sxs-lookup"><span data-stu-id="e31e2-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="e31e2-117">عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="e31e2-117">Quote</span></span>

<span data-ttu-id="e31e2-118">عند ربط مشروع بعرض أسعار أو عند قيامك بإنشاء مشروع من عرض أسعار، فإنه يتم تعيين مرحلة المشروع إلى **عرض أسعار**، ويتم تحديث تواريخ البدء والانتهاء المقدرة.</span><span class="sxs-lookup"><span data-stu-id="e31e2-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="e31e2-119">عندما يكون المشروع في مرحلة **عرض الأسعار**، تعرض علامة التبويب **المبيعات** في **كيان المشروع** تفاصيل عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="e31e2-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="e31e2-120">الخطة</span><span class="sxs-lookup"><span data-stu-id="e31e2-120">Plan</span></span>

<span data-ttu-id="e31e2-121">عندما تفوز بعرض أسعار مقترن بمشروع، ويتم نقل الشروع إلى مرحلة **العقد**، فإنه يتم تحديث مرحلة المشروع إلى **الخطة**.</span><span class="sxs-lookup"><span data-stu-id="e31e2-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="e31e2-122">عندما يكون المشروع في مرحلة **الخطة**، تعرض صفحة **كيان المشروع** تفاصيل العقد.</span><span class="sxs-lookup"><span data-stu-id="e31e2-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="e31e2-123">تسليم</span><span class="sxs-lookup"><span data-stu-id="e31e2-123">Deliver</span></span>

<span data-ttu-id="e31e2-124">عند اكتمال خطة المشروع، وتكون مستعدًا لبدء المشروع، يتعين على مدير المشروع تحديث مرحلة المشروع إلى **التسليم** لإظهار أن المشروع قد بدأ.</span><span class="sxs-lookup"><span data-stu-id="e31e2-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="e31e2-125">‏‫مكتمل‬</span><span class="sxs-lookup"><span data-stu-id="e31e2-125">Complete</span></span> 

<span data-ttu-id="e31e2-126">عند اكتمال العمل الخاص بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **مكتمل**.</span><span class="sxs-lookup"><span data-stu-id="e31e2-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="e31e2-127">ومن خلال تحديث مرحلة المشروع إلى **مكتمل**، يشير مدير المشروع إلى أن العمل قد تم بنسبة 100 بالمائة، ولكنه تم فتح المشروع بحيث يمكن تسجيل أي إدخالات زمنية أو مصروفات معلقة.</span><span class="sxs-lookup"><span data-stu-id="e31e2-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="e31e2-128">إغلاق</span><span class="sxs-lookup"><span data-stu-id="e31e2-128">Close</span></span>

<span data-ttu-id="e31e2-129">عندما يتم تسجيل جميع الحركات الخاصة بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **الإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="e31e2-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="e31e2-130">وعند هذه النقطة، لا يمكن تسجيل أي حركات، ويتم تعيين المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="e31e2-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]