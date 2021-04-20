---
title: الجديد أو المتغير في إصدار التحديث 30، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 30، الإصدار 3 من Project Service Automation‬.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 1169ee13c42e982cb30a40d92df660f8933786a9
ms.sourcegitcommit: b4a05c7d5512d60abdb0d05bedd390e288e8adc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/02/2021
ms.locfileid: "5852823"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a><span data-ttu-id="c25a2-103">الجديد أو المتغير في إصدار التحديث 30، الإصدار 3 من Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="c25a2-103">What's new or changed in Project Service Automation Update Release 30, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="c25a2-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c25a2-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="c25a2-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="c25a2-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="c25a2-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="c25a2-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="c25a2-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="c25a2-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="c25a2-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="c25a2-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="c25a2-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في إصدار التحديث 30، الإصدار 3 من Project Service Automation‬.</span><span class="sxs-lookup"><span data-stu-id="c25a2-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 30.</span></span> <span data-ttu-id="c25a2-110">لدى هذا الإصدار رقم البنية V3.10.51.61 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر أبريل 2021.</span><span class="sxs-lookup"><span data-stu-id="c25a2-110">This version has a build number of V3.10.51.61 and is generally available through a self-update in April 2021.</span></span>

## <a name="update-release-30"></a><span data-ttu-id="c25a2-111">إصدار التحديث 30</span><span class="sxs-lookup"><span data-stu-id="c25a2-111">Update Release 30</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="c25a2-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="c25a2-112">Bug fixes</span></span>

<span data-ttu-id="c25a2-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="c25a2-113">**Time and Expense**</span></span>

<span data-ttu-id="c25a2-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="c25a2-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="c25a2-115">يحدث خطأ عند إنشاء إدخال وقت وحفظه في الصفحة **إنشاء سريع** إذا تمت إزالة حقل **الدور**.</span><span class="sxs-lookup"><span data-stu-id="c25a2-115">An error occurs when you create and save a time entry on the **Quick Create** page if the **Role** field is removed.</span></span>
- <span data-ttu-id="c25a2-116">يطبق عامل تصفية "إدخال الوقت" عامل تشغيل التصفية الخاطئ.</span><span class="sxs-lookup"><span data-stu-id="c25a2-116">The Time Entry filter applies the wrong filter operator.</span></span>
- <span data-ttu-id="c25a2-117">لا تظهر الجداول الزمنية المنسوخة بشكل تلقائي عند تحديد **نسخ الأسبوع** على عنصر تحكم إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="c25a2-117">Copied timesheets aren't automatically displayed when you select **Copy Week** on the time entry control.</span></span>

<span data-ttu-id="c25a2-118">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="c25a2-118">**Resource Management**</span></span>

<span data-ttu-id="c25a2-119">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="c25a2-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="c25a2-120">عند تمديد الحجز، تكون حالة الحجز المعينة إلى الحجز الثابت غير صحيحة.</span><span class="sxs-lookup"><span data-stu-id="c25a2-120">When you extend a booking, the booking status assigned to the hard booking is incorrect.</span></span> <span data-ttu-id="c25a2-121">يراعي تمديد الحجز حالة الحجز المعرفة على أنها **ملتزم بها** في بيانات تعريف إعداد الحجز.</span><span class="sxs-lookup"><span data-stu-id="c25a2-121">Extending a booking respects the booking status defined as **Committed** in the booking setup metadata.</span></span>
- <span data-ttu-id="c25a2-122">إذا لم يتم تحديد حالة حجز صالحة، لا تتم ترجمة رسالة الخطأ على نحو صحيح.</span><span class="sxs-lookup"><span data-stu-id="c25a2-122">When a valid booking status isn't specified, the error message is not correctly localized.</span></span>

<span data-ttu-id="c25a2-123">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="c25a2-123">**Project Management**</span></span>

<span data-ttu-id="c25a2-124">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="c25a2-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="c25a2-125">لا يمكن إنشاء المشروعات بعملة واحدة وتتضمن المهام ذات الصلة بعملة أخرى.</span><span class="sxs-lookup"><span data-stu-id="c25a2-125">Projects can't be created in one currency and include related tasks in another currency.</span></span>

<span data-ttu-id="c25a2-126">**‏المبيعات**</span><span class="sxs-lookup"><span data-stu-id="c25a2-126">**Sales**</span></span>

<span data-ttu-id="c25a2-127">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="c25a2-127">The following issues have been fixed:</span></span>

- <span data-ttu-id="c25a2-128">عند نسخ قائمة أسعار، لا يتم تحديث الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c25a2-128">When a price list is copied, prices aren't updated.</span></span>
- <span data-ttu-id="c25a2-129">يفشل إقفال عرض أسعار كفائز إغلاق إذا كان لدى تفاصيل التكلفة قيمة للأصل.</span><span class="sxs-lookup"><span data-stu-id="c25a2-129">Closing a quote as won fails when the cost detail has a value for origin.</span></span>
- <span data-ttu-id="c25a2-130">في كيان **مهمة المشروع**، أعيدت تسمية **التكلفة المقدرة** إلى **التكلفة المخططة (بالعملة الأساسية)**.</span><span class="sxs-lookup"><span data-stu-id="c25a2-130">On the **Project Task** entity, **Estimated Cost** has been renamed to **Planned Cost (Base)**.</span></span>
- <span data-ttu-id="c25a2-131">يتم إنشاء استثناء مرجعي فارغ عند إنشاء الفواتير أو حذفها.</span><span class="sxs-lookup"><span data-stu-id="c25a2-131">A null reference exception is generated when invoices are created or deleted.</span></span>
