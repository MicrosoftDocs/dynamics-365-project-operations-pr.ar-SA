---
title: نسخ مشروع
description: يقدم هذا الموضوع معلومات حول نسخ المشاريع في Dynamics 365 Project Operations.
author: ruhercul
ms.date: 05/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c3055ab5b8c07faa2bc9167956d283e2a66029dd
ms.sourcegitcommit: 173f2b1f4e063c440a5f78d76d456c62aadbd89e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/24/2021
ms.locfileid: "6091238"
---
# <a name="copy-a-project"></a><span data-ttu-id="cabdd-103">نسخ مشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-103">Copy a project</span></span>

<span data-ttu-id="cabdd-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="cabdd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cabdd-105">باستخدام Dynamics 365 Project Operations، يمكنك إنشاء مشاريع جديدة بسرعة من خلال تحديد **نسخ المشروع** على نموذج **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="cabdd-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="cabdd-106">لنسخ مشروع، افتح المشروع الذي تريد نسخه، ثم حدد **نسخ المشروع**.</span><span class="sxs-lookup"><span data-stu-id="cabdd-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="cabdd-107">سينسخ الإجراء ما يلي:</span><span class="sxs-lookup"><span data-stu-id="cabdd-107">The action will copy the following:</span></span>

- <span data-ttu-id="cabdd-108">خصائص المشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-108">Project properties</span></span> 
- <span data-ttu-id="cabdd-109">هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="cabdd-109">Work breakdown structure</span></span>
- <span data-ttu-id="cabdd-110">أعضاء فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-110">Project team members</span></span>
- <span data-ttu-id="cabdd-111">تقديرات المشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-111">Project estimates</span></span>
- <span data-ttu-id="cabdd-112">تقديرات مصروفات المشاريع</span><span class="sxs-lookup"><span data-stu-id="cabdd-112">Project expense estimates</span></span>
- <span data-ttu-id="cabdd-113">تقديرات مواد المشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-113">Project material estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="cabdd-114">خصائص المشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-114">Project properties</span></span>

<span data-ttu-id="cabdd-115">عند نسخ المشروع، يتم نسخ القيم الموجودة في الحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="cabdd-115">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="cabdd-116">اسم</span><span class="sxs-lookup"><span data-stu-id="cabdd-116">Name</span></span>
- <span data-ttu-id="cabdd-117">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="cabdd-117">Description</span></span>
- <span data-ttu-id="cabdd-118">العميل</span><span class="sxs-lookup"><span data-stu-id="cabdd-118">Customer</span></span>
- <span data-ttu-id="cabdd-119">قالب التقويم</span><span class="sxs-lookup"><span data-stu-id="cabdd-119">Calendar Template</span></span>
- <span data-ttu-id="cabdd-120">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="cabdd-120">Currency</span></span>
- <span data-ttu-id="cabdd-121">الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cabdd-121">Contracting Unit</span></span>
- <span data-ttu-id="cabdd-122">مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-122">Project Manager</span></span>
- <span data-ttu-id="cabdd-123">الموقف</span><span class="sxs-lookup"><span data-stu-id="cabdd-123">Status</span></span>
- <span data-ttu-id="cabdd-124">الحالة الإجمالية للمشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-124">Overall Project Status</span></span>
- <span data-ttu-id="cabdd-125">التعليقات</span><span class="sxs-lookup"><span data-stu-id="cabdd-125">Comments</span></span>
- <span data-ttu-id="cabdd-126">التقديرات</span><span class="sxs-lookup"><span data-stu-id="cabdd-126">Estimates</span></span>
- <span data-ttu-id="cabdd-127">تاريخ البدء المقدر: هذا هو التاريخ الذي يتم فيه إنشاء المشروع من النسخة.</span><span class="sxs-lookup"><span data-stu-id="cabdd-127">Estimated Start Date: This is the date that the project is created from the copy.</span></span>
- <span data-ttu-id="cabdd-128">تاريخ الانتهاء المقدر: يتم ضبط هذا التاريخ استنادًا إلى تاريخ بدء المشروع الجديد الذي تم الانتهاء منه من النسخة.</span><span class="sxs-lookup"><span data-stu-id="cabdd-128">Estimated Finish Date: This date is adjusted based on the start date of the new project that was made from the copy.</span></span>
- <span data-ttu-id="cabdd-129">الجهد (بالساعات)</span><span class="sxs-lookup"><span data-stu-id="cabdd-129">Effort (Hours)</span></span>
- <span data-ttu-id="cabdd-130">تكلفة العمالة المقدّرة</span><span class="sxs-lookup"><span data-stu-id="cabdd-130">Estimated Labor Cost</span></span>
- <span data-ttu-id="cabdd-131">تكلفة المصروفات المقدّرة</span><span class="sxs-lookup"><span data-stu-id="cabdd-131">Estimated Expense Cost</span></span>
- <span data-ttu-id="cabdd-132">تكلفة المواد المقدّرة</span><span class="sxs-lookup"><span data-stu-id="cabdd-132">Estimated Material Cost</span></span>

