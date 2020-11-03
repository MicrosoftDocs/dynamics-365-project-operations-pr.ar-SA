---
title: جدولة موارد لمشروع
description: كيفية جدولة الموارد لمشروع في Project Service
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: db69348aac96cbfaaa865228c9230cbda4b1e784
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070850"
---
# <a name="schedule-resources-for-a-project-project-service"></a><span data-ttu-id="67210-103">جدولة الموارد لمشروع (Project Service)</span><span class="sxs-lookup"><span data-stu-id="67210-103">Schedule resources for a project (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="67210-104">يمكنك التحقق من توفر الموارد للحصول على نظرة عامة حول مواردك المحجوزة، أو يمكنك تصفية طريقة العرض حسب المهارات والفريق الموقع وخيارات أخرى.</span><span class="sxs-lookup"><span data-stu-id="67210-104">You can check resource availability to get an overall view of how booked your resources are, or you can filter the view by skills, team, location, and other options.</span></span>  
  
<span data-ttu-id="67210-105">تعرض لوحة الجدولة قائمة الموارد ومدى توافرها.</span><span class="sxs-lookup"><span data-stu-id="67210-105">The schedule board shows list of resources and their availability.</span></span> <span data-ttu-id="67210-106">حدد وضع طريقة عرض لإظهار التوفر حسب **الساعات** أو **اليوم** أو **الأسبوع** أو **الشهر**.</span><span class="sxs-lookup"><span data-stu-id="67210-106">Select a view mode to show availability by **Hours** , **Day** , **Week** , or **Month**.</span></span>  
  
