---
title: الاختبار بواسطة بيانات العرض التوضيحي
description: كيفية تنزيل بيانات العرض التوضيحي والاختبار بواسطتها في تطبيق Project Service Automation.
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: b195e5c8-63bc-4e90-914c-f29b8d565942
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 76dd5ff14cbafbfc5341885f0469a6e3e71dd66f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748688"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="7f0ab-103">الاختبار بواسطة بيانات العرض التوضيحي (Project Service)</span><span class="sxs-lookup"><span data-stu-id="7f0ab-103">Experiment with demo data (Project Service)</span></span>

<span data-ttu-id="7f0ab-104">للتعرف إلى Dynamics 365 Project Service Automation، من المفيد توفير بيئة تم تكوينها مسبقاً لاستكشافها.</span><span class="sxs-lookup"><span data-stu-id="7f0ab-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="7f0ab-105">لهذا الغرض، قمنا بإنشاء حزمة تثبيت بيانات عينة منفصلة (باللغة الإنجليزية فقط في هذا الوقت) تسهل التعرف على هذه الحلول.</span><span class="sxs-lookup"><span data-stu-id="7f0ab-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="7f0ab-106">تكون حزمة التثبيت متاحة على [مركز التنزيل لـ Microsoft](https://go.microsoft.com/fwlink/?linkid=859966).</span><span class="sxs-lookup"><span data-stu-id="7f0ab-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="7f0ab-107">يؤدي تشغيل تثبيت Package Deployer إلى تنفيذ الإجراءات التالية:</span><span class="sxs-lookup"><span data-stu-id="7f0ab-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="7f0ab-108">إنشاء أو تعيين المعلمات الافتراضية التي تعزز سلوك Project Service</span><span class="sxs-lookup"><span data-stu-id="7f0ab-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="7f0ab-109">استيراد بيانات العينة مثل الموارد القابلة للحجز والأدوار والمبيعات وقوائم أسعار التكلفة والوحدات التنظيمية وسجلات عملية المبيعات ذات الصلة وأوامر العمل والمشروعات</span><span class="sxs-lookup"><span data-stu-id="7f0ab-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="7f0ab-110">**لا توجد أي طريقة لإزالة تثبيت بيانات العرض التوضيحي.**</span><span class="sxs-lookup"><span data-stu-id="7f0ab-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="7f0ab-111">وبالتالي، يجب استخدام هذه الحزمة فقط على العرض التوضيحي والتقييم والتدريب وأنظمة الاختبار.</span><span class="sxs-lookup"><span data-stu-id="7f0ab-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="7f0ab-112">لمزيد من المعلومات، راجع هذه [المدونة](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span><span class="sxs-lookup"><span data-stu-id="7f0ab-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="7f0ab-113">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="7f0ab-113">See Also</span></span>  
 <span data-ttu-id="7f0ab-114">[دليل المسؤول](../project-service/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="7f0ab-114">[Administrator Guide](../project-service/admin-guide.md) </span></span>  
 <span data-ttu-id="7f0ab-115">[دليل مدير الحسابات](../project-service/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="7f0ab-115">[Account Manager Guide](../project-service/account-manager-guide.md) </span></span>  
 <span data-ttu-id="7f0ab-116">[دليل مدير المشروع](../project-service/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="7f0ab-116">[Project Manager Guide](../project-service/project-manager-guide.md) </span></span>  
 <span data-ttu-id="7f0ab-117">[دليل إدارة الموارد](../project-service/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="7f0ab-117">[Resource Manager Guide](../project-service/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="7f0ab-118">دليل الوقت والمصروفات والتعاون</span><span class="sxs-lookup"><span data-stu-id="7f0ab-118">Time, Expense, and Collaboration Guide</span></span>](../project-service/time-expense-collaboration-guide.md)
