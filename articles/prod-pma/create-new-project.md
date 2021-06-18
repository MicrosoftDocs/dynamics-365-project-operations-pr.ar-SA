---
title: إنشاء مشروع جديد
description: يقدم هذا الموضوع معلومات عن كيفية إنشاء مشروع جديد.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8218747366be8536601cb007318c642ac122536b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006225"
---
# <a name="create-a-new-project"></a><span data-ttu-id="91797-103">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="91797-103">Create a new project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="91797-104">أكمل الخطوات التالية لإنشاء مشروع جديد.</span><span class="sxs-lookup"><span data-stu-id="91797-104">Complete the following steps to create a new project.</span></span>

1. <span data-ttu-id="91797-105">في صفحة **إدارة المشاريع**، حدد **مشروع جديد**، وأدخل القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="91797-105">On the **Project management** page, select **New project**, and enter the following values:</span></span>

    - <span data-ttu-id="91797-106">**نوع المشروع:** الوقت والمادة</span><span class="sxs-lookup"><span data-stu-id="91797-106">**Project type:** Time and material</span></span>
    - <span data-ttu-id="91797-107">**اسم المشروع:** مرحلة ترقية XYZ رقم 2</span><span class="sxs-lookup"><span data-stu-id="91797-107">**Project name:** XYZ Upgrade Phase 2</span></span>
    - <span data-ttu-id="91797-108">**مجموعة المشاريع:** TM\_WIP</span><span class="sxs-lookup"><span data-stu-id="91797-108">**Project group:** TM\_WIP</span></span>
    - <span data-ttu-id="91797-109">**معرف عقد المشروع:** 00000002</span><span class="sxs-lookup"><span data-stu-id="91797-109">**Project contract ID:** 00000002</span></span>

2. <span data-ttu-id="91797-110">حدد **إنشاء مشروع**</span><span class="sxs-lookup"><span data-stu-id="91797-110">Select **Create project**.</span></span>

## <a name="assign-a-resource-to-a-project"></a><span data-ttu-id="91797-111">تعيين مورد لمشروع</span><span class="sxs-lookup"><span data-stu-id="91797-111">Assign a resource to a project</span></span>

1. <span data-ttu-id="91797-112">في صفحة **العمال**، في قائمة **العمال**، حدد سجل العامل الذي قمت مسبقًا بإعداد الكفاءات له وافتح سجل العامل.</span><span class="sxs-lookup"><span data-stu-id="91797-112">On the **Workers** page, in the **Workers** list, select the record for the worker that you previously set up competencies for, and open the worker record.</span></span>
2. <span data-ttu-id="91797-113">في جزء الإجراءات، ضمن علامة التبويب **المشروع** في مجموعة **الإعداد**، حدد **تعيين المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="91797-113">On the Action Pane, on the **Project** tab, in the **Setup** group, select **Assign projects**.</span></span>
3. <span data-ttu-id="91797-114">في صفحة **تعيينات المشاريع للتحقق من صحة الموارد**، ضمن علامة التبويب **المشاريع**، في حقل **إضافة المشروع إلى المشاريع المحددة**، قم بالتصفية في مشروع **مرحلة ترقية XYZ رقم 2**.</span><span class="sxs-lookup"><span data-stu-id="91797-114">On the **Resource validation project assignments** page, on the **Projects** tab, in the **Add the project to selected projects** field, filter on the **XYZ Upgrade Phase 2** project.</span></span>
4. <span data-ttu-id="91797-115">من جزء **المشاريع المتبقية**، حدد مشروعا ، ثم حدد زر السهم لأضافته إلى جزء **المشاريع المحدد**.</span><span class="sxs-lookup"><span data-stu-id="91797-115">In the **Remaining projects** pane, select a project, and then select the arrow button to add it to the **Selected projects** pane.</span></span>

<span data-ttu-id="91797-116">يمكنك أيضا تعيين فئات لمورد كما تطلب الأمر.</span><span class="sxs-lookup"><span data-stu-id="91797-116">You can also assign categories for a resource as you require.</span></span> <span data-ttu-id="91797-117">يكون نوع الفئة إما **تكلفة** أو **إيراد**.</span><span class="sxs-lookup"><span data-stu-id="91797-117">The category type is either **Cost** or **Revenue**.</span></span> <span data-ttu-id="91797-118">يتم تحديد نوع الفئة بواسطة مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="91797-118">The category type is determined by your organization.</span></span> <span data-ttu-id="91797-119">إذا لم يتم تعيين إيه فئات لأحد الموارد ، ستبحث المالية عن الفئة الافتراضية في الأسعار المقدرة للتكلفة والإيرادات.</span><span class="sxs-lookup"><span data-stu-id="91797-119">If no categories are assigned for a resource, Finance looks up the default category on hour prices for cost and revenue.</span></span>

