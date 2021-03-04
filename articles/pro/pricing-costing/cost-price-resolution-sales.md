---
title: حل أسعار التكلفة على التقديرات والقيم الفعلية - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية حل أسعار التكلفة على التقديرات والقيم الفعلية.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d2afaa2231f4044dbcbfa24b91aec39289275a91
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764541"
---
# <a name="resolve-cost-prices-on-estimates-and-actuals---lite"></a><span data-ttu-id="48255-103">حل أسعار التكلفة على التقديرات والقيم الفعلية - خفيف</span><span class="sxs-lookup"><span data-stu-id="48255-103">Resolve cost prices on estimates and actuals - lite</span></span>

<span data-ttu-id="48255-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="48255-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="48255-105">لحل أسعار التكلفة وقائمة أسعار التكلفة للتقديرات والقيم الفعلية، يستخدم النظام المعلومات الموجودة في حقول **التاريخ** و **العملة** و **وحدة التعاقد** للمشروع ذي الصلة.</span><span class="sxs-lookup"><span data-stu-id="48255-105">To resolve cost prices and the cost price list for estimates and actuals, the system uses the information in the **Date**, **Currency**, and **Contracting Unit** fields of the related project.</span></span> <span data-ttu-id="48255-106">بعد حل قائمة أسعار التكلفة، يقوم التطبيق بحل معدل التكلفة.</span><span class="sxs-lookup"><span data-stu-id="48255-106">After the cost price list is resolved, the application resolves the cost rate.</span></span>

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-time"></a><span data-ttu-id="48255-107">حل معدلات التكلفة على بنود القيم الفعلية وتقديرات الوقت</span><span class="sxs-lookup"><span data-stu-id="48255-107">Resolving cost rates on actual and estimate lines for Time</span></span>

<span data-ttu-id="48255-108">تشير بنود تقديرات الوقت إلى تفاصيل عرض الأسعار وشروط التعاقد لتعيينات الوقت والموارد على مشروع.</span><span class="sxs-lookup"><span data-stu-id="48255-108">Estimate lines for Time refer to the quote and contract line details for time and resource assignments on a project.</span></span>

<span data-ttu-id="48255-109">وبعد حل قائمة أسعار التكلفة، تتم مطابقة حقلي **الدور** و **وحدة تعيين الموارد** في سطر القدير للوقت مقابل بنود أسعار الدور في قائمة  الأسعار.</span><span class="sxs-lookup"><span data-stu-id="48255-109">After a cost price list is resolved, the **Role** and **Resourcing Unit** fields on the estimate line for Time are matched against the role price lines in the price list.</span></span> <span data-ttu-id="48255-110">تفترض هذه مطابقة أنك تستخدم أبعاد التسعير القياسية لتكلفة العمالة.</span><span class="sxs-lookup"><span data-stu-id="48255-110">This match assumes that you're using the standard pricing dimensions for labor cost.</span></span> <span data-ttu-id="48255-111">إذا قمت بتكوين النظام لمطابقة الحقول بدلاً من، أو بالإضافة إلى **الدور** و **وحدة تعيين الموارد**، فسيتم استخدام مجموعة مختلفة لاسترداد بند سعر دور مطابق.</span><span class="sxs-lookup"><span data-stu-id="48255-111">If you configured the system to match fields instead of, or in addition to **Role** and **Resourcing Unit**, then a different combination will be used to retrieve a matching role price line.</span></span> <span data-ttu-id="48255-112">إذا عثر التطبيق على بند سعر دور يحتوي على سعر التكلفة لمجموعة **الدور** و **وحدة تعيين الموارد**، فهذا هو معدل التكلفة الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="48255-112">If the application finds a role price line that has a cost rate for the **Role** and **Resourcing Unit** combination, that is the default cost rate.</span></span> <span data-ttu-id="48255-113">إذا تعذر على التطبيق مطابقة قيم **الدور** و **وحدة تعيين الموارد**، فهو يسترد عندئذٍ بنود أسعار الدور مع دور مطابق، ولكن قيم فارغة في **وحدة تعيين الموارد**.</span><span class="sxs-lookup"><span data-stu-id="48255-113">If the application can't match the **Role** and **Resourcing Unit** values, then it retrieves role price lines with a matching role, but null values of the **Resourcing Unit**.</span></span> <span data-ttu-id="48255-114">يتم تعيين قيمة افتراضية لمعدل التكلفة من هذا السجل بعد أن يصبح لديه سجل سعر الدور.</span><span class="sxs-lookup"><span data-stu-id="48255-114">After it has a matching role price record, the cost rate defaults from that record.</span></span> 

