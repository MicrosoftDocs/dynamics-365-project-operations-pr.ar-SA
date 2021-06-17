---
title: الاحتفاظ بأعضاء الفريق
description: يوفر هذا الموضوع معلومات حول حجز الموارد المسماة لفرق المشروع وتعيين مهام لها.
author: ruhercul
ms.date: 10/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 00312c5a701768e0042e7e0236477c192690ded3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998620"
---
# <a name="maintain-team-members"></a><span data-ttu-id="e4d29-103">الاحتفاظ بأعضاء الفريق</span><span class="sxs-lookup"><span data-stu-id="e4d29-103">Maintain team members</span></span>

<span data-ttu-id="e4d29-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="e4d29-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e4d29-105">يمكنك إضافة مورد مسمى إلى فريق مشروعك عن طريق حجزه مباشرة إلى الفريق.</span><span class="sxs-lookup"><span data-stu-id="e4d29-105">You can add a named resource to your project team by booking them directly to the team.</span></span>

1. <span data-ttu-id="e4d29-106">في Dynamics 365 Project Operations، انتقل إلى **المشاريع**، وحدد فتح المشروع الذي تريد إجراء الحجز له.</span><span class="sxs-lookup"><span data-stu-id="e4d29-106">In Dynamics 365 Project Operations, go to **Projects**, and select the open the project that you're booking for.</span></span>
2. <span data-ttu-id="e4d29-107">في صفحة **المشروع**، في علامة تبويب **الفريق**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e4d29-107">On the **Project** page, on the **Team** tab, select **New**.</span></span> 
3. <span data-ttu-id="e4d29-108">في مربع الحوار **الإنشاء السريع لفريق المشروع**، حدد المورد القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="e4d29-108">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="e4d29-109">سيتم ملء حقل **الدور** بالدور الافتراضي للمورد إذا كان لديه واحد معين.</span><span class="sxs-lookup"><span data-stu-id="e4d29-109">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="e4d29-110">يمكنك تغيير الدور.</span><span class="sxs-lookup"><span data-stu-id="e4d29-110">You can change the role.</span></span> 
4. <span data-ttu-id="e4d29-111">حدد تاريخي البدء والانتهاء الذي سيكون مطلوبًا للمورد، وحدد طريقة التوزيع لسعة المورد.</span><span class="sxs-lookup"><span data-stu-id="e4d29-111">Select the from and to dates that the resource will be needed, and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="e4d29-112">حدد **نعم** في الحقل **الموافق على المشروع** إذا كنت ترغب في أن يكون عضو الفريق هو مانح الموافقة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="e4d29-112">In the **Project Approver** field, select **Yes** if you want the team member to be a project approver.</span></span> <span data-ttu-id="e4d29-113">بإمكان عضو الفريق الموافقة على إدخالات الوقت المرسل وإدخالات المصروفات لهذا المشروع.</span><span class="sxs-lookup"><span data-stu-id="e4d29-113">The team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="e4d29-114">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e4d29-114">Select **Save**.</span></span>

<span data-ttu-id="e4d29-115">يمكنك الآن تعيين مورد محجوز إلى المهام في المشروع.</span><span class="sxs-lookup"><span data-stu-id="e4d29-115">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="e4d29-116">في صفحة **المشروع**، على علامة التبويب **جدولة**، يمكنك تعيين المهام إلى المورد الجديد.</span><span class="sxs-lookup"><span data-stu-id="e4d29-116">On the **Project** page, on the **Schedule** tab, assign tasks to the new resource.</span></span> <span data-ttu-id="e4d29-117">منتقي الموارد الذي يتم تشغيله من حقل **الموارد** في شبكة المهمام سيُظهر أعضاء الفريق الذي يمكنك تحديده.</span><span class="sxs-lookup"><span data-stu-id="e4d29-117">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>


<span data-ttu-id="e4d29-118">في Project Operations، لا ترتبط حجوزات الموارد وتعيينات المهام بشكل محكم.</span><span class="sxs-lookup"><span data-stu-id="e4d29-118">In Project Operations, resource bookings and task assignments aren't tightly coupled.</span></span> <span data-ttu-id="e4d29-119">عند استخدام منتقي الموارد في الجدول، يمكنك تعيين مهام إلى أعضاء الفريق لمزيد من الساعات التي تزيد عن تغطية الحجوزات في المشروع.</span><span class="sxs-lookup"><span data-stu-id="e4d29-119">When you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>

<span data-ttu-id="e4d29-120">يتم عرض الاختلافات بين حجوزات وتعيينات أعضاء الفريق في علامتي التبويب **الفريق** و **تسوية الموارد**.</span><span class="sxs-lookup"><span data-stu-id="e4d29-120">The differences between team member bookings and assignments are shown on the **Team** and **Resource Reconciliation** tabs.</span></span> <span data-ttu-id="e4d29-121">كما يمكنك تسوية الاختلافات بين حجوزات وتعيينات الموارد على مستوى أكثر تفصيلاً.</span><span class="sxs-lookup"><span data-stu-id="e4d29-121">You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

<span data-ttu-id="e4d29-122">استخدم منتقي المورد في علامة التبويب **جدولة** للبحث عن موارد قابلة للحجز ليس جزءًا من فريق المشروع وتحديدها.</span><span class="sxs-lookup"><span data-stu-id="e4d29-122">Use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="e4d29-123">تظهر هذه الموارد في منتقي الموارد على أنها **موارد أخرى**.</span><span class="sxs-lookup"><span data-stu-id="e4d29-123">These resources are shown in the resource picker as **Other Resources**.</span></span>

<span data-ttu-id="e4d29-124">عندما تجرير التحديد، يُضاف المورد إلى فريق المشروع ويتم تعيينه للمهمة، ولكن لا يتم إنشاء أيه حجوزات.</span><span class="sxs-lookup"><span data-stu-id="e4d29-124">When you make a selection, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

<span data-ttu-id="e4d29-125">يمكنك استخدام إمكانية الحجز الموسع في علامة تبويب **التسوية** أو **لوحة الجدولة** لحجز قدرة المورد إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="e4d29-125">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

<span data-ttu-id="e4d29-126">بعد حجز عضو الفريق في المشروع، يمكنك استخدام **المحافظة على الحجوزات** أو استخدام **لوحة الجدولة** مباشره لإدارة الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="e4d29-126">After a team member is booked on your project, you can use **Maintain bookings** or the **Schedule Board** directly to manage their bookings.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]