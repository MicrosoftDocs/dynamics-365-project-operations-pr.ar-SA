---
title: تقديرات الموارد
description: يقدم هذا الموضوع معلومات حول كيفية حساب تقديرات الموارد في Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 98a61746f172b50bf6fa29cb0d21462cd616f417
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286502"
---
# <a name="resource-estimates"></a><span data-ttu-id="963af-103">تقديرات الموارد</span><span class="sxs-lookup"><span data-stu-id="963af-103">Resource estimates</span></span>

<span data-ttu-id="963af-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="963af-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="963af-105">تأتي تقديرات الموارد من المجهود الموزع على الوقت الذي تم تحديده في هيكل تنظيم العمل بالإضافة إلى أبعاد التسعير القابلة للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="963af-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="963af-106">بشكل عام، يكون الحساب من خلال **المعدل/ساعة لكل دور x الساعات.**</span><span class="sxs-lookup"><span data-stu-id="963af-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="963af-107">يتم تخزين المجهود الموزع على الوقت لكل مورد في سجل تعيين المورد.</span><span class="sxs-lookup"><span data-stu-id="963af-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="963af-108">ويتم تخزين التسعير في قائمة أسعار محددة مسبقًا.</span><span class="sxs-lookup"><span data-stu-id="963af-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="963af-109">يتم تطبيق تحويل الوحدات على أساس قائمة الأسعار القابلة للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="963af-109">Unit conversion is applied based on the applicable price list.</span></span>

![تقديرات الموارد](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="963af-111">سعر التكلفة الافتراضي وعملة التكلفة</span><span class="sxs-lookup"><span data-stu-id="963af-111">Default cost price and cost currency</span></span>

<span data-ttu-id="963af-112">يتم تعيين أسعار التكلفة افتراضيًا من الوحدة التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="963af-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="963af-113">سعر الفاتورة الافتراضي وعملة المبيعات</span><span class="sxs-lookup"><span data-stu-id="963af-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="963af-114">يتم تطبيق أسعار المبيعات مرة واحدة لكل صفقة.</span><span class="sxs-lookup"><span data-stu-id="963af-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="963af-115">التسلسل الهرمي لقائمة أسعار المبيعات الافتراضي هو كالتالي:</span><span class="sxs-lookup"><span data-stu-id="963af-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="963af-116">المنظمة</span><span class="sxs-lookup"><span data-stu-id="963af-116">Organization</span></span>
2. <span data-ttu-id="963af-117">العميل</span><span class="sxs-lookup"><span data-stu-id="963af-117">Customer</span></span>
3. <span data-ttu-id="963af-118">عرض الأسعار/العقد</span><span class="sxs-lookup"><span data-stu-id="963af-118">Quote/contract</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]