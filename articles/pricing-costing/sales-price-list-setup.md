---
title: إعداد قائمة أسعار المبيعات
description: يوفر هذا الموضوع معلومات حول قوائم أسعار المبيعات لتسعير المشروع.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2a66802adfcadab7b4d34149b146ca3cb27c903e
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896445"
---
# <a name="sales-price-list-setup"></a><span data-ttu-id="735c9-103">إعداد قائمة أسعار المبيعات</span><span class="sxs-lookup"><span data-stu-id="735c9-103">Sales price list setup</span></span>

<span data-ttu-id="735c9-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="735c9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="735c9-105">بالنسبة لعروض أسعار المشروع والعقود، تحتوي قائمة أسعار المشروع على نموذج تجاوز سعر يختلف عن قائمة أسعار المنتجات.</span><span class="sxs-lookup"><span data-stu-id="735c9-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="735c9-106">في بند عرض الأسعار المستند إلى كتالوج المنتجات، يمكنك تجاوز السعر إلى الأدوار والفئات مباشرة في بند عرض الأسعار ، نظرا لأن كل بند من بنود العرض يشير إلى صنف كتالوج واحد بالضبط.</span><span class="sxs-lookup"><span data-stu-id="735c9-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="735c9-107">ومع ذلك، في بند عرض الأسعار على أساس المشروع، لا يمكنك تجاوز السعر إلى الأدوار والفئات مباشرة على بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="735c9-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="735c9-108">يمكنك استخدم قائمة أسعار المشروع للعمل مع نموذجين مختلفين للتجاوز.</span><span class="sxs-lookup"><span data-stu-id="735c9-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="735c9-109">نوصي بأن تكون لديك قائمة أسعار منفصلة لموارد المشروع وعناصر الكتالوج ، نظرا لحدوث اختلافات في السلوك بين الاثنين عند تجاوز التسعير.</span><span class="sxs-lookup"><span data-stu-id="735c9-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="735c9-110">يمكن لكل من الكيانات التالية أن يحتوي علي واحدة أو أكثر من قوائم أسعار المبيعات المقترنة لتسعير المشروع:</span><span class="sxs-lookup"><span data-stu-id="735c9-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="735c9-111">العميل (حساب)</span><span class="sxs-lookup"><span data-stu-id="735c9-111">Customer (account)</span></span> 
- <span data-ttu-id="735c9-112">الفرصة</span><span class="sxs-lookup"><span data-stu-id="735c9-112">Opportunity</span></span> 
- <span data-ttu-id="735c9-113">عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="735c9-113">Quote</span></span> 
- <span data-ttu-id="735c9-114">عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="735c9-114">Project Contract</span></span>

<span data-ttu-id="735c9-115">تتم الإشارة إلى اقتران هذه الكيانات بقائمة أسعار بواسطة قوائم أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="735c9-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="735c9-116">يمكنك ربط قائمة أسعار واحدة أو أكثر باستخدام كيانات العميل والفرصة وعرض الأسعار وعقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="735c9-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="735c9-117">لا يتم إدخال قائمة أسعار المشروع الافتراضية تلقائيا في سجل العميل.</span><span class="sxs-lookup"><span data-stu-id="735c9-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="735c9-118">ومع ذلك، يمكنك يدويًا إرفاق قائمة أسعار مشروع بسجل العميل.</span><span class="sxs-lookup"><span data-stu-id="735c9-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="735c9-119">بالرغم من ذلك، ينبغي إرفاق قائمة أسعار مشروع يدويًا عندما يكون لديك اتفاقية تسعير مخصصة مع العميل.</span><span class="sxs-lookup"><span data-stu-id="735c9-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="735c9-120">عندما تكون قائمة أسعار المشروع مرفقة بكيان مبيعات، فإنه يتم التحقق من المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="735c9-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="735c9-121">قائمه الأسعار تتضمن سياق **المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="735c9-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="735c9-122">يجب أن تتطابق عملة قائمة الأسعار مع عملة العميل.</span><span class="sxs-lookup"><span data-stu-id="735c9-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="735c9-123">في عقد المشروع، يُستخدم ترتيب الأسبقية التالي لتعيين قوائم أسعار المشروع ذات الصلة تلقائيًا:</span><span class="sxs-lookup"><span data-stu-id="735c9-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="735c9-124">اقتباس</span><span class="sxs-lookup"><span data-stu-id="735c9-124">Quote</span></span>
2. <span data-ttu-id="735c9-125">الفرصة</span><span class="sxs-lookup"><span data-stu-id="735c9-125">Opportunity</span></span>
3. <span data-ttu-id="735c9-126">العميل</span><span class="sxs-lookup"><span data-stu-id="735c9-126">Customer</span></span> 
4. <span data-ttu-id="735c9-127">الإعدادات العمومية</span><span class="sxs-lookup"><span data-stu-id="735c9-127">Global settings</span></span> 

<span data-ttu-id="735c9-128">عند إدخال قائمة أسعار مشروع بشكل افتراضي، يتحقق النظام من أن العملة تطابق عملة العميل، وأن قوائم الأسعار الافتراضية التي التي إدخالها لها سياق **المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="735c9-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="735c9-129">يمكنك ربط قوائم أسعار مشروع متعددة باستخدام كيانات مبيعات العميل والفرصة وعرض الأسعار وعقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="735c9-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="735c9-130">تدعم هذه الإمكانية الأسعار الافتراضية المحددة بتاريخ لعقد المشروع الذي يعمل بفترة طويلة، حيث يمكنك طلب أكثر من قائمة أسعار واحدة لحساب التحديثات الخاصة بالأسعار التي تحدث بسبب التضخم.</span><span class="sxs-lookup"><span data-stu-id="735c9-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="735c9-131">ومع ذلك، إذا كانت قوائم الأسعار التي قمت بربطها بالعميل أو الفرصة أو عرض الأسعار أو كيان عقد المشروع بها تراكب بشأن تاريخ السريان، فقد تكون الأسعار الافتراضية غير صحيحة.</span><span class="sxs-lookup"><span data-stu-id="735c9-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="735c9-132">بالتالي، يتعين عليك التأكد من أن قوائم أسعار المشروع ذات تاريخ سريان متراكب غير مقترنة بهذه الكيانات.</span><span class="sxs-lookup"><span data-stu-id="735c9-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>
