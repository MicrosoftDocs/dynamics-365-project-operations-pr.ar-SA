---
title: إنشاء قائمة أسعار
description: كيفية إنشاء قائمة أسعار في Project Service
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: bdd05aea-27a3-431d-9a80-2e220fb25e53
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 756af2fe3bc73d478b0355493aae6f0e49ac5835
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748744"
---
# <a name="create-a-price-list-project-service"></a><span data-ttu-id="adee7-103">إنشاء قائمة أسعار (Project Service)</span><span class="sxs-lookup"><span data-stu-id="adee7-103">Create a price list (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="adee7-104">توفر قوائم الأسعار قالبًا يستطيع مدراء الحسابات استخدامه لإنشاء عروض الأسعار والمشاريع، ولتحديد تكاليف المشروع.</span><span class="sxs-lookup"><span data-stu-id="adee7-104">Price lists provide a template your account managers can use for creating quotes and projects, and for establishing the costs of a project.</span></span> <span data-ttu-id="adee7-105">إنها توفر قائمة عناصر بنود تتضمن الأدوار والمصروفات والسعر الذي ستفرضه لكل واحد منها.</span><span class="sxs-lookup"><span data-stu-id="adee7-105">They provide a line item list of roles and expenses, and the price you will charge for each.</span></span> <span data-ttu-id="adee7-106">يمكنك إنشاء قوائم أسعار متعددة بحيث يمكنك الحفاظ على هياكل أسعار مستقلة خاصة بالمناطق المختلفة التي تبيع منتجاتك فيها أو خاصة بقنوات بيع مختلفة.</span><span class="sxs-lookup"><span data-stu-id="adee7-106">You can create multiple price lists so that you can maintain separate price structures for different regions you sell your products in or for different sales channels.</span></span> <span data-ttu-id="adee7-107">من المستحسن إنشاء قائمة أسعار واحدة على الأقل لكل عملة تخطط لإعداد فواتير العملاء بها.</span><span class="sxs-lookup"><span data-stu-id="adee7-107">It’s a good idea to create at least one price list for every currency you plan to bill your customers in.</span></span>  
  
<span data-ttu-id="adee7-108">لإنشاء تقديرات مالية للعمل الذي يجب تسليمه، تأكد من أن كل مشروع يحتوي على قائمة بالتكاليف المتأخرة وسعر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="adee7-108">To create financial estimates for the work to be delivered, make sure every project has a backing cost and sales price list.</span></span> <span data-ttu-id="adee7-109">اعمل على إعداد قائمة التكلفة الافتراضية وأسعار المبيعات التي تنطبق على كافة المشاريع التي تم إنشاؤها في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="adee7-109">Set up a default cost and sales pricelist that applies to all projects created in your organization.</span></span>  
  
<span data-ttu-id="adee7-110">تعتمد قوائم الأسعار على الأدوار وفئات المصروفات، ولذلك قبل إنشاء قائمة الأسعار، تأكد من تكوين الأدوار وفئات المصروفات التي تريد استخدامها أثناء إنشاء قائمة الأسعار.</span><span class="sxs-lookup"><span data-stu-id="adee7-110">Price lists rely on roles and expense categories, so before you create a price list, make sure you’ve already configured the roles and expense categories you want to use while creating the price list.</span></span>  
  
1.  <span data-ttu-id="adee7-111">اذهب إلى **Project Service > قوائم الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="adee7-111">Go to **Project Service > Price Lists**.</span></span>  
  
2.  <span data-ttu-id="adee7-112">انقر فوق **جديد**.</span><span class="sxs-lookup"><span data-stu-id="adee7-112">Click **New**.</span></span>  
  
3.  <span data-ttu-id="adee7-113">في **السياق**، حدد ما إذا كانت قائمة الأسعار هذه تعود إلى فئة **التكلفة** أو **الشراء** أو **المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="adee7-113">In **Context**, select whether this price list is for **Cost**, **Purchase**, or **Sales**.</span></span>  
  
4.  <span data-ttu-id="adee7-114">في **الاسم**، أدخل اسمًا لقائمة الأسعار.</span><span class="sxs-lookup"><span data-stu-id="adee7-114">In **Name**, enter a name for the price list.</span></span>  
  
5.  <span data-ttu-id="adee7-115">في **العملة**، حدد العملة التي سوف تستخدمها لإعداد الفواتير أو التكلفة.</span><span class="sxs-lookup"><span data-stu-id="adee7-115">In **Currency**, select the currency you’re going to use for billing or costing.</span></span>  
  
