---
title: تعيين مورد للعمل على مهمة
description: يوفر هذا الموضوع معلومات حول كيفية تعيين الموارد إلى المهام.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
ms.topic: article
ms.prod: Project Service
ms.technology: Dynamics 365 Project Service Automation 3.x
ms.assetid: 3ea9516c-0276-4e30-b308-f792f64d608b
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 509f7a4464b2e810900b31a78219ba696192a18b
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748756"
---
# <a name="assign-a-resource-to-a-task"></a><span data-ttu-id="006e8-103">تعيين مورد للعمل على مهمة</span><span class="sxs-lookup"><span data-stu-id="006e8-103">Assign a resource to a task</span></span>

<span data-ttu-id="006e8-104">هناك ثلاثة طرق لتعيين مورد لتنفيذ مهمة في Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="006e8-104">There are three ways to assign a resource to a task in Microsoft Dynamics 365 Project Service Automation.</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="006e8-105">حجز مورد كعضو فريق، ثم تعيين المورد لتنفيذ مهمة</span><span class="sxs-lookup"><span data-stu-id="006e8-105">Book a resource as a team member, and then assign the resource to a task</span></span>

<span data-ttu-id="006e8-106">يمكنك إضافة مورد إلى فريق المشروع، ثم تعيين المورد لتنفيذ المهام في جدول المشروع.</span><span class="sxs-lookup"><span data-stu-id="006e8-106">You can add a resource to the project team, and then assign the resource to tasks in the project schedule.</span></span>

1. <span data-ttu-id="006e8-107">في علامة تبويب **عضو الفريق**، أضف عضو فريق جديدًا بتحديد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="006e8-107">On the **Team Member** tab, add a new team member by selecting **New**.</span></span> 

2. <span data-ttu-id="006e8-108">تفتح لوحة **الإنشاء السريع لعضو الفريق**، حيث يمكنك تحديد اسم المورد القابل للحجز وتعيين دور.</span><span class="sxs-lookup"><span data-stu-id="006e8-108">The **Team Member Quick Create** panel opens, where you can select the bookable resource name and set a role.</span></span> 

    <span data-ttu-id="006e8-109">حدد أحد أساليب التوزيع التالية لحجز المورد:</span><span class="sxs-lookup"><span data-stu-id="006e8-109">Select one of the following allocation methods for the resource’s booking:</span></span>

    - <span data-ttu-id="006e8-110">**القدرة الإنتاجية الكاملة** هذا الأسلوب يحجز القدرة الإنتاجية الكاملة للمورد لتواريخ "من" و"إلى" المحددة.</span><span class="sxs-lookup"><span data-stu-id="006e8-110">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="006e8-111">**النسبة المئوية للقدرة الإنتاجية‬** هذا الأسلوب يحجز المورد للنسبة المئوية من القدرة الإنتاجية لتواريخ "من" و"إلى" المحددة.</span><span class="sxs-lookup"><span data-stu-id="006e8-111">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="006e8-112">**توزيع بالتساوي حسب الساعات‬‬** هذا الأسلوب يحجز المورد لعدد محدد من الساعات، ويؤدي إلى توزيع الوقت بطريقة متساوية لكل يوم على مدى تواريخ "من" و"إلى" المحددة.‬</span><span class="sxs-lookup"><span data-stu-id="006e8-112">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing them evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="006e8-113">**الحمل في البداية حسب الساعات‬** هذا الأسلوب يحجز المورد لعدد محدد من الساعات، ويؤدي إلى توزيع الحمل في البداية لساعات العمل لكل يوم على مدى تواريخ "من" و"إلى" المحددة.‬</span><span class="sxs-lookup"><span data-stu-id="006e8-113">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>
    - <span data-ttu-id="006e8-114">**بلا** هذا الأسلوب يضيف المورد إلى الفريق، ولكنه لا ينشئ أية حجوزات تستوعب قدرته الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="006e8-114">**None** adds the resource to the team but doesn’t create any bookings that absorb their capacity.</span></span>

