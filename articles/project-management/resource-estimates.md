---
title: تقديرات الموارد
description: يقدم هذا الموضوع معلومات حول كيفية حساب تقديرات الموارد في Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070564"
---
# <a name="resource-estimates"></a><span data-ttu-id="8ba60-103">تقديرات الموارد</span><span class="sxs-lookup"><span data-stu-id="8ba60-103">Resource estimates</span></span>

<span data-ttu-id="8ba60-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="8ba60-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8ba60-105">تأتي تقديرات الموارد من المجهود الموزع على الوقت الذي تم تحديده في هيكل تنظيم العمل بالإضافة إلى أبعاد التسعير القابلة للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="8ba60-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="8ba60-106">بشكل عام، يكون الحساب من خلال **المعدل/ساعة لكل دور x الساعات.**</span><span class="sxs-lookup"><span data-stu-id="8ba60-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="8ba60-107">يتم تخزين المجهود الموزع على الوقت لكل مورد في سجل تعيين المورد.</span><span class="sxs-lookup"><span data-stu-id="8ba60-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="8ba60-108">ويتم تخزين التسعير في قائمة أسعار محددة مسبقًا.</span><span class="sxs-lookup"><span data-stu-id="8ba60-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="8ba60-109">يتم تطبيق تحويل الوحدات على أساس قائمة الأسعار القابلة للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="8ba60-109">Unit conversion is applied based on the applicable price list.</span></span>

![تقديرات الموارد](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="8ba60-111">سعر التكلفة الافتراضي وعملة التكلفة</span><span class="sxs-lookup"><span data-stu-id="8ba60-111">Default cost price and cost currency</span></span>

<span data-ttu-id="8ba60-112">يتم تعيين أسعار التكلفة افتراضيًا من الوحدة التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="8ba60-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="8ba60-113">سعر الفاتورة الافتراضي وعملة المبيعات</span><span class="sxs-lookup"><span data-stu-id="8ba60-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="8ba60-114">يتم تطبيق أسعار المبيعات مرة واحدة لكل صفقة.</span><span class="sxs-lookup"><span data-stu-id="8ba60-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="8ba60-115">التسلسل الهرمي لقائمة أسعار المبيعات الافتراضي هو كالتالي:</span><span class="sxs-lookup"><span data-stu-id="8ba60-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="8ba60-116">المنظمة</span><span class="sxs-lookup"><span data-stu-id="8ba60-116">Organization</span></span>
2. <span data-ttu-id="8ba60-117">العميل</span><span class="sxs-lookup"><span data-stu-id="8ba60-117">Customer</span></span>
3. <span data-ttu-id="8ba60-118">عرض الأسعار/العقد</span><span class="sxs-lookup"><span data-stu-id="8ba60-118">Quote/contract</span></span>
