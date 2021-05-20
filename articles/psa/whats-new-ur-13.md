---
title: الجديد أو المتغير في إصدار التحديث 13، الإصدار 3 من Project Service Automation
description: يقدم هذا الموضوع معلومات حول الجديد في إصدار التحديث 13، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: a4ebc2e6ca3f6be0a05a7240d762d7a8cf92d81b
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949438"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="f12b2-103">الإصدار 3 من Project Service Automation، إصدار التحديث 13</span><span class="sxs-lookup"><span data-stu-id="f12b2-103">Project Service Automation Update Release 13, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="f12b2-104">يسرنا الإعلان عن آخر تحديث لتطبيق Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="f12b2-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="f12b2-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="f12b2-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="f12b2-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f12b2-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f12b2-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="f12b2-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="f12b2-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f12b2-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f12b2-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 13.</span><span class="sxs-lookup"><span data-stu-id="f12b2-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="f12b2-110">يتضمن هذا الإصدار رقم البنية V3.10.3.18 وهو متوفر وفق الجدول التالي:</span><span class="sxs-lookup"><span data-stu-id="f12b2-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="f12b2-111">**التوافر العام (ذاتي التحديث):** نوفمبر 2019</span><span class="sxs-lookup"><span data-stu-id="f12b2-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="f12b2-112">**تحديث تلقائي:** ديسمبر 2019</span><span class="sxs-lookup"><span data-stu-id="f12b2-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="f12b2-113">إصدار التحديث 13</span><span class="sxs-lookup"><span data-stu-id="f12b2-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="f12b2-114">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="f12b2-114">Bug fixes</span></span>

- <span data-ttu-id="f12b2-115">الوقت والمصروفات</span><span class="sxs-lookup"><span data-stu-id="f12b2-115">Time and Expense</span></span>

     - <span data-ttu-id="f12b2-116">إصلاح: لا تعمل وظيفة البحث في صفحة **الموافقة على المصروفات** عند البحث حسب غرض المصروفات.</span><span class="sxs-lookup"><span data-stu-id="f12b2-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="f12b2-117">إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="f12b2-117">Resource Management</span></span>

     - <span data-ttu-id="f12b2-118">إصلاح: تم تحديث الأرقام الموجودة في التسوية ليتم ضبطها إلى اليمين.</span><span class="sxs-lookup"><span data-stu-id="f12b2-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="f12b2-119">إصلاح: لا يمكن تعيين الموارد المسامة إلى المهام من خلال علامة تبويب **الجدول**.</span><span class="sxs-lookup"><span data-stu-id="f12b2-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="f12b2-120">إدارة المشروع</span><span class="sxs-lookup"><span data-stu-id="f12b2-120">Project Management</span></span>

     - <span data-ttu-id="f12b2-121">إصلاح: استثناء مرجع فارغ عند تعيين عضو الفريق عندما يفتقد **TransactionType** معلومات الإعداد لكل من **الوحدة** و **DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="f12b2-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="f12b2-122">‏‏Sales</span><span class="sxs-lookup"><span data-stu-id="f12b2-122">Sales</span></span>

     - <span data-ttu-id="f12b2-123">إصلاح: سجلات نوع الحركة المكررة ترجع خطأ عند إنشاء سجلات أسعار الأدوار.</span><span class="sxs-lookup"><span data-stu-id="f12b2-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="f12b2-124">‏‫تم الإصلاح: الأزرار الإضافية **فرصة جديدة** و **عرض الأسعار** و **بند الأمر** و **إضافة منتج** مرئية في الأوامر في الشبكة الفرعية الفرص وعروض الأسعار ومنتجات الأوامر والبنود القائمة على المشروع.</span><span class="sxs-lookup"><span data-stu-id="f12b2-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines subgrid.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]