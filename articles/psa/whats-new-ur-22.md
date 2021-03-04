---
title: الجديد أو المتغير في إصدار التحديث 22، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 22.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 07/28/2020
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
ms.openlocfilehash: db4cbb9f9daadcb1911325f8bee987d5e480e1cf
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150967"
---
# <a name="project-service-automation-update-release-22-v3"></a><span data-ttu-id="2de29-103">الإصدار 3 من Project Service Automation، إصدار التحديث 22</span><span class="sxs-lookup"><span data-stu-id="2de29-103">Project Service Automation Update Release 22, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="2de29-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="2de29-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="2de29-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="2de29-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="2de29-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="2de29-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="2de29-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="2de29-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="2de29-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="2de29-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="2de29-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 22.</span><span class="sxs-lookup"><span data-stu-id="2de29-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 22.</span></span> <span data-ttu-id="2de29-110">لدى هذا الإصدار رقم البنية V 3.10.33.48 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر يونيو 2020.</span><span class="sxs-lookup"><span data-stu-id="2de29-110">This version has a build number of V 3.10.33.48 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-22"></a><span data-ttu-id="2de29-111">إصدار التحديث 22</span><span class="sxs-lookup"><span data-stu-id="2de29-111">Update Release 22</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="2de29-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="2de29-112">Bug fixes</span></span>



<span data-ttu-id="2de29-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="2de29-113">**Time and Expense**</span></span>

<span data-ttu-id="2de29-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2de29-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="2de29-115">لا تتم إضافة **إدخالات الوقت** تلقائيًا في جدولة إدخالات الوقت بعد الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="2de29-115">**Time entries** are not automatically added in the Time entries schedule after import.</span></span>
- <span data-ttu-id="2de29-116">لا يتعرف منتقي تاريخ شبكة **إدخال الوقت** على الإعدادات الإقليمية الخاصة بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="2de29-116">The **Time Entry** grid date picker does not recognize a user's regional settings.</span></span>

<span data-ttu-id="2de29-117">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="2de29-117">**Resource Management**</span></span>

<span data-ttu-id="2de29-118">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2de29-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="2de29-119">في الوضع اليدوي، لا يتم التعرف على التغييرات التي تم إجراؤها على مخططات **تعيين الموارد** عند إنشاء **متطلبات الموارد**.</span><span class="sxs-lookup"><span data-stu-id="2de29-119">In manual mode, changes to **Resource Assignment** contours are not recognized when generating **Resource Requirements**.</span></span>
- <span data-ttu-id="2de29-120">لا تدعم **طلبات الموارد** حالات الطلبات المخصصة.</span><span class="sxs-lookup"><span data-stu-id="2de29-120">**Resource Requests** do not support custom request statuses.</span></span>

<span data-ttu-id="2de29-121">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="2de29-121">**Project Management**</span></span>

<span data-ttu-id="2de29-122">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2de29-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="2de29-123">لن يؤدي استخدام النقر المزدوج فوق EstimateGridControl إلى تحليل أرقام التنسيق الهولندية بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="2de29-123">Using double-click on EstimateGridControl will not correctly parse Dutch format numbers.</span></span>
- <span data-ttu-id="2de29-124">لا يتم تحديث الساعات المعينة بشكل صحيح عند تغيير التعيينات باستخدام الوظيفة الإضافية لعميل سطح مكتب Microsoft Project.</span><span class="sxs-lookup"><span data-stu-id="2de29-124">Assigned hours do not update correctly when assignments are changed using the Microsoft Project desktop client add-in.</span></span>
- <span data-ttu-id="2de29-125">تعرض شبكات تعقب المشروع وتقديراته رمز عملة مبيعات غير صحيح عندما تختلف عملة العقد عن عملة العميل ويتم تكوين المؤسسة لعرض رموز العملات بدلاً من رموز العملات.</span><span class="sxs-lookup"><span data-stu-id="2de29-125">Project Tracking and Estimates grids display incorrect sales currency code when contract currency is different than customer currency and organization is configured to display currency codes instead of currency symbols.</span></span>
- <span data-ttu-id="2de29-126">سيضيف تاريخ انتهاء عضو الفريق يومًا واحدًا إذا كان جدول ساعات العمل هو 24 ساعة في اليوم.</span><span class="sxs-lookup"><span data-stu-id="2de29-126">A Team member's finish date will add one day if the work hour schedule is 24-hours per day.</span></span>
- <span data-ttu-id="2de29-127">في جدول المشروع، لا تؤدي إضافة فئة حركة إلى مهمة إلى تشغيل الحفظ التلقائي.</span><span class="sxs-lookup"><span data-stu-id="2de29-127">On the Project Schedule, adding a Transaction Category to a task does not trigger auto save.</span></span>
- <span data-ttu-id="2de29-128">يتم عرض الخطأ التالي عند إضافة عضو فريق إلى قالب المشروع: "لا يمكن إقران متطلبات الموارد بقوالب المشروع".</span><span class="sxs-lookup"><span data-stu-id="2de29-128">The following error is displayed when adding a team member to the Project Template: "Resource requirements cannot be associated with project templates".</span></span> 
- <span data-ttu-id="2de29-129">يعرض البرنامج النصي لقاعدة الشريط "msdyn.Approval.CanApproveOrReject" خطأ انتهاء المهلة.</span><span class="sxs-lookup"><span data-stu-id="2de29-129">Ribbon rule script "msdyn.Approval.CanApproveOrReject" displays a timeout error.</span></span>

<span data-ttu-id="2de29-130">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="2de29-130">**Sales**</span></span>

<span data-ttu-id="2de29-131">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2de29-131">The following issues have been fixed:</span></span>

- <span data-ttu-id="2de29-132">لا يتم عرض رسالة خطأ التحقق من الصحة عند تحديد قائمة أسعار التكلفة في بحث قائمة الأسعار في نموذج/كيان "قائمة أسعار مشروع عرض أسعار جديد".</span><span class="sxs-lookup"><span data-stu-id="2de29-132">Validation error message not displayed when a Cost Price List is selected in Price List lookup on 'New Quote Project Price List' form/entity.</span></span>
- <span data-ttu-id="2de29-133">لا يؤدي إغلاق عرض الأسعار كمكسب إلى لانتقال إلى العقد الذي تم إنشاؤه إذا كان BPF مرفقًا لعرض الأسعار في المرحلة النهائية.</span><span class="sxs-lookup"><span data-stu-id="2de29-133">Closing the quote as won does not navigate to the created contract if a BPF attached to the quote is in the final stage.</span></span>
- <span data-ttu-id="2de29-134">يتم ربط **المبيعات غير المفوترة** المعكوسة بتكلفة أصلية عند استدعاء إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="2de29-134">Reversing **Unbilled Sales** is linked to original cost when a time entry is recalled.</span></span>
- <span data-ttu-id="2de29-135">وبعد تحديد الزر **تأكيد**، لا تتغير حالة الفاتورة إلى **مؤكدة** ما لم يتم تحديث الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="2de29-135">After selecting the **Confirm** button, the invoice status doesn't change to **Confirmed** unless the invoice is refreshed.</span></span>
