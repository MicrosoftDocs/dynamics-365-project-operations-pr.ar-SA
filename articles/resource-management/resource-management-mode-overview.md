---
title: نظرة عامة على أوضاع إدارة الموارد
description: يوفر هذا الموضوع معلومات حول وظائف إدارة الموارد في Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4a8e605109e48b50da68abeee989f8ac8d3d659c
ms.sourcegitcommit: cf79185c8c84c55fbae55f9cfc1b17840e072b49
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/01/2020
ms.locfileid: "3930075"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="752f1-103">نظرة عامة على أوضاع إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="752f1-103">Resource management modes overview</span></span>

<span data-ttu-id="752f1-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="752f1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="752f1-105">يدعم Dynamics 365 Project Operations وضعين لكي تقوم بتنفيذ سير مهام الحجز الكلية.</span><span class="sxs-lookup"><span data-stu-id="752f1-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="752f1-106">يتم تعريف وضع الإدارة كمعلمة مشروع ويمكن تعديلها إذا احتاج العمل الخاص بك إلى التغيير.</span><span class="sxs-lookup"><span data-stu-id="752f1-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="752f1-107">الوضع المركزي</span><span class="sxs-lookup"><span data-stu-id="752f1-107">Central mode</span></span>
<span data-ttu-id="752f1-108">بالنسبة للمؤسسات التي تقوم بالتخصيص المركزي للموارد بشأن المشاريع، يوفر الوضع المركزي طريقة لضمان أن مديري المشروع يمكنهم تعريف متطلبات الموارد على مستوى المشروع.</span><span class="sxs-lookup"><span data-stu-id="752f1-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="752f1-109">يتم تفويض استيفاء متطلبات الموارد إلى مدير موارد.</span><span class="sxs-lookup"><span data-stu-id="752f1-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="752f1-110">يمكن لمديري المشاريع قبول أو رفض الموارد المقترحة من قبل مدير الموارد.</span><span class="sxs-lookup"><span data-stu-id="752f1-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![الوضع المركزي](./media/resource-management-central.png)

<span data-ttu-id="752f1-112">لإدارة الموارد من خلال الوضع المركزي، راجع:</span><span class="sxs-lookup"><span data-stu-id="752f1-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="752f1-113">تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد</span><span class="sxs-lookup"><span data-stu-id="752f1-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="752f1-114">حجز موارد مسماة من متطلبات الموارد</span><span class="sxs-lookup"><span data-stu-id="752f1-114">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="752f1-115">إرسال طلب المورد</span><span class="sxs-lookup"><span data-stu-id="752f1-115">Submit a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="752f1-116">استيفاء طلب موارد</span><span class="sxs-lookup"><span data-stu-id="752f1-116">Fulfill a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="752f1-117">قبول مورد مشروع مقترح أو رفضه من طلب مورد</span><span class="sxs-lookup"><span data-stu-id="752f1-117">Accept or reject a proposed project resource from a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="752f1-118">الوضع المختلط</span><span class="sxs-lookup"><span data-stu-id="752f1-118">Hybrid mode</span></span>
<span data-ttu-id="752f1-119">في المؤسسات التي تتطلب مرونة في تخصيص الموارد، يقوم الوضع المختلط بتمكين مديري المشاريع ومديري الموارد من القدرة على حجز الموارد.</span><span class="sxs-lookup"><span data-stu-id="752f1-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![الوضع المختلط](./media/resource-management-hybrid.png)

<span data-ttu-id="752f1-121">بالإضافة إلى عملية الوضع المركزي المدعومة، راجع الموضوعات التالية لإدارة كافة تدفقات الحجز المدعومة الأخرى في الوضع المختلط:</span><span class="sxs-lookup"><span data-stu-id="752f1-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="752f1-122">حجز مورد مباشرة إلى مشروع:</span><span class="sxs-lookup"><span data-stu-id="752f1-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="752f1-123">حجز موارد مسماة قابل للحجز إلى فريق مشروع وتعيين المهام</span><span class="sxs-lookup"><span data-stu-id="752f1-123">Book named bookable resources to a project team and assign tasks</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="752f1-124">حجز مورد ممن متطلبات الموارد:</span><span class="sxs-lookup"><span data-stu-id="752f1-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="752f1-125">تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد</span><span class="sxs-lookup"><span data-stu-id="752f1-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="752f1-126">حجز موارد مسماة من متطلبات الموارد</span><span class="sxs-lookup"><span data-stu-id="752f1-126">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
