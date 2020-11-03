---
title: تكوين إعدادات معلمات إضافية
description: كيفية تكوين إعدادات معلمات إضافية في Project Service
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
ms.openlocfilehash: 24a4fe83471da916fb91cfe20e739279c08d8e5e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070644"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="4bddc-103">تكوين إعدادات معلمات إضافية (Project Service)</span><span class="sxs-lookup"><span data-stu-id="4bddc-103">Configure additional parameter settings (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="4bddc-104">بعد تكوين العناصر في المواضيع السابقة، أنت بحاجة لتعيين معلمات إضافية للمشروع لاستخدامها في مشاريعك.</span><span class="sxs-lookup"><span data-stu-id="4bddc-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="4bddc-105">عندما قمت في بادئ الأمر بتثبيت [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، أنشأت إعداد معلمات لإنشاء أولاً كافة السجلات المطلوبة لكي يعمل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="4bddc-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="4bddc-106">والآن حان وقت الرجوع وتكوين حقول إضافية لهذه الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="4bddc-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="4bddc-107">سوف تحتاج إلى تكوين الإعدادات التالية:</span><span class="sxs-lookup"><span data-stu-id="4bddc-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="4bddc-108">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="4bddc-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="4bddc-109">تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="4bddc-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="4bddc-110">قالب ساعات العمل</span><span class="sxs-lookup"><span data-stu-id="4bddc-110">Work hours template</span></span>  
  
-   <span data-ttu-id="4bddc-111">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="4bddc-111">Price list</span></span>  
 
<span data-ttu-id="4bddc-112">في هذه الخطوة، ستشير أيضًا إلى نوع تخصيص الموارد المطلوب:</span><span class="sxs-lookup"><span data-stu-id="4bddc-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="4bddc-113">**مركزي**.</span><span class="sxs-lookup"><span data-stu-id="4bddc-113">**Central**.</span></span> <span data-ttu-id="4bddc-114">بإمكان مديري الموارد فقط تخصيص الموارد للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="4bddc-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="4bddc-115">**مختلط**.</span><span class="sxs-lookup"><span data-stu-id="4bddc-115">**Hybrid**.</span></span> <span data-ttu-id="4bddc-116">بإمكان مديري الموارد ومديري المشاريع ومديري الحسابات تخصيص الموارد للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="4bddc-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="4bddc-117">لتعيين معلمات المشروع:</span><span class="sxs-lookup"><span data-stu-id="4bddc-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="4bddc-118">انتقل إلى **Project Service > المعلمات‬**.</span><span class="sxs-lookup"><span data-stu-id="4bddc-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="4bddc-119">انقر فوق إعداد المعلمات الذي تريد تكوينه (الإعداد الذي قمت بإنشائه عند تثبيت [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للمرة الأولى)، أو انقر فوق **جديد** لإنشاء إعداد جديد.</span><span class="sxs-lookup"><span data-stu-id="4bddc-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="4bddc-120">في الناحية **عام** ، يمكنك تعيين كافة الخيارات الخاصة بمعلمات المشروع.</span><span class="sxs-lookup"><span data-stu-id="4bddc-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="4bddc-121">في الناحية **قائمة الأسعار** ، انقر فوق **+** لإضافة قائمة أسعار، وحدد قائمة أسعار في القائمة المنسدلة **قائمة أسعار معلمات المشروع** ، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="4bddc-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="4bddc-122">انقر فوق الزر **حفظ** في الزاوية السفلية اليسرى من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="4bddc-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="4bddc-123">يجب المحافظة على سجل معلمة المشروع كي يعمل Project Service بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="4bddc-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="4bddc-124">لا ينبغي حذف هذا السجل.</span><span class="sxs-lookup"><span data-stu-id="4bddc-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="4bddc-125">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="4bddc-125">See Also</span></span>  
 [<span data-ttu-id="4bddc-126">إعداد الموارد</span><span class="sxs-lookup"><span data-stu-id="4bddc-126">Set up resources</span></span>](../psa/set-up-resources.md)
