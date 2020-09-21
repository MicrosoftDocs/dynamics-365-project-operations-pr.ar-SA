---
title: تكامل Microsoft Project Client
description: يمكن أن يكون تخطيط جدول المشروع والحفاظ عليه أمرًا معقدًا ، لذلك يحتاج مديرو المشاريع إلى استخدام الأدوات التي تساعدهم في إدارة هذه المهمة. يوفر التكامل مع Microsoft Project Client الدعم لفتح وإدارة هيكل تقسيم عمل المشروع.
author: KimANelson
manager: AnnBe
ms.date: 12/11/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: c6478e05-50ee-4993-87f4-6ce9cb78f076
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: e35e1e54bad659d1329c333479830b680a17cbb0
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748715"
---
# <a name="microsoft-project-client-integration"></a><span data-ttu-id="521a8-104">تكامل Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="521a8-104">Microsoft Project client integration</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="521a8-105">يمكن أن يكون تخطيط جدول المشروع والحفاظ عليه أمرًا معقدًا ، لذلك يحتاج مديرو المشاريع إلى استخدام الأدوات التي تساعدهم في إدارة هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="521a8-105">Planning and maintaining a project schedule can be complex, so project managers need to use tools that help them manage this task.</span></span> <span data-ttu-id="521a8-106">يوفر التكامل مع Microsoft Project Client الدعم لفتح وإدارة هيكل تقسيم عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="521a8-106">Integration with Microsoft Project Client provides support to open and manage a project work breakdown structure.</span></span> <span data-ttu-id="521a8-107">يمكن لمدير المشروع نشر أي تغييرات مرة أخرى إلى هيكل تنظيم عمل مشروع Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="521a8-107">The project manager can publish any changes back to the Dynamics 365 Finance project work breakdown structure.</span></span>

> [!NOTE]
> <span data-ttu-id="521a8-108">إذا كنت تستخدم تحديث يوليو (الإصدار 10.0.4)، فيجب عليك تثبيت قاعدة المعارف 4054797 و4055884.</span><span class="sxs-lookup"><span data-stu-id="521a8-108">If you are using the July update (version 10.0.4), you must install KB 4054797 and 4055884.</span></span>

## <a name="configure-the-microsoft-project-client-add-in"></a><span data-ttu-id="521a8-109">تكوين الوظيفة الإضافية لـ Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="521a8-109">Configure the Microsoft Project Client add-in</span></span>
<span data-ttu-id="521a8-110">لتمكين التكامل مع Microsoft Project Client، يلزم تثبيت الوظيفة الإضافية لـ Microsoft Dynamics 365 في تطبيق Microsoft Project الخاص بعميل المستخدم.</span><span class="sxs-lookup"><span data-stu-id="521a8-110">To enable the integration with Microsoft Project Client, a Microsoft Dynamics 365 add-in is required to be installed in the user’s client Microsoft Project application.</span></span> <span data-ttu-id="521a8-111">ويتم ذلك من خلال فتح **مساحة عمل إدارة المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="521a8-111">This is done by opening the **Project management workspace**.</span></span>

<span data-ttu-id="521a8-112">•   انقر فوق **تكوين الوظيفة الإضافية لعميل المشروع** من قسم **الارتباطات** > **الإعداد** في مساحة العمل.</span><span class="sxs-lookup"><span data-stu-id="521a8-112">•   Click **Configure project client add-in** from the **Links** > **Setup** section of the workspace.</span></span>

<span data-ttu-id="521a8-113">•   انقر **فتح**، ثم انقر فوق **تشغيل** عند المطالبة.</span><span class="sxs-lookup"><span data-stu-id="521a8-113">•   Click **Open**, then click **Run** when prompted.</span></span>

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a><span data-ttu-id="521a8-114">فتح وتحرير مسودة هيكل تنظيم العمل الحالي في Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="521a8-114">Open and edit an existing draft work breakdown structure in Microsoft Project Client</span></span>
<span data-ttu-id="521a8-115">إذا كان مشروع في Dynamics 365 Finance يشتمل على هيكل تنظيم عمل تم إنشاؤه بالفعل، يمكن فتح هيكل تنظيم العمل في تطبيق Microsoft Project Client إذا كان هيكل تنظيم العمل في حالة مسودة.</span><span class="sxs-lookup"><span data-stu-id="521a8-115">If a project in Dynamics 365 Finance already has a work breakdown structure created, the work breakdown structure can be opened in the Microsoft Project Client application if the work breakdown structure is in a draft status.</span></span> <span data-ttu-id="521a8-116">للفتح من صفحة **المشروع**، انقر فوق **فتح في Microsoft Project** علامة التبويب **خطة**. يمكن أيضًا فتح هذه الصفحة من تطبيق Microsoft Project Client عن طريق النقر فوق **فتح** في علامة التبويب **Microsoft Dynamics 365**. حدد **الكيان القانوني** و**المشروع** من القائمة.</span><span class="sxs-lookup"><span data-stu-id="521a8-116">To open from the **Project** page, click **Open in Microsoft Project** link from the **Plan** tab. This page can also be opened from within the Microsoft Project Client application by clicking **Open** in the **Microsoft Dynamics 365** tab. Select the **Legal entity** and **Project** from the list.</span></span>

