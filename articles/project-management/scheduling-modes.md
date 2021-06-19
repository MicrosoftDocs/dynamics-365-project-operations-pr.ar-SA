---
title: أوضاع الجدولة
description: يقدم هذا الموضوع معلومات أوضاع الجدولة.
author: ruhercul
ms.date: 05/28/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 508ff1df8f7e31066712fab6f8871dfdb107a43b
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116691"
---
# <a name="scheduling-modes"></a><span data-ttu-id="5625c-103">أوضاع الجدولة</span><span class="sxs-lookup"><span data-stu-id="5625c-103">Scheduling modes</span></span>

<span data-ttu-id="5625c-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="5625c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="5625c-105">يوفر Dynamics 365 Project Operations إمكانية للمؤسسات لتحديد كيفية إدارة التغييرات على المتغيرات الرئيسية في المهام داخل هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="5625c-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="5625c-106">استنادا إلى الاحتياجات الخاصة للمنظمة، يمكن لمديري المشروع إجراء تغييرات على وضع الجدولة عند إنشاء مشروع.</span><span class="sxs-lookup"><span data-stu-id="5625c-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="5625c-107">هناك ثلاثة أوضاع جدولة متوفرة في Project Operations:</span><span class="sxs-lookup"><span data-stu-id="5625c-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="5625c-108">المدة الثابتة (هذا هو الوضع الافتراضي)</span><span class="sxs-lookup"><span data-stu-id="5625c-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="5625c-109">الجهد الثابت (*العمل*)</span><span class="sxs-lookup"><span data-stu-id="5625c-109">Fixed effort (*Work*)</span></span>
  - <span data-ttu-id="5625c-110">وحدات ثابتة</span><span class="sxs-lookup"><span data-stu-id="5625c-110">Fixed units</span></span>

<span data-ttu-id="5625c-111">تتحدد القيم المتأثرة بتعريف وضع جدولة معين بالمعادلة التالية:</span><span class="sxs-lookup"><span data-stu-id="5625c-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="5625c-112">الجهد = المدة x الوحدات</span><span class="sxs-lookup"><span data-stu-id="5625c-112">Effort  = Duration x Units</span></span>

<span data-ttu-id="5625c-113">عند تعريف وضع الجدولة لمشروع، فإنك تقوم بإعداد إحدى هذه القيم، والتي لا يمكن تغييرها بعد ذلك.</span><span class="sxs-lookup"><span data-stu-id="5625c-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="5625c-114">وتثبيت هذه القيمة في أماكن ثابتة يعطي أولوية لهذه القيمة، ومن ثم يتم إخطار النظام بعدم تغييرها عند تغيير القيمتين الأخرتين.</span><span class="sxs-lookup"><span data-stu-id="5625c-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="5625c-115">يوفر الجدول التالي معلومات حول تأثيرات اختيار وضع معين.</span><span class="sxs-lookup"><span data-stu-id="5625c-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="5625c-116">**في هذه المهمة**</span><span class="sxs-lookup"><span data-stu-id="5625c-116">**In this task**</span></span>             | <span data-ttu-id="5625c-117">**إذا راجعت الوحدات**</span><span class="sxs-lookup"><span data-stu-id="5625c-117">**If you revise units**</span></span>   | <span data-ttu-id="5625c-118">**إذا راجعت المدة**</span><span class="sxs-lookup"><span data-stu-id="5625c-118">**If you revise duration**</span></span> | <span data-ttu-id="5625c-119">**إذا راجعت الجهد**</span><span class="sxs-lookup"><span data-stu-id="5625c-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="5625c-120">مهمة وحدات ثابتة</span><span class="sxs-lookup"><span data-stu-id="5625c-120">Fixed units task</span></span>     | <span data-ttu-id="5625c-121">يتم إعادة حساب المدة.</span><span class="sxs-lookup"><span data-stu-id="5625c-121">Duration is recalculated.</span></span> | <span data-ttu-id="5625c-122">يتم إعادة حساب الجهد.</span><span class="sxs-lookup"><span data-stu-id="5625c-122">Effort is recalculated.</span></span>    | <span data-ttu-id="5625c-123">يتم إعادة حساب المدة.</span><span class="sxs-lookup"><span data-stu-id="5625c-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="5625c-124">مهمة الجهد الثابت</span><span class="sxs-lookup"><span data-stu-id="5625c-124">Fixed effort task</span></span>    | <span data-ttu-id="5625c-125">يتم إعادة حساب المدة.</span><span class="sxs-lookup"><span data-stu-id="5625c-125">Duration is recalculated.</span></span> | <span data-ttu-id="5625c-126">يتم إعادة حساب الوحدات.</span><span class="sxs-lookup"><span data-stu-id="5625c-126">Units are recalculated.</span></span>    | <span data-ttu-id="5625c-127">يتم إعادة حساب المدة.</span><span class="sxs-lookup"><span data-stu-id="5625c-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="5625c-128">مهمة المدة الثابتة</span><span class="sxs-lookup"><span data-stu-id="5625c-128">Fixed duration task</span></span>  | <span data-ttu-id="5625c-129">يتم إعادة حساب الجهد.</span><span class="sxs-lookup"><span data-stu-id="5625c-129">Effort is recalculated.</span></span>   | <span data-ttu-id="5625c-130">يتم إعادة حساب الجهد.</span><span class="sxs-lookup"><span data-stu-id="5625c-130">Effort is recalculated.</span></span>    | <span data-ttu-id="5625c-131">يتم إعادة حساب الوحدات.</span><span class="sxs-lookup"><span data-stu-id="5625c-131">Units are recalculated.</span></span>   |

