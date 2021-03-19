---
title: نسخ مشروع
description: يقدم هذا الموضوع معلومات حول نسخ المشاريع في Dynamics 365 Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 02/22/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: af1942e81691d9e13fdcbbf68599c1a8a4004582
ms.sourcegitcommit: 24528bb9c0ef8898077cb3bc672daa211c0e73aa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "5479503"
---
# <a name="copy-a-project"></a><span data-ttu-id="5de0e-103">نسخ مشروع</span><span class="sxs-lookup"><span data-stu-id="5de0e-103">Copy a project</span></span>

<span data-ttu-id="5de0e-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="5de0e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5de0e-105">باستخدام Dynamics 365 Project Operations، يمكنك إنشاء مشاريع جديدة بسرعة من خلال تحديد **نسخ المشروع** على نموذج **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="5de0e-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="5de0e-106">لنسخ مشروع، افتح المشروع الذي تريد نسخه، ثم حدد **نسخ المشروع**.</span><span class="sxs-lookup"><span data-stu-id="5de0e-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="5de0e-107">سينسخ هذا الإجراء:</span><span class="sxs-lookup"><span data-stu-id="5de0e-107">The action will copy:</span></span>

- <span data-ttu-id="5de0e-108">خصائص المشروع (يتم نسخ تاريخ البدء المقدر من المشروع المصدر)</span><span class="sxs-lookup"><span data-stu-id="5de0e-108">Project properties (The estimated start date is copied from the source project)</span></span>
- <span data-ttu-id="5de0e-109">هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="5de0e-109">The Work breakdown structure</span></span>
- <span data-ttu-id="5de0e-110">أعضاء فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="5de0e-110">Project team members</span></span>
- <span data-ttu-id="5de0e-111">تقديرات المشروع</span><span class="sxs-lookup"><span data-stu-id="5de0e-111">Project estimates</span></span>
- <span data-ttu-id="5de0e-112">تقديرات مصروفات المشاريع</span><span class="sxs-lookup"><span data-stu-id="5de0e-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="5de0e-113">خصائص المشروع</span><span class="sxs-lookup"><span data-stu-id="5de0e-113">Project properties</span></span>

<span data-ttu-id="5de0e-114">عند نسخ المشروع، يتم نسخ القيم الموجودة في الحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="5de0e-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="5de0e-115">اسم</span><span class="sxs-lookup"><span data-stu-id="5de0e-115">Name</span></span>
- <span data-ttu-id="5de0e-116">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="5de0e-116">Description</span></span>
- <span data-ttu-id="5de0e-117">العميل</span><span class="sxs-lookup"><span data-stu-id="5de0e-117">Customer</span></span>
- <span data-ttu-id="5de0e-118">قالب التقويم</span><span class="sxs-lookup"><span data-stu-id="5de0e-118">Calendar Template</span></span>
- <span data-ttu-id="5de0e-119">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="5de0e-119">Currency</span></span>
- <span data-ttu-id="5de0e-120">الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="5de0e-120">Contracting Unit</span></span>
- <span data-ttu-id="5de0e-121">مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="5de0e-121">Project Manager</span></span>
- <span data-ttu-id="5de0e-122">الموقف</span><span class="sxs-lookup"><span data-stu-id="5de0e-122">Status</span></span>
- <span data-ttu-id="5de0e-123">الحالة الإجمالية للمشروع</span><span class="sxs-lookup"><span data-stu-id="5de0e-123">Overall Project Status</span></span>
- <span data-ttu-id="5de0e-124">التعليقات</span><span class="sxs-lookup"><span data-stu-id="5de0e-124">Comments</span></span>
- <span data-ttu-id="5de0e-125">التقديرات</span><span class="sxs-lookup"><span data-stu-id="5de0e-125">Estimates</span></span>
- <span data-ttu-id="5de0e-126">تاريخ البدء المقدر</span><span class="sxs-lookup"><span data-stu-id="5de0e-126">Estimated Start Date</span></span>
- <span data-ttu-id="5de0e-127">تاريخ الانتهاء</span><span class="sxs-lookup"><span data-stu-id="5de0e-127">Finish Date</span></span>
- <span data-ttu-id="5de0e-128">الجهد (بالساعات)</span><span class="sxs-lookup"><span data-stu-id="5de0e-128">Effort (Hours)</span></span>
- <span data-ttu-id="5de0e-129">تكلفة العالمة المقدرة</span><span class="sxs-lookup"><span data-stu-id="5de0e-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="5de0e-130">تكلفة المصروفات المقدرة</span><span class="sxs-lookup"><span data-stu-id="5de0e-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="5de0e-131">هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="5de0e-131">Work breakdown structure</span></span>

<span data-ttu-id="5de0e-132">عند نسخ المشروع، يتم نسخ هيكل تنظيم العمل المحمّل بالكامل للمورد.</span><span class="sxs-lookup"><span data-stu-id="5de0e-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="5de0e-133">تم استبدال الموارد المسماة بالموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="5de0e-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="5de0e-134">إذا لم تتوفر لدى الموارد المسماة نفس ساعات عمل المورد العام، فسيُعاد حساب الجدول وقد تتغير مدد المهام.</span><span class="sxs-lookup"><span data-stu-id="5de0e-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="5de0e-135">أعضاء فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="5de0e-135">Project team members</span></span>

<span data-ttu-id="5de0e-136">عندما يتم نسخ فريق مشروع من المشروع المصدر، يتم نسخ الموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="5de0e-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="5de0e-137">يتم أيضًا الاحتفاظ بتعيينات الموارد العامة كما كانت في المشروع المصدر.</span><span class="sxs-lookup"><span data-stu-id="5de0e-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="5de0e-138">سيتم تحويل الموارد المسامة إلى أعضاء فريق عام.</span><span class="sxs-lookup"><span data-stu-id="5de0e-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="5de0e-139">التقديرات</span><span class="sxs-lookup"><span data-stu-id="5de0e-139">Estimates</span></span>

<span data-ttu-id="5de0e-140">عند نسخ المشروع، يتم نسخ كل من بنود تقدير الموارد والمصروفات من المشروع المصدر.</span><span class="sxs-lookup"><span data-stu-id="5de0e-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="5de0e-141">للحصول على معلومات حول كيفية الوصول إلى "نسخ المشروع" برمجيًا، راجع [تطوير قوالب المشروع مع نسخ المشروع‬‬](dev-copy-project.md).</span><span class="sxs-lookup"><span data-stu-id="5de0e-141">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
