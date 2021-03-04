---
title: تكوين Project Service Automation
description: خطوات لتكوين Project Service
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
ms.openlocfilehash: ec5381f91b1fe5198bd93ac8d6015b1fea38738d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146917"
---
# <a name="configure-project-service"></a><span data-ttu-id="5c7c4-103">تكوين Project Service</span><span class="sxs-lookup"><span data-stu-id="5c7c4-103">Configure Project Service</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="5c7c4-104">قبل أن تتمكن من استخدام قدرات التشغيل التلقائي لدى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] في [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] لإدارة الحسابات والمشاريع والموارد، تحتاج إلى إكمال بعض خطوات التكوين لضمان مطابقة حل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] مع احتياجات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="5c7c4-105">تتضمن هذه الخطوات:</span><span class="sxs-lookup"><span data-stu-id="5c7c4-105">These steps include:</span></span>  
  
-   <span data-ttu-id="5c7c4-106">[إعداد الوحدات الزمنية](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="5c7c4-107">تكوين وحدات الوقت في كتالوج المنتجات التي ستستخدمها كأساس لجدولة المشاريع وفوترتها.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="5c7c4-108">[إعداد العملات وأسعار الصرف](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="5c7c4-109">إعداد العملات لاستخدامها لمشاريعك.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="5c7c4-110">[إنشاء الوحدات التنظيمية](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="5c7c4-111">إعداد المجموعات التي تستخدمها شركتك لتقسيم أعمالها، سواء حسب الموقع الجغرافي أو الوظائف المهنية أو الأقسام المنطقية الأخرى.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="5c7c4-112">[إعداد تكرارات الفاتورة](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="5c7c4-113">إعداد الفترات الزمنية التي تريد استخدامها لفوترة العملاء.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="5c7c4-114">[تكوين فئات المعاملات](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="5c7c4-115">إعداد فئات المعاملات التي يمكن للمستشارين تحميلها مصروفاتهم القابلة للفوترة ومصروفاتهم.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="5c7c4-116">[تكوين فئات المصروفات](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="5c7c4-117">إعداد الفئات التي يمكن للمستشارين تحميلها مصروفاتهم القابلة للفوترة ومصروفاتهم غير القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="5c7c4-118">[إنشاء أصناف في كتالوج المنتجات](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="5c7c4-119">إضافة المنتجات التي تبيعها، مثل تراخيص البرامج، إلى كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="5c7c4-120">[إنشاء قائمة أسعار](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="5c7c4-121">تكوين قوائم أسعار مختلفة، استنادًا إلى الرسوم التي تريد فرضها على العملاء لكل دور يتطلبه مشروعهم.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="5c7c4-122">[إعداد الموارد](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="5c7c4-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="5c7c4-123">إضافة المهارات والكفاءات وأدوار الموارد ومعلومات حول الموارد الأخرى التي ستحتاجها لمشاريعك.</span><span class="sxs-lookup"><span data-stu-id="5c7c4-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="5c7c4-124">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="5c7c4-124">See Also</span></span>  
 <span data-ttu-id="5c7c4-125">[نظرة عامة على Project Service Automation](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="5c7c4-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="5c7c4-126">[تكوين Project Service Automation](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="5c7c4-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="5c7c4-127">[دليل مدير الحسابات](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5c7c4-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="5c7c4-128">[دليل مدير المشروع](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5c7c4-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="5c7c4-129">[دليل إدارة الموارد](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5c7c4-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="5c7c4-130">دليل الوقت والمصروفات والتعاون</span><span class="sxs-lookup"><span data-stu-id="5c7c4-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)
