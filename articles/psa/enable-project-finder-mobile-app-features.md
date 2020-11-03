---
title: تمكين ميزات تطبيق Project Finder Mobile
description: كيفية تمكين ميزات تطبيق Project Finder Mobile في Project Service
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
ms.openlocfilehash: 749c5682dc2e639843a0a8a085fe8af65502d433
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070651"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a><span data-ttu-id="9f54e-103">تمكين ميزات تطبيق Project Finder Mobile (Project Service)</span><span class="sxs-lookup"><span data-stu-id="9f54e-103">Enable Project Finder Mobile app features (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="9f54e-104">بإمكان الموارد استخدام تطبيق Project Finder Mobile‬‬ على الهاتف مع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للبحث عن مشاريع جديدة للعمل عليها وتحديث مجموعات مهاراتها.</span><span class="sxs-lookup"><span data-stu-id="9f54e-104">Your resources can use the Project Finder Mobile app on their phone with [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to find new projects to work on and update their skill sets.</span></span>  
  
 <span data-ttu-id="9f54e-105">يتوفر التطبيق لهواتف [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] وأيضًا [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].</span><span class="sxs-lookup"><span data-stu-id="9f54e-105">The app is available for [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] phones, and [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].</span></span>  
  
 <span data-ttu-id="9f54e-106">إنك تحتاج إلى تعيين بضعة خيارات في إعداد المعلمات لكي تسمح وحدتك التنظيمية للمستخدمين بعرض متطلبات موارد المشروع وتحديث مهاراتها.</span><span class="sxs-lookup"><span data-stu-id="9f54e-106">You need to set a couple of options in the parameters setting for your organizational unit to allow users to view projects' resource requirements and update their skills.</span></span>  
  
> [!NOTE]
>  <span data-ttu-id="9f54e-107">يعمل تطبيق Project Finder Mobile‬‬ فقط مع [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)]، وليس مع عمليات التثبيت المحلية.</span><span class="sxs-lookup"><span data-stu-id="9f54e-107">The Project Finder Mobile app only works with [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], not with on-premises installations.</span></span>  
  
1. <span data-ttu-id="9f54e-108">انتقل إلى **Project Service > المعلمات‬**.</span><span class="sxs-lookup"><span data-stu-id="9f54e-108">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="9f54e-109">انقر فوق إعداد المعلمات الذي تريد استخدامه للسماح بميزات تطبيق Project Finder Mobile‬‬.</span><span class="sxs-lookup"><span data-stu-id="9f54e-109">Click the parameters setting you want to use for allowing the Project Finder Mobile app features.</span></span>  
  
3. <span data-ttu-id="9f54e-110">في الناحية **عام** عيّن **متطلبات الموارد المرئية للموارد‬** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9f54e-110">In the **General** area, set **Resource requirements visible to resources** to **Yes**.</span></span>  
  
4. <span data-ttu-id="9f54e-111">عيّن **السماح بتحديث المهارة بواسطة المورد‬** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9f54e-111">Set **Allow skill update by resource** to **Yes**.</span></span>  
  
   <span data-ttu-id="9f54e-112">![ProjectService_ProjectFinderEnable](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")</span><span class="sxs-lookup"><span data-stu-id="9f54e-112">![ProjectService_ProjectFinderEnable](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")</span></span>  
  
   <span data-ttu-id="9f54e-113">هذا إعداد عمومي.</span><span class="sxs-lookup"><span data-stu-id="9f54e-113">This is a global setting.</span></span> <span data-ttu-id="9f54e-114">بإمكان مدراء المشاريع تعيين ما إذا كان أحد المشاريع الفردية سيكون مرئيًا في صفحة **فريق المشروع**.</span><span class="sxs-lookup"><span data-stu-id="9f54e-114">Project managers can set whether an individual project will be visible on that project's **Project Team** page.</span></span>  
  
   <span data-ttu-id="9f54e-115">![ProjectService_ProjectTeamVisible](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")</span><span class="sxs-lookup"><span data-stu-id="9f54e-115">![ProjectService_ProjectTeamVisible](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")</span></span>  
  
## <a name="email-notifications"></a><span data-ttu-id="9f54e-116">إعلامات البريد الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="9f54e-116">Email notifications</span></span>  
 <span data-ttu-id="9f54e-117">ترسل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] رسائل البريد الإلكتروني فيما يتعلق بطلبات الموارد للمستلمين التاليين في الأوقات التالية:</span><span class="sxs-lookup"><span data-stu-id="9f54e-117">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sends emails regarding resource requests to the following recipients at the following times:</span></span>  
  
|<span data-ttu-id="9f54e-118">المستلم</span><span class="sxs-lookup"><span data-stu-id="9f54e-118">Recipient</span></span>|<span data-ttu-id="9f54e-119">الحدث</span><span class="sxs-lookup"><span data-stu-id="9f54e-119">Event</span></span>|  
|---------------|-----------|  
|<span data-ttu-id="9f54e-120">مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="9f54e-120">Project manager</span></span>|<span data-ttu-id="9f54e-121">-   عند تسجيل أحد الموارد للعمل على مشروع باستخدام تطبيق Project Finder Mobile.</span><span class="sxs-lookup"><span data-stu-id="9f54e-121">-   When a resource signs up for a project with the Project Finder Mobile app.</span></span>|  
|<span data-ttu-id="9f54e-122">المورد</span><span class="sxs-lookup"><span data-stu-id="9f54e-122">Resource</span></span>|<span data-ttu-id="9f54e-123">-   عندما يلبي مورد آخر عمل المشروع الذي قام المورد بالتسجيل للعمل عليه.</span><span class="sxs-lookup"><span data-stu-id="9f54e-123">-   When the project work the resource has signed up for has already been fulfilled by another resource.</span></span><br /><span data-ttu-id="9f54e-124">-   عند الموافقة على طلب الموافقة على المهارات أو رفضه.</span><span class="sxs-lookup"><span data-stu-id="9f54e-124">-   When their skill approval request has been approved or rejected.</span></span><br /><span data-ttu-id="9f54e-125">-   عند الموافقة على التسجيل للعمل على المشروع أو رفضه.</span><span class="sxs-lookup"><span data-stu-id="9f54e-125">-   When their project sign up request has been approved or rejected.</span></span>|  
  
## <a name="privacy-notice"></a><span data-ttu-id="9f54e-126">إشعار الخصوصية</span><span class="sxs-lookup"><span data-stu-id="9f54e-126">Privacy notice</span></span>  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a><span data-ttu-id="9f54e-127">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="9f54e-127">See Also</span></span>  
 [<span data-ttu-id="9f54e-128">إعداد الموارد</span><span class="sxs-lookup"><span data-stu-id="9f54e-128">Set up resources</span></span>](../psa/set-up-resources.md)
