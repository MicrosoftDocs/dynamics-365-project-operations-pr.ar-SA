---
title: إعداد معدلات التكلفة والمبيعات لمنتجات الكتالوج
description: يقدم هذا الموضوع معلومات حول كيفية إعداد معدلات التكلفة والمبيعات لأصناف في كتالوج المنتجات.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5178a9143536bf4b2573403125325017861cdd5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070711"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products"></a><span data-ttu-id="93f14-103">إعداد معدلات التكلفة والمبيعات لمنتجات الكتالوج</span><span class="sxs-lookup"><span data-stu-id="93f14-103">Set up cost and sales rates for catalog products</span></span>

<span data-ttu-id="93f14-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="93f14-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="93f14-105">تعتبر عملية إعداد التسعير لأصناف كتالوج المنتجات في Dynamics 365 Project Operations مماثلة لعملية إعدادها في Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="93f14-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="93f14-106">وبسبب عدم إمكانية تقدير المنتجات أو استخدامها في المشروعات في Project Operations، فلا حاجة إلى تعيين أسعار كتالوج المنتجات على قوائم أسعار المشروع لعروض الأسعار والعقود.</span><span class="sxs-lookup"><span data-stu-id="93f14-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="93f14-107">يجب إعداد أسعار كتالوج المنتجات في حقل **سعر المنتج** في عرض أسعار أو عقد أو حساب.</span><span class="sxs-lookup"><span data-stu-id="93f14-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="93f14-108">لا تعمل على إعداد أسعار كتالوج المنتجات في قوائم أسعار المشروع لهذه الكيانات.</span><span class="sxs-lookup"><span data-stu-id="93f14-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="93f14-109">تعتبر قوائم أسعار المشروع حصرية في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="93f14-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="93f14-110">هناك منطق أعمال خاص بالتطبيق ينسخ قوائم الأسعار من عرض أسعار إلى عقد.</span><span class="sxs-lookup"><span data-stu-id="93f14-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="93f14-111">والنتيجة هي قائمة أسعار مشروع خاصة بالعقد.</span><span class="sxs-lookup"><span data-stu-id="93f14-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="93f14-112">بإمكان عملية النسخ أن تؤخر عملية الفوز بعرض الأسعار إذا كانت قائمة الأسعار على عرض الأسعار كبيرة للغاية.</span><span class="sxs-lookup"><span data-stu-id="93f14-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="93f14-113">لا يتم نسخ قوائم أسعار المنتجات لإنشاء قوائم أسعار مخصصة على العقود.</span><span class="sxs-lookup"><span data-stu-id="93f14-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="93f14-114">وهذا يعني أن قوائم أسعار المنتجات لا تؤثر على أداء عملية الفوز بعرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="93f14-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