> [!NOTE]
> <span data-ttu-id="48255-115">إذا قمت بتكوين ترتيب أولويات مختلف لقيم **الدور** و **وحدة تعيين الموارد**، أو إذا كانت لديك أبعاد أخرى لديها ترتيب أولويات أعلى، فسيتغير هذا السلوك وفقًا لذلك.</span><span class="sxs-lookup"><span data-stu-id="48255-115">If you configure a different prioritization of **Role** and **Resourcing Unit**, or if you have other dimensions that have higher priority, this behavior will change accordingly.</span></span> <span data-ttu-id="48255-116">يسترد النظام سجلات أسعار الأدوار مع قيم تطابق كل واحدة من قيم أبعاد التسعير حسب الأولوية مع صفوف لديها قيم فارغة للأبعاد الأخيرة في ترتيب الأولويات.</span><span class="sxs-lookup"><span data-stu-id="48255-116">The system retrieves role price records with values that match each of the pricing dimension values in order of priority with rows that have null values for those dimensions coming last.</span></span>

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-expense"></a><span data-ttu-id="48255-117">حل معدلات التكلفة على بنود القيم الفعلية وتقديرات المصروفات</span><span class="sxs-lookup"><span data-stu-id="48255-117">Resolving cost rates on actual and estimate lines for Expense</span></span>

<span data-ttu-id="48255-118">تشير بنود المصروفات إلى تفاصيل عرض الأسعار وشروط التعاقد لبنود المصروفات وبنود تقديرات المصروفات على مشروع.</span><span class="sxs-lookup"><span data-stu-id="48255-118">Estimate lines for Expense refer to the quote and contract line details for expenses and the expense estimate lines on a project.</span></span>

<span data-ttu-id="48255-119">بعد حل قائمة أسعار التكلفة، يستخدم النظام مجموعة من حقول **الفئة** و **الوحدة** في سطر تقدير المصروفات للمطابقة مقابل بنود **أسعار الفئة** في قائمة الأسعار التي تم حلها.</span><span class="sxs-lookup"><span data-stu-id="48255-119">After a cost price list is resolved, the system uses a combination of the **Category** and **Unit** fields on the expense estimate line to match against the **Category Price** lines on the resolved price list.</span></span> <span data-ttu-id="48255-120">إذا عثر النظام على بند سعر فئة له معدل تكلفة لمجموعة الحقلين **الفئة** و **الوحدة**، سيتم تعيين معدل التكلفة كافتراضي.</span><span class="sxs-lookup"><span data-stu-id="48255-120">If the system finds a category price line that has a cost rate for the **Category** and **Unit** field combination, the cost rate is defaulted.</span></span> <span data-ttu-id="48255-121">إذا كان النظام لا يستطيع مطابقة قيم **الفئة** و **الوحدة**، أو إذا كان قادرًا على العثور على سطر سعر فئة مطابق ولكن أسلوب التسعير ليس **السعر لكل وحدة**، فسوف يتم تعيين معدل التكلفة الافتراضية إلى الصفر (0).</span><span class="sxs-lookup"><span data-stu-id="48255-121">If the system can't match the **Category** and **Unit** values, or if it's able to find a matching category price line but the pricing method isn't **Price Per Unit**, the cost rate defaults to zero(0).</span></span>
