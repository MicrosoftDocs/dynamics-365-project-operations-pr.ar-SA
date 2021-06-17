---
title: تكوين إعدادات معلمات إضافية
description: كيفية تكوين إعدادات معلمات إضافية في Project Service
author: JohnPBurrows
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
ms.openlocfilehash: f4e883e71beacffb6e2b0b56967046c3f38f7d50
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001095"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="60c4d-103">تكوين إعدادات معلمات إضافية (Project Service)</span><span class="sxs-lookup"><span data-stu-id="60c4d-103">Configure additional parameter settings (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="60c4d-104">بعد تكوين العناصر في المواضيع السابقة، أنت بحاجة لتعيين معلمات إضافية للمشروع لاستخدامها في مشاريعك.</span><span class="sxs-lookup"><span data-stu-id="60c4d-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="60c4d-105">عندما قمت في بادئ الأمر بتثبيت [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، أنشأت إعداد معلمات لإنشاء أولاً كافة السجلات المطلوبة لكي يعمل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="60c4d-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="60c4d-106">والآن حان وقت الرجوع وتكوين حقول إضافية لهذه الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="60c4d-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="60c4d-107">سوف تحتاج إلى تكوين الإعدادات التالية:</span><span class="sxs-lookup"><span data-stu-id="60c4d-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="60c4d-108">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="60c4d-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="60c4d-109">تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="60c4d-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="60c4d-110">قالب ساعات العمل</span><span class="sxs-lookup"><span data-stu-id="60c4d-110">Work hours template</span></span>  
  
-   <span data-ttu-id="60c4d-111">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="60c4d-111">Price list</span></span>  
 
<span data-ttu-id="60c4d-112">في هذه الخطوة، ستشير أيضًا إلى نوع تخصيص الموارد المطلوب:</span><span class="sxs-lookup"><span data-stu-id="60c4d-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="60c4d-113">**مركزي**.</span><span class="sxs-lookup"><span data-stu-id="60c4d-113">**Central**.</span></span> <span data-ttu-id="60c4d-114">بإمكان مديري الموارد فقط تخصيص الموارد للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="60c4d-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="60c4d-115">**مختلط**.</span><span class="sxs-lookup"><span data-stu-id="60c4d-115">**Hybrid**.</span></span> <span data-ttu-id="60c4d-116">بإمكان مديري الموارد ومديري المشاريع ومديري الحسابات تخصيص الموارد للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="60c4d-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="60c4d-117">لتعيين معلمات المشروع:</span><span class="sxs-lookup"><span data-stu-id="60c4d-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="60c4d-118">انتقل إلى **Project Service > المعلمات‬**.</span><span class="sxs-lookup"><span data-stu-id="60c4d-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="60c4d-119">انقر فوق إعداد المعلمات الذي تريد تكوينه (الإعداد الذي قمت بإنشائه عند تثبيت [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للمرة الأولى)، أو انقر فوق **جديد** لإنشاء إعداد جديد.</span><span class="sxs-lookup"><span data-stu-id="60c4d-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="60c4d-120">في الناحية **عام**، يمكنك تعيين كافة الخيارات الخاصة بمعلمات المشروع.</span><span class="sxs-lookup"><span data-stu-id="60c4d-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="60c4d-121">في الناحية **قائمة الأسعار**، انقر فوق **+** لإضافة قائمة أسعار، وحدد قائمة أسعار في القائمة المنسدلة **قائمة أسعار معلمات المشروع**، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="60c4d-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="60c4d-122">انقر فوق الزر **حفظ** في الزاوية السفلية اليسرى من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="60c4d-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="60c4d-123">يجب المحافظة على سجل معلمة المشروع كي يعمل Project Service بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="60c4d-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="60c4d-124">لا ينبغي حذف هذا السجل.</span><span class="sxs-lookup"><span data-stu-id="60c4d-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="60c4d-125">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="60c4d-125">See Also</span></span>  
 [<span data-ttu-id="60c4d-126">إعداد الموارد</span><span class="sxs-lookup"><span data-stu-id="60c4d-126">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]