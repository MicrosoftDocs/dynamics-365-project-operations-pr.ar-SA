---
title: إنشاء فريق مشروع
description: يقدم هذا الموضوع معلومات عن كيفية إنشاء فرق المشروع وإدارتها.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kdwns
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8d3d39aa28565692bf894ff8d4fc8f8c3c5542d4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006180"
---
# <a name="create-a-project-team"></a><span data-ttu-id="6b0f4-103">إنشاء فريق مشروع</span><span class="sxs-lookup"><span data-stu-id="6b0f4-103">Create a project team</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="6b0f4-104">لاستخدام الأدوار التي تم اعدادها مسبقا في مشروع ، يجب ان يقوم مدير المشروع باقران الأدوار بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-104">To use the roles that were previously set up in a project, a project manager must associate the roles with the project.</span></span> <span data-ttu-id="6b0f4-105">يمكن تعيين ادوار متعددة لمشروع.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-105">Multiple roles can be assigned for a project.</span></span> <span data-ttu-id="6b0f4-106">لمنع الارتباك، تتم تسميه هذه الأدوار تلقائيا اثناء الحجز.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-106">To prevent confusion, these roles are automatically labeled during reservation.</span></span> <span data-ttu-id="6b0f4-107">علي سبيل المثال، إذا كان مدير المشروع يتطلب ثلاثه مهندسين للبرامج، فانه يتم إنشاء ثلاثه ادوار مهندس برامج لها **مهندس برامج 1**، و **مهندس برامج 2**، و **مهندس برامج 3** عند القيام بالتسميات الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-107">For example, if the project manager requires three software engineers, three Software engineer roles that have **software engineer 1**, **software engineer 2**, and **software engineer 3** as their labels are automatically generated.</span></span> <span data-ttu-id="6b0f4-108">إذا كانت السمات الخاصة بالدور قد تم تعيينها مسبقا للدور ، سيتم تطبيقها كعامل تصفيه اثناء عمليات البحث عن مورد.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-108">If role characteristics were previously set for the role, they are applied as a filter during searches for a resource.</span></span> <span data-ttu-id="6b0f4-109">يمكن أضافه سمات اضافيه وفقا لما هو مطلوب لإجراء مزيد من التنقيح علي البحث.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-109">Additional characteristics can be added as required to further refine the search.</span></span>

<span data-ttu-id="6b0f4-110">يمكن أيضا تخصيص إعدادات طريقه العرض لمنح طريقه عرض أفضل لأتاحه الموارد.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-110">View settings can also be customized to give a better view of resource availability.</span></span> <span data-ttu-id="6b0f4-111">هناك خيارات لعرض التوفر بالساعة واليوم والأسبوعي والشهري وربع السنه والمتوفر السنوي.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-111">There are options to show hourly, daily, weekly, monthly, quarterly, and annual availability.</span></span> <span data-ttu-id="6b0f4-112">كما يوجد خيار لإظهار السعه المتوفرة والمتبقية في الموارد.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-112">There is also an option to show available and remaining capacity on resources.</span></span> <span data-ttu-id="6b0f4-113">هذا الخيار مفيد لأداره الوقت ، عندما تقوم بتقدير الوقت المتاح للانشطه أو أتاحه المورد.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-113">This option is useful for time management, when you're estimating available time for activities or resource availability.</span></span>

<span data-ttu-id="6b0f4-114">يمكن لمدير المشروع تحديد دور في الصفحة ثم إذا كان هناك مورد متوفر يناسب المطلب ، فحدد لحجز مورد لملء الدور.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-114">The project manager can select a role on the page and then, if there is an available resource that fits the requirement, select to reserve a resource to fill the role.</span></span> <span data-ttu-id="6b0f4-115">لاحظ انه ليس من الضروري ان يتم حجز الموارد عند هذه النقطة في مرحله التخطيط.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-115">Note that the resources don't have to be reserved at this point in the planning stage.</span></span> <span data-ttu-id="6b0f4-116">عند إنشاء WBS ، يمكنك استبدال ادوار بموارد ستافيد للمشروع.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-116">When you create a WBS, you can replace roles with staffed resources for the project.</span></span> <span data-ttu-id="6b0f4-117">إذا تم استبدال الأدوار بالموارد الستافيده في WBS ، سيقوم اعداد المورد تلقائيا بتحديث سرد وجدوله فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-117">If roles are replaced with staffed resources in the WBS, the resource setup automatically updates the project team listing and scheduling.</span></span>

