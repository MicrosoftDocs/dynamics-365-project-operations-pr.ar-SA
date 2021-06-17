---
title: إعداد موارد المشاريع
description: يوفر هذا الموضوع معلومات حول إعداد أو طلب موارد المشروع.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 49e0ca6254518079d2e01d92ac2e31d119468c4b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997675"
---
# <a name="set-up-project-resources"></a><span data-ttu-id="9e61f-103">إعداد موارد المشاريع</span><span class="sxs-lookup"><span data-stu-id="9e61f-103">Set up project resources</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="9e61f-104">يجب عليك إعداد تقويم وربطه بموظف أو عامل.</span><span class="sxs-lookup"><span data-stu-id="9e61f-104">You must set up a calendar and associate it with an employee or a worker.</span></span> <span data-ttu-id="9e61f-105">يستخدم التقويم لجدوله المشروع ووقت العمل للموارد التي تم حجزها للمشروع.</span><span class="sxs-lookup"><span data-stu-id="9e61f-105">The calendar is used to schedule the project and the working time of the resources that are reserved for the project.</span></span> <span data-ttu-id="9e61f-106">اثناء اعداد التقويم ، يمكن لمديري المشاريع القيام بتسوية الموارد كجزء من تحسين الموارد.</span><span class="sxs-lookup"><span data-stu-id="9e61f-106">During calendar setup, project managers can do resource leveling as part of resource optimization.</span></span> <span data-ttu-id="9e61f-107">وفقا لجدول التقويم ، يمكن وضع القيود علي الموارد.</span><span class="sxs-lookup"><span data-stu-id="9e61f-107">Based on the calendar schedule, restrictions can be put on resources.</span></span> <span data-ttu-id="9e61f-108">يمكنك اعداد تقويم في صفحة **التقويمات**.</span><span class="sxs-lookup"><span data-stu-id="9e61f-108">You can set up a calendar on the **Calendars** page.</span></span>

<span data-ttu-id="9e61f-109">عندما تقوم باعداد عامل كمورد مشروع ، يمكنك تحديد من العاملين الذين يعملون في الشركة التي تقوم باعداد الموارد لها.</span><span class="sxs-lookup"><span data-stu-id="9e61f-109">When you set up a worker as a project resource, you can select from workers who work in the company that you're setting up resources for.</span></span> <span data-ttu-id="9e61f-110">وبدلا من ذلك ، يمكنك تحديد العاملين من الشركات الأخرى في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="9e61f-110">Alternatively, you can select workers from other companies in your organization.</span></span> <span data-ttu-id="9e61f-111">يُعرف هؤلاء العمال بموارد الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="9e61f-111">These workers are known as intercompany resources.</span></span>

<span data-ttu-id="9e61f-112">توضح الإجراءات التالية كيفيه اعداد عامل كمورد مشروع في الشركة الخاصة بك وكيفيه اعداد مورد مشروع بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="9e61f-112">The following procedures explain how to set up a worker as a project resource in your company and how to set up an intercompany project resource.</span></span>

## <a name="set-up-a-worker-as-a-project-resource"></a><span data-ttu-id="9e61f-113">تعيين عامل كمورد مشروع</span><span class="sxs-lookup"><span data-stu-id="9e61f-113">Set up a worker as a project resource</span></span>

1. <span data-ttu-id="9e61f-114">في صفحة **العمال**، في قائمة **العمال** ، حدد العامل الذي تقوم بإضافته كمورد مشروع ، وافتح سجل العامل.</span><span class="sxs-lookup"><span data-stu-id="9e61f-114">On the **Workers** page, in the **Workers** list, select the worker that you're adding as a project resource, and open the worker record.</span></span>
2. <span data-ttu-id="9e61f-115">في جزء الإجراء، حدد **المشروع** &gt; **إعداد** &gt; **إعداد المشروع**.</span><span class="sxs-lookup"><span data-stu-id="9e61f-115">On the Action Pane, select **Project** &gt; **Setup** &gt; **Project setup**.</span></span>
3. <span data-ttu-id="9e61f-116">حدد تقويما، ثم أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="9e61f-116">Select a calendar, and then close the page.</span></span>

