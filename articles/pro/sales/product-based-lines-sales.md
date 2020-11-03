---
title: بنود الفرصة المستندة إلى المنتج
description: يوفر هذا الموضوع معلومات حول عناصر بنود الفرصة المستندة إلى المنتج في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 17ffcf8dc94d42102115281d281d6b553cf1fa17
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070570"
---
# <a name="product-based-opportunity-lines"></a><span data-ttu-id="b3208-103">بنود الفرصة المستندة إلى المنتج</span><span class="sxs-lookup"><span data-stu-id="b3208-103">Product-based opportunity lines</span></span>

<span data-ttu-id="b3208-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="b3208-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b3208-105">بنود الفرصة المستندة إلى المنتج هي عناصر البند في الفرصة.</span><span class="sxs-lookup"><span data-stu-id="b3208-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="b3208-106">يتم تسليم هذه البنود إلى العميل كعناصر بنود مميزة في الفاتورة النهائية بدون أية خدمات مضافة القيمة.</span><span class="sxs-lookup"><span data-stu-id="b3208-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="b3208-107">لا يتم تعقب الإنفاق والاستهلاك المرتبطين في المهام الخاصة بأي مشاريع ذات صلة.</span><span class="sxs-lookup"><span data-stu-id="b3208-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="b3208-108">يمكن أن تكون البنود المستندة إلى المنتج هي عناصر الكتالوج أو منتجات مدونة.</span><span class="sxs-lookup"><span data-stu-id="b3208-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="b3208-109">تتبع معظم الوظائف في البنود المستندة إلى المنتج الخاصة بالفرصة الوظائف التي يوفرها تطبيق Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="b3208-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="b3208-110">لمزيد من المعلومات حول بنود الفرصة المستندة إلى المنتج، راجع [إضافة منتجات إلى فرصة مبيعات](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="b3208-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="b3208-111">تمثل **ميزانية العميل** أحد مفاهيم بنود الفرص المستندة إلى المنتج الخاصة بالفرص المستندة إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="b3208-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="b3208-112">استخدم هذا الحقل لتعقب المبلغ الذي يرغب العميل في دفعه لصنف البند.</span><span class="sxs-lookup"><span data-stu-id="b3208-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="b3208-113">وفي حاله تعيين أسلوب الإيراد الخاص بملخص الفرصة إلى **محسوب من النظام** ، يتم تلخيص قيم موازنة العميل في البنود المستندة إلى المنتج والمشروع لحساب الإيراد المقدر.</span><span class="sxs-lookup"><span data-stu-id="b3208-113">If the revenue method of the Opportunity summary is set to **System Calculated** , the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
