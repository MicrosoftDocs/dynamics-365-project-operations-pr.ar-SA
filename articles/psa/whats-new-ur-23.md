---
title: الجديد أو المتغير في إصدار التحديث 23، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 23.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: adf893a0627ae59f2132bb46686110dafda01d3d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006450"
---
# <a name="project-service-automation-update-release-23-v3"></a><span data-ttu-id="2e884-103">الإصدار 3 من Project Service Automation، إصدار التحديث 23</span><span class="sxs-lookup"><span data-stu-id="2e884-103">Project Service Automation Update Release 23, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="2e884-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="2e884-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="2e884-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="2e884-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="2e884-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="2e884-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="2e884-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="2e884-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="2e884-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="2e884-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="2e884-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 23.</span><span class="sxs-lookup"><span data-stu-id="2e884-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 23.</span></span> <span data-ttu-id="2e884-110">يتضمن هذا الإصدار رقم البنية V 3.10.34.30 وهو متوفر بشكل عام من خلال تحديث ذاتي في أغسطس 2020.</span><span class="sxs-lookup"><span data-stu-id="2e884-110">This version has a build number of V 3.10.34.30 and is generally available through a self-update in August 2020.</span></span>

## <a name="update-release-23"></a><span data-ttu-id="2e884-111">إصدار التحديث 23</span><span class="sxs-lookup"><span data-stu-id="2e884-111">Update Release 23</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="2e884-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="2e884-112">Bug fixes</span></span>

<span data-ttu-id="2e884-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="2e884-113">**Time and Expense**</span></span>

<span data-ttu-id="2e884-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2e884-114">The following issues have been fixed:</span></span>
- <span data-ttu-id="2e884-115">معالجة الحالة الطرفية في **حذف عضو فريق المشروع** لتوفير استثناء ذي معنىً.</span><span class="sxs-lookup"><span data-stu-id="2e884-115">Handle edge case in **Project Team Member Delete** to provide a meaningful exception.</span></span>
- <span data-ttu-id="2e884-116">ينتج عن استيراد التعيين شاشة إزالة فارغة.</span><span class="sxs-lookup"><span data-stu-id="2e884-116">Assignment import results in a blank remove screen.</span></span>

<span data-ttu-id="2e884-117">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="2e884-117">**Resource Management**</span></span>

<span data-ttu-id="2e884-118">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2e884-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="2e884-119">تعرض **بطاقة مورد شبكة استخدام المورد** بيانات غير صحيحة عندما يزيد مقياس الوقت عن خمسة أيام.</span><span class="sxs-lookup"><span data-stu-id="2e884-119">The **Resource utilization grid resource card** shows incorrect data when the time scale is more than five days.</span></span>
- <span data-ttu-id="2e884-120">عندما يقوم العملاء بإنشاء مورد قابل للحجز، يفشل المكون الإضافي بشكل متقطع في إضافة المورد إلى مجموعة Microsoft Office 365 بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="2e884-120">When customers create a bookable resource, the plug-in intermittently fails to automatically add the resource to a Microsoft Office 365 group.</span></span>
- <span data-ttu-id="2e884-121">تُظهر طريقة عرض **التسوية** الحدود اليدوية بشكل غير صحيح في طريق عرض **الأسبوع** أو **الشهر**.</span><span class="sxs-lookup"><span data-stu-id="2e884-121">**Reconciliation** view displays manual contours incorrectly in the **Week** or **Month** view.</span></span>

<span data-ttu-id="2e884-122">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="2e884-122">**Project Management**</span></span>

<span data-ttu-id="2e884-123">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2e884-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="2e884-124">يتسبب عدد كبير من كيانات **RetrieveMultiple لإعدادات المستخدم** في حدوث في تراجع أداء عمليات الموافقة على المشروع والعمليات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="2e884-124">An excessive number of **RetrieveMultiple for usersettings** entities are causing degraded performance for project approvals and other operations.</span></span>
- <span data-ttu-id="2e884-125">يقتصر البحث عن مورد شبكة **تخطيط المهمة** على عرض خمسة أعضاء فقط من فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="2e884-125">The **Task Planning** grid resource lookup is limited to only show up to five team members from the project team.</span></span> 
- <span data-ttu-id="2e884-126">لا يقوم البحث عن مورد شبكة **تخطيط المهمة** بتصفية الموارد غير النشطة.</span><span class="sxs-lookup"><span data-stu-id="2e884-126">The **Task Planning** grid resource lookup does not filter inactive resources.</span></span>
- <span data-ttu-id="2e884-127">الوضع اليدوي لا يعمل كما هو متوقع في هيكل تنظيم عمل تخطيط المشروع.</span><span class="sxs-lookup"><span data-stu-id="2e884-127">Manual mode is not working as expected in the project planning work breakdown structure.</span></span>
- <span data-ttu-id="2e884-128">شبكة **تخطيط المهمة** تعرض **فئات الحركة غير النشطة**.</span><span class="sxs-lookup"><span data-stu-id="2e884-128">The **Task Planning** grid shows **Inactive Transaction Categories**.</span></span>
- <span data-ttu-id="2e884-129">يتم تقريب شبكة **تعيينات الموارد** بشكل غير صحيح عندما تحتوي مهمة على تعيينات متعددة.</span><span class="sxs-lookup"><span data-stu-id="2e884-129">The **Resource Assignment** grid rounds incorrectly when a task has multiple assignments.</span></span>
- <span data-ttu-id="2e884-130">تختلف قيم التقريب ما بين التكلفة المخططة والتكلفة الفعلية لمهمة واحدة.</span><span class="sxs-lookup"><span data-stu-id="2e884-130">Rounding values are different between planned cost and actual cost for a single task.</span></span>

<span data-ttu-id="2e884-131">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="2e884-131">**Sales**</span></span>

<span data-ttu-id="2e884-132">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2e884-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="2e884-133">يؤدي النقر المزدوج فوق **إحضار جميع فئات الحركات** إلى إنشاء أسطر متعددة.</span><span class="sxs-lookup"><span data-stu-id="2e884-133">**Fetch All Transaction Categories** double-click creates multiple lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]