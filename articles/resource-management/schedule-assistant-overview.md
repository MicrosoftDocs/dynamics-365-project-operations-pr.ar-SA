---
title: نظرة عامة على مساعد الجدولة
description: يقدم هذا الموضوع معلومات حول التعامل مع مساعد الجدولة لحجز الموارد.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: da551e805f395e466952df1dbb7d193bdddba358
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907804"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="68745-103">نظرة عامة على مساعد الجدولة</span><span class="sxs-lookup"><span data-stu-id="68745-103">Schedule assistant overview</span></span>

<span data-ttu-id="68745-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="68745-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="68745-105">يتم استخدام مساعد الجدولة لحجز الموارد استنادا إلى المتطلبات المحددة بواسطة مدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="68745-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="68745-106">يعتمد مساعد الجدولة على المعلمات التي تم توفيرها في متطلب المورد للعثور على المورد.</span><span class="sxs-lookup"><span data-stu-id="68745-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="68745-107">يوصي مساعد الجدولة بالموارد التي تطابق المتطلبات ذات الصلة، مثل إطارات الوقت أو المهارات اللازمة.</span><span class="sxs-lookup"><span data-stu-id="68745-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="68745-108">بعد تحديد الموارد المناسبة، يمكن لمورد أو مدير المشروع حجز المورد للعمل.</span><span class="sxs-lookup"><span data-stu-id="68745-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68745-109">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="68745-109">Prerequisites</span></span>

<span data-ttu-id="68745-110">يعد مساعد الجدولة جزءًا من حل Universal Resource Scheduling.</span><span class="sxs-lookup"><span data-stu-id="68745-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="68745-111">يتم تضمين هذا الحل وتثبيته مع Dynamics 365 Project Operations وDynamics 365 Field Service وDynamics 365 Customer Service.</span><span class="sxs-lookup"><span data-stu-id="68745-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="68745-112">الموارد والمتطلبات المتطابقة</span><span class="sxs-lookup"><span data-stu-id="68745-112">Matching requirements and resources</span></span>

<span data-ttu-id="68745-113">ويعتمد متطلب المورد الذي تم إنشاؤه على التفاصيل مثل:</span><span class="sxs-lookup"><span data-stu-id="68745-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="68745-114">الخصائص</span><span class="sxs-lookup"><span data-stu-id="68745-114">Characteristics</span></span>
-   <span data-ttu-id="68745-115">الأدوار</span><span class="sxs-lookup"><span data-stu-id="68745-115">Roles</span></span>
-   <span data-ttu-id="68745-116">وحدات العمل</span><span class="sxs-lookup"><span data-stu-id="68745-116">Business units</span></span>
-   <span data-ttu-id="68745-117">تفضيلات الموارد</span><span class="sxs-lookup"><span data-stu-id="68745-117">Resource preferences</span></span>
-   <span data-ttu-id="68745-118">محيطات المجهود</span><span class="sxs-lookup"><span data-stu-id="68745-118">Effort contours</span></span>
-   <span data-ttu-id="68745-119">المنطقة الزمنية</span><span class="sxs-lookup"><span data-stu-id="68745-119">Time zone</span></span>

<span data-ttu-id="68745-120">يستخدم مساعد الجدولة هذه التفاصيل لتصفية الموارد.</span><span class="sxs-lookup"><span data-stu-id="68745-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="68745-121">تشغيل مساعد الجدولة</span><span class="sxs-lookup"><span data-stu-id="68745-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="68745-122">هناك طريقتان لتشغيل مساعد الجدولة.</span><span class="sxs-lookup"><span data-stu-id="68745-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="68745-123">إذا كنت تستخدم الوضع المختلط، ففي شبكة أعضاء الفريق يمكنك تحديد أي عضو فريق بمتطلبات مورد غير مستوفاة، ثم تحديد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="68745-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="68745-124">إذا كنت تستخدم الوضع المركزي، فسيعثر مدير المورد على المورد ويحدده.</span><span class="sxs-lookup"><span data-stu-id="68745-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="68745-125">عوامل تصفية مساعد الجدولة</span><span class="sxs-lookup"><span data-stu-id="68745-125">Schedule assistant filters</span></span>

<span data-ttu-id="68745-126">بعد تشغيل مساعد الجدولة، يتم عرض التفاصيل من متطلبات المورد كقيم مصفاة في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="68745-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="68745-127">يمكن لمدير الموارد أو مدير المشروع ضبط النتائج بشكل دقيق من خلال ضبط عوامل التصفية لتلبية احتياجات الجدولة.</span><span class="sxs-lookup"><span data-stu-id="68745-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="68745-128">يظهر جزء عامل التصفية الخيارات المتعلقة بالعمل، بما في ذلك:</span><span class="sxs-lookup"><span data-stu-id="68745-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="68745-129">بدء وانتهاء العمل</span><span class="sxs-lookup"><span data-stu-id="68745-129">Work start and end</span></span>
-   <span data-ttu-id="68745-130">الخصائص</span><span class="sxs-lookup"><span data-stu-id="68745-130">Characteristics</span></span>
-   <span data-ttu-id="68745-131">الأدوار</span><span class="sxs-lookup"><span data-stu-id="68745-131">Roles</span></span>
-   <span data-ttu-id="68745-132">الوحدات التنظيمية</span><span class="sxs-lookup"><span data-stu-id="68745-132">Organizational units</span></span>
-   <span data-ttu-id="68745-133">شركة تعيين الموارد‬</span><span class="sxs-lookup"><span data-stu-id="68745-133">Resourcing company</span></span>
-   <span data-ttu-id="68745-134">أنواع الموارد</span><span class="sxs-lookup"><span data-stu-id="68745-134">Resource types</span></span>
-   <span data-ttu-id="68745-135">الموارد المفضلة</span><span class="sxs-lookup"><span data-stu-id="68745-135">Preferred resources</span></span>
