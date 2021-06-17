---
title: قوائم أسعار المنتجات
description: يقدم هذا الموضوع معلومات حول قوائم الأسعار في تسعير الكتالوج المستخدمة لعروض أسعار وعقود المشروع.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 02d274725983e50adc35a4cae1ac60c35be346a4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004920"
---
# <a name="product-price-lists"></a><span data-ttu-id="f433b-103">قوائم أسعار المنتجات</span><span class="sxs-lookup"><span data-stu-id="f433b-103">Product price lists</span></span>

<span data-ttu-id="f433b-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="f433b-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

 <span data-ttu-id="f433b-105">في Project Operations، تدعم **قوائم أسعار المنتج** وكيانات بنود قائمة الأسعار ذات الصلة الوظائف الخاصة بتسعير المنتجات على عرض الأسعار القائم على المشروع وشروط تعاقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f433b-105">In Project Operations, **Product price lists** and related price list item entities support functionality for pricing products on product-based quote and contract lines.</span></span> <span data-ttu-id="f433b-106">بالنسبة للمنتجات المستخدمة في المشروعات، يتم استخدام سجلات بنود قائمة الأسعار لقوائم أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="f433b-106">For products used on projects, the price list item records for project price lists are used.</span></span> 

<span data-ttu-id="f433b-107">ينبغي إعداد المنتجات بحيث يكون لها قوائم تكلفة وأسعار افتراضية في كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="f433b-107">Products should be set up so that they have default cost and price lists in the product catalog.</span></span> <span data-ttu-id="f433b-108">استخدم قائمة الأسعار والتكلفة القياسية والتكلفة الحالية لتكوين التكلفة الافتراضية وأسعار القوائم.</span><span class="sxs-lookup"><span data-stu-id="f433b-108">Use the list price, standard cost, and current cost to configure default cost and list prices.</span></span> <span data-ttu-id="f433b-109">يتم استخدام الأسعار الافتراضية للقائمة في بند عرض الأسعار أو بند عقد المشروع فقط عندما لا يتمكن النظام من العثور على بند قائمة أسعار لهذا المنتج في قائمة أسعار المنتجات الخاصة بعرض الأسعار أو عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f433b-109">The default list prices are used on a quote line or a project contract line only when the system can't find a price list line for that product in the product price list for the quote or project contract.</span></span>

<span data-ttu-id="f433b-110">يمكن تغيير سعر تكلفة بنود كتالوجات المنتجات بين عروض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f433b-110">The cost price of product catalog lines can be changed between quotes.</span></span> <span data-ttu-id="f433b-111">هذه الإمكانية مهمة، لأنه في حالة عدم تعقب التكاليف بشكل دقيق، لا يمكنك تحديد الأرباح التشغيلية في مشاركات المشاريع.</span><span class="sxs-lookup"><span data-stu-id="f433b-111">This capability is important, because if you don't accurately track costs, you can't determine operational profits on project engagements.</span></span> <span data-ttu-id="f433b-112">بشكل افتراضي، يتم استخدام التكلفة القياسية للمنتج كسعر التكلفة.</span><span class="sxs-lookup"><span data-stu-id="f433b-112">By default, the standard cost of the product is used as the cost price.</span></span> <span data-ttu-id="f433b-113">ومع ذلك، يمكن تحديث سعر التكلفة الافتراضي في بند عرض الأسعار في حالة وجود سعر تكلفة مختلف لعرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f433b-113">However, the default cost price can be updated on the quote line if there's a different cost price for that quote.</span></span>

## <a name="price-list-items"></a><span data-ttu-id="f433b-114">بنود قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="f433b-114">Price list items</span></span>

<span data-ttu-id="f433b-115">يمكنك إضافة منتجات من كتالوج منتجات إلى قوائم أسعار مختلفة.</span><span class="sxs-lookup"><span data-stu-id="f433b-115">You can add products from a product catalog to different price lists.</span></span> <span data-ttu-id="f433b-116">تشير بنود قائمة الأسعار الخاصة بالمنتجات إلى وحدة محددة دائما.</span><span class="sxs-lookup"><span data-stu-id="f433b-116">Price list lines for products always reference a specific unit.</span></span> <span data-ttu-id="f433b-117">يمكن تكوين أسعار أحد المنتجات في بنود قائمة الأسعار على أنها مبلغ عملة.</span><span class="sxs-lookup"><span data-stu-id="f433b-117">Pricing for a product on price list items can be configured as a currency amount.</span></span> <span data-ttu-id="f433b-118">بدلاً من ذلك ، يمكن تكوينه كدالة لسعر القائمة أو التكلفة الحالية أو التكلفة القياسية.</span><span class="sxs-lookup"><span data-stu-id="f433b-118">Alternatively, it can be configured as a function of the list price, current cost, or standard cost.</span></span>