6.  <span data-ttu-id="adee7-116">في **الوحدة الزمنية**، حدد الفترة الزمنية حيث ينطبق السعر، مثل اليوم أو الساعة.</span><span class="sxs-lookup"><span data-stu-id="adee7-116">In **Time Unit**, specify the period of time the price applies to, such as day or hour.</span></span>  
  
7.  <span data-ttu-id="adee7-117">املأ **تاريخ البدء** و**تاريخ الانتهاء** و**الوصف** حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="adee7-117">Fill in the **Start Date**, **End Date**, and **Description** as needed.</span></span>  
  
8.  <span data-ttu-id="adee7-118">انقر فوق **حفظ** لإنشاء السجل حتى يمكنك متابعة تحريره.</span><span class="sxs-lookup"><span data-stu-id="adee7-118">Click **Save** to create the record so you can continue editing it.</span></span>  
  
9. <span data-ttu-id="adee7-119">لإضافة دور سعر إلى قائمة الأسعار، انقر فوق **+** تحت **أسعار الأدوار**.</span><span class="sxs-lookup"><span data-stu-id="adee7-119">To add a role price to the price list, click **+** under **Role prices**.</span></span>  
  
10. <span data-ttu-id="adee7-120">في الجزء **سعر الدور**، قم بملء التفاصيل، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="adee7-120">In the **Role Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="adee7-121">تابع إضافة أسعار الأدوار كما تقتضي الحاجة.</span><span class="sxs-lookup"><span data-stu-id="adee7-121">Continue adding role prices as necessary.</span></span> <span data-ttu-id="adee7-122">عندما تنهي عملك، انقر فوق الزر **حفظ** في الزاوية السفلية اليسرى من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="adee7-122">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
11. <span data-ttu-id="adee7-123">لإضافة سعر فئة مصروفات إلى قائمة الأسعار، انقر فوق **+** تحت **أسعار الفئات**.</span><span class="sxs-lookup"><span data-stu-id="adee7-123">To add an expense category price to the price list, click **+** under **Category prices**.</span></span>  
  
12. <span data-ttu-id="adee7-124">في الجزء **سعر فئة المعاملة‬**، قم بملء التفاصيل، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="adee7-124">In the **Transaction Category Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="adee7-125">تابع إضافة أسعار الفئات كما تقتضي الحاجة.</span><span class="sxs-lookup"><span data-stu-id="adee7-125">Continue adding category prices as necessary.</span></span> <span data-ttu-id="adee7-126">عندما تنهي عملك، انقر فوق الزر **حفظ** في الزاوية السفلية اليسرى من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="adee7-126">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
13. <span data-ttu-id="adee7-127">لإضافة عناصر قائمة الأسعار إلى قائمة الأسعار، انقر فوق **+** تحت **بنود قائمة الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="adee7-127">To add price list items to the price list, click **+** under **Price List Items**.</span></span>  
  
14. <span data-ttu-id="adee7-128">في الجزء **بنود قائمة الأسعار**، قم بملء التفاصيل، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="adee7-128">In the **Price List Item** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="adee7-129">تابع إضافة بنود قائمة الأسعار كما تقتضي الحاجة.</span><span class="sxs-lookup"><span data-stu-id="adee7-129">Continue adding price list items as necessary.</span></span> <span data-ttu-id="adee7-130">عندما تنهي عملك، انقر فوق الزر **حفظ** في الزاوية السفلية اليسرى من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="adee7-130">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
15. <span data-ttu-id="adee7-131">لإضافة علاقات المناطق إلى قائمة الأسعار، انقر فوق **+** تحت **علاقات المناطق**.</span><span class="sxs-lookup"><span data-stu-id="adee7-131">To add territory relationships to the price list, click **+** under **Territory Relationships**.</span></span>  
  
16. <span data-ttu-id="adee7-132">في النافذة **اتصال جديد**، قم بملء التفاصيل، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="adee7-132">In the **New Connection** window, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="adee7-133">تابع إضافة علاقات المناطق كما تقتضي الحاجة.</span><span class="sxs-lookup"><span data-stu-id="adee7-133">Continue adding territory relationships as necessary.</span></span> <span data-ttu-id="adee7-134">عندما تنهي عملك، انقر فوق الزر **حفظ** في الزاوية السفلية اليسرى من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="adee7-134">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="adee7-135">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="adee7-135">See Also</span></span>  
 [<span data-ttu-id="adee7-136">تكوين Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="adee7-136">Configure Project Service Automation</span></span>](../project-service/configure.md)
