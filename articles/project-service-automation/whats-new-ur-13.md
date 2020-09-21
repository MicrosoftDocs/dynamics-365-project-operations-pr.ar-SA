---
title: ما الجديد في إصدار التحديث 13، الإصدار 3 من Project Service Automation
description: يقدم هذا الموضوع معلومات حول الجديد في إصدار التحديث 13، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: c6f6a5b6-b5bb-467c-b7c7-7fb962504c6d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5f1b6b3879c94a77ab62082aad1e470a3ba66552
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748654"
---
# <a name="project-service-automation-v3-update-release-13"></a><span data-ttu-id="80e44-103">الإصدار 3 من Project Service Automation، إصدار التحديث 13</span><span class="sxs-lookup"><span data-stu-id="80e44-103">Project Service Automation V3, Update Release 13</span></span>
<span data-ttu-id="80e44-104">يسرنا الإعلان عن آخر تحديث لتطبيق Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="80e44-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="80e44-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="80e44-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="80e44-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="80e44-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="80e44-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="80e44-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="80e44-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="80e44-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="80e44-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 13.</span><span class="sxs-lookup"><span data-stu-id="80e44-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="80e44-110">يتضمن هذا الإصدار رقم البنية V3.10.3.18 وهو متوفر وفق الجدول التالي:</span><span class="sxs-lookup"><span data-stu-id="80e44-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="80e44-111">**التوافر العام (ذاتي التحديث):** نوفمبر 2019</span><span class="sxs-lookup"><span data-stu-id="80e44-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="80e44-112">**تحديث تلقائي:** ديسمبر 2019</span><span class="sxs-lookup"><span data-stu-id="80e44-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="80e44-113">إصدار التحديث 13</span><span class="sxs-lookup"><span data-stu-id="80e44-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="80e44-114">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="80e44-114">Bug fixes</span></span>

- <span data-ttu-id="80e44-115">الوقت والمصروفات</span><span class="sxs-lookup"><span data-stu-id="80e44-115">Time and Expense</span></span>

     - <span data-ttu-id="80e44-116">إصلاح: لا تعمل وظيفة البحث في صفحة **الموافقة على المصروفات** عند البحث حسب غرض المصروفات.</span><span class="sxs-lookup"><span data-stu-id="80e44-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="80e44-117">إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="80e44-117">Resource Management</span></span>

     - <span data-ttu-id="80e44-118">إصلاح: تم تحديث الأرقام الموجودة في التسوية ليتم ضبطها إلى اليمين.</span><span class="sxs-lookup"><span data-stu-id="80e44-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="80e44-119">إصلاح: لا يمكن تعيين الموارد المسامة إلى المهام من خلال علامة تبويب **الجدول**.</span><span class="sxs-lookup"><span data-stu-id="80e44-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="80e44-120">إدارة المشروع</span><span class="sxs-lookup"><span data-stu-id="80e44-120">Project Management</span></span>

     - <span data-ttu-id="80e44-121">إصلاح: استثناء مرجع فارغ عند تعيين عضو الفريق عندما يفتقد **TransactionType** معلومات الإعداد لكل من **الوحدة** و**DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="80e44-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="80e44-122">‏‏Sales</span><span class="sxs-lookup"><span data-stu-id="80e44-122">Sales</span></span>

     - <span data-ttu-id="80e44-123">إصلاح: سجلات نوع الحركة المكررة ترجع خطأ عند إنشاء سجلات أسعار الأدوار.</span><span class="sxs-lookup"><span data-stu-id="80e44-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="80e44-124">إصلاح: تظهر أزرار إضافية لكل من **فرصة جديدة** و**عرض أسعار** و**بند الأمر‬** و**إضافة منتج** في الأوامر الخاصة بالفرص وعروض الاسعار ومنتجات الأوامر والشبكة الفرعية للبنود المستندة إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="80e44-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines sub-grid.</span></span>


