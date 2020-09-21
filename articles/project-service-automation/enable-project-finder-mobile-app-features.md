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
ms.prod: ''
ms.technology: ''
ms.assetid: 038c5c66-f136-4c7e-88c2-30ada80bbf38
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 9265ee78b20899026277e5af8e589112cd9fac74
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748589"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a>تمكين ميزات تطبيق Project Finder Mobile (Project Service)

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

بإمكان الموارد استخدام تطبيق Project Finder Mobile‬‬ على الهاتف مع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للبحث عن مشاريع جديدة للعمل عليها وتحديث مجموعات مهاراتها.  
  
 يتوفر التطبيق لهواتف [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] وأيضًا [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].  
  
 إنك تحتاج إلى تعيين بضعة خيارات في إعداد المعلمات لكي تسمح وحدتك التنظيمية للمستخدمين بعرض متطلبات موارد المشروع وتحديث مهاراتها.  
  
> [!NOTE]
>  يعمل تطبيق Project Finder Mobile‬‬ فقط مع [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)]، وليس مع عمليات التثبيت المحلية.  
  
1. انتقل إلى **Project Service > المعلمات‬**.  
  
2. انقر فوق إعداد المعلمات الذي تريد استخدامه للسماح بميزات تطبيق Project Finder Mobile‬‬.  
  
3. في الناحية **عام** عيّن **متطلبات الموارد المرئية للموارد‬** إلى **نعم**.  
  
4. عيّن **السماح بتحديث المهارة بواسطة المورد‬** إلى **نعم**.  
  
   ![ProjectService_ProjectFinderEnable](../project-service/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")  
  
   هذا إعداد عمومي. بإمكان مدراء المشاريع تعيين ما إذا كان أحد المشاريع الفردية سيكون مرئيًا في صفحة **فريق المشروع**.  
  
   ![ProjectService_ProjectTeamVisible](../project-service/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")  
  
## <a name="email-notifications"></a>إعلامات البريد الإلكتروني  
 ترسل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] رسائل البريد الإلكتروني فيما يتعلق بطلبات الموارد للمستلمين التاليين في الأوقات التالية:  
  
|المستلم|الحدث|  
|---------------|-----------|  
|مدير المشروع|-   عند تسجيل أحد الموارد للعمل على مشروع باستخدام تطبيق Project Finder Mobile.|  
|المورد|-   عندما يلبي مورد آخر عمل المشروع الذي قام المورد بالتسجيل للعمل عليه.<br />-   عند الموافقة على طلب الموافقة على المهارات أو رفضه.<br />-   عند الموافقة على التسجيل للعمل على المشروع أو رفضه.|  
  
## <a name="privacy-notice"></a>إشعار الخصوصية  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a>راجع أيضًا  
 [إعداد الموارد](../project-service/set-up-resources.md)