<span data-ttu-id="9e61f-117">يمكنك أيضًا تحديد مشاريع افتراضية لمورد كنوع من التعيين المسبق.</span><span class="sxs-lookup"><span data-stu-id="9e61f-117">You can also specify default projects for a resource as a type of pre-assignment.</span></span> <span data-ttu-id="9e61f-118">يمكن استخدام التعيينات المسبقة عندما يعرف مدير المورد أو مدير المشروع المشاريع التي سيعمل المورد عليها مقدما.</span><span class="sxs-lookup"><span data-stu-id="9e61f-118">Pre-assignments can be used when the resource manager or project manager knows which projects the resource will be working on in advance.</span></span> <span data-ttu-id="9e61f-119">يمكن أيضا ان تستند التعيينات المسبقة إلى طلب المستخدم أو عميل المشروع.</span><span class="sxs-lookup"><span data-stu-id="9e61f-119">Pre-assignments can also be based on the request of a project sponsor or customer.</span></span> <span data-ttu-id="9e61f-120">لتعيين مشروع مسبقًا، في صفحة **تعيين المشاريع**، في علامة التبويب **المشاريع**، في قائمة **المشاريع المتبقية**، حدد المشروع المناسب.</span><span class="sxs-lookup"><span data-stu-id="9e61f-120">To pre-assign a project, on the **Assign projects** page, on the **Projects** tab, in the **Remaining projects** list, select the appropriate project.</span></span>

## <a name="set-up-an-intercompany-resource"></a><span data-ttu-id="9e61f-121">إعداد مورد بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="9e61f-121">Set up an intercompany resource</span></span>

<span data-ttu-id="9e61f-122">عندما تقوم بإعداد عامل كمورد بين الشركات الشقيقة ، يجب عليك إكمال الإعداد في كل من الشركة المُقرضة والشركة المقترضة.</span><span class="sxs-lookup"><span data-stu-id="9e61f-122">When you set up a worker as an intercompany resource, you must complete the setup in both the lending company and the borrowing company.</span></span>

### <a name="in-the-lending-company"></a><span data-ttu-id="9e61f-123">في الشركة المقرضة</span><span class="sxs-lookup"><span data-stu-id="9e61f-123">In the lending company</span></span>

1. <span data-ttu-id="9e61f-124">في Finance ، تحقق من تحديد الشركة المُقرضة ، ثم أكمل الإجراء الوارد في القسم السابق ، "إعداد عامل كمورد مشروع".</span><span class="sxs-lookup"><span data-stu-id="9e61f-124">In Finance, verify that the lending company is selected, and then complete the procedure in the previous section, "Set up a worker as a project resource."</span></span>
2. <span data-ttu-id="9e61f-125">في صفحة **المحاسبة بين الشركات الشقيقة**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9e61f-125">On the **Intercompany accounting** page, select **New**.</span></span>
3. <span data-ttu-id="9e61f-126">في حقل **معرف الكيان القانوني** ، حدد الشركة المقرضة.</span><span class="sxs-lookup"><span data-stu-id="9e61f-126">In the **Legal entity ID** field, select the lending company.</span></span> <span data-ttu-id="9e61f-127">املأ الحقول المتبقية بالشكل المناسب ، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9e61f-127">Fill in the remaining fields as appropriate, and then select **Save**.</span></span>
4. <span data-ttu-id="9e61f-128">في صفحة **سعر التحويل**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9e61f-128">On the **Transfer price** page, select **New**.</span></span>
5. <span data-ttu-id="9e61f-129">في حقل **الكيان القانوني المقترض**، حدد الشركة المناسبة.</span><span class="sxs-lookup"><span data-stu-id="9e61f-129">In the **Borrowing legal entity** field, select the appropriate company.</span></span>
6. <span data-ttu-id="9e61f-130">لإقراض الشركة المقترضة فقط المورد الذي أنشأته في بداية هذا القسم، في حقل **المورد**، حدد اسم المورد الذي قمت بإنشائه.</span><span class="sxs-lookup"><span data-stu-id="9e61f-130">To lend the borrowing company only the resource that you created at the beginning of this section, in the **Resource** field, select the name of the resource that you created.</span></span> <span data-ttu-id="9e61f-131">لجعل كافة الموارد في الشركة المقرضة متوفرة لشركه مقترضة، اترك حقل **المورد** فارغا.</span><span class="sxs-lookup"><span data-stu-id="9e61f-131">To make all resources in the lending company available to the borrowing company, leave the **Resource** field blank.</span></span>
7. <span data-ttu-id="9e61f-132">في صفحة **معلمات إدارة المشاريع ومحاسبتها**، ضمن علامة التبويب **بين الشركات الشقيقة**، قم بتعيين خيار **تمكين جدوله الموارد والجداول بين الشركات الشقيقة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9e61f-132">On the **Project management and accounting parameters** page, on the **Intercompany** tab, set the **Enable intercompany resource scheduling and timesheets** option to **Yes**.</span></span>