3. <span data-ttu-id="006e8-115">في شبكة **الجدولة** لمهمة ما، حدد أيقونة **الموارد** في خلية المورد، ثم تحت **أعضاء الفريق**، حدد عضو الفريق الذي أضفته للتو.</span><span class="sxs-lookup"><span data-stu-id="006e8-115">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell, and then under **Team Members**, select the team member you just added.</span></span> 

> [!NOTE]
> <span data-ttu-id="006e8-116">في علامتي التبويب **عضو الفريق** و**التسوية**، يُظهر المورد الساعات المحجوزة والساعات المعينة.</span><span class="sxs-lookup"><span data-stu-id="006e8-116">On the **Team Member** and **Reconciliation** tabs, the resource shows booked and assigned hours.</span></span> <span data-ttu-id="006e8-117">من المفترض أن تكون هذه الساعات مماثلة، ولكن هذا ليس مطلوبًا لأن الحجوزات والتعيينات غير مرتبطة بشكل وثيق.</span><span class="sxs-lookup"><span data-stu-id="006e8-117">The hours should be the same, but it isn't required as bookings and assignments are not tightly coupled.</span></span> <span data-ttu-id="006e8-118">توفر لك علامة تبويب **التسوية** تفاصيل عندما تكون هذه الساعات مختلفة، على سبيل المثال، عندما تقوم بتعيين مورد لعدد من الساعات يتجاوز الساعات المحجوزة.</span><span class="sxs-lookup"><span data-stu-id="006e8-118">The **Reconciliation** tab gives you details when they are different, such as when you assign a resource more hours than you have booked.</span></span> <span data-ttu-id="006e8-119">إذا لزم الأمر، يمكنك تصحيح المعلومات بتمديد حجوزات المورد أو تغيير التعيين.</span><span class="sxs-lookup"><span data-stu-id="006e8-119">If needed, you can correct the information by extending the resource's bookings or changing the assignment.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="006e8-120">إنشاء عضو فريق عام من خلال تعيين المهام</span><span class="sxs-lookup"><span data-stu-id="006e8-120">Create a generic team member through task assignment</span></span>

<span data-ttu-id="006e8-121">عندما تنشئ عضو فريق عام عن طريق تعيين المهام، فإنك تنشئ موردًا نائبًا أو عامًا يصف خصائص المورد المسمى الذي تريده في النهاية أن يعمل على المهام.</span><span class="sxs-lookup"><span data-stu-id="006e8-121">When you create a generic team member through task assignment, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="006e8-122">وعليك بعد ذلك إنشاء متطلب (أو ترسل طلبًا باستخدام المتطلب) يتم استخدامها للبحث عن المورد المسمى وحجزه.</span><span class="sxs-lookup"><span data-stu-id="006e8-122">You then generate a requirement (or submit a request using the requirement) that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="006e8-123">على شبكة **الجدولة** لمهمة ما، حدد أيقونة **المورد** في خلية المورد.</span><span class="sxs-lookup"><span data-stu-id="006e8-123">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="006e8-124">اكتب اسمًا يُستخدم كاسم مورد نائب.</span><span class="sxs-lookup"><span data-stu-id="006e8-124">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="006e8-125">على سبيل المثال، مدير مشروع.</span><span class="sxs-lookup"><span data-stu-id="006e8-125">For example, Program Manager.</span></span>

3. <span data-ttu-id="006e8-126">حدد **إنشاء**، وفي حقل **إنشاء سريع لعضو فريق المشروع**، قم بتعيين دور للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="006e8-126">Select **Create**, and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>

