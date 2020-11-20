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
ms.openlocfilehash: 8a219ef0166565a550a7836ffeae37ffd514a001
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129167"
---
# <a name="configure-project-service"></a><span data-ttu-id="ae9b1-103">تكوين Project Service</span><span class="sxs-lookup"><span data-stu-id="ae9b1-103">Configure Project Service</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="ae9b1-104">قبل أن تتمكن من استخدام قدرات التشغيل التلقائي لدى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] في [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] لإدارة الحسابات والمشاريع والموارد، تحتاج إلى إكمال بعض خطوات التكوين لضمان مطابقة حل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] مع احتياجات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="ae9b1-105">تتضمن هذه الخطوات:</span><span class="sxs-lookup"><span data-stu-id="ae9b1-105">These steps include:</span></span>  
  
-   <span data-ttu-id="ae9b1-106">[إعداد الوحدات الزمنية](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="ae9b1-107">تكوين وحدات الوقت في كتالوج المنتجات التي ستستخدمها كأساس لجدولة المشاريع وفوترتها.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="ae9b1-108">[إعداد العملات وأسعار الصرف](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="ae9b1-109">إعداد العملات لاستخدامها لمشاريعك.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="ae9b1-110">[إنشاء الوحدات التنظيمية](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="ae9b1-111">إعداد المجموعات التي تستخدمها شركتك لتقسيم أعمالها، سواء حسب الموقع الجغرافي أو الوظائف المهنية أو الأقسام المنطقية الأخرى.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="ae9b1-112">[إعداد تكرارات الفاتورة](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="ae9b1-113">إعداد الفترات الزمنية التي تريد استخدامها لفوترة العملاء.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="ae9b1-114">[تكوين فئات المعاملات](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="ae9b1-115">إعداد فئات المعاملات التي يمكن للمستشارين تحميلها مصروفاتهم القابلة للفوترة ومصروفاتهم.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="ae9b1-116">[تكوين فئات المصروفات](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="ae9b1-117">إعداد الفئات التي يمكن للمستشارين تحميلها مصروفاتهم القابلة للفوترة ومصروفاتهم غير القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="ae9b1-118">[إنشاء أصناف في كتالوج المنتجات](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="ae9b1-119">إضافة المنتجات التي تبيعها، مثل تراخيص البرامج، إلى كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="ae9b1-120">[إنشاء قائمة أسعار](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="ae9b1-121">تكوين قوائم أسعار مختلفة، استنادًا إلى الرسوم التي تريد فرضها على العملاء لكل دور يتطلبه مشروعهم.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="ae9b1-122">[إعداد الموارد](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b1-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="ae9b1-123">إضافة المهارات والكفاءات وأدوار الموارد ومعلومات حول الموارد الأخرى التي ستحتاجها لمشاريعك.</span><span class="sxs-lookup"><span data-stu-id="ae9b1-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="ae9b1-124">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="ae9b1-124">See Also</span></span>  
 <span data-ttu-id="ae9b1-125">[نظرة عامة على Project Service Automation](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="ae9b1-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="ae9b1-126">[تكوين Project Service Automation](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="ae9b1-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="ae9b1-127">[دليل مدير الحسابات](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae9b1-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="ae9b1-128">[دليل مدير المشروع](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae9b1-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="ae9b1-129">[دليل إدارة الموارد](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae9b1-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="ae9b1-130">دليل الوقت والمصروفات والتعاون</span><span class="sxs-lookup"><span data-stu-id="ae9b1-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)
