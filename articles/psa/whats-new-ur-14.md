---
title: الجديد أو المتغير في إصدار التحديث 14، الإصدار 3 من Project Service Automation
description: يقدم هذا الموضوع معلومات حول الجديد في إصدار التحديث 14، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
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
ms.openlocfilehash: 00ce5c68b1141c88671f0534f7500bf0d7eebd8e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070602"
---
# <a name="project-service-automation-update-release-14-v3"></a><span data-ttu-id="19962-103">الإصدار 3 من Project Service Automation، إصدار التحديث 14</span><span class="sxs-lookup"><span data-stu-id="19962-103">Project Service Automation Update Release 14, V3</span></span>
<span data-ttu-id="19962-104">يسرنا الإعلان عن آخر تحديث لتطبيق Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="19962-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="19962-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="19962-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="19962-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="19962-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="19962-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="19962-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="19962-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="19962-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="19962-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في PSA V3، إصدار التحديث 14.</span><span class="sxs-lookup"><span data-stu-id="19962-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="19962-110">يتضمن هذا الإصدار رقم البنية V3.10.4.21 وهو متوفر وفق الجدول التالي:</span><span class="sxs-lookup"><span data-stu-id="19962-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="19962-111">**التوافر العام (ذاتي التحديث):** يناير 2020</span><span class="sxs-lookup"><span data-stu-id="19962-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="19962-112">**تحديث تلقائي:** فبراير 2020</span><span class="sxs-lookup"><span data-stu-id="19962-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="19962-113">إصدار التحديث 14</span><span class="sxs-lookup"><span data-stu-id="19962-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="19962-114">التحسينات</span><span class="sxs-lookup"><span data-stu-id="19962-114">Enhancements</span></span>

- <span data-ttu-id="19962-115">‏‏Sales</span><span class="sxs-lookup"><span data-stu-id="19962-115">Sales</span></span>

     - <span data-ttu-id="19962-116">يتم نسخ قيم الحقول المخصصة من **تفاصيل بند عرض الأسعار‬‬** إلى **تفاصيل بنود عقد المشروع‬** عند تحديث عرض أسعار إلى **إغلاق كمكتسب**.</span><span class="sxs-lookup"><span data-stu-id="19962-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="19962-117">المشاريع المؤكدة يمكن **إغلاقها كخاسرة**.</span><span class="sxs-lookup"><span data-stu-id="19962-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="19962-118">إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="19962-118">Resource Management</span></span>

     - <span data-ttu-id="19962-119">عند تمديد الحجوزات، ستتم مطالبة المستخدمين بواسطة مربع حوار تأكيد لتلخيص نتائج الحجز وتوفير ارتباط إلى "المحافظة على الحجوزات‬".</span><span class="sxs-lookup"><span data-stu-id="19962-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="19962-120">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="19962-120">Bug fixes</span></span>

- <span data-ttu-id="19962-121">الوقت والمصروفات</span><span class="sxs-lookup"><span data-stu-id="19962-121">Time and Expense</span></span>

     - <span data-ttu-id="19962-122">إصلاح: تم تحسين تجربة المستخدم عندما لم يحدد المستخدم أي إدخالات لتصحيحها.</span><span class="sxs-lookup"><span data-stu-id="19962-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="19962-123">إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="19962-123">Resource Management</span></span>

     - <span data-ttu-id="19962-124">إصلاح: يؤدي حجز مورد عدة مرات إلى تجاوز اسم المورد القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="19962-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="19962-125">‏‏Sales</span><span class="sxs-lookup"><span data-stu-id="19962-125">Sales</span></span>

     - <span data-ttu-id="19962-126">إصلاح: لا يتم حساب إجمالي سعر المبيعات حتى يقوم المستخدم أيضًا بإدخال سعر التكلفة لتقديرات المصروفات في المشروع.</span><span class="sxs-lookup"><span data-stu-id="19962-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="19962-127">ثابت: يفشل إغلاق عرض أسعار على أنه **فائز** إذا لم يكن عقد المشروع المقترن به في حالة **المسودة**.</span><span class="sxs-lookup"><span data-stu-id="19962-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>

