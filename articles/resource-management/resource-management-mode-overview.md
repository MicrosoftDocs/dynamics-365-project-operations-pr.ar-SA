---
title: نظرة عامة على أوضاع إدارة الموارد
description: يوفر هذا الموضوع معلومات حول وظيفة إدارة الموارد في Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 872f4f2878f474e16674932f23fe192c6a8de6eb
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279437"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="70678-103">نظرة عامة على أوضاع إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="70678-103">Resource management modes overview</span></span>

<span data-ttu-id="70678-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="70678-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="70678-105">يدعم Dynamics 365 Project Operations وضعين حتى تتمكن من تنفيذ سير مهام الحجز الإجمالي.</span><span class="sxs-lookup"><span data-stu-id="70678-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="70678-106">يتم تعريف وضع الإدارة كمعلمة مشروع ويمكن تعديلها إذا احتاج العمل الخاص بك إلى التغيير.</span><span class="sxs-lookup"><span data-stu-id="70678-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="70678-107">الوضع المركزي</span><span class="sxs-lookup"><span data-stu-id="70678-107">Central mode</span></span>
<span data-ttu-id="70678-108">بالنسبة للمؤسسات التي تقوم بالتخصيص المركزي للموارد بشأن المشاريع، يوفر الوضع المركزي طريقة لضمان أن مديري المشروع يمكنهم تعريف متطلبات الموارد على مستوى المشروع.</span><span class="sxs-lookup"><span data-stu-id="70678-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="70678-109">يتم تفويض استيفاء متطلبات الموارد إلى مدير موارد.</span><span class="sxs-lookup"><span data-stu-id="70678-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="70678-110">يمكن لمديري المشاريع قبول أو رفض الموارد المقترحة من قبل مدير الموارد.</span><span class="sxs-lookup"><span data-stu-id="70678-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![الوضع المركزي](./media/resource-management-central.png)

<span data-ttu-id="70678-112">لإدارة الموارد من خلال الوضع المركزي، راجع:</span><span class="sxs-lookup"><span data-stu-id="70678-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="70678-113">تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد</span><span class="sxs-lookup"><span data-stu-id="70678-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="70678-114">حجز موارد مسماة من متطلبات الموارد</span><span class="sxs-lookup"><span data-stu-id="70678-114">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="70678-115">إرسال طلب المورد</span><span class="sxs-lookup"><span data-stu-id="70678-115">Submit a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="70678-116">استيفاء طلب موارد</span><span class="sxs-lookup"><span data-stu-id="70678-116">Fulfill a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="70678-117">قبول مورد مشروع مقترح أو رفضه من طلب مورد</span><span class="sxs-lookup"><span data-stu-id="70678-117">Accept or reject a proposed project resource from a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="70678-118">الوضع المختلط</span><span class="sxs-lookup"><span data-stu-id="70678-118">Hybrid mode</span></span>
<span data-ttu-id="70678-119">في المؤسسات التي تتطلب مرونة في تخصيص الموارد، يقوم الوضع المختلط بتمكين مديري المشاريع ومديري الموارد من القدرة على حجز الموارد.</span><span class="sxs-lookup"><span data-stu-id="70678-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![الوضع المختلط](./media/resource-management-hybrid.png)

<span data-ttu-id="70678-121">بالإضافة إلى عملية الوضع المركزي المدعومة، راجع الموضوعات التالية لإدارة كافة تدفقات الحجز المدعومة الأخرى في الوضع المختلط:</span><span class="sxs-lookup"><span data-stu-id="70678-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="70678-122">حجز مورد مباشرة إلى مشروع:</span><span class="sxs-lookup"><span data-stu-id="70678-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="70678-123">حجز موارد مسماة قابل للحجز إلى فريق مشروع وتعيين المهام</span><span class="sxs-lookup"><span data-stu-id="70678-123">Book named bookable resources to a project team and assign tasks</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="70678-124">حجز مورد ممن متطلبات الموارد:</span><span class="sxs-lookup"><span data-stu-id="70678-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="70678-125">تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد</span><span class="sxs-lookup"><span data-stu-id="70678-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="70678-126">حجز موارد مسماة من متطلبات الموارد</span><span class="sxs-lookup"><span data-stu-id="70678-126">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]