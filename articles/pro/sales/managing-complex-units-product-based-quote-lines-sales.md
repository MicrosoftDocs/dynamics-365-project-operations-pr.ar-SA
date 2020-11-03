---
title: إدارة الوحدات المعقدة لكل مستخدم، لكل شهر لبنود عرض الأسعار المستندة إلى المنتج
description: يقدم هذا الموضوع معلومات حول إدارة الوحدات المعقدة لبنود عروض الأسعار المستندة إلى المنتج.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 741230e69302138cce8f7379f520f7178e1c80af
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070576"
---
# <a name="managing-complex-units-such-as-per-user-per-month-for-product-based-quote-lines"></a><span data-ttu-id="5bff4-103">إدارة الوحدات المعقدة لكل مستخدم، لكل شهر لبنود عرض الأسعار المستندة إلى المنتج</span><span class="sxs-lookup"><span data-stu-id="5bff4-103">Managing complex units such as per-user, per-month for product-based quote lines</span></span>

<span data-ttu-id="5bff4-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="5bff4-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5bff4-105">يستخدم Dynamics 365 Project Operations عوامل الكمية لدعم بيع المنتجات المستندة إلى الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="5bff4-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="5bff4-106">بالنسبة للمنتجات المستندة إلى الاشتراك، يتم التعبير عن الكمية الموجودة في عرض الأسعار أو سطر عقد المشروع كعدد من أشهر المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="5bff4-106">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="5bff4-107">وعادةً ما يتم تخزين برنامج الاشتراك في الكتالوج كالسعر لكل مستخدم في الشهر.</span><span class="sxs-lookup"><span data-stu-id="5bff4-107">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="5bff4-108">وأثناء عمليه المبيعات، عادةً ما يكون السعر الموجود في بند عرض الأسعار هو السعر لكل مستخدم والذي تم التفاوض عليه بواسطة مندوب مبيعات IT.</span><span class="sxs-lookup"><span data-stu-id="5bff4-108">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="5bff4-109">تحتوي كل صفقة على عدد مختلف من المستخدمين وعدد من أشهر الاشتراكات المختلفة.</span><span class="sxs-lookup"><span data-stu-id="5bff4-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="5bff4-110">الكمية المستخدمة لحساب مبلغ بند عرض الأسعار هي حاصل ضرب عدد المستخدمين وعدد أشهر الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="5bff4-110">The quantity used to compute the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="5bff4-111">ولدعم هذا النوع من البيع، قدم Project Operations مفهوم عوامل الكمية.</span><span class="sxs-lookup"><span data-stu-id="5bff4-111">To support this type of sale, Project Operations introduced the concept of quantity factors.</span></span> <span data-ttu-id="5bff4-112">تعتمد عوامل الكمية على سمات المنتج في Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5bff4-112">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="5bff4-113">عندما تقوم بتكوين خصائص محددة لأحد المنتجات، يتيح لك Project Operations وضع علامة على مجموعة فرعية من هذه الخصائص، أو كل الخصائص، كعوامل كمية.</span><span class="sxs-lookup"><span data-stu-id="5bff4-113">When you configure specific properties for a product, Project Operations lets you flag a subset, or all of the properties, as quantity factors.</span></span>

<span data-ttu-id="5bff4-114">يتحقق Project Operations من أن الخصائص الرقمية أو خصائص المنتج التي تحتوي على نوع بيانات رقمية فقط يتم تمييزها كعوامل كمية.</span><span class="sxs-lookup"><span data-stu-id="5bff4-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="5bff4-115">عندما تقوم بإضافة منتج يحتوي على عوامل كمية إلى بند عرض أسعار، يصبح حقل **الكمية** للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="5bff4-115">When you add a product with quantity factors to a quote line, the **Quantity** field becomes read-only.</span></span> <span data-ttu-id="5bff4-116">بعد إدخال قيم لخصائص المنتج التي هي عوامل الكمية، يحسب كمية بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="5bff4-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the quote line.</span></span>

