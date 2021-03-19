---
title: بنود عرض أسعار يستند إلى منتج
description: يقدم هذا الموضوع معلومات حول عروض الأسعار المستندة إلى المنتجات.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 8bde88f5f2d00c09129c6a9363c09f6f6ad1dd90
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284072"
---
# <a name="product-based-quote-lines"></a><span data-ttu-id="f5225-103">بنود عرض أسعار يستند إلى منتج</span><span class="sxs-lookup"><span data-stu-id="f5225-103">Product-based quote lines</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


<span data-ttu-id="f5225-104">يمكنك إنشاء بنود عرض أسعار مستندة إلى المنتجات في Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f5225-104">You can create product-based quote lines in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="f5225-105">يمكن أن تكون بنود عرض الأسعار المستندة إلى المنتج خطوط "للكتابة"، أو يمكن أن تكون عناصر من كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="f5225-105">Product-based quote lines can be "write-in" lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="f5225-106">كتالوج المنتجات</span><span class="sxs-lookup"><span data-stu-id="f5225-106">Product catalog</span></span>

<span data-ttu-id="f5225-107">تحتوي المنتجات الموجودة في كتالوج منتج Dynamics 365 على وحدة ومجموعة وحدة افتراضية.</span><span class="sxs-lookup"><span data-stu-id="f5225-107">The products in a Dynamics 365 product catalog have a default unit and unit group.</span></span> <span data-ttu-id="f5225-108">إذا كانت هناك عدة منتجات تشترك في نفس مجموعة السمات ، فيمكنك إنشاء مجموعة منتجات لديها هذه السمات أيضًا.</span><span class="sxs-lookup"><span data-stu-id="f5225-108">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="f5225-109">جميع المنتجات في عائلة منتج واحد ترث نفس مجموعة السمات.</span><span class="sxs-lookup"><span data-stu-id="f5225-109">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="f5225-110">على سبيل المثال ، تبيع الشركة تراخيص الاشتراك لمجموعة متنوعة من البرامج.</span><span class="sxs-lookup"><span data-stu-id="f5225-110">For example, a company sells subscription licenses for a variety of software.</span></span> <span data-ttu-id="f5225-111">تشتمل كافة برامج الاشتراك على السمتين التاليتين:</span><span class="sxs-lookup"><span data-stu-id="f5225-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="f5225-112">عدد المستخدمين</span><span class="sxs-lookup"><span data-stu-id="f5225-112">Number of users</span></span> 
- <span data-ttu-id="f5225-113">مدة الاشتراك (بالشهور)</span><span class="sxs-lookup"><span data-stu-id="f5225-113">Subscription duration (in months)</span></span>

<span data-ttu-id="f5225-114">هناك طريقة جيدة للحفاظ على هذا النوع من الكتالوجات هي إنشاء مجموعة منتجات تسمى **برامج الاشتراك**، والتي تحتوي على **عدد المستخدمين** و **مدة الاشتراك** كسمات.</span><span class="sxs-lookup"><span data-stu-id="f5225-114">A good way to maintain this type of catalog is to create a product family that is named **Subscription Software**, and that has **Number of users** and **Subscription duration** as attributes.</span></span> <span data-ttu-id="f5225-115">يمكنك بعد ذلك إضافة منتجات فردية، مثل **Dynamics 365 Sales** أو **Dynamics 365 Field Service** إلى مجموعة منتجات **برامج الاشتراك**.</span><span class="sxs-lookup"><span data-stu-id="f5225-115">You can then add individual products, such as **Dynamics 365 Sales** or **Dynamics 365 Field Service** to the **Subscription Software** product family.</span></span>

## <a name="adding-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="f5225-116">إضافة عناصر كتالوج المنتجات إلى عرض أسعار مشروع</span><span class="sxs-lookup"><span data-stu-id="f5225-116">Adding product catalog items to a project quote</span></span>