## <a name="set-up-project-resource-and-role-characteristics"></a><span data-ttu-id="91797-120">اعداد مورد المشروع وخصائص الدور</span><span class="sxs-lookup"><span data-stu-id="91797-120">Set up project resource and role characteristics</span></span>

<span data-ttu-id="91797-121">يمكن لمدير المشروع استخدام وظيفة موارد المشروع لإنشاء الأدوار المطلوبة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="91797-121">A project manager can use the project resourcing functionality to create the roles that are required for the project.</span></span> <span data-ttu-id="91797-122">يمكن استخدام الأدوار في حاله ما إذا كانت الموارد المؤكدة لا تزال غير معروفه عند حجز الموارد.</span><span class="sxs-lookup"><span data-stu-id="91797-122">Roles can be used if confirmed resources are still unknown when resources are being reserved.</span></span> <span data-ttu-id="91797-123">يمكن حجز الأدوار بشكل مؤقت كموارد مخططه ، ومن ثم يمكنك متابعه مراحل تخطيط المشروع.</span><span class="sxs-lookup"><span data-stu-id="91797-123">Roles can be temporarily reserved as planned resources, so that you can continue the project planning stages.</span></span>

<span data-ttu-id="91797-124">[![مثال لدور](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span><span class="sxs-lookup"><span data-stu-id="91797-124">[![Example of a role](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span></span> 

<span data-ttu-id="91797-125">**السيناريو:** Contoso تم تعيينها لإكمال مشروع وقت ومادة يحتوي على ميثاق مشروع تمت الموافقة عليه.</span><span class="sxs-lookup"><span data-stu-id="91797-125">**Scenario:** Contoso was hired to complete a Time and material project that has an approved project charter.</span></span> <span data-ttu-id="91797-126">لا يزال مدير المشروع المبتدئ في إكمال نطاق المشروع.</span><span class="sxs-lookup"><span data-stu-id="91797-126">The junior project manager is still completing the scope of the project.</span></span> <span data-ttu-id="91797-127">تقوم أداره الموارد حاليا بتعريف الموارد المحددة التي سيتم حجزها للعمل علي المشروع الجديد.</span><span class="sxs-lookup"><span data-stu-id="91797-127">The resource manager is currently identifying specific resources that will be reserved to work on the new project.</span></span> <span data-ttu-id="91797-128">وبسبب الطبيعة الهامه للمشروع ، طلب المشروع الراعي مدير المشروع الأول كاحد الأدوار.</span><span class="sxs-lookup"><span data-stu-id="91797-128">Because of the critical nature of the project, the project sponsor requested Senior project manager as one of the roles.</span></span> <span data-ttu-id="91797-129">يجب ان يحصل مدير الموارد علي المورد الجديد وتعريف الدور في النظام في حال طلب مدير المشروع المبتدئ معلومات المورد اثناء تخطيط المشروع.</span><span class="sxs-lookup"><span data-stu-id="91797-129">The resource manager must acquire the new resource and define the role in the system in case the junior project manager requires the resource information during project planning.</span></span>

<span data-ttu-id="91797-130">توضح الخطوات التالية كيف يمكن لمدير الموارد اعداد دور مدير المشروع الأول وربط خصائص الموارد معه.</span><span class="sxs-lookup"><span data-stu-id="91797-130">The following steps show how the resource manager can set up the Senior project manager role and associate resource characteristics with it.</span></span> <span data-ttu-id="91797-131">وبعد ذلك ، يمكن استخدام الدور للبحث عن الموارد المتوفرة التي تطابق اختصاصات الموارد المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="91797-131">Later, the role can be used to search for available resources that match the required resource competencies.</span></span>

1. <span data-ttu-id="91797-132">في صفحة **إعداد الأدوار**، حدد **جديد**، وأدخل القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="91797-132">On the **Setup roles** page, select **New**, and enter the following values:</span></span>

    - <span data-ttu-id="91797-133">**معرف الدور:** مدير المشروع الأول</span><span class="sxs-lookup"><span data-stu-id="91797-133">**Role ID:** Senior Project Manager</span></span>
    - <span data-ttu-id="91797-134">**الوصف:** مدير المشروع الأول</span><span class="sxs-lookup"><span data-stu-id="91797-134">**Description:** Senior Project Manager</span></span>

2. <span data-ttu-id="91797-135">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="91797-135">Select **Create**.</span></span>
3. <span data-ttu-id="91797-136">حدد دور **مدير المشروع الأول**، ثم حدد **تكوين الخصائص**.</span><span class="sxs-lookup"><span data-stu-id="91797-136">Select the **Senior Project Manager** role, and then select **Configure characteristics**.</span></span>
4. <span data-ttu-id="91797-137">في حقل **نوع الخصائص**، حدد **المهارة**.</span><span class="sxs-lookup"><span data-stu-id="91797-137">In the **Characteristics type** field, select **Skill**.</span></span>
5. <span data-ttu-id="91797-138">في حقل **الخصائص المتوفرة**، أدخل المهارة المراد البحث عنها.</span><span class="sxs-lookup"><span data-stu-id="91797-138">In the **Available characteristics** field, enter the skill to search for.</span></span>
6. <span data-ttu-id="91797-139">في حقل **نوع الخصائص**، حدد **الشهادة**.</span><span class="sxs-lookup"><span data-stu-id="91797-139">In the **Characteristic type** field, select **Certificate**.</span></span>
7. <span data-ttu-id="91797-140">في حقل **الخصائص المتوفرة**، أدخل نوع الشهادة المراد البحث عنها.</span><span class="sxs-lookup"><span data-stu-id="91797-140">In the **Available characteristics** field, enter the certificate type to search for.</span></span>

## <a name="assign-a-project-resource-to-a-project"></a><span data-ttu-id="91797-141">تعيين مورد مشروع لمشروع</span><span class="sxs-lookup"><span data-stu-id="91797-141">Assign a project resource to a project</span></span>

1. <span data-ttu-id="91797-142">في صفحة **جميع المشاريع**، حدد مشروع **مرحله الترقية XYZ رقم 2**.</span><span class="sxs-lookup"><span data-stu-id="91797-142">On the **All projects** page, select the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="91797-143">في علامة التبويب **فريق المشروع والجدولة**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="91797-143">On the **Project team and scheduling** tab, select **Add**.</span></span>
3. <span data-ttu-id="91797-144">في حقل **الدور**، حدد **عضو الفريق**.</span><span class="sxs-lookup"><span data-stu-id="91797-144">In the **Role** field, select **Team member**.</span></span>
4. <span data-ttu-id="91797-145">حدد **حجز من تقويم**.</span><span class="sxs-lookup"><span data-stu-id="91797-145">Select **Book from calendar**.</span></span>
5. <span data-ttu-id="91797-146">في صفحة **توافر الموارد**، قم بتحديد **إعدادات العرض**.</span><span class="sxs-lookup"><span data-stu-id="91797-146">On the **Resource availability** page, select **View settings**.</span></span>
6. <span data-ttu-id="91797-147">في صفحة **ضبط إعدادات العرض**، أدخل القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="91797-147">On the **Adjust view settings** page, enter the following values:</span></span>

    - <span data-ttu-id="91797-148">**تنسيق طريقة عرض نطاق التاريخ:** اليوم</span><span class="sxs-lookup"><span data-stu-id="91797-148">**Format for date range view:** Day</span></span>
    - <span data-ttu-id="91797-149">**عرض أوصاف التوافر:** نعم</span><span class="sxs-lookup"><span data-stu-id="91797-149">**Display availability descriptions:** Yes</span></span>
    - <span data-ttu-id="91797-150">**عرض القدرة الإنتاجية المتبقية:** نعم</span><span class="sxs-lookup"><span data-stu-id="91797-150">**Display remaining capacity:** Yes</span></span>

7. <span data-ttu-id="91797-151">في قائمة الموارد، حدد موردًا.</span><span class="sxs-lookup"><span data-stu-id="91797-151">In the list of resources, select a resource.</span></span>
8. <span data-ttu-id="91797-152">حدد **حجز محدد** و **القدرة الإنتاجية الكاملة**.</span><span class="sxs-lookup"><span data-stu-id="91797-152">Select **Hard book** and **Full capacity**.</span></span>

## <a name="assign-a-resource-to-a-default-role"></a><span data-ttu-id="91797-153">تعيين مورد لدور افتراضي</span><span class="sxs-lookup"><span data-stu-id="91797-153">Assign a resource to a default role</span></span>

<span data-ttu-id="91797-154">يمكن لمساعده مشروع أو مديري الموارد التنقل لأسفل في الموارد التي يمكن حجزها لأحد المشروعات.</span><span class="sxs-lookup"><span data-stu-id="91797-154">To help project or resource managers can drill down further on the resources that can be reserved for a project.</span></span> <span data-ttu-id="91797-155">يمكنك اقران دور افتراضي بمورد موجود أو مورد تم الحصول عليه حديثا.</span><span class="sxs-lookup"><span data-stu-id="91797-155">You can associate a default role with an existing resource or a newly acquired resource.</span></span> <span data-ttu-id="91797-156">علي سبيل المثال ، عندما تم توظيف يريد عصمت-، فانه لديه الخبرة والمهارات لملء دور محلل الاعمال.</span><span class="sxs-lookup"><span data-stu-id="91797-156">For example, when Daniel was hired, he had the experience and skills to fill the Business analyst role.</span></span> <span data-ttu-id="91797-157">مدير الموارد المعين لهذا الدور كدور افتراضي ليريد عصمت-.</span><span class="sxs-lookup"><span data-stu-id="91797-157">The resource manager assigned this role as Daniel's default role.</span></span> <span data-ttu-id="91797-158">لذا ، يقوم مدير الموارد باضافه يريد عصمت-إلى تجمع من محللي الاعمال المتوفرين للعمل في المشاريع.</span><span class="sxs-lookup"><span data-stu-id="91797-158">Therefore, the resource manager added Daniel to a pool of business analysts who are available to work on projects.</span></span>

<span data-ttu-id="91797-159">واثناء حجز الموارد ، يمكن لمديري المشاريع تصفيه موارد الأدوار المتوفرة للعمل مع المشروعات.</span><span class="sxs-lookup"><span data-stu-id="91797-159">During resource reservation, project managers can filter the role resources that are available to work on projects.</span></span> <span data-ttu-id="91797-160">ويمكنهم استخدام هذه المعلومات كمعيار واحد عند تنفيذ تحليل القرارات متعددة المعايير اثناء استيفاء المورد.</span><span class="sxs-lookup"><span data-stu-id="91797-160">They can use this information as one criterion when they perform multi-criteria decision analysis during resource fulfillment.</span></span> <span data-ttu-id="91797-161">كما يمكنهم أيضا أضافه خصائص موارد أخرى إلى عامل التصفية للبحث عن الموارد التي لها مهارات وتعليم وخبره معينه لمشروع محدد.</span><span class="sxs-lookup"><span data-stu-id="91797-161">They can also add other resource characteristics to the filter to search for resources that have specific skills, education, and experience for a given project.</span></span>

<span data-ttu-id="91797-162">**السيناريو:** بدأ مشروع تمت الموافقة عليه ، وتم حجز دور مدير المشروع الأول كمورد مخطط اثناء مرحله تخطيط المشروع.</span><span class="sxs-lookup"><span data-stu-id="91797-162">**Scenario:** An approved project has started, and the Senior project manager role was reserved as a planned resource during the project planning stage.</span></span> <span data-ttu-id="91797-163">وقامت مدير الموارد الآن بالحصول علي مورد لتلبيه دور مدير المشروع الأول.</span><span class="sxs-lookup"><span data-stu-id="91797-163">The resource manager has now acquired a resource to fulfill the Senior project manager role.</span></span>

1. <span data-ttu-id="91797-164">في صفحة **قائمة الموارد**، حدد **Daniel Goldschmidt**.</span><span class="sxs-lookup"><span data-stu-id="91797-164">On the **Resources list** page, select **Daniel Goldschmidt**.</span></span>
2. <span data-ttu-id="91797-165">في صفحة **دور المورد**، حدد **جديد**، وأدخل القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="91797-165">On the **Resource role** page, select **New**, and enter the following values:</span></span>

    - <span data-ttu-id="91797-166">**سارٍ:** أدخل التاريخ الحالي.</span><span class="sxs-lookup"><span data-stu-id="91797-166">**Effective:** Enter the current date.</span></span>
    - <span data-ttu-id="91797-167">**انتهاء الصلاحية:** أدخل **أبدًا**.</span><span class="sxs-lookup"><span data-stu-id="91797-167">**Expiration:** Enter **Never**.</span></span>
    - <span data-ttu-id="91797-168">**الدور:** أدخل **مدير المشروع الأول**.</span><span class="sxs-lookup"><span data-stu-id="91797-168">**Role:** Enter **Senior Project Manager**.</span></span>

3. <span data-ttu-id="91797-169">حدد **حفظ**، ثم أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="91797-169">Select **Save**, and then close the page.</span></span>
4. <span data-ttu-id="91797-170">في علامة التبويب **الكفاءات**، أضف مهارة **ProjectMgmt** وشهادة **PMP**.</span><span class="sxs-lookup"><span data-stu-id="91797-170">On the **Competencies** tab, add the **ProjectMgmt** skill and the **PMP** certificate.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]