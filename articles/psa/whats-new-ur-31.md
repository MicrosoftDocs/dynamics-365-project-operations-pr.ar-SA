---
title: الجديد أو المتغير في إصدار التحديث 31، للإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 31، الإصدار 3 من Project Service Automation‬.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: 160187ba7b96547e85a7a4ec4bf84c86d8fd8257
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999115"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="2153f-103">الجديد أو المتغير في إصدار التحديث 31، للإصدار 3 من Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="2153f-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="2153f-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="2153f-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="2153f-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="2153f-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="2153f-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="2153f-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="2153f-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="2153f-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="2153f-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="2153f-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="2153f-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في في إصدار التحديث 31، الإصدار 3 من Project Service Automation‬.</span><span class="sxs-lookup"><span data-stu-id="2153f-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="2153f-110">لدى هذا الإصدار رقم البنية V3.10.52.77 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر مايو 2021.</span><span class="sxs-lookup"><span data-stu-id="2153f-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="2153f-111">إصدار التحديث 31</span><span class="sxs-lookup"><span data-stu-id="2153f-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="2153f-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="2153f-112">Bug fixes</span></span>

<span data-ttu-id="2153f-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="2153f-113">**Time and Expense**</span></span>

<span data-ttu-id="2153f-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2153f-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="2153f-115">كانت أزرار أوامر التحكم في إدخال الوقت في صفحة **الموارد القابلة للحجز** محيرة.</span><span class="sxs-lookup"><span data-stu-id="2153f-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="2153f-116">تم إنشاء استثناء مرجعي فارغ في **Project.SetTrackingFields** عند الموافقة على إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="2153f-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="2153f-117">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="2153f-117">**Resource Management**</span></span>

<span data-ttu-id="2153f-118">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2153f-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="2153f-119">لا يعرض  **إنشاء عضو الفريق**  بشكل صحيح إعداد بيانات تعريف إعداد الحجز لـ **حالة الحجز الملتزم بها في السجل الافتراضي‬**.</span><span class="sxs-lookup"><span data-stu-id="2153f-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="2153f-120">عند الترقية من PSA 1.X إلى 3.X، تفشل عملية الترقية في **UpgradeResourceRequirements**.</span><span class="sxs-lookup"><span data-stu-id="2153f-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="2153f-121">**‏المبيعات**</span><span class="sxs-lookup"><span data-stu-id="2153f-121">**Sales**</span></span>

<span data-ttu-id="2153f-122">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="2153f-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="2153f-123">يحول الإيراد الفعلي المبالغ إلى عملة المشروع في شبكة التعقب.</span><span class="sxs-lookup"><span data-stu-id="2153f-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="2153f-124">يكون افتراضي العملة غير واضح عند إنشاء خطوط سطور دفتر اليومية وسطور عرض الأسعار وشروط التعاقد في السيناريوهات التي تختلف فيها العملة الأساسية للمنظمة عن عملة المشروع.</span><span class="sxs-lookup"><span data-stu-id="2153f-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="2153f-125">لا يتم تصفية استعلام **التحقق من صحة دفتر يومية التصحيحات المعلقة** حسب المشروع.</span><span class="sxs-lookup"><span data-stu-id="2153f-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="2153f-126">يتم حساب المبيعات المتبقية بشكل غير صحيح على المشروع.</span><span class="sxs-lookup"><span data-stu-id="2153f-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="2153f-127">تفشل عروض الأسعار المستندة إلى جهة اتصال عند إنشائها دون قائمة أسعار.</span><span class="sxs-lookup"><span data-stu-id="2153f-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="2153f-128">لا يظهر مؤشر تقدم المعالجة الدائري عند تحديد **تأكيد الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="2153f-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="2153f-129">لا يظهر مؤشر تقدم المعالجة الدائري عند تحديد **إنشاء الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="2153f-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="2153f-130">لا يلغي إغلاق عرض الأسعار الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="2153f-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







