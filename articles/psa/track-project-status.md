---
title: تعقب حالة مشروع
description: كيفية تعقب حالة المشروع في Project Service
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
ms.openlocfilehash: 00b6d874b42a415fe567d17e49c0ea319d8952a0
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127817"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="b4dc7-103">تعقب حالة المشروع (Project Service)</span><span class="sxs-lookup"><span data-stu-id="b4dc7-103">Track a project’s status (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="b4dc7-104">استخدم [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] لتعقب تقدم مشروع العميل.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="b4dc7-105">عندما تتقدم المشاركة، يتم تحديث مراحل المشروع لعكس مرحلة المشاركة:</span><span class="sxs-lookup"><span data-stu-id="b4dc7-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="b4dc7-106">**جديد**</span><span class="sxs-lookup"><span data-stu-id="b4dc7-106">**New**</span></span>    | <span data-ttu-id="b4dc7-107">عند إنشاء مشروع، يتم تعيين المرحلة إلى **جديد**.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="b4dc7-108">إذا قمت بإنشاء المشروع من قالب، فقد يتضمن المشروع في هذه المرحلة جدولاً وتقديرات وبيانات الفريق.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="b4dc7-109">وإلا، فقد يكون مخطط المشروع وتحتاج إلى إدخال بقية مكونات المشروع يدويًا.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="b4dc7-110">**اقتباس**</span><span class="sxs-lookup"><span data-stu-id="b4dc7-110">**Quote**</span></span>   |      <span data-ttu-id="b4dc7-111">عند ربط مشروع بعرض أسعار أو إنشائه من عرض أسعار، يتم تعيين مرحلة المشروع إلى **عرض أسعار**، ويتم أيضًا تحديث تواريخ البدء والانتهاء المقدرة.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="b4dc7-112">عندما يكون المشروع في مرحلة عرض الأسعار، تظهر تفاصيل حول عرض الأسعار على علامة التبويب **Sales** على صفحة **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="b4dc7-113">**الخطة**</span><span class="sxs-lookup"><span data-stu-id="b4dc7-113">**Plan**</span></span>   |                                     <span data-ttu-id="b4dc7-114">عندما تفوز بعرض أسعار مقترن بمشروع، وعندما تتقدم مرحلة المشاركة إلى مرحلة العقد، يتم تحديث مرحلة المشروع إلى **الخطة**.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="b4dc7-115">تظهر تفاصيل العقد على علامة التبويب **Sales** على صفحة **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="b4dc7-116">**إكمال**</span><span class="sxs-lookup"><span data-stu-id="b4dc7-116">**Complete**</span></span> |                    <span data-ttu-id="b4dc7-117">عند اكتمال العمل في المشروع، يمكنك تبديل المرحلة إلى **اكتمال**.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="b4dc7-118">عند تعيين مرحلة المشروع إلى مرحلة الاكتمال، فهذا يعني أن العمل اكتمل بنسبة 100%، ولكن المشروع يبقى مفتوحًا لتسجيل أي إدخالات وقت أو مصروفات معلقة.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="b4dc7-119">**إغلاق**</span><span class="sxs-lookup"><span data-stu-id="b4dc7-119">**Close**</span></span>   |           <span data-ttu-id="b4dc7-120">عند تسجيل كافة المعاملات في المشروع وعندما لا تتوقع تسجيل المزيد منها، يمكنك تعيين المرحلة إلى **إغلاق** يدويًا.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="b4dc7-121">عند تعيين المشروع إلى **إغلاق**، سيتعذر عليك تسجيل المزيد من المعاملات على المشروع وسوف يكون المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="b4dc7-122">لتعقب حالة مشروع</span><span class="sxs-lookup"><span data-stu-id="b4dc7-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="b4dc7-123">انتقل إلى **Project Service > المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="b4dc7-124">انقر فوق المشروع الذي تريد العمل عليه.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="b4dc7-125">في الشريط عبر الجزء العلوي من الشاشة، حدد السهم لأسفل الموجود بجوار اسم المشروع، ثم انقر فوق **تتبع المشروع**.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="b4dc7-126">حدد **تعقب الجهد‬** أو **تعقب التكلفة‬** في القائمة المنسدلة أعلى قائمة المهام.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="b4dc7-127">انقر نقرًا مزدوجًا فوق أي مهمة لتحريرها.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-127">Double-click any task to edit it.</span></span> <span data-ttu-id="b4dc7-128">يمكنك أيضًا نقل أو تغيير حجم الأشرطة في مخطط جانت لتغيير وقت المهمة والتقدم الحاصل فيها.</span><span class="sxs-lookup"><span data-stu-id="b4dc7-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="b4dc7-129">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="b4dc7-129">See Also</span></span>  
 [<span data-ttu-id="b4dc7-130">دليل مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="b4dc7-130">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
