---
title: الجديد أو المتغير في الإصدار 3 من Project Service Automation، إصدار التحديث 18
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 18.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d7ea200531dd24d56a829f879e3a2532a9b38dc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070598"
---
# <a name="project-service-automation-update-release-18-v3"></a><span data-ttu-id="7c635-103">الإصدار 3 من Project Service Automation، إصدار التحديث 18</span><span class="sxs-lookup"><span data-stu-id="7c635-103">Project Service Automation Update Release 18, V3</span></span>

<span data-ttu-id="7c635-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7c635-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="7c635-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="7c635-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="7c635-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="7c635-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="7c635-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="7c635-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="7c635-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="7c635-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="7c635-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 18.</span><span class="sxs-lookup"><span data-stu-id="7c635-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 18.</span></span> <span data-ttu-id="7c635-110">لدى هذا الإصدار رقم البنية V3.10.8.12 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر أبريل 2020.</span><span class="sxs-lookup"><span data-stu-id="7c635-110">This version has a build number of V3.10.8.12 and is generally available through a self-update in April 2020.</span></span>

## <a name="update-release-18"></a><span data-ttu-id="7c635-111">إصدار التحديث 18</span><span class="sxs-lookup"><span data-stu-id="7c635-111">Update Release 18</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="7c635-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="7c635-112">Bug fixes</span></span>

<span data-ttu-id="7c635-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="7c635-113">**Time and Expense**</span></span>

- <span data-ttu-id="7c635-114">إصلاح: تقوم عمليات سير المهام **استدعاء** و **طلب** و **إلغاء الموافقة** بطرح استثناء مع رسائل خطأ غير واضحة.</span><span class="sxs-lookup"><span data-stu-id="7c635-114">Fixed: **Recall** , **Request** , and **Cancel Approval** flows throw exceptions with unclear error messages.</span></span>
- <span data-ttu-id="7c635-115">إصلاح: عند فشل **إلغاء الموافقة** لمصروفات معينة، لن يتم طرح أي خطأ استثناء ملائم.</span><span class="sxs-lookup"><span data-stu-id="7c635-115">Fixed: When **Cancel Approval** fails for an expense, a relevant exception error is not thrown.</span></span>
- <span data-ttu-id="7c635-116">إصلاح: تتعامل شبكة إدخال الوقت بشكل غير صحيح مع أيام العطل في أستراليا بعد تبديل التوقيت الصيفي في أكتوبر.</span><span class="sxs-lookup"><span data-stu-id="7c635-116">Fixed: The Time Entry grid incorrectly handles non-working days in Australia after the daylight savings time (DST) switch in October.</span></span>
- <span data-ttu-id="7c635-117">إصلاح: يمنع المنطق الافتراضي غير الصحيح إرسال المصروفات.</span><span class="sxs-lookup"><span data-stu-id="7c635-117">Fixed: Incorrect defaulting logic prevents submission of expenses.</span></span>
- <span data-ttu-id="7c635-118">إصلاح: عند فشل الموافقة على إدخال الوقت، تبقى الموافقة في الحالة **معلقة**.</span><span class="sxs-lookup"><span data-stu-id="7c635-118">Fixed: When time entry approval fails, the approval remains in a state of **Pending**.</span></span>
- <span data-ttu-id="7c635-119">إصلاح: أخطاء SQL في الموافقات المجمعة (حالة التوقف التام/المهلة).</span><span class="sxs-lookup"><span data-stu-id="7c635-119">Fixed: SQL Errors on bulk approvals (deadlock/timeout).</span></span>
- <span data-ttu-id="7c635-120">إصلاح: مشاكل ملحوظة في الأداء في تجربة المستخدم بسبب تحديث أعضاء الفريق أثناء الموافقة على إدخالات الوقت.</span><span class="sxs-lookup"><span data-stu-id="7c635-120">Fixed: Significant performance issues in the user experience caused by updating team members while approving time entries.</span></span>

<span data-ttu-id="7c635-121">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="7c635-121">**Project Management**</span></span>

- <span data-ttu-id="7c635-122">إصلاح: تم نقل إعلام المنطقة الزمنية من طريقة عرض **التسوية** إلى نموذج **المشروع** الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="7c635-122">Fixed: Time zone notification moved from the **Reconciliation** view to the **Project** main form.</span></span>
- <span data-ttu-id="7c635-123">إصلاح: لا يتم تعيين قالب التقويم يتم بشكل صحيح إلى الإعداد الافتراضي عند فتح نموذج مشروع جديد.</span><span class="sxs-lookup"><span data-stu-id="7c635-123">Fixed: Calendar template is not correctly defaulting when a new project form opens.</span></span>
- <span data-ttu-id="7c635-124">إصلاح: بالنسبة إلى المستعرضات المستندة إلى Chromium، يتعذر على المستخدمين تحديد المهام السابقة بسهولة لحذفها.</span><span class="sxs-lookup"><span data-stu-id="7c635-124">Fixed: For chromium-based browsers, users are unable to easily select predecessor tasks to delete.</span></span>
- <span data-ttu-id="7c635-125">إصلاح: يؤدي إنشاء أو نسخ **مشروع من قالب فارغ** إلى إحضار تعيينات ليست ذات صلة.</span><span class="sxs-lookup"><span data-stu-id="7c635-125">Fixed: Creating or copying **Project from Empty template** fetches unrelated assignments.</span></span>
- <span data-ttu-id="7c635-126">إصلاح: في حالات قصوى معينة، يؤدي إنشاء تعيين جديد من نتائج شبكة المهام إلى إنشاء سجلات مكررة.</span><span class="sxs-lookup"><span data-stu-id="7c635-126">Fixed: In specific edge cases, creating a new assignment from the task grid results in duplicate records being created.</span></span>
- <span data-ttu-id="7c635-127">إصلاح: في الوضع اليدوي، يتعذر على المستخدمين تحديث تواريخ بدء المهام بحيث تقع بعد التاريخ الحالي المحفوظ.</span><span class="sxs-lookup"><span data-stu-id="7c635-127">Fixed: In manual mode, users are unable to update task start dates to be later than the current date saved.</span></span>

<span data-ttu-id="7c635-128">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="7c635-128">**Resource Management**</span></span>

- <span data-ttu-id="7c635-129">إصلاح: يقوم صف الإجمالي الفرعي في طريقة عرض **التسوية** بحساب الفرق في الحجوزات بشكل غير صحيح بعد تمديد الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="7c635-129">Fixed: **Reconciliation** view subtotal row incorrectly calculates bookings variance after extending bookings.</span></span>
- <span data-ttu-id="7c635-130">إصلاح: تعرض طريقة عرض **التسوية** بشكل غير صحيح تعيينات الموارد بشكل غير صحيح عندما يكون تقويم مورد قابل للحجز غير متطابق مع تقويم المشروع.</span><span class="sxs-lookup"><span data-stu-id="7c635-130">Fixed: **Reconciliation** view incorrectly displays resource assignments when the bookable resource has a calendar that does not match the project calendar.</span></span>

<span data-ttu-id="7c635-131">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="7c635-131">**Sales**</span></span>

- <span data-ttu-id="7c635-132">إصلاح: عند إعادة الموافقة على إدخالات الوقت ( **موافقة > إلغاء >** موافقة من جديد)، يتم إنشاء قيم فعلية مكررة غير خاضعة للرسوم.‬</span><span class="sxs-lookup"><span data-stu-id="7c635-132">Fixed: When time entries are re-approved ( **Approve > Cancel >** approve again), a duplicate non-chargeable actual is created.</span></span>