<span data-ttu-id="f5225-117">تحتوي صفحات عرض أسعار المشروع وعقد المشروع على أقسام لنوعين من البنود: البنود المستندة إلى المشروع والبنود المستندة إلى المنتج.</span><span class="sxs-lookup"><span data-stu-id="f5225-117">Project quote and project contract pages have sections for two types of lines: project-based lines and product-based lines.</span></span> <span data-ttu-id="f5225-118">بالنسبة للبنود المستندة إلى المنتجات، يُستخدم Dynamics 365 لإضافة عناصر من كتالوج منتجات إلى عرض أسعار.</span><span class="sxs-lookup"><span data-stu-id="f5225-118">For product-based lines, Dynamics 365 is used to add items from a product catalog to a quote.</span></span> <span data-ttu-id="f5225-119">تتضمن القائمة المنسدلة الموجودة في سطر عرض الأسعار أو سطر عقد المشروع جميع المنتجات والوحدات الموجودة في قائمة أسعار المنتج المرفقة بسعر العرض أو عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f5225-119">The drop-down list on the quote line or project contract line includes all the products and units in the product price list that is attached to the quote or project contract.</span></span> <span data-ttu-id="f5225-120">يمكنك أيضًا إضافة المنتجات التي لا تكون جزءًا من قائمة أسعار منتجات عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f5225-120">You can also add products that aren't part of quote's product price list.</span></span>

<span data-ttu-id="f5225-121">بالإضافة إلى ذلك ، يمكنك اختيار المنتجات من قوائم الأسعار الأخرى ، أو يمكنك تحديد المنتجات مباشرة من كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="f5225-121">Additionally, you can select products from other price lists, or you can select products directly from the product catalog.</span></span> <span data-ttu-id="f5225-122">عند تحديد المنتجات مباشرةً من كتالوج المنتجات ، يتم استخدام قائمة الأسعار الافتراضية لهذا المنتج للحصول على سعر مبيعات المنتج.</span><span class="sxs-lookup"><span data-stu-id="f5225-122">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="f5225-123">إذا لم يتم تعيين قائمة أسعار افتراضية، سيتم تعيين السعر إلى 0 (صفر).</span><span class="sxs-lookup"><span data-stu-id="f5225-123">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="f5225-124">إذا كان بند عرض أسعار يعتمد على كتالوج المنتجات، فيمكنك تجاوز سعر البيع مباشرة على بند عرض أسعار.</span><span class="sxs-lookup"><span data-stu-id="f5225-124">If a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="f5225-125">لاحظ أن بند عرض الأسعار في Dynamics 365 يحتوي على حقل **تسعير**.</span><span class="sxs-lookup"><span data-stu-id="f5225-125">Note that a quote line in Dynamics 365 has a **Pricing** field.</span></span> <span data-ttu-id="f5225-126">هناك قيمتان متوفرتان:</span><span class="sxs-lookup"><span data-stu-id="f5225-126">Two values are available:</span></span>

- <span data-ttu-id="f5225-127">تجاوز التسعير</span><span class="sxs-lookup"><span data-stu-id="f5225-127">Override pricing</span></span>  
- <span data-ttu-id="f5225-128">استخدام الافتراضي</span><span class="sxs-lookup"><span data-stu-id="f5225-128">Use default</span></span>

<span data-ttu-id="f5225-129">إذا قمت بتعيين هذا الحقل **تجاوز التسعير**، فلا يقوم Dynamics 365 بتعيين سعر افتراضي.</span><span class="sxs-lookup"><span data-stu-id="f5225-129">If you set this field to **Override pricing**, Dynamics 365 doesn't set a default price.</span></span> <span data-ttu-id="f5225-130">يجب عليك إدخال سعر للمنتج في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f5225-130">You must enter a price for the product on the quote line.</span></span> <span data-ttu-id="f5225-131">إذا قمت بتعيين هذا الحقل إلى **الاستخدام الافتراضي**، يستخدم Dynamics 365 سعر المبيعات الافتراضي ويقوم بتأمين الحقل لمنع التحرير.</span><span class="sxs-lookup"><span data-stu-id="f5225-131">If you set this field to **Use default**, Dynamics 365 uses the default sales price and locks the field to prevent editing.</span></span>

<span data-ttu-id="f5225-132">بعد تثبيت PSA، يتم إدخال أسعار المبيعات الافتراضية في البنود المستندة إلى المنتج في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f5225-132">After you install PSA, default sales prices are entered on the product-based lines on a quote.</span></span> <span data-ttu-id="f5225-133">ثم يتم تعيين حقل **التسعير** إلى **تجاوز التسعير** حتى يمكنك تحرير السعر الافتراضي في بنود عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f5225-133">The **Pricing** field is then set to **Override pricing** so that you can edit the default price on the quote lines.</span></span>

