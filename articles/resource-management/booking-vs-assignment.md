---
title: الحجوزات في مقابل التعيينات
description: يوفر هذا الموضوع معلومات حول الاختلافات بين حجوزات الموارد وتعيينات الموارد.
author: ruhercul
manager: Annbe
ms.date: 01/08/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 9e346766e6ccbb3dff59ef12072a1cd63f1e4231
ms.sourcegitcommit: 260ce052fed760bb44c514517806049ca13a5459
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/08/2021
ms.locfileid: "4841156"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="bcfc8-103">الحجوزات في مقابل التعيينات</span><span class="sxs-lookup"><span data-stu-id="bcfc8-103">Bookings vs assignments</span></span>

<span data-ttu-id="bcfc8-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="bcfc8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bcfc8-105">الحجوزات هي تخصيص الموارد الثابت أو المبدئي لمشروع.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="bcfc8-106">تستهلك الحجوزات الثابتة سعة المورد.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="bcfc8-107">تمثل الحجوزات المفاهيم المؤسسية للفرق بحيث يمكنها أن تفهم كيفية تفاعل الموارد عبر العديد من المشاريع.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="bcfc8-108">يعتبر Dynamics 365 Project Operations الحجوزات مفهومًا على مستوى المشروع.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="bcfc8-109">بخلاف الحجوزات، التعيينات هي التزام الموارد بمهام المشروع في جدول المشروع.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="bcfc8-110">بإمكان الموارد أن تكون مسماة أو عامة.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-110">The resources can be named or generic.</span></span>  <span data-ttu-id="bcfc8-111">وعندما يُشتق متطلب مورد من تعيينات مهام المشروع، فإن Project Operations تستخدم محيط المجهود الخاص تعيين الموارد لبناء محيطات لتفاصيل متطلب المورد.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="bcfc8-112">ومع ذلك، لا يتم الاحتفاظ بمرجع إلى تعيينات الموارد.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="bcfc8-113">لا تقوم التحديثات على الحجوزات المشتقة من متطلبات المورد بتحديث أية تعيينات للمورد.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="bcfc8-114">وبشكل عام، سيكون مجموع الحجوزات لمورد مساويًا لمجموع تعيينات المورد عبر مهمة أو أكثر.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="bcfc8-115">ومع ذلك، لا يفرض Project Operations هذه الاتفاقية.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="bcfc8-116">تعرض طريقة عرض **التسوية** لمدير المشروع الأماكن حيث لا تتطابق حجوزات وتعيينات المورد.</span><span class="sxs-lookup"><span data-stu-id="bcfc8-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>