<span data-ttu-id="5625c-132">لمزيد من المعلومات حول تأثيرات وضع معين، راجع [تغيير نوع المهمة لجدولة أكثر دقة](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="5625c-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="5625c-133">في موضوع، يتم استخدام مصطلح **العمل** بدلا من **الجهد**.</span><span class="sxs-lookup"><span data-stu-id="5625c-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="5625c-134">تغيير وضع الجدولة للمؤسسة</span><span class="sxs-lookup"><span data-stu-id="5625c-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="5625c-135">أكمل الخطوات التالية لتعريف وضع الجدولة في مؤسسة.</span><span class="sxs-lookup"><span data-stu-id="5625c-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="5625c-136">انتقل إلى **الإعدادات** \> **عام** \> **المعلمات**، وحدد معلمة المشروع.</span><span class="sxs-lookup"><span data-stu-id="5625c-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="5625c-137">في صفحة **معلمات المشروع**، حدد وضع الجدولة الافتراضي للمنظمة، ثم حدد القدرة لمدير المشروع لتجاوز الإعداد عند إنشاء مشروع جديد.</span><span class="sxs-lookup"><span data-stu-id="5625c-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="5625c-138">تغيير إعداد وضع الجدولة في مشروع</span><span class="sxs-lookup"><span data-stu-id="5625c-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="5625c-139">إذا كانت المؤسسة تسمح لمدير المشروع بتجاوز وضع الجدولة الافتراضي، فيمكن لمدير المشروع إجراء هذا التغيير عند إنشاء مشروع جديد.</span><span class="sxs-lookup"><span data-stu-id="5625c-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="5625c-140">ومع ذلك، لا يمكن تغيير وضع الجدولة بعد حفظ المشروع.</span><span class="sxs-lookup"><span data-stu-id="5625c-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="5625c-141">مشاريع المنسوخة</span><span class="sxs-lookup"><span data-stu-id="5625c-141">Copied projects</span></span>

<span data-ttu-id="5625c-142">نظرا لإنشاء المشروع عند تنفيذ إجراء نسخ المشروع، لا يمكن لمدير المشروع تعيين وضع الجدولة.</span><span class="sxs-lookup"><span data-stu-id="5625c-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="5625c-143">يتخذ المشروع الوجهة دائمًا قيمته الافتراضية من الوضع المحدد على المستوى المؤسسي.</span><span class="sxs-lookup"><span data-stu-id="5625c-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="5625c-144">المهام المنسوخة</span><span class="sxs-lookup"><span data-stu-id="5625c-144">Copied tasks</span></span>

<span data-ttu-id="5625c-145">عند نسخ مهمة من مشروع إلى آخر، فإن المهمة ترث وضع جدولة المشروع الوجهة.</span><span class="sxs-lookup"><span data-stu-id="5625c-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
