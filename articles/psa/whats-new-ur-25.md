---
title: الجديد أو المتغير في إصدار التحديث 25، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 25، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 30822ec64b31e110202a587dd941bdff60116712
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280427"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a><span data-ttu-id="c7c9e-103">الجديد أو المتغير في إصدار التحديث 25، الإصدار 3 من Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="c7c9e-103">What's new or changed in Project Service Automation Update Release 25, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="c7c9e-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="c7c9e-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="c7c9e-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="c7c9e-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="c7c9e-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="c7c9e-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="c7c9e-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو المتغير ة في إصدار التحديث 25، الإصدار 3 من Project Service Automation. يتضمن هذا الإصدار رقم البنية V 3.10.43.76 وهو يتوفر بشكل عام عبر تحديث ذاتي في أكتوبر 2020.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 25 This version has a build number of V 3.10.43.76 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-25"></a><span data-ttu-id="c7c9e-110">إصدار التحديث 25</span><span class="sxs-lookup"><span data-stu-id="c7c9e-110">Update Release 25</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="c7c9e-111">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="c7c9e-111">Bug fixes</span></span>

<span data-ttu-id="c7c9e-112">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="c7c9e-112">**Time and Expense**</span></span>

<span data-ttu-id="c7c9e-113">تم إصلاح المشاكل التالية:</span><span class="sxs-lookup"><span data-stu-id="c7c9e-113">The following issue has been fixed:</span></span>

- <span data-ttu-id="c7c9e-114">مخطط إدخال الوقت يعرض بيانات إضافية استنادًا إلى فاصل زمني بحجم كبير جدًا تم استرداده.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-114">Time entry chart showing additional data based on too large of an interval being retrieved.</span></span>

<span data-ttu-id="c7c9e-115">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="c7c9e-115">**Resource Management**</span></span>

<span data-ttu-id="c7c9e-116">تم إصلاح المشاكل التالية:</span><span class="sxs-lookup"><span data-stu-id="c7c9e-116">The following issue has been fixed:</span></span>

- <span data-ttu-id="c7c9e-117">تمت إضافة كود Package Deployer لتخطي استيراد تصحيح Universal Resource Scheduling في حال وجود تصحيح من إصدار أعلى.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-117">Added package deployer code to skip the Universal Resource Scheduling patch import if a higher version patch already exists.</span></span>

<span data-ttu-id="c7c9e-118">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="c7c9e-118">**Project Management**</span></span>

<span data-ttu-id="c7c9e-119">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="c7c9e-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="c7c9e-120">تصحيح اختلافات التقريب وسعر الصرف التي تؤدي إلى تكلفة مخططة غير صحيحة في شبكة تعقب المشروع.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-120">Corrected rounding and exchange rate discrepancies resulting in incorrect planned cost in the project tracking grid.</span></span>
- <span data-ttu-id="c7c9e-121">دعم القدرة على عرض شبكتين أو أكثر من شبكات التفاعل على نموذج **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-121">Support the ability to display two or more react grids on the **Project** form.</span></span>
- <span data-ttu-id="c7c9e-122">توفير التحقق من الصحة لمعالجة القدرة على تعيين مهمة قبل تاريخ انتهاء التقويم، مما يؤدي إلى تعيين مورد فاشل.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-122">Provided validation to address the ability to assign a task past the calendar end date, which results in a failed resource assignment.</span></span>
- <span data-ttu-id="c7c9e-123">معالجة محسنة للأخطاء لمعالجة استثناء القيمة الفارغة الذي ينشأ مما يلي:</span><span class="sxs-lookup"><span data-stu-id="c7c9e-123">Improved error handling to address Null Reference Exception generated from the following:</span></span>

    - <span data-ttu-id="c7c9e-124">المكون الإضافي **PreValidateProjectTeamMemberCreate‎**</span><span class="sxs-lookup"><span data-stu-id="c7c9e-124">**PreValidateProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="c7c9e-125">**PreValidateProjectTaskCreate** عند إنشاء مهمة مشروع بدون مشروع مقترن</span><span class="sxs-lookup"><span data-stu-id="c7c9e-125">**PreValidateProjectTaskCreate** when a project task is created without an associated project</span></span>
    - <span data-ttu-id="c7c9e-126">المكون الإضافي **PreProjectTeamMemberCreate‎**</span><span class="sxs-lookup"><span data-stu-id="c7c9e-126">**PreProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="c7c9e-127">المكون الإضافي **PostProjectTeamMemberDelete‎**</span><span class="sxs-lookup"><span data-stu-id="c7c9e-127">**PostProjectTeamMemberDelete** plug-in</span></span>
    - <span data-ttu-id="c7c9e-128">المكون الإضافي **PreValidateProjectTaskDelete**</span><span class="sxs-lookup"><span data-stu-id="c7c9e-128">**PreValidateProjectTaskDelete** plug-in</span></span>

<span data-ttu-id="c7c9e-129">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="c7c9e-129">**Sales**</span></span>

<span data-ttu-id="c7c9e-130">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="c7c9e-130">The following issues have been fixed:</span></span>

- <span data-ttu-id="c7c9e-131">معالجة محسنة للأخطاء لمعالجة استثناء القيمة الفارغة الذي ينشأ من **Copy Project: Estimates HelperResource Management**.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-131">Improved error handling to address Null Reference Exceptions generated from **Copy Project: Estimates HelperResource Management**.</span></span>
- <span data-ttu-id="c7c9e-132">الخيار **غير جاهز للفوترة** على **تراكم فوترة الوقت والمواد‬** لا يمسح حالة الفوترة.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-132">**Not ready to Invoice** on a **Time and Material Billing Backlog** doesn't clear the billing status.</span></span>
- <span data-ttu-id="c7c9e-133">أزرار **الأسعار** ذات التسمية المصححة على علامة تبويب **دور السعر** و **أصناف الكتالوج**.</span><span class="sxs-lookup"><span data-stu-id="c7c9e-133">Corrected mislabeled **Prices** buttons on the **Role Price** and **Catalog Items** tab.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]