---
title: إدارة الوحدات المعقدة لكل مستخدم، لكل شهر لبنود عرض الأسعار المستندة إلى المنتج - خفيف
description: يقدم هذا الموضوع معلومات حول إدارة الوحدات المعقدة لبنود عروض الأسعار المستندة إلى المنتج.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2ee46da2f663ef4f5f8fc7f9f89b6fcfd09a1798
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175560"
---
# <a name="managing-complex-units-such-as-per-user-per-month-for-product-based-quote-lines---lite"></a><span data-ttu-id="ad179-103">إدارة الوحدات المعقدة لكل مستخدم، لكل شهر لبنود عرض الأسعار المستندة إلى المنتج - خفيف</span><span class="sxs-lookup"><span data-stu-id="ad179-103">Managing complex units such as per-user, per-month for product-based quote lines - lite</span></span>

<span data-ttu-id="ad179-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="ad179-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ad179-105">يستخدم Dynamics 365 Project Operations عوامل الكمية لدعم بيع المنتجات المستندة إلى الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="ad179-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="ad179-106">بالنسبة للمنتجات المستندة إلى الاشتراك، يتم التعبير عن الكمية الموجودة في عرض الأسعار أو سطر عقد المشروع كعدد من أشهر المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="ad179-106">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="ad179-107">وعادةً ما يتم تخزين برنامج الاشتراك في الكتالوج كالسعر لكل مستخدم في الشهر.</span><span class="sxs-lookup"><span data-stu-id="ad179-107">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="ad179-108">وأثناء عمليه المبيعات، عادةً ما يكون السعر الموجود في بند عرض الأسعار هو السعر لكل مستخدم والذي تم التفاوض عليه بواسطة مندوب مبيعات IT.</span><span class="sxs-lookup"><span data-stu-id="ad179-108">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="ad179-109">تحتوي كل صفقة على عدد مختلف من المستخدمين وعدد من أشهر الاشتراكات المختلفة.</span><span class="sxs-lookup"><span data-stu-id="ad179-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="ad179-110">الكمية المستخدمة لحساب مبلغ بند عرض الأسعار هي حاصل ضرب عدد المستخدمين وعدد أشهر الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="ad179-110">The quantity used to compute the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="ad179-111">ولدعم هذا النوع من البيع، قدم Project Operations مفهوم عوامل الكمية.</span><span class="sxs-lookup"><span data-stu-id="ad179-111">To support this type of sale, Project Operations introduced the concept of quantity factors.</span></span> <span data-ttu-id="ad179-112">تعتمد عوامل الكمية على سمات المنتج في Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="ad179-112">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="ad179-113">عندما تقوم بتكوين خصائص محددة لأحد المنتجات، يتيح لك Project Operations وضع علامة على مجموعة فرعية من هذه الخصائص، أو كل الخصائص، كعوامل كمية.</span><span class="sxs-lookup"><span data-stu-id="ad179-113">When you configure specific properties for a product, Project Operations lets you flag a subset, or all of the properties, as quantity factors.</span></span>

<span data-ttu-id="ad179-114">يتحقق Project Operations من أن الخصائص الرقمية أو خصائص المنتج التي تحتوي على نوع بيانات رقمية فقط يتم تمييزها كعوامل كمية.</span><span class="sxs-lookup"><span data-stu-id="ad179-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="ad179-115">عندما تقوم بإضافة منتج يحتوي على عوامل كمية إلى بند عرض أسعار، يصبح حقل **الكمية** للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="ad179-115">When you add a product with quantity factors to a quote line, the **Quantity** field becomes read-only.</span></span> <span data-ttu-id="ad179-116">بعد إدخال قيم لخصائص المنتج التي هي عوامل الكمية، يحسب كمية بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="ad179-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the quote line.</span></span>

<span data-ttu-id="ad179-117">على سبيل المثال، قد يشتمل Dynamics 365 Sales على الخصائص التالية:</span><span class="sxs-lookup"><span data-stu-id="ad179-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="ad179-118">**عدد المستخدمين**: عدد المستخدمين</span><span class="sxs-lookup"><span data-stu-id="ad179-118">**No of users**: The number of users</span></span>
- <span data-ttu-id="ad179-119">**عدد الأشهر**: عدد أشهر الاشتراك</span><span class="sxs-lookup"><span data-stu-id="ad179-119">**No of Months**: The number of subscription months</span></span>
- <span data-ttu-id="ad179-120">**SKU للمنتج**</span><span class="sxs-lookup"><span data-stu-id="ad179-120">**Product SKU**</span></span>

<span data-ttu-id="ad179-121">يمكنك تعليم الخاصيتين **عدد المستخدمين** و **عدد الأشهر** كعوامل كمية من خلال تحرير خصائص بند المنتج.</span><span class="sxs-lookup"><span data-stu-id="ad179-121">You can flag the **No of Users** and **No of Months** properties as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="ad179-122">لإنشاء عوامل كمية من خصائص المنتج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ad179-122">To create Quantity factors from Product properties, follow these steps:</span></span>

1. <span data-ttu-id="ad179-123">في جزء التنقل الأيسر في Project Operations، انتقل إلى **المبيعات** > **المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="ad179-123">On the Project Operations left navigation pane, go to **Sales** > **Products**.</span></span>
2. <span data-ttu-id="ad179-124">افتح المنتج الذي يتعين عليك تكوين عوامل الكمية له.</span><span class="sxs-lookup"><span data-stu-id="ad179-124">Open the product for which you need to configure quantity factors.</span></span> <span data-ttu-id="ad179-125">تأكد من أن المنتج له خصائص تم تكوينها بالفعل.</span><span class="sxs-lookup"><span data-stu-id="ad179-125">Make sure the product has properties already configured.</span></span>
3. <span data-ttu-id="ad179-126">في صفحة **معلومات المشروع** الخاصة بالمنتج، حدد علامة التبويب **عوامل الكمية**.</span><span class="sxs-lookup"><span data-stu-id="ad179-126">On the **Project Information** page for the Product, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="ad179-127">في جزء الشبكة الفرعية، حدد **+ حساب حقل جديد**.</span><span class="sxs-lookup"><span data-stu-id="ad179-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="ad179-128">ادخل اسم معامل الكمية وحدد قيمة الخاصية التي يتم تعيينها لحساب الحقل.</span><span class="sxs-lookup"><span data-stu-id="ad179-128">Enter the name of the Quantity factor and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="ad179-129">حفظ النموذج وإغلاقه.</span><span class="sxs-lookup"><span data-stu-id="ad179-129">Save and close the form.</span></span> <span data-ttu-id="ad179-130">كرر هذه الخطوات مع كافة الخصائص لاستخدامها لحساب الكمية لبند عرض الأسعار المستند إلى منتج.</span><span class="sxs-lookup"><span data-stu-id="ad179-130">Repeat these steps for all properties to use for computing the quantity for the product-based quote line.</span></span>

<span data-ttu-id="ad179-131">عندما تقوم بإنشاء بند عرض أسعار يستند إلى أساس المنتج لمنتج ما، سيتم تأمين كمية بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="ad179-131">When you create a product-based quote line for a product, the quantity of the quote line will be locked.</span></span> <span data-ttu-id="ad179-132">سيتم حساب الكمية كمنتج لقيم الخصائص التي تقوم بإدخالها لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="ad179-132">The quantity will be computed as a product of the property values that you input for that quote line.</span></span>
