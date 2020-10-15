---
title: حساب تكاليف بنود عروض الأسعار المستندة إلى المنتج
description: يقدم هذا الموضوع معلومات حول تطبيق سعر تكلفة على بند عرض أسعار قائم على المنتج.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 17b377eab5bcbc1a2327cb3ff87cc75d8de40953
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906046"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="b3284-103">حساب تكاليف بنود عروض الأسعار المستندة إلى المنتج</span><span class="sxs-lookup"><span data-stu-id="b3284-103">Costing product-based quote lines</span></span>

<span data-ttu-id="b3284-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="b3284-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="b3284-105">تحتوي بنود عرض الأسعار القائمة على المنتج في Dynamics 365 Project Operations على حقل **سعر التكلفة**.</span><span class="sxs-lookup"><span data-stu-id="b3284-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="b3284-106">يستخدم هذا الحقل لتتبع سعر التكلفة للمنتج في بند عرض الأسعار وحسابات الربحية اللاحقة.</span><span class="sxs-lookup"><span data-stu-id="b3284-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="b3284-107">عند إنشاء بند عرض أسعار قائم على المنتج لمنتج كتالوج، يتم تحديد تكلفة بند عرض الأسعار القائم على المنتج بشكل افتراضي من حقل **التكلفة القياسية** في كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="b3284-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="b3284-108">يتم إعداد حقل "التكلفة القياسية" في كتالوج المنتجات بالعملة الأساسية للمؤسسة.</span><span class="sxs-lookup"><span data-stu-id="b3284-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="b3284-109">يتم تحويل تكلفة الوحدة الافتراضية في بند عرض الأسعار القائم على المنتج إلى عملة المبيعات في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="b3284-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="b3284-110">تكلفة الوحدة على بند عرض أسعار قائم على المنتج</span><span class="sxs-lookup"><span data-stu-id="b3284-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="b3284-111">الغرض من وجود تكلفة الوحدة على بند عرض أسعار قائم على المنتج هو السماح بتكاليف مختلفة لأحد المنتجات لكل عملية بيع.</span><span class="sxs-lookup"><span data-stu-id="b3284-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="b3284-112">هذا ليس سيناريو نموذجيًا، ولكن قد يتم خصم تكلفة المنتج في بعض الأحيان من قِبل المورّد بحسب عميل البيع النهائي.</span><span class="sxs-lookup"><span data-stu-id="b3284-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="b3284-113">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="b3284-113">For example:</span></span>

<span data-ttu-id="b3284-114">تقوم شركة Fabrikam Robotics بتثبيت أذرع آلية في بنود تجميع شركة A Datum Corporation'.</span><span class="sxs-lookup"><span data-stu-id="b3284-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="b3284-115">توفر شركة Fabrikam خدمات التثبيت ولكن يتم شراء الأذرع الآلية من Trey robotics.</span><span class="sxs-lookup"><span data-stu-id="b3284-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="b3284-116">إذا فتحت عملية تثبيت الأذرع الآلية في A Datum Corporation مجال صناعة جديدًا للأذرع الآلية في شركة Trey، فقد تمنح Trey شركة Fabrikam خصمًا خاصًا لهذه الصفقة.</span><span class="sxs-lookup"><span data-stu-id="b3284-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="b3284-117">وفي هذه الحالة، ستقوم شركة Fabrikam بإنشاء خط عرض أسعار قائم على المنتج للأذرع الآلية وستدخل سعر وحدة خاصًا لعرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="b3284-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="b3284-118">تختلف هذه التكلفة عن التكلفة القياسية للأذرع الآلية لشركة Trey.</span><span class="sxs-lookup"><span data-stu-id="b3284-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>
