---
title: نظرة عامة على بنود عرض الأسعار القائمة على المنتج - خفيف
description: يقدم هذا الموضوع معلومات حول العمل مع بنود عرض الأسعار القائمة على المنتج.
author: rumant
ms.date: 10/30/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 8b904f9abd3d2505c5397906f63a5ae8ff4be41b
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369765"
---
# <a name="product-based-quote-lines-overview---lite"></a><span data-ttu-id="0067f-103">نظرة عامة على بنود عرض الأسعار القائمة على المنتج - خفيف</span><span class="sxs-lookup"><span data-stu-id="0067f-103">Product-based quote lines overview - lite</span></span>

<span data-ttu-id="0067f-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="0067f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0067f-105">يمكنك إنشاء بنود عرض أسعار مستندة إلى المنتجات في Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="0067f-105">You can create product-based quote lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="0067f-106">يمكن إضافة بنود عرض الأسعار القائمة على المنتج يدويًا، أو يمكنها أو تكون عبارة عن عناصر من كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="0067f-106">Product-based quote lines can be manually added, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="0067f-107">كتالوج المنتجات</span><span class="sxs-lookup"><span data-stu-id="0067f-107">Product catalog</span></span>

<span data-ttu-id="0067f-108">يحتوي كل منتج في كتالوج المنتجات على وحدة ومجموعة وحدات افتراضية.</span><span class="sxs-lookup"><span data-stu-id="0067f-108">Each product in the product catalog has a default unit and unit group.</span></span> <span data-ttu-id="0067f-109">عند وجود عدة منتجات تشارك مجموعة السمات نفسها، يمكنك إنشاء مجموعة منتجات تشارك هذه السمات.</span><span class="sxs-lookup"><span data-stu-id="0067f-109">If multiple products share the same set of attributes, you can create a product family that share those attributes.</span></span> 

<span data-ttu-id="0067f-110">على سبيل المثال ، تبيع الشركة تراخيص الاشتراك لأنواع مختلفة من البرامج.</span><span class="sxs-lookup"><span data-stu-id="0067f-110">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="0067f-111">تشتمل كافة برامج الاشتراك على السمتين التاليتين:</span><span class="sxs-lookup"><span data-stu-id="0067f-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="0067f-112">عدد المستخدمين</span><span class="sxs-lookup"><span data-stu-id="0067f-112">Number of users</span></span>
- <span data-ttu-id="0067f-113">مدة الاشتراك مقاسة بالأشهر</span><span class="sxs-lookup"><span data-stu-id="0067f-113">A subscription duration measured in months</span></span>

<span data-ttu-id="0067f-114">للحفاظ على نوع الكتالوج هذا، أنشئ مجموعة منتجات تسمى **برامج الاشتراك**، ثم أضف عدد المستخدمين ومدة الاشتراك كسمات.</span><span class="sxs-lookup"><span data-stu-id="0067f-114">To maintain this type of catalog, create a product family named **Subscription Software** and add the number of users and the subscription duration as attributes.</span></span> <span data-ttu-id="0067f-115">بعد ذلك، يمكنك إضافة منتجات فردية إلى مجموعة منتجات **برنامج الاشتراك**.</span><span class="sxs-lookup"><span data-stu-id="0067f-115">Next, you can add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="0067f-116">إضافة عناصر كتالوج المنتجات إلى عرض أسعار مشروع</span><span class="sxs-lookup"><span data-stu-id="0067f-116">Add product catalog items to a project quote</span></span>

<span data-ttu-id="0067f-117">تحتوي صفحات **عرض أسعار المشروع** و **عقد المشروع** على أقسام للبنود القائمة على المشروع والبنود القائمة على المنتج.</span><span class="sxs-lookup"><span data-stu-id="0067f-117">The **Project Quote** and **Project Contract** pages have sections for project-based lines and product-based lines.</span></span> <span data-ttu-id="0067f-118">بالنسبة إلى البنود القائمة على المنتج، تتضمن القائمة المنسدلة الموجودة في بند عرض الأسعار أو شرط تعاقد المشروع جميع المنتجات والوحدات الموجودة في قائمة أسعار المنتج.</span><span class="sxs-lookup"><span data-stu-id="0067f-118">For product-based lines, the drop-down list on the quote line or project contract line includes all the products and units in the product price list.</span></span> <span data-ttu-id="0067f-119">يمكنك أيضًا إضافة منتجات ليست جزءًا من قائمة أسعار منتجات عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="0067f-119">You can also add products that aren't part of the product price list.</span></span>

<span data-ttu-id="0067f-120">بالإضافة إلى ذلك، يمكنك اختيار المنتجات من قوائم أسعار أخرى، أو يمكنك التحديد مباشرة من كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="0067f-120">Additionally, you can select products from other price lists or directly from the product catalog.</span></span> <span data-ttu-id="0067f-121">عند تحديد المنتجات مباشرةً من كتالوج المنتجات ، يتم استخدام قائمة الأسعار الافتراضية لهذا المنتج للحصول على سعر مبيعات المنتج.</span><span class="sxs-lookup"><span data-stu-id="0067f-121">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="0067f-122">إذا لم يتم تعيين قائمة أسعار افتراضية، سيتم تعيين السعر إلى صفر (0).</span><span class="sxs-lookup"><span data-stu-id="0067f-122">If a default price list isn't set, the price is set to zero (0).</span></span>

<span data-ttu-id="0067f-123">إذا كان بند عرض أسعار يستند إلى كتالوج المنتجات، فيمكنك تجاوز سعر البيع مباشرة على بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="0067f-123">When a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="0067f-124">بند عرض أسعار في حقل **التسعير** مع قيمتين متوفرتين:</span><span class="sxs-lookup"><span data-stu-id="0067f-124">A quote line in **Pricing** field with two available values:</span></span>

- <span data-ttu-id="0067f-125">**تجاوز التسعير**</span><span class="sxs-lookup"><span data-stu-id="0067f-125">**Override Pricing**</span></span>
- <span data-ttu-id="0067f-126">**‏‏استخدام الافتراضي**</span><span class="sxs-lookup"><span data-stu-id="0067f-126">**Use Default**</span></span>

<span data-ttu-id="0067f-127">إذا حددت **تجاوز التسعير**، فلن يتم تعيين السعر الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="0067f-127">If you select **Override Pricing**, the default price isn't set.</span></span> <span data-ttu-id="0067f-128">بدلاً من ذلك، يجب عليك إدخال سعر للمنتج في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="0067f-128">Instead, you must enter a price for the product on the quote line.</span></span> <span data-ttu-id="0067f-129">إذا قمت بتحديد **استخدام الافتراضي**، سيتم استخدام سعر المبيعات الافتراضي ويتم تامين الحقل للتحرير.</span><span class="sxs-lookup"><span data-stu-id="0067f-129">If you select **Use Default**, the default sales price is used and the field is locked for editing.</span></span>

<span data-ttu-id="0067f-130">بيتم إدخال أسعار المبيعات الافتراضية في البنود المستندة إلى المنتج في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="0067f-130">Default sales prices are entered on the product-based lines of a quote.</span></span> <span data-ttu-id="0067f-131">ثم يتم تعيين حقل **التسعير** إلى **تجاوز التسعير** حتى يمكنك تحرير السعر الافتراضي في بنود عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="0067f-131">The **Pricing** field is then set to **Override Pricing** so that you can edit the default price on the quote lines.</span></span> <span data-ttu-id="0067f-132">هذا تجاوز خاص في Project Operations لسلوك للبنود القائمة على المنتج في Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="0067f-132">This is a Project Operations-specific override to the product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]