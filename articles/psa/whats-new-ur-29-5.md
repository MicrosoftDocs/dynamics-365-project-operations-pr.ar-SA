---
title: الجديد أو المتغير في إصدار التحديث 29.5، الإصلاح العاجل، الإصدار V3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 29.5، الإصدار V3 من Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/26/2021
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
ms.openlocfilehash: d5050945c4ab7c1da61b07ec08bed20f32e166b9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999160"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-295-v3"></a><span data-ttu-id="5db5c-103">الجديد أو المتغير في إصدار التحديث 29.5، الإصدار 3 من Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5db5c-103">What's new or changed in Project Service Automation Update Release 29.5, V3</span></span>

<span data-ttu-id="5db5c-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5db5c-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="5db5c-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="5db5c-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="5db5c-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="5db5c-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="5db5c-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="5db5c-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="5db5c-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution.md).</span><span class="sxs-lookup"><span data-stu-id="5db5c-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution.md).</span></span>

<span data-ttu-id="5db5c-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في إصدار التحديث 29.5، الإصدار 3 من Project Service Automation‬.</span><span class="sxs-lookup"><span data-stu-id="5db5c-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.5.</span></span> <span data-ttu-id="5db5c-110">يتضمن هذا الإصدار رقم البنية V3.10.47.150 وهو متوفر بشكل عام من خلال تحديث ذاتي في يناير 2021.</span><span class="sxs-lookup"><span data-stu-id="5db5c-110">This version has a build number of V3.10.47.150 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-295"></a><span data-ttu-id="5db5c-111">إصدار التحديث 29.5</span><span class="sxs-lookup"><span data-stu-id="5db5c-111">Update Release 29.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="5db5c-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="5db5c-112">Bug fixes</span></span>


<span data-ttu-id="5db5c-113">**‏المبيعات**</span><span class="sxs-lookup"><span data-stu-id="5db5c-113">**Sales**</span></span>

<span data-ttu-id="5db5c-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="5db5c-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="5db5c-115">يحدث استثناء مرجع فارغ محتلم في **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** عندما تقوم بإغلاق عرض أسعار كفائز ولا يتضمن عرض الأسعار قائمة أسعار.</span><span class="sxs-lookup"><span data-stu-id="5db5c-115">A possible null reference exception occurs in **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** when you close a quote as won and the quote has no price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
