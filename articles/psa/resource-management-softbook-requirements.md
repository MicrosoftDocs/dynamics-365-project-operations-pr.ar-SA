---
title: متطلبات الحجز المبدئي
description: يوفر هذا الموضوع معلومات حول كيفية الوفاء بمتطلبات الحجز المبدئي.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: bc58c805bfe1a3087600b8d4a6be2d1bcdd18188
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997900"
---
# <a name="soft-book-requirements"></a><span data-ttu-id="d3292-103">متطلبات الحجز المبدئي</span><span class="sxs-lookup"><span data-stu-id="d3292-103">Soft-book requirements</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="d3292-104">يمكن حجز متطلب المورد بشكل ثابت.</span><span class="sxs-lookup"><span data-stu-id="d3292-104">A resource requirement can be hard-booked.</span></span> <span data-ttu-id="d3292-105">ينشئ الحجز الثابت اقتراحًا يستهلك القدرة الإنتاجية للمورد.</span><span class="sxs-lookup"><span data-stu-id="d3292-105">A hard booking creates a proposal that consumes a resource's capacity.</span></span> <span data-ttu-id="d3292-106">ثم يتم إرسال الاقتراح مرة أخرى إلى الطالب للحصول على الموافقة.</span><span class="sxs-lookup"><span data-stu-id="d3292-106">The proposal is then sent back to the requester for approval.</span></span> <span data-ttu-id="d3292-107">يضيف الحجز المبدئي موردًا بطريقة مبدئية إلى فريق مشروع وله حالة مختلفة على لوحة الجدولة، ولكنه لا يستهلك القدرة الإنتاجية للمورد.</span><span class="sxs-lookup"><span data-stu-id="d3292-107">A soft booking tentatively adds a resource to a project team and has a different status on the Schedule Board, but it doesn't consume the resource's capacity.</span></span> <span data-ttu-id="d3292-108">لحجز مورد بشكل مبدئي من لوحة الجدولة، قم بتعيين حقل **حالة الحجز** إلى **مبدئي**.</span><span class="sxs-lookup"><span data-stu-id="d3292-108">To soft-book a resource from the Schedule Board, set the **Booking Status** field to **Soft**.</span></span>

![تعيين حالة الحجز إلى مبدئي](media/Resource-Management-image77.png)

<span data-ttu-id="d3292-110">عند وجود علامة التبويب **فريق** في طريقة عرض **أعضاء الفريق المسمى**، يظهر المورد هناك.</span><span class="sxs-lookup"><span data-stu-id="d3292-110">When the **Team** tab is in the **Named Team Members** view, the resource appears there.</span></span> <span data-ttu-id="d3292-111">ويتم الإبلاغ عن الساعات الحجوزة مبدئيًا في عمود **الساعات المحجوزة مبدئيًا**.</span><span class="sxs-lookup"><span data-stu-id="d3292-111">The soft-booked hours are reported in the **Soft Booked Hours** column.</span></span>

![طريقة عرض الساعات المحجوزة مبدئيًا في أعضاء الفريق المسمى](media/Resource-Management-image78.png)

<span data-ttu-id="d3292-113">يمكن تعيين أعضاء الفريق الذين تم إجراء حجز مبدئي لهم للمهام.</span><span class="sxs-lookup"><span data-stu-id="d3292-113">Soft-booked team members can be assigned to tasks.</span></span>

![تعيين عضو فريق محجوز مبدئيًا لمهمة](media/Resource-Management-image79.png)

<span data-ttu-id="d3292-115">في علامة التبويب **التسوية**، لا يتم عرض أي حجوزات لمورد الحجز المبدئي، لأن علامة التبويب **التسوية** تراعي الحجوزات الثابتة فقط.</span><span class="sxs-lookup"><span data-stu-id="d3292-115">On the **Reconciliation** tab, no bookings are shown for a soft-book resource, because the **Reconciliation** tab considers only hard-bookings.</span></span>

![المورد المحجوز مبدئيًا دون حجوزات في علامة تبويب التسوية](media/Resource-Management-image80.png)

> [!NOTE]
> <span data-ttu-id="d3292-117">لا يمكنك حجز مورد من متطلب تم إنشاؤه من عضو فريق عام.</span><span class="sxs-lookup"><span data-stu-id="d3292-117">You can't soft-book a resource from a requirement that was generated from a generic team member.</span></span>

<span data-ttu-id="d3292-118">وفي لوحه الجدولة، يتم استخدام ألوان مختلفة لعمليات الحجز المبدئية لأحد الموارد.</span><span class="sxs-lookup"><span data-stu-id="d3292-118">On the Schedule Board, a different coloring is used for soft bookings for a resource.</span></span>

![الحجوزات المبدئية في لوحة الجدولة](media/Resource-Management-image81.png)

<span data-ttu-id="d3292-120">لتحويل الحجز المبدئي إلى حجز ثابت، في لوحة الجدولة، انقر بزر الماوس الأيمن فوق الحجز المبدئي، ثم حدد **تغيير الحالة** \>**حجز ثابت**\> **ثابت**.</span><span class="sxs-lookup"><span data-stu-id="d3292-120">To convert a soft booking to a hard booking, on the Schedule Board, right-click the soft booking, and then select **Change Status** \> **Hard Book** \> **Hard**.</span></span>

![تغيير حالة الحجز إلى "ثابت"](media/Resource-Management-image82.png)

<span data-ttu-id="d3292-122">يتم تغيير الحجز، ويتم تغيير الحالة في لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="d3292-122">The booking is changed, and the status is changed on the Schedule Board.</span></span> <span data-ttu-id="d3292-123">نظرًا لأن حالة الحجز هي **ثابت** الآن، يتم عرض المورد على أنه محجوز، ويتم قدرته الإنتاجية وتوافره.</span><span class="sxs-lookup"><span data-stu-id="d3292-123">Because the booking status is now **Hard**, the resource is shown as booked, and its capacity and availability are adjusted.</span></span>

<span data-ttu-id="d3292-124">يمكنك استخدام نفس الأسلوب لإلغاء حجز ثابت أو حجز مبدئي من لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="d3292-124">You can use the same method to cancel a hard booking or a soft booking from the Schedule Board.</span></span>

<span data-ttu-id="d3292-125">لتحويل مورد تم حجزه مبدئيًا إلى الحجز بشكل ثابت في علامة التبويب **فريق** في المشروع، حدد المورد، ثم حدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="d3292-125">To convert a resource that is soft-booked to hard-booked on the project's **Team** tab, select the resource, and then select **Confirm**.</span></span>

![تأكيد الأمر](media/Resource-Management-image83.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]