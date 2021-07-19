---
title: نظرة عامة على شروط التعاقد المستندة إلى المنتج - خفيف
description: يقدم هذا الموضوع معلومات حول شروط التعاقد المستندة إلى المنتج.
author: rumant
ms.date: 10/07/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 8464eefbce9ba266360e10039e2a0be78982d8fa
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369720"
---
# <a name="product-based-contract-lines-overview---lite"></a><span data-ttu-id="8ca23-103">نظرة عامة على شروط التعاقد المستندة إلى المنتج - خفيف</span><span class="sxs-lookup"><span data-stu-id="8ca23-103">Product-based contract lines overview - lite</span></span>

<span data-ttu-id="8ca23-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="8ca23-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8ca23-105">يمكنك إنشاء شروط تعاقد مستندة إلى المنتجات في Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="8ca23-105">You can create product-based contract lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="8ca23-106">بإمكان شروط التعاقد المستندة إلى المنتج أن تكون بنودًا يتم إنشاؤها يدويًا أو يمكنها أن تكون عناصر من كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="8ca23-106">Product-based contract lines can be manually created lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="8ca23-107">كتالوج المنتجات</span><span class="sxs-lookup"><span data-stu-id="8ca23-107">Product catalog</span></span>

<span data-ttu-id="8ca23-108">توجد لدى المنتجات الموجودة في كتالوج المنتجات وحدة ومجموعة وحدات افتراضية.</span><span class="sxs-lookup"><span data-stu-id="8ca23-108">The products in the product catalog have a default unit and unit group.</span></span> <span data-ttu-id="8ca23-109">إذا كانت هناك عدة منتجات تشترك في نفس مجموعة السمات ، فيمكنك إنشاء مجموعة منتجات لديها هذه السمات أيضًا.</span><span class="sxs-lookup"><span data-stu-id="8ca23-109">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="8ca23-110">جميع المنتجات في عائلة منتج واحد ترث نفس مجموعة السمات.</span><span class="sxs-lookup"><span data-stu-id="8ca23-110">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="8ca23-111">على سبيل المثال ، تبيع الشركة تراخيص الاشتراك لأنواع مختلفة من البرامج.</span><span class="sxs-lookup"><span data-stu-id="8ca23-111">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="8ca23-112">تشتمل كافة برامج الاشتراك على السمتين التاليتين:</span><span class="sxs-lookup"><span data-stu-id="8ca23-112">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="8ca23-113">عدد المستخدمين</span><span class="sxs-lookup"><span data-stu-id="8ca23-113">Number of users</span></span>
- <span data-ttu-id="8ca23-114">مدة الاشتراك (بالشهور)</span><span class="sxs-lookup"><span data-stu-id="8ca23-114">Subscription duration (in months)</span></span>

<span data-ttu-id="8ca23-115">للمحافظة على هذا النوع من الكتالوجات، أنشئ مجموعة منتجات باسم **برنامج الاشتراك**.</span><span class="sxs-lookup"><span data-stu-id="8ca23-115">To maintain this type of catalog, create a product family that is named **Subscription Software**.</span></span> <span data-ttu-id="8ca23-116">أضف السمات، **عدد المستخدمين** و **مدة الاشتراك** إلى مجموعة المنتجات.</span><span class="sxs-lookup"><span data-stu-id="8ca23-116">Add the attributes, **Number of users** and **Subscription duration** to the product family.</span></span> <span data-ttu-id="8ca23-117">بعد ذلك، أضف منتجات فردية إلى مجموعة المنتجات **برامج الاشتراك**.</span><span class="sxs-lookup"><span data-stu-id="8ca23-117">Then, add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-contract"></a><span data-ttu-id="8ca23-118">إضافة عناصر كتالوج المنتجات إلى عقد مشروع</span><span class="sxs-lookup"><span data-stu-id="8ca23-118">Add product catalog items to a project Contract</span></span>