<span data-ttu-id="5bff4-117">على سبيل المثال، قد يشتمل Dynamics 365 Sales على الخصائص التالية:</span><span class="sxs-lookup"><span data-stu-id="5bff4-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="5bff4-118">**عدد المستخدمين** : عدد المستخدمين</span><span class="sxs-lookup"><span data-stu-id="5bff4-118">**No of users** : The number of users</span></span>
- <span data-ttu-id="5bff4-119">**عدد الأشهر** : عدد أشهر الاشتراك</span><span class="sxs-lookup"><span data-stu-id="5bff4-119">**No of Months** : The number of subscription months</span></span>
- <span data-ttu-id="5bff4-120">**SKU للمنتج**</span><span class="sxs-lookup"><span data-stu-id="5bff4-120">**Product SKU**</span></span>

<span data-ttu-id="5bff4-121">يمكنك تعليم الخاصيتين **عدد المستخدمين** و **عدد الأشهر** كعوامل كمية من خلال تحرير خصائص بند المنتج.</span><span class="sxs-lookup"><span data-stu-id="5bff4-121">You can flag the **No of Users** and **No of Months** properties as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="5bff4-122">لإنشاء عوامل كمية من خصائص المنتج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="5bff4-122">To create Quantity factors from Product properties, follow these steps:</span></span>

1. <span data-ttu-id="5bff4-123">في جزء التنقل الأيسر في Project Operations، انتقل إلى **المبيعات** > **المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="5bff4-123">On the Project Operations left navigation pane, go to **Sales** > **Products**.</span></span>
2. <span data-ttu-id="5bff4-124">افتح المنتج الذي يتعين عليك تكوين عوامل الكمية له.</span><span class="sxs-lookup"><span data-stu-id="5bff4-124">Open the product for which you need to configure quantity factors.</span></span> <span data-ttu-id="5bff4-125">تأكد من أن المنتج له خصائص تم تكوينها بالفعل.</span><span class="sxs-lookup"><span data-stu-id="5bff4-125">Make sure the product has properties already configured.</span></span>
3. <span data-ttu-id="5bff4-126">في صفحة **معلومات المشروع** الخاصة بالمنتج، حدد علامة التبويب **عوامل الكمية**.</span><span class="sxs-lookup"><span data-stu-id="5bff4-126">On the **Project Information** page for the Product, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="5bff4-127">في جزء الشبكة الفرعية، حدد **+ حساب حقل جديد**.</span><span class="sxs-lookup"><span data-stu-id="5bff4-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="5bff4-128">ادخل اسم معامل الكمية وحدد قيمة الخاصية التي يتم تعيينها لحساب الحقل.</span><span class="sxs-lookup"><span data-stu-id="5bff4-128">Enter the name of the Quantity factor and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="5bff4-129">حفظ النموذج وإغلاقه.</span><span class="sxs-lookup"><span data-stu-id="5bff4-129">Save and close the form.</span></span> <span data-ttu-id="5bff4-130">كرر هذه الخطوات مع كافة الخصائص لاستخدامها لحساب الكمية لبند عرض الأسعار المستند إلى منتج.</span><span class="sxs-lookup"><span data-stu-id="5bff4-130">Repeat these steps for all properties to use for computing the quantity for the product-based quote line.</span></span>

<span data-ttu-id="5bff4-131">عندما تقوم بإنشاء بند عرض أسعار يستند إلى أساس المنتج لمنتج ما، سيتم تأمين كمية بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="5bff4-131">When you create a product-based quote line for a product, the quantity of the quote line will be locked.</span></span> <span data-ttu-id="5bff4-132">سيتم حساب الكمية كمنتج لقيم الخصائص التي تقوم بإدخالها لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="5bff4-132">The quantity will be computed as a product of the property values that you input for that quote line.</span></span>
