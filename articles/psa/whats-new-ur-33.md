---
title: الجديد أو المتغير في تحديث Project Service Automation الإصدار 33, V3
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في تحديث Project Service Automation، الإصدار 33, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334494"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a><span data-ttu-id="851fd-103">الجديد أو المتغير في تحديث Project Service Automation الإصدار 33, V3</span><span class="sxs-lookup"><span data-stu-id="851fd-103">What's new or changed in Project Service Automation Update Release 33, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="851fd-104">يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="851fd-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="851fd-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="851fd-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="851fd-106">وهو متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="851fd-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="851fd-107">لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="851fd-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="851fd-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="851fd-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="851fd-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، تحديث الإصدار 33.</span><span class="sxs-lookup"><span data-stu-id="851fd-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 33.</span></span> <span data-ttu-id="851fd-110">يحتوي هذا الإصدار على رقم إصدار V3.10.54.98 وهو متاح بشكل عام من خلال التحديث الذاتي في يوليو 2021.</span><span class="sxs-lookup"><span data-stu-id="851fd-110">This version has a build number of V3.10.54.98 and is generally available through a self-update in July 2021.</span></span>

## <a name="update-release-33"></a><span data-ttu-id="851fd-111">إصدار التحديث 33</span><span class="sxs-lookup"><span data-stu-id="851fd-111">Update Release 33</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="851fd-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="851fd-112">Bug fixes</span></span>

<span data-ttu-id="851fd-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="851fd-113">**Time and Expense**</span></span>

<span data-ttu-id="851fd-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="851fd-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="851fd-115">يمكن تعديل حقلين مقفلين، **msdyn_description** و **msdyn_externaldescription** بعد الإرسال.</span><span class="sxs-lookup"><span data-stu-id="851fd-115">Two locked fields, **msdyn_description** and **msdyn_externaldescription** are editable after submission.</span></span>
- <span data-ttu-id="851fd-116">تظهر رسالة خطأ إذا تم إنشاء مصاريف لا تتعلق بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="851fd-116">An error message occurs if an expense is created that isn't related to a project.</span></span>
- <span data-ttu-id="851fd-117">عند إنشاء إدخال وقت، يتم تعيين دور المورد إلى دور غير نشط بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="851fd-117">When a time entry is created, the resource role defaults to an inactive role.</span></span>
- <span data-ttu-id="851fd-118">لا يتم حذف سطور دفتر اليومية المرتبطة بالمصروفات التي تم استرجاعها وحذفها.</span><span class="sxs-lookup"><span data-stu-id="851fd-118">Journal lines associated with a recalled and deleted expense aren't deleted.</span></span>
- <span data-ttu-id="851fd-119">في **نموذج الإنشاء السريع لإدخال الوقت**، قم بتحديث طريقة العرض **قائمة مهام المشروع** لتغيير التاريخ المعروض افتراضيًا إلى تاريخ بدء المهمة.</span><span class="sxs-lookup"><span data-stu-id="851fd-119">On the **Time entry Quick Create Form**, update the **Project Task List** view to change the date displayed by default to the start date of the task.</span></span>
- <span data-ttu-id="851fd-120">عند إنشاء إدخال وقت من علامة التبويب **ذات الصلة** للمورد القابل للحجز، يتم إنشاء إدخال الوقت بشكل غير صحيح للمستخدم الذي سجّل الدخول بدلاً من المورد الأصلي القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="851fd-120">When you create a time entry from the **Related** tab of the bookable resource, the time entry is incorrectly created for the signed-in user instead of the parent bookable resource.</span></span>
- <span data-ttu-id="851fd-121">تتم إضافة الحقول الجديدة إلى مربع الحوار **الموافقة المجمعة MDD**.</span><span class="sxs-lookup"><span data-stu-id="851fd-121">New fields are added to the **Bulk approval MDD** dialog box.</span></span>

<span data-ttu-id="851fd-122">**تخطيط المشروع**</span><span class="sxs-lookup"><span data-stu-id="851fd-122">**Project planning**</span></span>

<span data-ttu-id="851fd-123">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="851fd-123">The following issues have been fixed:</span></span>
- <span data-ttu-id="851fd-124">إبطاء أداء إنشاء المشروع عند تطبيق قوالب ساعات عمل المشروع مع التقويمات المعقدة.</span><span class="sxs-lookup"><span data-stu-id="851fd-124">Slow project creation performance when project work hour templates are applied with complex calendars.</span></span>
- <span data-ttu-id="851fd-125">عندما يكون تاريخ البدء أكبر من تاريخ الانتهاء، يظهر خطأ في نسخ قالب المشروع بسبب الاختلافات في مكون الوقت لكل حقل.</span><span class="sxs-lookup"><span data-stu-id="851fd-125">When the start date is greater than the end date, an error displays on the copy project template because of differences in the time component of each field.</span></span>

<span data-ttu-id="851fd-126">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="851fd-126">**Resource management**</span></span>

<span data-ttu-id="851fd-127">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="851fd-127">The following issues have been fixed:</span></span>
- <span data-ttu-id="851fd-128">يتم استخدام معلمة غير صحيحة في استعلام استخدام الموارد ويؤدي XML إلى نتائج تصفية غير صحيحة على شبكة **‏‫استخدام الموارد**.</span><span class="sxs-lookup"><span data-stu-id="851fd-128">An incorrect parameter is used in the resource utilization query and the XML leads to incorrect filter results on the **Resource Utilization** grid.</span></span>
- <span data-ttu-id="851fd-129">يعرض تأكيد **تمديد الحجوزات** تاريخ انتهاء غير صحيح للحجوزات.</span><span class="sxs-lookup"><span data-stu-id="851fd-129">The **Extend Bookings** confirmation displays incorrect end date for bookings.</span></span>

<span data-ttu-id="851fd-130">**‏المبيعات**</span><span class="sxs-lookup"><span data-stu-id="851fd-130">**Sales**</span></span>

<span data-ttu-id="851fd-131">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="851fd-131">The following issues have been fixed:</span></span>
- <span data-ttu-id="851fd-132">تظهر رسالة خطأ إذا تم إنشاء سعر فئة بقيم مفقودة.</span><span class="sxs-lookup"><span data-stu-id="851fd-132">An error message occurs if a category price is created with missing values.</span></span>
- <span data-ttu-id="851fd-133">تظهر رسالة خطأ إذا تم إنشاء حدث شروط التعاقد بدون سطر الأمر.</span><span class="sxs-lookup"><span data-stu-id="851fd-133">An error message occurs if a contract line milestone is created without an order line.</span></span>