> [!NOTE]
> <span data-ttu-id="cabdd-133">تُعد عملية نسخ المشروع عملية تشغيل طويلة.</span><span class="sxs-lookup"><span data-stu-id="cabdd-133">Copy project is a long running operation.</span></span> <span data-ttu-id="cabdd-134">يتم أيضًا نسخ سجلات المشروع وسماته ذات الصلة والعديد من الكيانات المرتبطة.</span><span class="sxs-lookup"><span data-stu-id="cabdd-134">Project records, their relevant attributes, and many related entities are also copied.</span></span> <span data-ttu-id="cabdd-135">نظرًا لطبيعة التشغيل الطويلة للعملية، بعد بدء النسخ، يتم تأمين صفحة المشروع الهدف للتحرير حتى تكتمل عملية النسخ.</span><span class="sxs-lookup"><span data-stu-id="cabdd-135">Because of the long running nature of the operation, after the copy starts, the target project page is locked for editing until the copy operation is complete.</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="cabdd-136">هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="cabdd-136">Work breakdown structure</span></span>

<span data-ttu-id="cabdd-137">عند نسخ المشروع، يتم نسخ هيكل تنظيم العمل المحمّل بالكامل للمورد.</span><span class="sxs-lookup"><span data-stu-id="cabdd-137">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="cabdd-138">تم استبدال الموارد المسماة بالموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="cabdd-138">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="cabdd-139">إذا لم تتوفر لدى الموارد المسماة نفس ساعات عمل المورد العام، فسيُعاد حساب الجدول وقد تتغير مدد المهام.</span><span class="sxs-lookup"><span data-stu-id="cabdd-139">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="cabdd-140">أعضاء فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="cabdd-140">Project team members</span></span>

<span data-ttu-id="cabdd-141">عندما يتم نسخ فريق مشروع من المشروع المصدر، يتم نسخ الموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="cabdd-141">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="cabdd-142">يتم أيضًا الاحتفاظ بتعيينات الموارد العامة كما كانت في المشروع المصدر.</span><span class="sxs-lookup"><span data-stu-id="cabdd-142">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="cabdd-143">سيتم تحويل الموارد المسامة إلى أعضاء فريق عام.</span><span class="sxs-lookup"><span data-stu-id="cabdd-143">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="cabdd-144">التقديرات</span><span class="sxs-lookup"><span data-stu-id="cabdd-144">Estimates</span></span>

<span data-ttu-id="cabdd-145">وعند نسخ المشروع، يتم نسخ بنود الموارد والمصروفات وتقديرات المواد من المشروع المصدر.</span><span class="sxs-lookup"><span data-stu-id="cabdd-145">When the project is copied, resource, expense and material estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="cabdd-146">للحصول على معلومات حول كيفية الوصول إلى "نسخ المشروع" برمجيًا، راجع [تطوير قوالب المشروع مع نسخ المشروع‬‬](dev-copy-project.md).</span><span class="sxs-lookup"><span data-stu-id="cabdd-146">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
