---
title: إنشاء قالب ساعات عمل
description: كيفية إنشاء قالب ساعات العمل في Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 54d7385a2bb161c7dd02d882090790debaef3bdb
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148762"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="4b59c-103">إنشاء قالب ساعات العمل (Project Service)</span><span class="sxs-lookup"><span data-stu-id="4b59c-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="4b59c-104">قبل أن تتمكن من إنشاء جداول المشروع، ستحتاج إلى إعداد تقويم مشروع يحدد عدد ساعات العمل لاحتواء كل يوم في الجدول وأية حالات إغلاق الأعمال‬.</span><span class="sxs-lookup"><span data-stu-id="4b59c-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="4b59c-105">يمكنك القيام بذلك باستخدام قالب ساعات العمل، الذي يحتوي على تفاصيل حول ساعات العمل في اليوم وأيام الإجازات وحالات إغلاق الأعمال الأخرى.</span><span class="sxs-lookup"><span data-stu-id="4b59c-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="4b59c-106">عندما تقوم بإنشاء مشروع، يمكنك إقران قالب عمل بتقويم المشروع لتطبيق الجدول للمشروع.</span><span class="sxs-lookup"><span data-stu-id="4b59c-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="4b59c-107">هناك طريقتان لإنشاء قالب ساعات عمل:</span><span class="sxs-lookup"><span data-stu-id="4b59c-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="4b59c-108">إنشاء قالب ساعات عمل استنادًا إلى تقويم المورد.</span><span class="sxs-lookup"><span data-stu-id="4b59c-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="4b59c-109">إنشاء قالب ساعات عمل جديد.</span><span class="sxs-lookup"><span data-stu-id="4b59c-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="4b59c-110">لإنشاء قالب ساعات عمل استنادًا إلى تقويم المورد</span><span class="sxs-lookup"><span data-stu-id="4b59c-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="4b59c-111">انتقل إلى **Project Service > الموارد‬‏‎**.</span><span class="sxs-lookup"><span data-stu-id="4b59c-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="4b59c-112">حدد المورد الذي تريد إسناد ساعات عملك إليه.</span><span class="sxs-lookup"><span data-stu-id="4b59c-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="4b59c-113">انقر فوق **حفظ التقويم باسم‬**، وأدخل اسمًا لقالب ساعات العمل، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="4b59c-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="4b59c-114">عند الانتهاء من تغيير الخيارات، انقر فوق **حفظ وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="4b59c-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="4b59c-115">انقر فوق الزر **حفظ** في الركن الأيمن السفلي من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="4b59c-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="4b59c-116">لإنشاء قالب ساعات عمل جديد</span><span class="sxs-lookup"><span data-stu-id="4b59c-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="4b59c-117">انتقل إلى **Project Service > قوالب ساعات العمل‬**.</span><span class="sxs-lookup"><span data-stu-id="4b59c-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="4b59c-118">انقر فوق **جديد**.</span><span class="sxs-lookup"><span data-stu-id="4b59c-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="4b59c-119">أدخل اسمًا لقالب ساعات العمل.</span><span class="sxs-lookup"><span data-stu-id="4b59c-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="4b59c-120">حدد موردًا لإسناد ساعات العمل إليه، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="4b59c-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="4b59c-121">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="4b59c-121">See Also</span></span>  
 [<span data-ttu-id="4b59c-122">إعداد الموارد</span><span class="sxs-lookup"><span data-stu-id="4b59c-122">Set up resources</span></span>](../psa/set-up-resources.md)
