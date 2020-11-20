---
title: إدارة الوحدات المعقدة لشروط التعاقد المستندة إلى المنتج - خفيف
description: يوفر هذا الموضوع معلومات حول دعم المنتجات المستندة إلى الاشتراك.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a58a13c8186f36e6031fe3c6f3c3a57ea920ac9e
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177360"
---
# <a name="manage-complex-units-for-product-based-contract-lines---lite"></a><span data-ttu-id="ea10c-103">إدارة الوحدات المعقدة لشروط التعاقد المستندة إلى المنتج - خفيف</span><span class="sxs-lookup"><span data-stu-id="ea10c-103">Manage complex units for product-based contract lines - lite</span></span>

<span data-ttu-id="ea10c-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="ea10c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ea10c-105">يستخدم Dynamics 365 Project Operations عوامل الكمية لدعم بيع المنتجات المستندة إلى الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="ea10c-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="ea10c-106">بالنسبة للمنتجات المستندة إلى الاشتراك، يتم التعبير عن الكمية الموجودة في العقد أو شرط تعاقد المشروع كعدد من أشهر المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="ea10c-106">For subscription-based products, the quantity on the contract or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="ea10c-107">يتم تخزين سعر برنامج الاشتراك في الكتالوج كالسعر لكل مستخدم في الشهر.</span><span class="sxs-lookup"><span data-stu-id="ea10c-107">The price of subscription software is stored in the catalog as the price per-user, per-month.</span></span> <span data-ttu-id="ea10c-108">أثناء عملية المبيعات، عادةً ما يكون السعر الموجود في شرط التعاقد السعر لكل مستخدم في الشهر الذي تم التفاوض عليه بواسطة مندوب المبيعات.</span><span class="sxs-lookup"><span data-stu-id="ea10c-108">During the sales process, the price on the contract line is usually the per-user, per-month price that was negotiated and discounted by the sales agent.</span></span> <span data-ttu-id="ea10c-109">تحتوي كل صفقة على عدد مختلف من المستخدمين وعدد من أشهر الاشتراكات المختلفة.</span><span class="sxs-lookup"><span data-stu-id="ea10c-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="ea10c-110">الكمية المستخدمة لحساب مبلغ شرط التعاقد هي حاصل ضرب عدد المستخدمين وعدد أشهر الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="ea10c-110">The quantity used to calculate the amount of the contract line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="ea10c-111">ولدعم هذا النوع من البيع، يدعم Project Operations مفهوم *عوامل الكمية*.</span><span class="sxs-lookup"><span data-stu-id="ea10c-111">To support this type of sale, Project Operations supports the concept of *quantity factors*.</span></span> <span data-ttu-id="ea10c-112">تعتمد عوامل الكمية على سمات المنتج.</span><span class="sxs-lookup"><span data-stu-id="ea10c-112">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="ea10c-113">عندما تقوم بتكوين خصائص محددة لأحد المنتجات، يمكنك وضع علامة على مجموعة فرعية من هذه الخصائص، أو كل الخصائص، كعوامل كمية.</span><span class="sxs-lookup"><span data-stu-id="ea10c-113">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="ea10c-114">يتحقق Project Operations من أن الخصائص الرقمية أو خصائص المنتج التي تحتوي على نوع بيانات رقمية فقط يتم تمييزها كعوامل كمية.</span><span class="sxs-lookup"><span data-stu-id="ea10c-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="ea10c-115">عند إضافة منتج يتضمن عوامل كمية مكوّنة إلى شرط تعاقد، يصبح حقل **الكمية** للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="ea10c-115">When a product with configured quantity factors is added to a contract line, the **Quantity** field  becomes read-only.</span></span> <span data-ttu-id="ea10c-116">بعد إدخال قيم لخصائص المنتج هي عوامل الكمية، يقوم Project Operations بحساب كمية شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="ea10c-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the contract line.</span></span>

<span data-ttu-id="ea10c-117">على سبيل المثال، قد يشتمل Dynamics 365 Sales على الخصائص التالية:</span><span class="sxs-lookup"><span data-stu-id="ea10c-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="ea10c-118">**عدد المستخدمين**: عدد المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="ea10c-118">**No of users**: The number of users.</span></span>
- <span data-ttu-id="ea10c-119">**عدد الأشهر**: عدد أشهر الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="ea10c-119">**No of Months**: The number of subscription months.</span></span>
- <span data-ttu-id="ea10c-120">**SKU‏‎ المنتج**: وحدة الاحتفاظ بالمخزون (SKU) للمنتج.</span><span class="sxs-lookup"><span data-stu-id="ea10c-120">**Product SKU**: The stock keeping unit (SKU) for the product.</span></span>

<span data-ttu-id="ea10c-121">يمكن تمييز الخاصيتين **عدد المستخدمين** و **عجج الأشهر** كعوامل كمية من خلال تحرير خصائص بند المنتج.</span><span class="sxs-lookup"><span data-stu-id="ea10c-121">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="ea10c-122">لإنشاء عوامل الكمية من خصائص المنتج، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="ea10c-122">To create quantity factors from product properties, complete the following steps.</span></span>

1. <span data-ttu-id="ea10c-123">في **Project Operations**، حدد **منتجات المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="ea10c-123">On the **Project Operations**, select **Sales-Products**.</span></span>
2. <span data-ttu-id="ea10c-124">افتح المنتج الذي تريد إعداد عوامل الكمية له.</span><span class="sxs-lookup"><span data-stu-id="ea10c-124">Open the product for which you need to set up quantity factors.</span></span> <span data-ttu-id="ea10c-125">تأكد من أن المنتج لديه خصائص تم إعدادها بالفعل.</span><span class="sxs-lookup"><span data-stu-id="ea10c-125">Make sure that the product has properties already set up.</span></span>
3. <span data-ttu-id="ea10c-126">من صفحة **معلومات المنتح**، حدد علامة التبويب **عوامل الكمية**.</span><span class="sxs-lookup"><span data-stu-id="ea10c-126">On the **Project Information** page, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="ea10c-127">في جزء الشبكة الفرعية، حدد **+ حساب حقل جديد**.</span><span class="sxs-lookup"><span data-stu-id="ea10c-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="ea10c-128">أدخل اسم **عامل الكمية** وحدد قيمة الخاصية التي يتم تعيينها لحساب الحقل.</span><span class="sxs-lookup"><span data-stu-id="ea10c-128">Enter the name of the **Quantity Factor** and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="ea10c-129">حفظ النموذج وإغلاقه.</span><span class="sxs-lookup"><span data-stu-id="ea10c-129">Save and close the form.</span></span>
7. <span data-ttu-id="ea10c-130">كرر الخطوات 2-6 لكل الخصائص التي ستشكل معًا الكمية الخاصة بشرط التعاقد القائم على المنتج.</span><span class="sxs-lookup"><span data-stu-id="ea10c-130">Repeat steps 2-6 for all the properties that together will make up the quantity for the product-based contract line.</span></span>

<span data-ttu-id="ea10c-131">مع إعداد عوامل الكمية، وعندما يقوم المستخدم بإنشاء شرط تعاقد لهذا المنتج، تكون كمية شرط التعاقد مؤمنة.</span><span class="sxs-lookup"><span data-stu-id="ea10c-131">With quantity factors set up, when the user creates a contract line for this product, the quantity of the contract line is locked.</span></span> <span data-ttu-id="ea10c-132">ثم يتم احتساب الكمية كمنتج لقيم الخاصية لشرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="ea10c-132">The quantity is then calculated as a product of the property values for that contract line.</span></span>
