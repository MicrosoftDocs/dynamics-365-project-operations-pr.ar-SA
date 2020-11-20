---
title: إعداد معدلات التكلفة والمبيعات لمنتجات الكتالوج - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية إعداد معدلات التكلفة والمبيعات لأصناف في كتالوج المنتجات.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 135b182af73bdab7a3520589431332ad059ec497
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176685"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="cbf1c-103">إعداد معدلات التكلفة والمبيعات لمنتجات الكتالوج - خفيف</span><span class="sxs-lookup"><span data-stu-id="cbf1c-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="cbf1c-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="cbf1c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="cbf1c-105">تعتبر عملية إعداد التسعير لأصناف كتالوج المنتجات في Dynamics 365 Project Operations مماثلة لعملية إعدادها في Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="cbf1c-106">وبسبب عدم إمكانية تقدير المنتجات أو استخدامها في المشروعات في Project Operations، فلا حاجة إلى تعيين أسعار كتالوج المنتجات على قوائم أسعار المشروع لعروض الأسعار والعقود.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="cbf1c-107">يجب إعداد أسعار كتالوج المنتجات في حقل **سعر المنتج** في عرض أسعار أو عقد أو حساب.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="cbf1c-108">لا تعمل على إعداد أسعار كتالوج المنتجات في قوائم أسعار المشروع لهذه الكيانات.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="cbf1c-109">تعتبر قوائم أسعار المشروع حصرية في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="cbf1c-110">هناك منطق أعمال خاص بالتطبيق ينسخ قوائم الأسعار من عرض أسعار إلى عقد.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="cbf1c-111">والنتيجة هي قائمة أسعار مشروع خاصة بالعقد.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="cbf1c-112">بإمكان عملية النسخ أن تؤخر عملية الفوز بعرض الأسعار إذا كانت قائمة الأسعار على عرض الأسعار كبيرة للغاية.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="cbf1c-113">لا يتم نسخ قوائم أسعار المنتجات لإنشاء قوائم أسعار مخصصة على العقود.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="cbf1c-114">وهذا يعني أن قوائم أسعار المنتجات لا تؤثر على أداء عملية الفوز بعرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="cbf1c-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