<span data-ttu-id="6b0f4-118">[![سرد فريق المشروع الذي يتضمن كلا من الأدوار والموارد الفعلية](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span><span class="sxs-lookup"><span data-stu-id="6b0f4-118">[![Project team listing that includes both roles and actual resources](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span></span> 

<span data-ttu-id="6b0f4-119">يتمتع مدير المشروع بالعديد من الخيارات لحجز مورد لمشروع، مثل **القدرة الإنتاجية المتبقية**، و **القدرة الإنتاجية الكاملة**، و **النسبة المئوية للقدرة الإنتاجية**، و **تحديد الساعات**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-119">The project manager has various options for booking a resource for a project, such as **Remaining capacity**, **Full capacity**, **Capacity percentage**, and **Specify hours**.</span></span> <span data-ttu-id="6b0f4-120">يمكن إلغاء خيارات الحجز هذه في اي وقت عند تغيير تعيينات الموارد.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-120">These booking options can be canceled at any time if resource assignments change.</span></span> <span data-ttu-id="6b0f4-121">هناك نوعان من أنواع الحجز مدعومين:</span><span class="sxs-lookup"><span data-stu-id="6b0f4-121">Two types of booking are supported:</span></span>

- <span data-ttu-id="6b0f4-122">**حجز محدد** – تمت الموافقة على حجز المورد وتأكيده للعمل على المشاركة للمدة المحددة.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-122">**Hard Book** – The resource reservation was approved and confirmed to work on the engagement for the specified duration.</span></span>
- <span data-ttu-id="6b0f4-123">**الحجز المبدئي** – تم تعيين حجوزات المورد مبدئيًا للعمل على المشاركة للمدة المحددة.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-123">**Soft book** – The resource reservations was tentatively set to work on the engagement for the specified duration.</span></span>

<span data-ttu-id="6b0f4-124">يوضح الإجراء التالي كيفية إنشاء فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-124">The following procedure explains how to create a project team.</span></span>

## <a name="create-a-project-team"></a><span data-ttu-id="6b0f4-125">إنشاء فريق مشروع</span><span class="sxs-lookup"><span data-stu-id="6b0f4-125">Create a project team</span></span>

1. <span data-ttu-id="6b0f4-126">في صفحة قائمة **جميع المشاريع**، حدد مشروعا، ثم حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-126">On the **All projects** list page, select a project, and then select **Edit**.</span></span>
2. <span data-ttu-id="6b0f4-127">في علامة التبويب **فريق المشروع والجدولة**، في حقل **تاريخ انتهاء العمل**، أدخل تاريخ بدء الجدولة بالإضافة إلى شهر واحد.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-127">On the **Project team and scheduling** tab, in the **Schedule end date** field, enter the schedule start date plus one month.</span></span> <span data-ttu-id="6b0f4-128">علي سبيل المثال، إذا كان تاريخ بدء الجدولة هو 24 يونيو 2017 (24/06/2017)، فأدخل **24/07/2017**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-128">For example, if the schedule start date is June 24, 2017 (24/06/2017), enter **24/07/2017**.</span></span>
3. <span data-ttu-id="6b0f4-129">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-129">Select **Add**.</span></span>
4. <span data-ttu-id="6b0f4-130">في جزء **إضافة أدوار إلى المشروع**، في حقل **الدور**، حدد **مدير المشروع الأول**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-130">In the **Add roles to the project** pane, in the **Role** field, select **Senior Project Manager**.</span></span>
5. <span data-ttu-id="6b0f4-131">حدد **الكفاءات المطلوبة**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-131">Select **Required competencies**.</span></span>
6. <span data-ttu-id="6b0f4-132">في صفحة **اختيار الخصائص**، يتم تحديد الخصائص التي قمت بتعيينها مسبقا لدور مدير المشروع الأول بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-132">On the **Choose characteristics** page, the characteristics that you previously set for the Senior project manager role are selected by default.</span></span> <span data-ttu-id="6b0f4-133">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-133">Select **OK**.</span></span>
7. <span data-ttu-id="6b0f4-134">في صفحة **إضافة الأدوار إلى المشروع**، في حقل **عدد الموارد**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-134">On the **Add roles to project** page, in the **Number of resources** field, enter **1**.</span></span>
8. <span data-ttu-id="6b0f4-135">في حقل **المورد**، يعرض البحث كافة الموارد التي لها الكفاءات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-135">In the **Resource** field, the lookup shows all resources that have the required competencies.</span></span> <span data-ttu-id="6b0f4-136">حدد **Daniel Goldschmidt**، ثم حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-136">Select **Daniel Goldschmidt**, and then select **Create**.</span></span>
9. <span data-ttu-id="6b0f4-137">في صفحة **المشروع**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-137">On the **Project** page, select **Add**.</span></span>
10. <span data-ttu-id="6b0f4-138">في جزء **إضافة أدوار إلى المشروع**، في حقل **الدور**، حدد **عضو الفريق**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-138">In the **Add roles to the project** pane, in the **Role** field, select **Team member**.</span></span> <span data-ttu-id="6b0f4-139">في حقل **عدد الموارد**، أدخل **5**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-139">In the **Number of resources** field, enter **5**.</span></span>
11. <span data-ttu-id="6b0f4-140">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-140">Select **Create**.</span></span>
12. <span data-ttu-id="6b0f4-141">في صفحة **المشاريع**، حدد **تنفيذ المورد**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-141">On the **Projects** page, select **Fulfill resource**.</span></span>

## <a name="monitor-project-teams"></a><span data-ttu-id="6b0f4-142">مراقبة فرق المشاريع</span><span class="sxs-lookup"><span data-stu-id="6b0f4-142">Monitor project teams</span></span>
1. <span data-ttu-id="6b0f4-143">في صفحة **جميع المشاريع**، حدد ارتباط **معرف المشروع** لمشروع **مرحلة ترقية XYZ رقم 2**.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-143">On the **All projects** page, select the **Project ID** link for the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="6b0f4-144">في علامة التبويب السريع **فريق المشروع والجدولة**، تحقق من صحة موارد المشروع المسردة.</span><span class="sxs-lookup"><span data-stu-id="6b0f4-144">On the **Project team and scheduling** FastTab, verify that the project resources that are listed are correct.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]