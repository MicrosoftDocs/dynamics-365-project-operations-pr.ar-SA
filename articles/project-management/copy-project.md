---
title: نسخ مشروع
description: يوفر هذا الموضوع معلومات حول نسخ المشاريع في Dynamics 365 Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: e35dc725e7938e9f59f7151dd1b37500fabf77a4
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907813"
---
# <a name="copy-a-project"></a><span data-ttu-id="d1652-103">نسخ مشروع</span><span class="sxs-lookup"><span data-stu-id="d1652-103">Copy a project</span></span>

<span data-ttu-id="d1652-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="d1652-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d1652-105">مع Dynamics 365 Project Operations، يمكنك بناء مشاريع جديدة بسرعة باستخدام الإجراء **نسخ المشروع** على نموذج **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="d1652-105">With Dynamics 365 Project Operations, you can quickly build new projects by using the **Copy Project** action on the **Projects** from.</span></span> <span data-ttu-id="d1652-106">لنسخ مشروع، حدد مشروعًا، ثم حدد **نسخ**.</span><span class="sxs-lookup"><span data-stu-id="d1652-106">To copy a project, select a project, and then select **Copy**.</span></span> <span data-ttu-id="d1652-107">سينسخ هذا الإجراء:</span><span class="sxs-lookup"><span data-stu-id="d1652-107">The action will copy:</span></span>

- <span data-ttu-id="d1652-108">خصائص المشروع</span><span class="sxs-lookup"><span data-stu-id="d1652-108">Project properties</span></span>
- <span data-ttu-id="d1652-109">هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="d1652-109">The Work breakdown structure</span></span>
- <span data-ttu-id="d1652-110">أعضاء فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="d1652-110">Project team members</span></span>
- <span data-ttu-id="d1652-111">تقديرات المشروع</span><span class="sxs-lookup"><span data-stu-id="d1652-111">Project estimates</span></span>
- <span data-ttu-id="d1652-112">تقديرات مصروفات المشاريع</span><span class="sxs-lookup"><span data-stu-id="d1652-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="d1652-113">خصائص المشروع</span><span class="sxs-lookup"><span data-stu-id="d1652-113">Project properties</span></span>

<span data-ttu-id="d1652-114">عند نسخ المشروع، يتم نسخ القيم الموجودة في الحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="d1652-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="d1652-115">اسم</span><span class="sxs-lookup"><span data-stu-id="d1652-115">Name</span></span>
- <span data-ttu-id="d1652-116">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="d1652-116">Description</span></span>
- <span data-ttu-id="d1652-117">العميل</span><span class="sxs-lookup"><span data-stu-id="d1652-117">Customer</span></span>
- <span data-ttu-id="d1652-118">قالب التقويم</span><span class="sxs-lookup"><span data-stu-id="d1652-118">Calendar Template</span></span>
- <span data-ttu-id="d1652-119">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="d1652-119">Currency</span></span>
- <span data-ttu-id="d1652-120">الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="d1652-120">Contracting Unit</span></span>
- <span data-ttu-id="d1652-121">مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="d1652-121">Project Manager</span></span>
- <span data-ttu-id="d1652-122">الموقف</span><span class="sxs-lookup"><span data-stu-id="d1652-122">Status</span></span>
- <span data-ttu-id="d1652-123">الحالة الإجمالية للمشروع</span><span class="sxs-lookup"><span data-stu-id="d1652-123">Overall Project Status</span></span>
- <span data-ttu-id="d1652-124">التعليقات</span><span class="sxs-lookup"><span data-stu-id="d1652-124">Comments</span></span>
- <span data-ttu-id="d1652-125">التقديرات</span><span class="sxs-lookup"><span data-stu-id="d1652-125">Estimates</span></span>
- <span data-ttu-id="d1652-126">تاريخ البدء المقدر</span><span class="sxs-lookup"><span data-stu-id="d1652-126">Estimated Start Date</span></span>
- <span data-ttu-id="d1652-127">تاريخ الانتهاء</span><span class="sxs-lookup"><span data-stu-id="d1652-127">Finish Date</span></span>
- <span data-ttu-id="d1652-128">الجهد (بالساعات)</span><span class="sxs-lookup"><span data-stu-id="d1652-128">Effort (Hours)</span></span>
- <span data-ttu-id="d1652-129">تكلفة العالمة المقدرة</span><span class="sxs-lookup"><span data-stu-id="d1652-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="d1652-130">تكلفة المصروفات المقدرة</span><span class="sxs-lookup"><span data-stu-id="d1652-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="d1652-131">هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="d1652-131">Work breakdown structure</span></span>

<span data-ttu-id="d1652-132">عند نسخ المشروع، يتم نسخ هيكل تنظيم العمل المحمّل بالكامل للمورد.</span><span class="sxs-lookup"><span data-stu-id="d1652-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="d1652-133">تم استبدال الموارد المسماة بالموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="d1652-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="d1652-134">إذا لم تتوفر لدى الموارد المسماة نفس ساعات عمل المورد العام، فسيُعاد حساب الجدول وقد تتغير مدد المهام.</span><span class="sxs-lookup"><span data-stu-id="d1652-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="d1652-135">أعضاء فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="d1652-135">Project team members</span></span>

<span data-ttu-id="d1652-136">عندما يتم نسخ فريق مشروع من المشروع المصدر، يتم نسخ الموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="d1652-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="d1652-137">يتم أيضًا الاحتفاظ بتعيينات الموارد العامة كما كانت في المشروع المصدر.</span><span class="sxs-lookup"><span data-stu-id="d1652-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="d1652-138">سيتم تحويل الموارد المسامة إلى أعضاء فريق عام.</span><span class="sxs-lookup"><span data-stu-id="d1652-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="d1652-139">التقديرات</span><span class="sxs-lookup"><span data-stu-id="d1652-139">Estimates</span></span>

<span data-ttu-id="d1652-140">عند نسخ المشروع، يتم نسخ كل من بنود تقدير الموارد والمصروفات من المشروع المصدر.</span><span class="sxs-lookup"><span data-stu-id="d1652-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span>