<span data-ttu-id="8ca23-119">تحتوي عقود المشروع على أقسام لنوعين من البنود: البنود المستندة إلى المشروع والبنود المستندة إلى المنتج.</span><span class="sxs-lookup"><span data-stu-id="8ca23-119">Project contracts have sections for two types of lines, project-based and product-based.</span></span> <span data-ttu-id="8ca23-120">تتضمن البنود المستندة إلى المنتج جميع المنتجات والوحدات الموجودة في قائمة أسعار المنتجات على العقد.</span><span class="sxs-lookup"><span data-stu-id="8ca23-120">Product-based lines include all of the products and units in the product price list on the contract.</span></span> <span data-ttu-id="8ca23-121">يمكن إضافة المنتجات التي لا تكون جزءًا من قائمة أسعار منتجات العقد.</span><span class="sxs-lookup"><span data-stu-id="8ca23-121">Products that aren't part of contract's product price list can be added.</span></span>

<span data-ttu-id="8ca23-122">يمكنك تحديد منتجات من قوائم أسعار أخرى أو من كتالوج المنتجات مباشرة.</span><span class="sxs-lookup"><span data-stu-id="8ca23-122">You can select products from other price lists, or directly from the product catalog.</span></span> <span data-ttu-id="8ca23-123">عند تحديد المنتجات مباشرةً من كتالوج المنتجات، يتم استخدام قائمة الأسعار الافتراضية لهذا المنتج لسعر مبيعات المنتج.</span><span class="sxs-lookup"><span data-stu-id="8ca23-123">When you select products directly from a product catalog, the default price list of that product is used for the product's sales price.</span></span> <span data-ttu-id="8ca23-124">إذا لم يتم تعيين قائمة أسعار افتراضية، سيتم تعيين السعر إلى 0 (صفر).</span><span class="sxs-lookup"><span data-stu-id="8ca23-124">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="8ca23-125">إذا كان شرط تعاقد يعتمد على كتالوج المنتجات، فيمكنك تجاوز سعر البيع مباشرة على البند.</span><span class="sxs-lookup"><span data-stu-id="8ca23-125">If a contract line is based on a product catalog, you can override the sales price directly on the line.</span></span> <span data-ttu-id="8ca23-126">يتضمن شرط التعاقد حقل **التسعير** مع القيمتين:</span><span class="sxs-lookup"><span data-stu-id="8ca23-126">A contract line has the **Pricing** field with the two values:</span></span>

- <span data-ttu-id="8ca23-127">**تجاوز التسعير**</span><span class="sxs-lookup"><span data-stu-id="8ca23-127">**Override pricing**</span></span>
- <span data-ttu-id="8ca23-128">**استخدام الافتراضي**</span><span class="sxs-lookup"><span data-stu-id="8ca23-128">**Use default**</span></span>

<span data-ttu-id="8ca23-129">إذا قمت بتعيين حقل **التسعير** إلى **تجاوز التسعير**، فلا يتم تعيين السعر الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="8ca23-129">If you set the **Pricing** field to **Override pricing**, the default price isn't set.</span></span> <span data-ttu-id="8ca23-130">أدخل سعرًا للمنتج على شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="8ca23-130">Enter a price for the product on the contract line.</span></span> <span data-ttu-id="8ca23-131">إذا قمت بتعيين الحقل إلى **استخدام الافتراضي**، سيتم استخدام سعر المبيعات الافتراضي ولا يمكن تحرير الحقل.</span><span class="sxs-lookup"><span data-stu-id="8ca23-131">If you set the field to **Use default**, the default sales price is used and the field can't be edited.</span></span>

<span data-ttu-id="8ca23-132">بعد تثبيت Project Operations، يتم إدخال أسعار المبيعات الافتراضية في البنود المستندة إلى المنتج على العقد.</span><span class="sxs-lookup"><span data-stu-id="8ca23-132">After you install Project Operations, default sales prices are entered on the product-based lines on a contract.</span></span> <span data-ttu-id="8ca23-133">ثم يتم تعيين حقل **التسعير** إلى **تجاوز التسعير** حتى يمكنك تحرير السعر الافتراضي في شروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="8ca23-133">The **Pricing** field is set to **Override pricing** so that you can edit the default price on the contract lines.</span></span> <span data-ttu-id="8ca23-134">هذا تجاوز خاص بـ Project Operations لسلوك البنود القائمة على المنتج في Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="8ca23-134">This is a Project Operations-specific override to product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]