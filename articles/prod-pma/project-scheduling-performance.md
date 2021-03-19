---
title: أداء جدولة موارد المشروع
description: يقدم هذا الموضوع معلومات حول كيفية تحسين أداء جدولة الموارد لعدد كبير من المشروعات.
author: Yowelle
manager: AnnBe
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: 34c31570778f9b64c23387112cf56fa1139cd0fd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288993"
---
# <a name="project-resource-scheduling-performance"></a><span data-ttu-id="26bbc-103">أداء جدولة موارد المشروع</span><span class="sxs-lookup"><span data-stu-id="26bbc-103">Project resource scheduling performance</span></span>

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


<span data-ttu-id="26bbc-104">قد تحدث مشاكل تتعلق بالأداء ذات صلة بجدولة الموارد عندما يصل عدد المشاريع إلى الآلاف.</span><span class="sxs-lookup"><span data-stu-id="26bbc-104">Performance issues related to resource scheduling can occur when the number of projects reaches into the thousands.</span></span> <span data-ttu-id="26bbc-105">لتحسين أداء جدولة الموارد، تتوفر ميزة تتيح للمستخدمين تقليل الوقت الذي يستغرقه بدء تشغيل نموذج توافر الموارد.</span><span class="sxs-lookup"><span data-stu-id="26bbc-105">To improve resource scheduling performance, a feature is available that allows users to reduce the time that it takes to launch the resource availability form.</span></span> <span data-ttu-id="26bbc-106">يؤدي هذا على وجه التحديد إلى إزالة عملية مزامنة تجميع سعة الموارد واستخدام الجدول **ResProjectResource** لتسريع البحث عن الموارد.</span><span class="sxs-lookup"><span data-stu-id="26bbc-106">Specifically, this removes the resource capacity roll-up synchronization process and uses the **ResProjectResource** table to speed up the resource lookup.</span></span> <span data-ttu-id="26bbc-107">لاحظ أن استخدام الجدول **ResRollup** سيتوقف.</span><span class="sxs-lookup"><span data-stu-id="26bbc-107">Note that the **ResRollup** table will no longer be used.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="26bbc-108">إذا كانت هناك تبعية على عملية مزامنة تجميع سعة الموارد أو الجدول **ResProjectResource**، فلا تستخدم هذه الميزة.</span><span class="sxs-lookup"><span data-stu-id="26bbc-108">If there is a dependency on either the resource capacity roll-up synchronization process or the **ResProjectResource** table, do not use this feature.</span></span>

## <a name="enable-resource-scheduling-performance-enhancement"></a><span data-ttu-id="26bbc-109">تمكين تحسين أداء جدولة الموارد</span><span class="sxs-lookup"><span data-stu-id="26bbc-109">Enable resource scheduling performance enhancement</span></span>
<span data-ttu-id="26bbc-110">لتمكين تحسين أداء جدولة الموارد، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="26bbc-110">To enable resource scheduling performance enhancement, complete the following steps.</span></span>

1. <span data-ttu-id="26bbc-111">انتقل إلى **إدارة الميزات** > **الكل**، وفي قائمة الميزات، حدد موقع **تمكين ميزة تحسين أداء جدولة الموارد**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-111">Go to **Feature management** > **All**, and in the feature list, locate **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="26bbc-112">حدد **تمكين الآن**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-112">Select **Enable now**.</span></span>

> [!NOTE]
> <span data-ttu-id="26bbc-113">إذا لم تتمكن من العثور على الميزة في القائمة، فحدد **التحقق من وجود تحديثات** لتحديث القائمة.</span><span class="sxs-lookup"><span data-stu-id="26bbc-113">If you can't find the feature in the list, select **Check for updates** to refresh the list.</span></span>

3. <span data-ttu-id="26bbc-114">قم بتحديث المستعرض، ثم انتقل إلى **إدارة المشاريع والمحاسبة** > **دوري** > **موارد المشروع** > **مزامنة سعة تقويمات الموارد عبر جميع الشركات**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-114">Refresh your browser, and then go to **Project management and accounting** > **Periodic** > **Project resources** > **Synchronize resource calendars capacity across all companies**.</span></span>
4. <span data-ttu-id="26bbc-115">قم بتعيين الخيار **إزالة سجلات السعة الموجودة** إلى **نعم** لإزالة البيانات السابقة.</span><span class="sxs-lookup"><span data-stu-id="26bbc-115">Set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="26bbc-116">إذا كنت ترغب في إنشاء بيانات تزايدية، فيمكنك تعيين الخيار إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-116">If you want generate incremental data, set it to **No**.</span></span>
5. <span data-ttu-id="26bbc-117">في الحقل **كود الفترة**، حدد الفترة التي ينبغي إنشاء البيانات بها.</span><span class="sxs-lookup"><span data-stu-id="26bbc-117">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="26bbc-118">إذا قمت بتحديد كود فترة، فلن يكون من الضروري تحديد تاريخ البدء والانتهاء.</span><span class="sxs-lookup"><span data-stu-id="26bbc-118">If you select a period code, a start and end date do not need to be defined.</span></span>
6. <span data-ttu-id="26bbc-119">إذا تركت حقل **كود الفترة** فارغًا،، فحدد تواريخ بدء وانتهاء محددة لإنشاء البيانات.</span><span class="sxs-lookup"><span data-stu-id="26bbc-119">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
7. <span data-ttu-id="26bbc-120">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-120">Select **OK**.</span></span>

 > [!NOTE]
 > <span data-ttu-id="26bbc-121">سيؤدي هذا إلى توزيع البيانات العامة في الجدول **ResCalendarCapacity** عبر جميع الشركات في بيئتك، بحيث تحتاج إلى تشغيل الوظيفة الدُفعية في كيان قانوني واحد فقط.</span><span class="sxs-lookup"><span data-stu-id="26bbc-121">This will distribute general data to the **ResCalendarCapacity** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="26bbc-122">البيانات الموجودة في هذه الوظيفة الدُفعية مطلوبة لحساب سعة الموارد من خلال التقويم المرتبط.</span><span class="sxs-lookup"><span data-stu-id="26bbc-122">The data in this batch job is needed to calculate resource capacity through the associated calendar.</span></span>

