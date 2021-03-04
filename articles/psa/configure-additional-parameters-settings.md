---
title: تكوين إعدادات معلمات إضافية
description: كيفية تكوين إعدادات معلمات إضافية في Project Service
author: JohnPBurrows
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
ms.openlocfilehash: 73264845808e12950a48eea2b79e54c393d9c024
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5151552"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="60141-103">تكوين إعدادات معلمات إضافية (Project Service)</span><span class="sxs-lookup"><span data-stu-id="60141-103">Configure additional parameter settings (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="60141-104">بعد تكوين العناصر في المواضيع السابقة، أنت بحاجة لتعيين معلمات إضافية للمشروع لاستخدامها في مشاريعك.</span><span class="sxs-lookup"><span data-stu-id="60141-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="60141-105">عندما قمت في بادئ الأمر بتثبيت [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، أنشأت إعداد معلمات لإنشاء أولاً كافة السجلات المطلوبة لكي يعمل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="60141-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="60141-106">والآن حان وقت الرجوع وتكوين حقول إضافية لهذه الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="60141-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="60141-107">سوف تحتاج إلى تكوين الإعدادات التالية:</span><span class="sxs-lookup"><span data-stu-id="60141-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="60141-108">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="60141-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="60141-109">تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="60141-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="60141-110">قالب ساعات العمل</span><span class="sxs-lookup"><span data-stu-id="60141-110">Work hours template</span></span>  
  
-   <span data-ttu-id="60141-111">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="60141-111">Price list</span></span>  
 
<span data-ttu-id="60141-112">في هذه الخطوة، ستشير أيضًا إلى نوع تخصيص الموارد المطلوب:</span><span class="sxs-lookup"><span data-stu-id="60141-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="60141-113">**مركزي**.</span><span class="sxs-lookup"><span data-stu-id="60141-113">**Central**.</span></span> <span data-ttu-id="60141-114">بإمكان مديري الموارد فقط تخصيص الموارد للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="60141-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="60141-115">**مختلط**.</span><span class="sxs-lookup"><span data-stu-id="60141-115">**Hybrid**.</span></span> <span data-ttu-id="60141-116">بإمكان مديري الموارد ومديري المشاريع ومديري الحسابات تخصيص الموارد للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="60141-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="60141-117">لتعيين معلمات المشروع:</span><span class="sxs-lookup"><span data-stu-id="60141-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="60141-118">انتقل إلى **Project Service > المعلمات‬**.</span><span class="sxs-lookup"><span data-stu-id="60141-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="60141-119">انقر فوق إعداد المعلمات الذي تريد تكوينه (الإعداد الذي قمت بإنشائه عند تثبيت [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للمرة الأولى)، أو انقر فوق **جديد** لإنشاء إعداد جديد.</span><span class="sxs-lookup"><span data-stu-id="60141-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="60141-120">في الناحية **عام**، يمكنك تعيين كافة الخيارات الخاصة بمعلمات المشروع.</span><span class="sxs-lookup"><span data-stu-id="60141-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="60141-121">في الناحية **قائمة الأسعار**، انقر فوق **+** لإضافة قائمة أسعار، وحدد قائمة أسعار في القائمة المنسدلة **قائمة أسعار معلمات المشروع**، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="60141-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="60141-122">انقر فوق الزر **حفظ** في الزاوية السفلية اليسرى من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="60141-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="60141-123">يجب المحافظة على سجل معلمة المشروع كي يعمل Project Service بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="60141-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="60141-124">لا ينبغي حذف هذا السجل.</span><span class="sxs-lookup"><span data-stu-id="60141-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="60141-125">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="60141-125">See Also</span></span>  
 [<span data-ttu-id="60141-126">إعداد الموارد</span><span class="sxs-lookup"><span data-stu-id="60141-126">Set up resources</span></span>](../psa/set-up-resources.md)
