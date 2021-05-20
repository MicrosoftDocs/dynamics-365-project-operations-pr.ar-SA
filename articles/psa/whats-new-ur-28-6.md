---
title: الجديد أو المتغير في إصدار التحديث 28.6، الإصلاح العاجل، الإصدار V3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 28.6، الإصدار V3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 9f6eba5e50f167ef96268c7c99798e248b48ff0f
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948516"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-286-v3"></a><span data-ttu-id="db8ae-103">الجديد أو المتغير في إصدار التحديث 28.6، الإصدار 3 من Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="db8ae-103">What's new or changed in Project Service Automation Update Release 28.6, V3</span></span>

<span data-ttu-id="db8ae-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="db8ae-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="db8ae-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="db8ae-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="db8ae-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="db8ae-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="db8ae-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="db8ae-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="db8ae-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="db8ae-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="db8ae-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار V3 من Project Service Automation، إصدار التحديث 28.6.</span><span class="sxs-lookup"><span data-stu-id="db8ae-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 28.6.</span></span> <span data-ttu-id="db8ae-110">يتضمن هذا الإصدار رقم البنية V3.10.46.147 وهو متوفر بشكل عام من خلال تحديث ذاتي في يناير 2021.</span><span class="sxs-lookup"><span data-stu-id="db8ae-110">This version has a build number of V3.10.46.147 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-286"></a><span data-ttu-id="db8ae-111">إصدار التحديث 28.6</span><span class="sxs-lookup"><span data-stu-id="db8ae-111">Update Release 28.6</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="db8ae-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="db8ae-112">Bug fixes</span></span>


<span data-ttu-id="db8ae-113">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="db8ae-113">**Resource Management**</span></span>

<span data-ttu-id="db8ae-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="db8ae-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="db8ae-115">عند العثور على توفر الموارد، يتم استدعاء **ExpandCalendar** لكل مورد لم يتم تطبيق قواعد التقويم عليه.</span><span class="sxs-lookup"><span data-stu-id="db8ae-115">When finding resource availability, **ExpandCalendar** is called for each resource that has no calendar rules applied.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]