8. <span data-ttu-id="26bbc-123">انتقل إلى **إدارة المشاريع والمحاسبة** > **دوري** > **موارد المشروع** > **تعبئة موارد المشروع عبر جميع الشركات** ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-123">Go to **Project management and accounting** > **Periodic** > **Project resources** > **Populate project resources across all companies** and then select **OK**.</span></span> <span data-ttu-id="26bbc-124">هذا هو البرنامج النصي لتحديث البيانات للبيانات العامة في الجدولين **ResProjectResource**, **ResCalendarDateTimeRange** و **ResEffectiveDateTimeRange**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-124">This is the data upgrade script for general data in the **ResProjectResource**, **ResCalendarDateTimeRange**, and **ResEffectiveDateTimeRange** tables.</span></span> <span data-ttu-id="26bbc-125">كما يتم تحديث قيم الحقل **PSAPRojSchedRole.RootActivity**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-125">Values for the **PSAPRojSchedRole.RootActivity** field are also updated.</span></span> <span data-ttu-id="26bbc-126">إذا لم يتم تشغيل هذا الأمر، ستتلقى تحذيرًا عندما تحاول تنفيذ عمليات جدولة الموارد.</span><span class="sxs-lookup"><span data-stu-id="26bbc-126">If this is not run, you will receive a warning when you try to execute resource scheduling operations.</span></span>
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a><span data-ttu-id="26bbc-127">إيقاف تشغيل تحسين أداء جدولة الموارد</span><span class="sxs-lookup"><span data-stu-id="26bbc-127">Turn off resource scheduling performance enhancement</span></span>

1. <span data-ttu-id="26bbc-128">انتقل إلى **إدارة الميزات** > **الكل**، وابحث عن **تمكين ميزة تحسين أداء جدولة الموارد**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-128">Go to **Feature management** > **All**  and search for **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="26bbc-129">حدد الميزة ، ثم حدد الزر **تعطيل**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-129">Select the feature, and then select the **Disable** button.</span></span>
3. <span data-ttu-id="26bbc-130">قم بتحديث المستعرض.</span><span class="sxs-lookup"><span data-stu-id="26bbc-130">Refresh your browser.</span></span>
4. <span data-ttu-id="26bbc-131">انتقل إلى **إدارة المشاريع والمحاسبة** > **دوري** > **مزامنة السعة** > **مزامنة عمليات تجميع سعة الموارد‬**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-131">Go to **Project management and accounting** > **Periodic** > **Capacity synchronization** > **Synchronize resource capacity roll-ups**.</span></span>
5. <span data-ttu-id="26bbc-132">في الصفحة **مزامنة تجميع سعة الموارد**، عيّن **إزالة سجلات السعة الموجودة** إلى **نعم** لإزالة البيانات السابقة.</span><span class="sxs-lookup"><span data-stu-id="26bbc-132">On the **Capacity roll-up synchronization** page, set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="26bbc-133">إذا كنت ترغب في إنشاء بيانات تزايدية، فيمكنك تعيين الخيار إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-133">If you want to generate incremental data, set it to **No**.</span></span>
6. <span data-ttu-id="26bbc-134">في الحقل **كود الفترة**، حدد الفترة التي ينبغي إنشاء البيانات بها.</span><span class="sxs-lookup"><span data-stu-id="26bbc-134">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="26bbc-135">إذا قمت بتحديد كود فترة، فلن يكون من الضروري تحديد تاريخ البدء والانتهاء.</span><span class="sxs-lookup"><span data-stu-id="26bbc-135">If you select a period code, a start and end date do not need to be defined.</span></span>
7. <span data-ttu-id="26bbc-136">إذا تركت حقل **كود الفترة** فارغًا،، فحدد تواريخ بدء وانتهاء محددة لإنشاء البيانات.</span><span class="sxs-lookup"><span data-stu-id="26bbc-136">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
8. <span data-ttu-id="26bbc-137">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-137">Select **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="26bbc-138">سيؤدي هذا إلى توزيع البيانات العامة في الجدول **‎ResRollup** عبر جميع الشركات في بيئتك، بحيث تحتاج إلى تشغيل الوظيفة الدُفعية في كيان قانوني واحد فقط.</span><span class="sxs-lookup"><span data-stu-id="26bbc-138">This will distribute general data to the **ResRollup** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="26bbc-139">هذه الوظيفة الدُفعية مطلوبة لجميع طرق عرض **توفر الموارد**.</span><span class="sxs-lookup"><span data-stu-id="26bbc-139">This batch job is needed for all **Resource Availability** views.</span></span> <span data-ttu-id="26bbc-140">إذا لم يتم تشغيل هذه الوظيفة الدُفعية، فسيتم إنشاء بيانات **ResRollup** على الفور، مما قد يستغرق بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="26bbc-140">If this batch job is not run, the **ResRollup** data will be generated on the fly, which can take time.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]