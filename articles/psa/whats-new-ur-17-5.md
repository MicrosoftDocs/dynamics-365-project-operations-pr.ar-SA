---
title: الجديد أو المتغير في إصدار التحديث 17.5، الإصلاح العاجل، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 17.5.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/13/2020
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
ms.openlocfilehash: b3d58cb4a2f8fea1495d143dd985ad17a5cc4130
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949258"
---
# <a name="project-service-automation-update-release-175-v3"></a><span data-ttu-id="f7ea4-103">الإصدار 3 من Project Service Automation، إصدار التحديث 17.5</span><span class="sxs-lookup"><span data-stu-id="f7ea4-103">Project Service Automation Update Release 17.5, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="f7ea4-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="f7ea4-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="f7ea4-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f7ea4-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="f7ea4-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f7ea4-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f7ea4-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها للإصدار 3، إصدار التحديث 17.5.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-109">This topic lists the features and fixes that are new or changed for V3, Update Release 17.5.</span></span> <span data-ttu-id="f7ea4-110">يتضمن هذا الإصدار رقم البنية V3.10.7.32 وهو متوفر بشكل عام من خلال تحديث ذاتي في مارس 2020.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-110">This version has a build number of V3.10.7.32 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-175"></a><span data-ttu-id="f7ea4-111">إصدار التحديث 17.5</span><span class="sxs-lookup"><span data-stu-id="f7ea4-111">Update Release 17.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="f7ea4-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="f7ea4-112">Bug fixes</span></span>


<span data-ttu-id="f7ea4-113">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="f7ea4-113">**Project Management**</span></span>

- <span data-ttu-id="f7ea4-114">تم الإصلاح: تمت معالجة مشاكل مزامنة على جانب الخادم التي تحدث عند تنفيذ مهام ذات مدة طويلة.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-114">Fixed: Addressed server-side synchronization issues that occur with long duration tasks.</span></span>
- <span data-ttu-id="f7ea4-115">تم الإصلاح: تمت معالجة قوالب ساعات العمل من 24 ساعة التي تضيف يومًا إضافيًا إلى المهام بطريقة غير دقيقة.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-115">Fixed: Addressed 24-hour work hour templates inaccurately adding an additional day to tasks.</span></span>
- <span data-ttu-id="f7ea4-116">تم الإصلاح: تمت معالجة قوالب ساعات العمل +13 GMT التي تنقل المهام بشكل غير دقيق إلى يوم يسبق اليوم المحدد.</span><span class="sxs-lookup"><span data-stu-id="f7ea4-116">Fixed: Addressed +13 GMT work hour templates inaccurately shifting tasks one day ahead.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]