<span data-ttu-id="f433b-119">تدعم وظائف التسعير خيارات التقريب المختلفة عندما يتم تكوين أسعار المنتجات كوظيفة لقائمة الأسعار أو التكلفة القياسية أو التكلفة الحالية.</span><span class="sxs-lookup"><span data-stu-id="f433b-119">Pricing functionality supports various rounding options when product prices are configured as a function of the list price, standard cost, or current cost.</span></span> <span data-ttu-id="f433b-120">بالإضافة إلى الاستفادة من طرق التسعير المتعددة وخيارات التقريب ، يمكنك ربط قوائم الخصم بعناصر قائمة الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f433b-120">In addition to taking advantage of multiple pricing methods and rounding options, you can associate discount lists with price list items.</span></span> 

 
## <a name="default-product-price-list"></a><span data-ttu-id="f433b-121">قائمة أسعار المنتجات الافتراضية</span><span class="sxs-lookup"><span data-stu-id="f433b-121">Default product price list</span></span>
<span data-ttu-id="f433b-122">يحتوي كل سجل عميل على حقل **قائمة الأسعار الافتراضية**، حيث يمكنك تحديد قائمة أسعار تطابق العملة الخاصة بالعميل.</span><span class="sxs-lookup"><span data-stu-id="f433b-122">Each customer record has a **Default Price List** field, where you can specify a price list that matches the currency of the customer.</span></span> <span data-ttu-id="f433b-123">لا يتم إدخال قيمة افتراضية تلقائيًا في هذا الحقل.</span><span class="sxs-lookup"><span data-stu-id="f433b-123">A default value isn't automatically entered in this field.</span></span> <span data-ttu-id="f433b-124">عند وجود اتفاقية تسعير مخصصة مع عميل محدد، يمكنك استخدام هذا الحقل لربط قائمة أسعار بهذا العميل.</span><span class="sxs-lookup"><span data-stu-id="f433b-124">When a custom pricing agreement with a specific customer exists, you can use this field to associate a price list with that customer.</span></span>

<span data-ttu-id="f433b-125">تستخدم كيانات الفرصة وعرض الأسعار وعقد المشروع الترتيب التالي لإدخال قوائم أسعار المنتجات الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="f433b-125">The Opportunity, Quote, and Project Contract entities use the following order to enter default product price lists.</span></span> <span data-ttu-id="f433b-126">يتم استخدام نفس الترتيب لقوائم أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="f433b-126">The same order is used for project price lists.</span></span>

1.  <span data-ttu-id="f433b-127">اقتباس</span><span class="sxs-lookup"><span data-stu-id="f433b-127">Quote</span></span>
2.  <span data-ttu-id="f433b-128">الفرصة</span><span class="sxs-lookup"><span data-stu-id="f433b-128">Opportunity</span></span>
3.  <span data-ttu-id="f433b-129">العميل</span><span class="sxs-lookup"><span data-stu-id="f433b-129">Customer</span></span>
4.  <span data-ttu-id="f433b-130">الإعدادات العمومية</span><span class="sxs-lookup"><span data-stu-id="f433b-130">Global settings</span></span> 

<span data-ttu-id="f433b-131">وبشكل افتراضي، يسرد حقل **المنتج** في بند عرض الأسعار كافة المنتجات النشطة في قائمة أسعار المنتجات الخاصة بعرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f433b-131">By default, the **Product** field on the quote line lists all the active products in the product price list of the quote.</span></span> <span data-ttu-id="f433b-132">إذا تم إلغاء تنشيط منتج، أو إذا كان منتج مسودة، فلن يتم سرده، حتى ولو كان موجودًا في قائمة الأسعار.</span><span class="sxs-lookup"><span data-stu-id="f433b-132">If a product has been inactivated, or if it's a draft product, it isn't listed, even if it's in the price list.</span></span> 

<span data-ttu-id="f433b-133">تتم إضافة بنود كتالوج المنتجات كبنود فاتورة في أول فاتورة تم إنشاؤها لعقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f433b-133">Product catalog lines are added as invoice lines on the first invoice that is created for a project contract.</span></span> <span data-ttu-id="f433b-134">في فاتورة المسودة، يمكن حذف بنود الفاتورة هذه.</span><span class="sxs-lookup"><span data-stu-id="f433b-134">On a draft invoice, those invoice lines can be deleted.</span></span> <span data-ttu-id="f433b-135">وفي هذه الحالة، ستظهر البنود في فاتورة تاليه حتى تتم فوترتها، أو حتى يتم إرسال الفاتورة إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="f433b-135">In that case, the lines will appear on a subsequent invoice until they are invoiced, or until the invoice is sent to the customer.</span></span> <span data-ttu-id="f433b-136">لا يمكنك فوترة كمية جزئية من بند فاتورة منتج.</span><span class="sxs-lookup"><span data-stu-id="f433b-136">You can't invoice a partial quantity of a product invoice line.</span></span> <span data-ttu-id="f433b-137">عند فوترة بنود المنتج من عقد المشروع، يتم إنشاء القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="f433b-137">When the product lines from the project contract are invoiced, actuals are created.</span></span> <span data-ttu-id="f433b-138">ومع ذلك، لا يتم ربط هذه القيم الفعلية بكيان المشروع ذي الصلة.</span><span class="sxs-lookup"><span data-stu-id="f433b-138">However, those actuals aren't linked to the related project entity.</span></span> <span data-ttu-id="f433b-139">وبمعني آخر، تكون بنود عقد المشروع المستندة إلى المنتج مستقلة عن أي استخدام قائم على المشروع.</span><span class="sxs-lookup"><span data-stu-id="f433b-139">In other words, product-based project contract lines are independent of any project-based use.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
