---
title: إعداد معدلات التكلفة والمبيعات لمنتجات الكتالوج - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية إعداد معدلات التكلفة والمبيعات لأصناف في كتالوج المنتجات.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f0941c549cc38f0938a5819e8cb6ca9912f14790
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274442"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="0b188-103">إعداد معدلات التكلفة والمبيعات لمنتجات الكتالوج - خفيف</span><span class="sxs-lookup"><span data-stu-id="0b188-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="0b188-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="0b188-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="0b188-105">يعمل إعداد التسعير لعناصر كتالوج المنتجات في Dynamics 365 Project Operations بنفس الطريقة كما في Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="0b188-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="0b188-106">في Project Operations، لا يمكن تقدير المنتجات أو استخدامها في المشروعات، لذلك لا يلزم تعيين أسعار كتالوج المنتجات في قوائم أسعار المشروع لعروض الأسعار والعقود.</span><span class="sxs-lookup"><span data-stu-id="0b188-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="0b188-107">استخدم حقل **سعر المنتج** مع عرض السعر أو العقد أو الحساب لإعداد أسعار كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="0b188-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="0b188-108">لا تحدد أسعار كتالوج المنتجات في قوائم أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="0b188-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="0b188-109">تعتبر قوائم أسعار المشروع حصرية في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="0b188-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="0b188-110">ينسخ منطق الأعمال الخاص بالتطبيق قوائم الأسعار من عرض الأسعار إلى عقد.</span><span class="sxs-lookup"><span data-stu-id="0b188-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="0b188-111">والنتيجة هي قائمة أسعار مشروع خاصة بالعقد.</span><span class="sxs-lookup"><span data-stu-id="0b188-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="0b188-112">بإمكان عملية النسخ أن تؤخر عملية الفوز بعرض الأسعار إذا كانت قائمة الأسعار على عرض الأسعار كبيرة للغاية.</span><span class="sxs-lookup"><span data-stu-id="0b188-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="0b188-113">لا يتم نسخ قوائم أسعار المنتجات لإنشاء قوائم أسعار مخصصة على العقود.</span><span class="sxs-lookup"><span data-stu-id="0b188-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="0b188-114">ونظرا لعدم وجود نسخ، فإن أداء عملية عرض الأسعار لن يتأثر.</span><span class="sxs-lookup"><span data-stu-id="0b188-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]