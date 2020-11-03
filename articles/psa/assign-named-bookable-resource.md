---
title: حجز موارد مسماة قابل للحجز إلى فريق مشروع وتعيين المهام
description: يوفر هذا الموضوع معلومات حول كيفية حجز موارد مسماة لفرق المشروع وتعيين مهام لها.
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 11/28/2018
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
ms.openlocfilehash: defc92e701ae6baf9d54f41dca123a09ef834c35
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070763"
---
# <a name="book-named-bookable-resources-to-a-project-team-and-assign-tasks"></a><span data-ttu-id="3041d-103">حجز موارد مسماة قابل للحجز إلى فريق مشروع وتعيين المهام</span><span class="sxs-lookup"><span data-stu-id="3041d-103">Book named bookable resources to a project team and assign tasks</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3041d-104">يمكنك إضافة مورد مسمى إلى فريق المشروع الخاص بك عن طريق حجزه مباشرة إلى الفريق.</span><span class="sxs-lookup"><span data-stu-id="3041d-104">You can  add a named resource to your project team by booking them directly onto the team.</span></span> <span data-ttu-id="3041d-105">للقيام بهذا، استكمل هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="3041d-105">To do this, complete the following steps.</span></span>

1. <span data-ttu-id="3041d-106">في Project Service Automation، اذهب إلى **المشروعات** , وحدد فتح المشروع الذي تريد الحجز له.</span><span class="sxs-lookup"><span data-stu-id="3041d-106">In  Project Service Automation, go to **Projects** , and select the open the project that you are booking for.</span></span>
2. <span data-ttu-id="3041d-107">في صفحة **المشروع** ، في علامة تبويب **الفريق** ، انقر فوق **جديد**.</span><span class="sxs-lookup"><span data-stu-id="3041d-107">On the **Project** page, on the **Team** tab, click **New**.</span></span> 

![إضافة عضو فريق من علامة التبويب "فريق"](media/RM-how-to-1.png)

3. <span data-ttu-id="3041d-109">في مربع الحوار **الإنشاء السريع لفريق المشروع** ، حدد المورد القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="3041d-109">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="3041d-110">سيتم ملء حقل **الدور** بالدور الافتراضي للمورد إذا كان لديه واحد معين.</span><span class="sxs-lookup"><span data-stu-id="3041d-110">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="3041d-111">ويمكنك تغيير الدور كلما دعت الحاجة.</span><span class="sxs-lookup"><span data-stu-id="3041d-111">You can change the role if needed.</span></span> 
4. <span data-ttu-id="3041d-112">حدد تاريخي البدء والانتهاء الذي سيكون مطلوبا للمورد وحدد طريقة التوزيع لقدرة المورد.</span><span class="sxs-lookup"><span data-stu-id="3041d-112">Select the from and to dates that the resource will be needed and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="3041d-113">إذا كنت ترغب في أن يكون عضو الفريق هو مانح الموافقة للمشروع ، فحدد **نعم** في الحقل **الموافق على المشروع**.</span><span class="sxs-lookup"><span data-stu-id="3041d-113">If you want the team member to be a project approver, select **Yes** in the **Project Approver** field.</span></span> <span data-ttu-id="3041d-114">سيعني ذلك أنه يمكن لعضو الفريق اعتماد الوقت المرسل وإدخالات المصروفات لهذا المشروع.</span><span class="sxs-lookup"><span data-stu-id="3041d-114">This will mean that the team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="3041d-115">انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="3041d-115">Click **Save**.</span></span>

![إضافة عضو فريق في نموذج الإنشاء السريع](media/RM-how-to-2.png)


<span data-ttu-id="3041d-117">يمكنك الآن تعيين مورد محجوز إلى المهام في المشروع.</span><span class="sxs-lookup"><span data-stu-id="3041d-117">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="3041d-118">في صفحة **المشروع** ، انقر فوق علامة التبويب **جدولة** لتعيين المهام إلى المورد الجديد.</span><span class="sxs-lookup"><span data-stu-id="3041d-118">On the **Project** page, click the **Schedule** tab to assign tasks to the new resource.</span></span> <span data-ttu-id="3041d-119">منتقي الموارد الذي يتم تشغيله من حقل **الموارد** في شبكة المهمام سيُظهر أعضاء الفريق الذي يمكنك تحديده.</span><span class="sxs-lookup"><span data-stu-id="3041d-119">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>

![تعيين عضو فريق لمهمة في علامة التبويب جدولة](media/RM-how-to-3.png)

<span data-ttu-id="3041d-121">في الإصدار 3 من Project Service Automation (PSA)، لا تكون حجوزات الموارد وتعيينات المهمة مقترنة بشكل محكم.</span><span class="sxs-lookup"><span data-stu-id="3041d-121">In version 3 for Project Service Automation (PSA), resource bookings and task assignments are not tightly coupled.</span></span> <span data-ttu-id="3041d-122">وهذا يعني أنه عند استخدام منتقي الموارد في الجدول، يمكنك تعيين مهام إلى أعضاء الفريق لمزيد من الساعات التي تزيد عن تغطية الحجوزات في المشروع.</span><span class="sxs-lookup"><span data-stu-id="3041d-122">This means that when you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>
<span data-ttu-id="3041d-123">يمكنك الاطلاع على الاختلافات بين حجوزات عضو الفريق والتعيينات في علامة التبويب **الفريق** أو في علامة تبويب **تسويه الموارد**. يمكنك أيضا تسوية الاختلافات بين عمليات الحجز والتعيينات للموارد بمستوى أكثر تفصيلا.</span><span class="sxs-lookup"><span data-stu-id="3041d-123">You can see the differences between team member bookings and assignments on the **Team** tab or on the **Resource Reconciliation** tab. You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

![علامة تبويب تسوية الموارد](media/RM-how-to-4.png)

<span data-ttu-id="3041d-125">يمكنك أيضا استخدام منتقي المورد في علامة التبويب **جدولة** للبحث عن موارد قابلة للحجز وتحديدها والتي لم تكن جزءا من فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="3041d-125">You can also use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="3041d-126">تظهر هذه المهام في منتقي الموارد على أنها **موارد أخرى**.</span><span class="sxs-lookup"><span data-stu-id="3041d-126">These are shown in the resource picker as **Other Resources**.</span></span>

![تعيين مورد عضو من خارج الفريق لمهمة](media/RM-how-to-5.png)

<span data-ttu-id="3041d-128">عند القيام بذلك، تتم إضافة المورد إلى فريق المشروع وتعيينه للمهمة، ولكن لا يتم إنشاء أيه حجوزات.</span><span class="sxs-lookup"><span data-stu-id="3041d-128">When you do this, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

![عضو الفريق مع التعيينات وبدون حجوزات](media/RM-how-to-6.png)

<span data-ttu-id="3041d-130">يمكنك استخدام إمكانية الحجز الموسع في علامة تبويب **التسوية** أو **لوحة الجدولة** لحجز قدرة المورد إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="3041d-130">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

![توسيع الحجوزات لعضو فريق في علامة التبويب تسوية الموارد](media/RM-how-to-7.png)

<span data-ttu-id="3041d-132">بعد حجز عضو الفريق في المشروع، يمكنك استخدام "الاحتفاظ بالحجوزات" أو استخدام لوحة الجدولة مباشره إدارة حجوزاتهم.</span><span class="sxs-lookup"><span data-stu-id="3041d-132">After a team member is booked on your project, you can use maintain bookings or use the Schedule Board directly to manage their bookings.</span></span>