> [!NOTE]
> <span data-ttu-id="521a8-117">إذا كنت تستخدم Internet Explorer كمستعرض، فستحتاج إلى النقر فوق **حفظ** للفتح يدويًا من الموقع الذي يتم تنزيل الملف إليه.</span><span class="sxs-lookup"><span data-stu-id="521a8-117">If you're using Internet Explorer as your browser, you will need to click **Save** to manually open from the location that the file is downloaded to.</span></span> <span data-ttu-id="521a8-118">أو انقر فوق **حفظ وفتح** لفتح الملف في Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="521a8-118">Or, click **Save and open** to open the file in Microsoft Project Client.</span></span> <span data-ttu-id="521a8-119">لا تقم بإعادة تسميه اسم الملف عند الحفظ.</span><span class="sxs-lookup"><span data-stu-id="521a8-119">Do not rename the file name when saving.</span></span>

<span data-ttu-id="521a8-120">قبل إجراء أي تعديلات على الملف باستخدام Microsoft Project Client، تحتاج إلى سحبه. انقر فوق **سحب** في علامة التبويب **Microsoft Dynamics 365**. سيمنع هذا المستخدمين الآخرين من تحرير هيكل تنظيم العمل من داخل Finance في نفس الوقت.</span><span class="sxs-lookup"><span data-stu-id="521a8-120">Before making any edits to the file using Microsoft Project Client, you need to check it out. Click **Check out** in the **Microsoft Dynamics 365** tab. This will prevent other users from editing the work breakdown structure from within Finance at the same time.</span></span> <span data-ttu-id="521a8-121">لنشر هيكل تنظيم العمل بعد إكمال أي تعديلات، انقر فوق **إيداع** في علامة التبويب **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="521a8-121">To publish the work breakdown structure after completing any edits, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

<span data-ttu-id="521a8-122">إذا تمت إضافة فريق مشروع بالفعل إلى المشروع في Finance ، فسيتم ملء قائمة الموارد بأعضاء الفريق.</span><span class="sxs-lookup"><span data-stu-id="521a8-122">If a project team has already been added to the project in Finance, the resource list will be populated with the team members.</span></span> <span data-ttu-id="521a8-123">إذا لم تتم إضافة فريق المشروع إلى المشروع بعد، يمكنك تحديد الموارد وبناء الفريق داخل Microsoft Project Client عن طريق النقر فوق الزر **موارد** في علامة التبويب **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="521a8-123">If a project team has not yet been added to the project, you can select resources and build the team within Microsoft Project Client by clicking the **Resources** button on the **Microsoft Dynamics 365** tab.</span></span> 

<span data-ttu-id="521a8-124">ستتم مزامنة البيانات التالية مره أخرى إلى Finance كجزء من عمليه الإيداع:</span><span class="sxs-lookup"><span data-stu-id="521a8-124">The following data will be synced back to Finance as part of the check-in process:</span></span>

<span data-ttu-id="521a8-125">•   اسم المهمة</span><span class="sxs-lookup"><span data-stu-id="521a8-125">•   Task name</span></span>

<span data-ttu-id="521a8-126">•   تاريخ البدء</span><span class="sxs-lookup"><span data-stu-id="521a8-126">•   Start date</span></span>

<span data-ttu-id="521a8-127">•   تاريخ الانتهاء</span><span class="sxs-lookup"><span data-stu-id="521a8-127">•   Finish date</span></span>

<span data-ttu-id="521a8-128">•   الأنشطة السابقة</span><span class="sxs-lookup"><span data-stu-id="521a8-128">•   Predecessors</span></span>

<span data-ttu-id="521a8-129">•   أسماء الموارد</span><span class="sxs-lookup"><span data-stu-id="521a8-129">•   Resource names</span></span>

<span data-ttu-id="521a8-130">•   الفئة</span><span class="sxs-lookup"><span data-stu-id="521a8-130">•   Category</span></span>

<span data-ttu-id="521a8-131">•   فئة المورد</span><span class="sxs-lookup"><span data-stu-id="521a8-131">•   Resource category</span></span>

<span data-ttu-id="521a8-132">•   ساعات العمل</span><span class="sxs-lookup"><span data-stu-id="521a8-132">•   Work hours</span></span>

<span data-ttu-id="521a8-133">•   الملاحظات</span><span class="sxs-lookup"><span data-stu-id="521a8-133">•   Notes</span></span>

<span data-ttu-id="521a8-134">•   الأولوية</span><span class="sxs-lookup"><span data-stu-id="521a8-134">•   Priority</span></span>

