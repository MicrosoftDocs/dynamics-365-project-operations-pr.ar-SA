---
title: إنشاء مشروع
description: كيفية إنشاء مشروع في Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/13/2020
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
ms.openlocfilehash: de26bb4c3fa0ee8abf6edf5494968d1d0403266a
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4133082"
---
# <a name="create-a-project-project-service"></a><span data-ttu-id="6cd4e-103">إنشاء مشروع (Project Service)</span><span class="sxs-lookup"><span data-stu-id="6cd4e-103">Create a project (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="6cd4e-104">يمكنك إنشاء مشروع باستخدام قدرات [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] في [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] عندما تريد إنشاء فرصة أو عرض أسعار أو عقد للخدمات القائمة على مشروع.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-104">Create a project using the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] when you want to create an opportunity, quote, or contract for project-based services.</span></span> <span data-ttu-id="6cd4e-105">تساعدك قدرات [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] على إدارة مشروعك بدءًا من الفرصة وصولاً إلى الاكتمال.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-105">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities help you manage your project from opportunity through completion.</span></span> <span data-ttu-id="6cd4e-106">عند إنشاء مشروع، ستقوم أيضًا بإنشاء هيكل تنظيم العمل، الذي يؤثر على عروض الأسعار وتقديرات التكاليف وإدارة الموارد.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-106">When you create a project, you’ll also create a work breakdown structure, which affects your quotes, cost estimates, and resource management.</span></span>  
  
1.  <span data-ttu-id="6cd4e-107">انتقل إلى **Project Service > المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-107">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="6cd4e-108">انقر فوق **مشروع جديد**.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-108">Click **New Project**.</span></span>  
  
3.  <span data-ttu-id="6cd4e-109">في الناحية **ملخص**، أدخل اسمًا للمشروع وقم بتعبئة أكبر عدد ممكن من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-109">In the **Summary** area, enter a name for your project, and then fill in as many of the details as you can.</span></span> <span data-ttu-id="6cd4e-110">تظهر علامة نجمية (\*) حمراء على الحقول المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-110">Items marked with a red asterisk (\*) are required.</span></span>  
  
4.  <span data-ttu-id="6cd4e-111">انقر فوق **حفظ** لإنشاء مشروعك حتى يمكنك متابعة تحريره.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-111">Click **Save** to create your project so you can continue editing it.</span></span>  
  
<span data-ttu-id="6cd4e-112">بعد ذلك، ستقوم بإنشاء هيكل تنظيم عمل لمشروعك لتحديد المهام والتوقيت وأدوار الموارد اللازمة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-112">Next, you’ll create a work breakdown structure for your project to define the tasks, timing, and resource roles needed for the project.</span></span>  

> [!NOTE]
> <span data-ttu-id="6cd4e-113">عند الجدولة، يراعي Project Service Automation المنطقة الزمنية لقالب **ساعات العمل** المطبّق.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-113">When scheduling, Project Service Automation respects the time zone of the applied **Work Hour** template.</span></span> <span data-ttu-id="6cd4e-114">ومع ذلك، عند عرض مهام الجدولة، يظهر تاريخي بدء وانتهاء مهمة في المنطقة الزمنية للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-114">However, when viewing the schedule tasks, the start and end dates of a task will be displayed in the user's time zone.</span></span> <span data-ttu-id="6cd4e-115">ينطبق ذلك على طرق العرض الأخرى الموزعة على الوقت في نموذج **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-115">This applies to other time-phased views in the **Project** form.</span></span> <span data-ttu-id="6cd4e-116">إذا لم تتطابق المنطقة الزمنية للمستخدم مع المنطقة الزمنية لقالب ساعات العمل المطبّق على المشروع، فسيظهر تحذير يوضح الفرق.</span><span class="sxs-lookup"><span data-stu-id="6cd4e-116">If the user's time zone does not match the time zone of the work hour template applied to the project, a warning which explains the difference will occur.</span></span> 
  
### <a name="see-also"></a><span data-ttu-id="6cd4e-117">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="6cd4e-117">See Also</span></span>  
 [<span data-ttu-id="6cd4e-118">دليل مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="6cd4e-118">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