<span data-ttu-id="67210-107">قبل استخدام لوحة الجدولة، من الضروري إعدادها.</span><span class="sxs-lookup"><span data-stu-id="67210-107">Before you use the schedule board, it’s important to set it up.</span></span> <span data-ttu-id="67210-108">لمزيد من المعلومات، راجع [تكوين لوحة الجدولة (Field Service أو Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span><span class="sxs-lookup"><span data-stu-id="67210-108">For more information, see [Configure the schedule board (Field Service or Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span></span>
  
<span data-ttu-id="67210-109">إذا كنت تستخدم إصدارًا أقدم، وللاطلاع على توفر الموارد، راجع [عرض توفر الموارد](../psa/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="67210-109">If you are using an older version, for resource availability, see [View resource availability](../psa/view-resource-availability.md).</span></span>  

> [!IMPORTANT]
>  <span data-ttu-id="67210-110">لاستخدام وظيفة الحجز على لوحة الجدولة وخدمات الترميز الجغرافي والموقع، تحتاج إلى تشغيل الخرائط.</span><span class="sxs-lookup"><span data-stu-id="67210-110">To use the schedule board booking functionality, geocoding, and location services, you need to turn on maps.</span></span>  
> 
> 1. <span data-ttu-id="67210-111">من القائمة الرئيسية، حدد **جدولة الموارد** > **الإدارة**.</span><span class="sxs-lookup"><span data-stu-id="67210-111">On the main menu, select **Resource Scheduling** > **Administration**.</span></span>  
> 2. <span data-ttu-id="67210-112">انقر فوق **معلمات الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="67210-112">Click **Scheduling parameters**.</span></span>  
> 3. <span data-ttu-id="67210-113">افتح سجل وقم بالتمرير لأسفل إلى قسم **Resource Scheduling Optimization**.</span><span class="sxs-lookup"><span data-stu-id="67210-113">Open record and scroll down to the **Resource Scheduling Optimization** section.</span></span>  
> 4. <span data-ttu-id="67210-114">في حقل **الاتصال بالخرائط** ، اختر **نعم**.</span><span class="sxs-lookup"><span data-stu-id="67210-114">On the **Connect to Maps** field, choose **Yes**.</span></span>  
> 5. <span data-ttu-id="67210-115">وافق على الشروط واحفظ السجل.</span><span class="sxs-lookup"><span data-stu-id="67210-115">Accept terms and save the record.</span></span>  
> 6. <span data-ttu-id="67210-116">من القائمة الرئيسية، حدد **Project Service** > **لوحة الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="67210-116">On the main menu, select **Project Service** > **Schedule board**.</span></span> <span data-ttu-id="67210-117">من هنا، توجد عدة طرق لجدولة متطلبات الحجز يدويًا.</span><span class="sxs-lookup"><span data-stu-id="67210-117">From here, there are several ways to manually schedule a booking requirement.</span></span> <span data-ttu-id="67210-118">اختر الطريقة التي تناسبك.</span><span class="sxs-lookup"><span data-stu-id="67210-118">Choose the method that works for you.</span></span>
  
## <a name="find-available-resources"></a><span data-ttu-id="67210-119">بحث عن الموارد المتوفرة</span><span class="sxs-lookup"><span data-stu-id="67210-119">Find available resources</span></span>

1.  <span data-ttu-id="67210-120">من قائمة **متطلبات الحجز** ، انقر بزر الماوس الأيمن فوق حجز غير مجدول، واختر واحدًا مما يلي:</span><span class="sxs-lookup"><span data-stu-id="67210-120">From the **Booking Requirement** list, right-click an unscheduled booking and choose one of the following:</span></span>  
  
- <span data-ttu-id="67210-121">اختر **بحث عن التوافر - الموارد الحالية‬** للبحث عن مورد متوفر من القائمة على لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="67210-121">Choose **Find availability - Current Resources** to find an available resource from the list on the schedule board.</span></span>  
- <span data-ttu-id="67210-122">اختر **‏‫بحث عن التوافر - جميع الموارد‬** ، للبحث عن مورد متوفر من الموارد في النظام</span><span class="sxs-lookup"><span data-stu-id="67210-122">Choose **Find availability - All Resources** , to find an available resource from resources in the system</span></span>  
   > [!NOTE]
   >  <span data-ttu-id="67210-123">عند القيام بذلك، سوف تظهر عوامل التصفية الخيارات الخاصة بمتطلبات الحجز المحدد.</span><span class="sxs-lookup"><span data-stu-id="67210-123">When you do this, the filters will show options for the selected booking requirement.</span></span>  
  
2. <span data-ttu-id="67210-124">عندما تشاهد الجزء الزمني المتوفر، انقر بزر الماوس الأيمن فوق الجزء الزمني على لوحة الجدولة واختر **احجز هنا**.</span><span class="sxs-lookup"><span data-stu-id="67210-124">When you see an available slot, right-click the time slot on the schedule board and choose **Book Here**.</span></span> <span data-ttu-id="67210-125">أو، اعمل على سحب وإفلات متطلبات الحجز في الجزء الزمني المتاح.</span><span class="sxs-lookup"><span data-stu-id="67210-125">Or, drag and drop the booking requirement to the available time slot.</span></span>  
  

## <a name="book-a-resource-using-the-daily-view-and-find-whos-under-booked"></a><span data-ttu-id="67210-126">حجز مورد باستخدام طريقة العرض اليومية والبحث عن مورد غير محجوز بشكل كافٍ</span><span class="sxs-lookup"><span data-stu-id="67210-126">Book a resource using the daily view and find who’s under-booked</span></span>
  
1.  <span data-ttu-id="67210-127">في لوحة الجدولة، حدد **وضع العرض** وحدد **أيام**.</span><span class="sxs-lookup"><span data-stu-id="67210-127">On the schedule board, select **View Mode** and select **Days**.</span></span>  
  
    <span data-ttu-id="67210-128">يؤدي ذلك إلى إظهار طريقة عرض الشبكة حيث يظهر عدد الساعات التي تم فيها حجز مورد في اليوم والأيام التي يكون فيها هذا المورد غير محجوز.</span><span class="sxs-lookup"><span data-stu-id="67210-128">This shows a grid view of how many hours a resource is booked per day and which days they are free.</span></span>  
  
2.  <span data-ttu-id="67210-129">انقر فوق اسم المورد الذي تريد حجزه، ثم حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="67210-129">Click the name of the resource you want to book, and then select **Book**.</span></span>  
  
3.  <span data-ttu-id="67210-130">في مربع الحوار **حجز المورد (إنشاء)** ، اختر المشروع الذي تريد حجز المورد له إلى جانب أسلوب الحجز وأوقات البدء والانتهاء.</span><span class="sxs-lookup"><span data-stu-id="67210-130">On the **Resource booking (create)** dialog box, choose the project that you want to book the resource for along with booking method and start and end times.</span></span>  
  
4.  <span data-ttu-id="67210-131">عند الانتهاء، حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="67210-131">When you’re done, select **Book**.</span></span>  
  
## <a name="view-to-the-schedule-board"></a><span data-ttu-id="67210-132">عرض لوحة الجدولة</span><span class="sxs-lookup"><span data-stu-id="67210-132">View to the schedule board</span></span>
  
1.  <span data-ttu-id="67210-133">اسحب متطلبات حجز غير مجدول من القائمة في الأسفل.</span><span class="sxs-lookup"><span data-stu-id="67210-133">Select an unscheduled booking requirement from the list at the bottom.</span></span>  
  
2.  <span data-ttu-id="67210-134">اسحب متطلبا الحجز إلى مورد/جزء زمني متوفر على لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="67210-134">Drag the booking requirement to an available resource/time slot on the schedule board.</span></span>  
  
3.  <span data-ttu-id="67210-135">عند الانتهاء، حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="67210-135">When you're done, select **Book**.</span></span>  
  
### <a name="additional-resources"></a><span data-ttu-id="67210-136">الموارد الإضافية</span><span class="sxs-lookup"><span data-stu-id="67210-136">Additional resources</span></span>  
 [<span data-ttu-id="67210-137">دليل إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="67210-137">Resource manager guide</span></span>](../psa/resource-manager-guide.md)