### <a name="in-the-borrowing-company"></a><span data-ttu-id="9e61f-133">في الشركة المقترضة</span><span class="sxs-lookup"><span data-stu-id="9e61f-133">In the borrowing company</span></span>

- <span data-ttu-id="9e61f-134">في صفحة **قائمة الموارد**، في عامل تصفية البحث ، أدخل اسم المورد الذي قمت بإنشائه للشركة المُقرضة ، للتحقق من أن الاسم مضمن في قائمة الموارد للشركة المقترضة.</span><span class="sxs-lookup"><span data-stu-id="9e61f-134">On the **Resources list** page, in the search filter, enter the name of the resource that you created for the lending company, to verify that the name is included in the resource list for the borrowing company.</span></span>

## <a name="request-project-resources"></a><span data-ttu-id="9e61f-135">طلب موارد المشروع</span><span class="sxs-lookup"><span data-stu-id="9e61f-135">Request project resources</span></span>
<span data-ttu-id="9e61f-136">تسمح وظيفة جدولة موارد المشروع فقط لمديري الموارد بتوزيع الموارد المعينة على المشاركات أو المشاريع.</span><span class="sxs-lookup"><span data-stu-id="9e61f-136">The functionality for project resource scheduling only lets resource managers distribute staffed resources on engagements or projects.</span></span> <span data-ttu-id="9e61f-137">لتمكين هذه الوظيفة ، أكمل المهام التالية ، أو تحقق من اكتمالها:</span><span class="sxs-lookup"><span data-stu-id="9e61f-137">To enable this functionality, complete the following tasks, or verify that they have been completed:</span></span>

- <span data-ttu-id="9e61f-138">قم بإعداد التسلسلات الرقمية.</span><span class="sxs-lookup"><span data-stu-id="9e61f-138">Set up number sequences.</span></span>
- <span data-ttu-id="9e61f-139">قم بإعداد تدفقات إدارة المشروع والمحاسبة.</span><span class="sxs-lookup"><span data-stu-id="9e61f-139">Set up project management and accounting workflows.</span></span>
- <span data-ttu-id="9e61f-140">قم بتمكين مهام سير العمل لطلب المورد.</span><span class="sxs-lookup"><span data-stu-id="9e61f-140">Enable resource request workflows.</span></span>

<span data-ttu-id="9e61f-141">بعد الانتهاء من المهام السابقة ، يمكنك إكمال المهام التالية كما تريد:</span><span class="sxs-lookup"><span data-stu-id="9e61f-141">After the preceding tasks have been completed, you can complete the following tasks as you require:</span></span>

- <span data-ttu-id="9e61f-142">قم بإنشاء طلب مورد من مورد يعمل بحجز مبدئي.</span><span class="sxs-lookup"><span data-stu-id="9e61f-142">Create a resource request from a soft-booked staffed resource.</span></span>
- <span data-ttu-id="9e61f-143">راقب طلبات الموارد.</span><span class="sxs-lookup"><span data-stu-id="9e61f-143">Monitor resource requests.</span></span>
- <span data-ttu-id="9e61f-144">يمكنك الوفاء بطلبات الموارد.</span><span class="sxs-lookup"><span data-stu-id="9e61f-144">Fulfill resource requests.</span></span>
- <span data-ttu-id="9e61f-145">اطلب موردًا موظفًا من WBS.</span><span class="sxs-lookup"><span data-stu-id="9e61f-145">Request a staffed resource from a WBS.</span></span>
- <span data-ttu-id="9e61f-146">احجز الموارد لمشروع دون الحاجة إلى طلب مورد يعمل به.</span><span class="sxs-lookup"><span data-stu-id="9e61f-146">Book resources to a project without having a request for a staffed resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]