4. <span data-ttu-id="006e8-127">يمكنك مواصلة تعيين المهام إلى هذا المورد النائب عن طريق تحديد المورد على **محدد المورد** للمهمة.</span><span class="sxs-lookup"><span data-stu-id="006e8-127">You can continue to assign tasks to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="006e8-128">تكون الموارد مدرجة ضمن **أعضاء الفريق**.</span><span class="sxs-lookup"><span data-stu-id="006e8-128">They’re listed under **Team Members**.</span></span>

5. <span data-ttu-id="006e8-129">عند الانتهاء من تعيين المورد العام، حدد المورد العام على علامة تبويب **الفريق**، وحدد **إنشاء المتطلب** لإنشاء متطلبات الموارد للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="006e8-129">When you’re done assigning the generic resource, select the generic resource on the **Team** tab, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>

6. <span data-ttu-id="006e8-130">حدد **حجز** للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="006e8-130">Select **Book** for the generic resource.</span></span> <span data-ttu-id="006e8-131">عندئذ يمكنك استخدام لوحة الجدولة للبحث عن مورد حقيقي وحجزه.</span><span class="sxs-lookup"><span data-stu-id="006e8-131">You can then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="006e8-132">يمكنك أيضًا إرسال متطلبات التنفيذ بواسطة مدير الموارد.</span><span class="sxs-lookup"><span data-stu-id="006e8-132">You can also submit the requirement for fulfillment by a resource manager.</span></span>

7. <span data-ttu-id="006e8-133">عند تنفيذ المورد العام بواسطة مورد مسمى، تتم إزالة المورد العام من الفريق ويتم تعيين تعيينات المهام الخاصة بالمورد العام إلى المورد المسمى الذي قام بتنفيذ متطلبات الموارد للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="006e8-133">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="006e8-134">تعيين مورد مسمى من قائمة جميع الموارد القابلة للحجز</span><span class="sxs-lookup"><span data-stu-id="006e8-134">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="006e8-135">يمكنك استخدام مربع البحث في **محدد المورد** للبحث عن جميع الموارد القابلة للحجز وتعيينها لتنفيذ مهام.</span><span class="sxs-lookup"><span data-stu-id="006e8-135">You can use the search box in the **Resource Selector** to search all bookable resources and assign them to a task.</span></span>

<span data-ttu-id="006e8-136">تُضاف الموارد التي تم تعيينها بهذه الطريقة إلى الفريق دون أية حجوزات.</span><span class="sxs-lookup"><span data-stu-id="006e8-136">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="006e8-137">وهذا يشبه إضافة عضو فريق وتحديد "بلا" كأسلوب توزيع.</span><span class="sxs-lookup"><span data-stu-id="006e8-137">This is similar to adding a team member and selecting None as the allocation method.</span></span> <span data-ttu-id="006e8-138">تظهر الموارد في علامتي التبويب **الفريق** و**التسوية** كموارد ذات تعيينات فقط ونقص في الحجز.</span><span class="sxs-lookup"><span data-stu-id="006e8-138">The resource is displayed in the **Team** and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="006e8-139">يمكنك حجز هذه الموارد إذا أردت استخدام توافرها.</span><span class="sxs-lookup"><span data-stu-id="006e8-139">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="006e8-140">على شبكة **الجدولة** لمهمة ما، حدد أيقونة **المورد** في خلية المورد.</span><span class="sxs-lookup"><span data-stu-id="006e8-140">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="006e8-141">ابدأ في كتابة اسم.</span><span class="sxs-lookup"><span data-stu-id="006e8-141">Start typing a name.</span></span> <span data-ttu-id="006e8-142">يتم عرض نتائج البحث عن الاسم في **محدد المورد** ضمن **الموارد الأخرى**.</span><span class="sxs-lookup"><span data-stu-id="006e8-142">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>

3. <span data-ttu-id="006e8-143">حدد المورد الذي ترغب في تعيينه للمهمة.</span><span class="sxs-lookup"><span data-stu-id="006e8-143">Select the resource that you want to assign to the task.</span></span>

