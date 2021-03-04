---
title: تحليل عروض أسعار المشروع
description: يوفر هذا الموضوع معلومات حول تحليل عروض أسعار المشروع.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 361a940261811467c46222c3d58c9504434ec882
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145207"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="3ff55-103">تحليل عروض أسعار المشروع</span><span class="sxs-lookup"><span data-stu-id="3ff55-103">Analysis of project quotes</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3ff55-104">يحلل Dynamics 365 Project Service Automation عروض أسعار المشروع لتقدير الربحية.</span><span class="sxs-lookup"><span data-stu-id="3ff55-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="3ff55-105">كما يحلل أيضًا مدى انسجام عرض الأسعار مع توقعات العملاء بشأن تاريخ التسليم أو تاريخ الاكتمال، وحول budget.tions.</span><span class="sxs-lookup"><span data-stu-id="3ff55-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="3ff55-106">تحليل الربحية</span><span class="sxs-lookup"><span data-stu-id="3ff55-106">Profitability analysis</span></span>

<span data-ttu-id="3ff55-107">يحلل Project Service Automation الربحية باستخدام إجمالي هامش الربح وإجمالي هامش الربح المعدل.</span><span class="sxs-lookup"><span data-stu-id="3ff55-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="3ff55-108">يتم حساب إجمالي هوامش الربح باستخدام المعادلات التالية:</span><span class="sxs-lookup"><span data-stu-id="3ff55-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="3ff55-109">يتم حساب إجمالي هامش الربح المعدل باستخدام المعادلة التالية:</span><span class="sxs-lookup"><span data-stu-id="3ff55-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="3ff55-110">وإذا كانت القيم الخاصة بإجمالي هامش الربح وإجمالي هامش الربح المعدل تختلف بهامش عريض، سيتم تصنيف جزء كبير من العمل في عرض الأسعار على أنه غير خاضع للرسوم.</span><span class="sxs-lookup"><span data-stu-id="3ff55-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="3ff55-111">تحليل توقعات العميل</span><span class="sxs-lookup"><span data-stu-id="3ff55-111">Analysis of customer expectations</span></span>

<span data-ttu-id="3ff55-112">يمكنك تحليل عروض الأسعار وإنشاء مخططات لتوقعات العملاء حول الجدول والميزانية إذا قمت بإدخال قيم للحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="3ff55-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="3ff55-113">حقل **تاريخ التسليم المطلوب** في رأس عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3ff55-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="3ff55-114">حقل **موازنة العميل** لكل بند عرض الأسعار (للبنود المستندة إلى المشروع والبنود المستندة إلى المنتج).</span><span class="sxs-lookup"><span data-stu-id="3ff55-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="3ff55-115">ويتم تحليل توقعات العملاء المتعلقة بالجدولة عن طريق مقارنة أحدث تاريخ انتهاء لتفاصيل بند عرض الأسعار مع تاريخ التسليم المطلوب عبر كافة بنود عرض الأسعار في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3ff55-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="3ff55-116">يتم تحليل توقعات العملاء المتعلقة بالموازنة عن طريق مقارنة مجموع موازنة العميل الإجمالية بمبلغ عرض الأسعار عبر كافة بنود عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3ff55-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>
