---
title: تحديث مشروع
description: يوفر هذا الموضوع معلومات حول تحديث المشاريع في Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 5c9cd0c7c6886bd454c5f2ef2ae7f20d1707293f
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070499"
---
# <a name="update-a-project"></a><span data-ttu-id="1541b-103">تحديث مشروع</span><span class="sxs-lookup"><span data-stu-id="1541b-103">Update a project</span></span>

<span data-ttu-id="1541b-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="1541b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1541b-105">فيما يلي ملخص للحقول التي يمكن تحديثها في مشروع بعد إنشائه وأي تبعات قابلة للتطبيق على التحديثات.</span><span class="sxs-lookup"><span data-stu-id="1541b-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="1541b-106">حقول تفاصيل المشروع</span><span class="sxs-lookup"><span data-stu-id="1541b-106">Project detail fields</span></span>

- <span data-ttu-id="1541b-107">**الاسم** : عنوان المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-107">**Name** : The title of the project.</span></span>
- <span data-ttu-id="1541b-108">**الوصف** : نظرة عامة على المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-108">**Description** : An overview of the project.</span></span>
- <span data-ttu-id="1541b-109">**العميل** : الشركة التي سيتم تسليم المشروع إليها.</span><span class="sxs-lookup"><span data-stu-id="1541b-109">**Customer** : The company the project will be delivered to.</span></span>
- <span data-ttu-id="1541b-110">**قالب التقويم** : ساعات عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-110">**Calendar template** : The working hours of the project.</span></span> <span data-ttu-id="1541b-111">عند تغيير الحقل، تتم إعادة حساب الجدول بأكمله.</span><span class="sxs-lookup"><span data-stu-id="1541b-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="1541b-112">**العملة** : عملة المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-112">**Currency** : The currency for the project.</span></span> <span data-ttu-id="1541b-113">يتم تعيين القيمة الافتراضية لهذا الحقل استنادا إلى العملة المحددة في الوحدة المتعاقدة.</span><span class="sxs-lookup"><span data-stu-id="1541b-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="1541b-114">عند تحديث الوحدة المتعاقدة، يتم تحديث الحقل أيضًا.</span><span class="sxs-lookup"><span data-stu-id="1541b-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="1541b-115">**الوحدة المتعاقدة** : الوحدة التنظيمية التي تمثل مجموعة الشركة أو القسم المسؤول بشكل أساسي عن كسب المبيعات وإدارة تسليم العمل والخدمات إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="1541b-115">**Contracting Unit** : The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="1541b-116">**مدير المشروع** : عضو فريق المشروع الذي لديه التخويل لمراجعة إدخالات الوقت والمصروفات والموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="1541b-116">**Project Manager** : The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="1541b-117">حقول التقدير</span><span class="sxs-lookup"><span data-stu-id="1541b-117">Estimate fields</span></span>

- <span data-ttu-id="1541b-118">**تاريخ البدء المقدر** : التاريخ الذي سيبدأ فيه المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-118">**Estimated Start Date** : The date that the project will begin.</span></span> <span data-ttu-id="1541b-119">عند تحديث هذا الحقل، سيتم تحريك أية مهام في المشروع بالتناسب مع تاريخ البدء الجديد.</span><span class="sxs-lookup"><span data-stu-id="1541b-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="1541b-120">**تاريخ الانتهاء** : التاريخ الذي تمت فيه جدولة نهاية المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-120">**Finish Date** : The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="1541b-121">**الجهد** : الجهد المقدر للمشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-121">**Effort** : The estimated effort of the project.</span></span> <span data-ttu-id="1541b-122">عند إضافة مهام إلى المشروع، لن يصبح هذا الحقل قابلا للتحرير.</span><span class="sxs-lookup"><span data-stu-id="1541b-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="1541b-123">**تكلفة العمالة المقدرة** : تكلفة العمالة المقدرة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-123">**Estimated Labor Cost** : The estimated labor cost of the project.</span></span> <span data-ttu-id="1541b-124">عند إضافة تكاليف المهام إلى المشروع، لن يصبح هذا الحقل قابلا للتحرير.</span><span class="sxs-lookup"><span data-stu-id="1541b-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="1541b-125">**المصروفات المقدرة:** المصروفات المقدرة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-125">**Estimated Expenses** : The estimated expenses of the project.</span></span> <span data-ttu-id="1541b-126">عند إضافة المصروفات إلى المشروع، لن يصبح هذا الحقل قابلا للتحرير.</span><span class="sxs-lookup"><span data-stu-id="1541b-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="1541b-127">الحقول الفعلية للمشروع</span><span class="sxs-lookup"><span data-stu-id="1541b-127">Project actual fields</span></span>
- <span data-ttu-id="1541b-128">**البدء الفعلي** : تاريخ بدء المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-128">**Actual Start** : The date that the project started.</span></span>
- <span data-ttu-id="1541b-129">**الانتهاء الفعلي** : يتم تحديثه عند اكتمال مشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-129">**Actual Finish** : To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="1541b-130">حقول حالة المشروع</span><span class="sxs-lookup"><span data-stu-id="1541b-130">Project status fields</span></span>

- <span data-ttu-id="1541b-131">**حالة المشروع الكلية** : حالة السلامة الكلية للمشروع والتي يوفرها مدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-131">**Overall Project Status** : The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="1541b-132">**التعليقات** : حقل سردي يتعلق بالسلامة الحالية للمشروع الذي يوفره مدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="1541b-132">**Comments** : A narrative regarding the current health of the project provided by the Project manager.</span></span>