> [!NOTE]
> <span data-ttu-id="521a8-135">إذا قمت بإضافة أي أعمدة أخرى إلى ملف Microsoft Project Client الخاص بك، فلن يتم حفظها في الملف ولن يتم عرضها عند فتح الملف مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="521a8-135">If you add any other columns to your Microsoft Project Client file, they will not be saved to the file and will not be displayed when the file is opened again.</span></span>

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="521a8-136">إنشاء هيكل تنظيم العمل لمشروع موجود باستخدام Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="521a8-136">Create the work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="521a8-137">لإنشاء هيكل تنظيم عمل جديد باستخدام Microsoft Project Client، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="521a8-137">To create a new work breakdown structure using Microsoft Project Client, follow these steps:</span></span>


1.  <span data-ttu-id="521a8-138">افتح Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="521a8-138">Open Microsoft Project Client.</span></span>

2.  <span data-ttu-id="521a8-139">في علامة التبويب **Microsoft Dynamics 365**، انقر فوق **فتح**.</span><span class="sxs-lookup"><span data-stu-id="521a8-139">On the **Microsoft Dynamics 365** tab, click **Open**.</span></span>

3.  <span data-ttu-id="521a8-140">حدد **الكيان القانوني** للمشروع.</span><span class="sxs-lookup"><span data-stu-id="521a8-140">Select the **Legal entity** for the project.</span></span>

4.  <span data-ttu-id="521a8-141">حدد **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="521a8-141">Select the **Project**.</span></span>

5.  <span data-ttu-id="521a8-142">انقر فوق **سحب** في علامة التبويب **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="521a8-142">Click **Check out** on the **Microsoft Dynamics 365** tab.</span></span>

6.  <span data-ttu-id="521a8-143">عندما تكون جاهزًا للنشر إلى Finance، انقر فوق **إيداع** في علامة التبويب **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="521a8-143">When ready to publish to Finance, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="521a8-144">استبدال هيكل تنظيم العمل لمشروع موجود باستخدام Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="521a8-144">Replace the existing work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="521a8-145">لإنشاء هيكل جديد لتنظيم العمل باستخدام Microsoft Project Client واستبدال هيكل تقسيم العمل الحالي لمشروع موجود، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="521a8-145">To create a new work breakdown structure using Microsoft Project Client and replace an existing work breakdown structure for an existing project, follow these steps:</span></span>

1.  <span data-ttu-id="521a8-146">افتح Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="521a8-146">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="521a8-147">قم بإنشاء الجدول الزمني في Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="521a8-147">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="521a8-148">في علامة التبويب **Microsoft Dynamics 365**، انقر فوق **حفظ التغييرات** > **استبدال المشروع الموجود**.</span><span class="sxs-lookup"><span data-stu-id="521a8-148">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Replace existing project**.</span></span>

4.  <span data-ttu-id="521a8-149">حدد **الكيان القانوني** للمشروع.</span><span class="sxs-lookup"><span data-stu-id="521a8-149">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="521a8-150">حدد **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="521a8-150">Select the **Project**.</span></span>

6.  <span data-ttu-id="521a8-151">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="521a8-151">Click **OK**.</span></span>

## <a name="create-a-new-project-from-within-microsoft-project-client"></a><span data-ttu-id="521a8-152">إنشاء مشروع جديد من داخل Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="521a8-152">Create a new project from within Microsoft Project Client</span></span>


1.  <span data-ttu-id="521a8-153">افتح Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="521a8-153">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="521a8-154">قم بإنشاء الجدول الزمني في Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="521a8-154">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="521a8-155">في علامة التبويب **Microsoft Dynamics 365**، انقر فوق **حفظ التغييرات** > **حفظ إلى مشروع جديد**.</span><span class="sxs-lookup"><span data-stu-id="521a8-155">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Save to new Project**.</span></span>

4.  <span data-ttu-id="521a8-156">حدد **الكيان القانوني** للمشروع.</span><span class="sxs-lookup"><span data-stu-id="521a8-156">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="521a8-157">أدخل **معرف المشروع**، إذا لزم الأمر.</span><span class="sxs-lookup"><span data-stu-id="521a8-157">Enter the **Project ID**, if necessary.</span></span>

6.  <span data-ttu-id="521a8-158">أدخل **اسم المشروع**.</span><span class="sxs-lookup"><span data-stu-id="521a8-158">Enter the **Project name**.</span></span>

7.  <span data-ttu-id="521a8-159">حدد **نوع المشروع**، و**مجموعة المشاريع**، و**معرف عقد المشروع**.</span><span class="sxs-lookup"><span data-stu-id="521a8-159">Select the **Project type**, **Project group** and the **Project contract ID**.</span></span> <span data-ttu-id="521a8-160">بدلاً من ذلك، يمكنك إنشاء عقد مشروع جديد بالنقر فوق **جديد**.</span><span class="sxs-lookup"><span data-stu-id="521a8-160">Alternatively, you can create a new project contract by clicking **New**.</span></span>

8.  <span data-ttu-id="521a8-161">حدد **التقويم** الذي سيتم استخدامه لتعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="521a8-161">Select the **Calendar** to be used for resourcing.</span></span>

11. <span data-ttu-id="521a8-162">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="521a8-162">Click **OK**.</span></span>