> ![تعيين تجاوز التسعير](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a><span data-ttu-id="f5225-135">عوامل الكمية للمنتجات</span><span class="sxs-lookup"><span data-stu-id="f5225-135">Quantity factors for products</span></span>

<span data-ttu-id="f5225-136">يستخدم PSA عوامل الكمية لدعم بيع المنتجات المستندة إلى الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="f5225-136">PSA uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="f5225-137">بالنسبة للمنتجات المستندة إلى الاشتراك، يتم التعبير عن الكمية الموجودة في عرض الأسعار أو سطر عقد المشروع كعدد من أشهر المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="f5225-137">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="f5225-138">وعادةً ما يتم تخزين برنامج الاشتراك في الكتالوج كالسعر لكل مستخدم في الشهر.</span><span class="sxs-lookup"><span data-stu-id="f5225-138">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="f5225-139">ومع ذلك، يمكنك استخدام أوصاف الوقت الأخرى بدلا من ذلك.</span><span class="sxs-lookup"><span data-stu-id="f5225-139">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="f5225-140">وأثناء عمليه المبيعات، عادةً ما يكون السعر الموجود في بند عرض الأسعار هو السعر لكل مستخدم والذي تم التفاوض عليه بواسطة مندوب مبيعات IT.</span><span class="sxs-lookup"><span data-stu-id="f5225-140">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="f5225-141">تحتوي كل صفقة على عدد مختلف من المستخدمين وعدد من أشهر الاشتراكات المختلفة.</span><span class="sxs-lookup"><span data-stu-id="f5225-141">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="f5225-142">الكمية المستخدمة لحساب مبلغ سطر عرض الأسعار هي حاصل ضرب عدد المستخدمين وعدد أشهر الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="f5225-142">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="f5225-143">ولدعم هذا النوع من البيع، قدم PSA مفهوم عوامل الكمية.</span><span class="sxs-lookup"><span data-stu-id="f5225-143">To support this type of sale, PSA introduced the concept of quantity factors.</span></span> <span data-ttu-id="f5225-144">تعتمد عوامل الكمية على سمات المنتج في Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f5225-144">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="f5225-145">عندما تقوم بتكوين خصائص محددة لأحد المنتجات، يتيح لك PSA وضع علامة على مجموعة فرعية من هذه الخصائص، أو كل الخصائص، كعوامل كمية.</span><span class="sxs-lookup"><span data-stu-id="f5225-145">When you configure specific properties for a product, PSA lets you flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="f5225-146">يتحقق PSA من أن الخصائص الرقمية أو خصائص المنتج التي تحتوي على نوع بيانات رقمية فقط يتم تمييزها كعوامل كمية.</span><span class="sxs-lookup"><span data-stu-id="f5225-146">PSA validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="f5225-147">عندما يكون المنتج الذي تم تكوين عوامل الكمية له قد تمت إضافته إلى بند عرض أسعار، يصبح حقل **الكمية** في بند عرض الأسعار حقلاً للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="f5225-147">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="f5225-148">بعد إدخال قيم لخصائص المنتج التي عوامل الكمية، يقوم PSA بحساب كمية بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f5225-148">After you enter values for product properties that are quantity factors, PSA computes the quantity of the quote line.</span></span>

<span data-ttu-id="f5225-149">على سبيل المثال، قد يشتمل Dynamics 365 على الخصائص التالية:</span><span class="sxs-lookup"><span data-stu-id="f5225-149">For example, Dynamics 365 might have the following properties:</span></span> 

- <span data-ttu-id="f5225-150">**عدد المستخدمين** - عدد المستخدمين</span><span class="sxs-lookup"><span data-stu-id="f5225-150">**No of users** - The number of users</span></span> 
- <span data-ttu-id="f5225-151">**عدد الأشهر** - عدد أشهر الاشتراك</span><span class="sxs-lookup"><span data-stu-id="f5225-151">**No of Months** - The number of subscription months</span></span>
- <span data-ttu-id="f5225-152">**SKU للمنتج**</span><span class="sxs-lookup"><span data-stu-id="f5225-152">**Product SKU**</span></span> 

<span data-ttu-id="f5225-153">يمكن تمييز الخاصيتين **عدد المستخدمين** و **عجج الأشهر** كعوامل كمية من خلال تحرير خصائص بند المنتج.</span><span class="sxs-lookup"><span data-stu-id="f5225-153">Tne **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 

> ![وضع علامة على عدد المستخدمين وعدد الأشهر كعوامل جودة](media/basic-guide-11.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]