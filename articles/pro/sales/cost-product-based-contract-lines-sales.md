---
title: حساب تكاليف شروط التعاقد المستندة إلى المنتج
description: يقدم هذا الموضوع معلومات حول الإنشاء
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7dfb9425174dddee52f9ee64f7a963e48a6bca70
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/20/2020
ms.locfileid: "4070875"
---
# <a name="costing-product-based-contract-lines"></a><span data-ttu-id="15f42-103">حساب تكاليف شروط التعاقد المستندة إلى المنتج</span><span class="sxs-lookup"><span data-stu-id="15f42-103">Costing product-based contract lines</span></span>

<span data-ttu-id="15f42-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="15f42-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="15f42-105">تتضمن شروط التعاقد المستندة إلى المشروع في Dynamics 365 Project Operations حقل **سعر التكلفة** ، الذي يخزّن سعر تكلفة المنتج لحسابات الربحية اللاحقة.</span><span class="sxs-lookup"><span data-stu-id="15f42-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="15f42-106">عند إنشاء شرط تعاقد يستند إلى المشروع لمنتج كتالوج، يتم تحديد تكلفة شرط التعاقد الذي يستند إلى المشروع بشكل افتراضي من حقل **التكلفة القياسية** في كتالوج المنتجات.</span><span class="sxs-lookup"><span data-stu-id="15f42-106">When a product-based contract line is created for a catalog product, the cost of the product-based contract line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="15f42-107">يتم إعداد حقل **التكلفة القياسية** في كتالوج المنتجات بالعملة الأساسية للمؤسسة.</span><span class="sxs-lookup"><span data-stu-id="15f42-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="15f42-108">عند تعيين تكلفة الوحدة بشكل افتراضي إلى بند التعاقد، يتم تحويلها إلى عملة المبيعات في العقد.</span><span class="sxs-lookup"><span data-stu-id="15f42-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="15f42-109">تكلفة الوحدة على شرط تعاقد يستند إلى المنتج</span><span class="sxs-lookup"><span data-stu-id="15f42-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="15f42-110">يؤدي وجود تكلفة الوحدة على شرط التعاقد المستند إلى المشروع إلى السماح بتكاليف مختلفة للمنتج تتعلق بكل عملية بيع للوحدة.</span><span class="sxs-lookup"><span data-stu-id="15f42-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="15f42-111">هناك سيناريوهات معينة حيث قد يتم خصم تكلفة المنتج للعميل من قِبل المورّد، على الرغم من أن هذا الأمر قد لا يكون ضروريًا في كل الأوقات.</span><span class="sxs-lookup"><span data-stu-id="15f42-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="15f42-112">فكر في السيناريو التالي:</span><span class="sxs-lookup"><span data-stu-id="15f42-112">Consider the following scenario:</span></span>

<span data-ttu-id="15f42-113">تقوم شركة Fabrikam Robotics بتثبيت أذرع آلية في بنود تجميع شركة Adatum Corporation.</span><span class="sxs-lookup"><span data-stu-id="15f42-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="15f42-114">توفر شركة Fabrikam خدمات التثبيت ولكن يتم شراء الأذرع الآلية من Trey Research.</span><span class="sxs-lookup"><span data-stu-id="15f42-114">Fabrikam provides installation services but the robotic arms are procured from Trey Research.</span></span> <span data-ttu-id="15f42-115">إذا فتحت عملية تثبيت الأذرع الآلية في Adatum Corporation مجال صناعة جديدًا لشركة Trey Research، فقد تمنح خصمًا خاصًا لهذه الصفقة لشركة Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="15f42-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="15f42-116">وفي هذه الحالة، تنشئ شركة Fabrikam شرط تعاقد يستند إلى المشروع للأذرع الآلية وتُدخل تكلفة الوحدة لهذا العقد تختلف عن التكلفة القياسية للأذرع الآلية من Trey Research.</span><span class="sxs-lookup"><span data-stu-id="15f42-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms and inputs a per unit cost for this contract that is different from the standard cost of robotic arms from Trey Research.</span></span>
