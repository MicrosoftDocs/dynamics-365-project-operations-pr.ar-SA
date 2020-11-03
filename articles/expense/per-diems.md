---
title: المصروفات اليومية
description: يقدم هذا الموضوع معلومات حول قواعد المصروفات اليومية المستخدمة في إدارة المصروفات.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 7d1c4ac7781cb711e2cc0d09606d422b4dd554f3
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070518"
---
# <a name="per-diems"></a><span data-ttu-id="dab2c-103">المصروفات اليومية</span><span class="sxs-lookup"><span data-stu-id="dab2c-103">Per diems</span></span>

<span data-ttu-id="dab2c-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="dab2c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="dab2c-105">والمصروف اليومي هو البدل الذي يتم دفعه للعامل الذي يقوم بالسفر للعمل.</span><span class="sxs-lookup"><span data-stu-id="dab2c-105">A per diem is an allowance that is paid to a worker who is traveling for work.</span></span> <span data-ttu-id="dab2c-106">في إدارة المصروفات، يمكنك إنشاء قواعد المصروفات اليومية للعديد من حالات السفر.</span><span class="sxs-lookup"><span data-stu-id="dab2c-106">In Expense management, you can create per diem rules for  various travel situations.</span></span> <span data-ttu-id="dab2c-107">ويمكن أن تستند معدلات المصروفات اليومية إلى الوقت من السنة أو موقع السفر أو كليهما.</span><span class="sxs-lookup"><span data-stu-id="dab2c-107">Per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="dab2c-108">عندما تقوم بإنشاء قاعدة مصروف يومي، يمكنك تحديد أنه سيتم اقتطاع النسبة المئوية لمعدل المصروف اليومي إذا تلقي أحد العمال وجبات أو خدمات مجانية.</span><span class="sxs-lookup"><span data-stu-id="dab2c-108">When you create a per diem  rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="dab2c-109">يمكنك أيضا تعيين الحد الأدنى والحد الأقصى لعدد الساعات التي يمكن لكل معدل مصروفات اليومية تطبيقها على سفر العامل.</span><span class="sxs-lookup"><span data-stu-id="dab2c-109">You can also set a minimum and maximum number of hours that the per diem rate can apply to a worker's travel.</span></span>

## <a name="configuration"></a><span data-ttu-id="dab2c-110">التكوين</span><span class="sxs-lookup"><span data-stu-id="dab2c-110">Configuration</span></span> 

1. <span data-ttu-id="dab2c-111">لإضافة مواقع المصروفات اليومية، انتقل إلى **الإعداد** > **الحسابات والأكواد** > **مواقع المصروفات اليومية**.</span><span class="sxs-lookup"><span data-stu-id="dab2c-111">To add per diem locations, go to **Set up** > **Calculations and codes** > **Per diem locations**.</span></span>
2. <span data-ttu-id="dab2c-112">بالنسبة لكل موقع من المواقع المضافة بالأعلى، حدد معدل المصروفات اليومية والعملة الصالحة بين تاريخ بداية ونهاية محددين لمصروفات الفندق والوجبات والمصروفات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="dab2c-112">For each of the locations added above, select a per diem rate and currency that is valid between a specific start and end date for hotel, meals, and other expenses.</span></span> <span data-ttu-id="dab2c-113">يتم تكوين معدلات المصروفات اليومية والعملات تحت **الإعداد** > **الحسابات والأكواد** > **المصروفات اليومية**.</span><span class="sxs-lookup"><span data-stu-id="dab2c-113">Per diem rates and currencies are configured under **Set up** > **Calculations and codes** > **Per diems**.</span></span>
3. <span data-ttu-id="dab2c-114">في صفحة **مواقع المصروفات اليومية** ، قم بتكوين مستويات معدلات المصروفات اليومية.</span><span class="sxs-lookup"><span data-stu-id="dab2c-114">On the **Per diem locations** page, configure per diem rate tiers.</span></span> <span data-ttu-id="dab2c-115">تتيح لك مستويات معدلات المصروفات اليومية تحديد النسبة المئوية التي يتم تقسيمها إلى البدل اليومي لمصروفات الفندق والوجبات والمصروفات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="dab2c-115">Per diem rate tiers allow you to define the percentage split of a daily allowance for hotel, meal, and other expenses.</span></span> 
4. <span data-ttu-id="dab2c-116">لتحديد تخفيض النسبة المئوية لوجبات للإفطار أو الغداء أو العشاء، قم بتحديث الحقول في صفحة **معلمات إدارة المصروفات** في علامة التبويب **المصروفات اليومية**.</span><span class="sxs-lookup"><span data-stu-id="dab2c-116">To specify the meal percentage reduction for breakfast, lunch, or dinner, update the fields on the **Expense management parameters** page on the **Per diem** tab.</span></span> 
    
## <a name="submit-expenses-using-per-diem"></a><span data-ttu-id="dab2c-117">إرسال المصروفات باستخدام المصروف اليومي</span><span class="sxs-lookup"><span data-stu-id="dab2c-117">Submit expenses using per diem</span></span>
<span data-ttu-id="dab2c-118">لإرسال المصروفات باستخدام المصروفات اليومية، استخدم فئة المصروفات **اليومية** عند إنشاء تقرير مصروفات.</span><span class="sxs-lookup"><span data-stu-id="dab2c-118">To submit expenses utilizing per diems, use the **Per diem** expense category when you create an expense report.</span></span> <span data-ttu-id="dab2c-119">أدخل **المصروف اليومي من تاريخ** و **المصروف اليومي إلى تاريخ** و **موقع المصروفات اليومية**.</span><span class="sxs-lookup"><span data-stu-id="dab2c-119">Enter the **Per diem from date** , **Per diem to date** ,  and the **Per diem location**.</span></span> <span data-ttu-id="dab2c-120">سيتم حساب المبلغ على أساس معدلات المصروفات اليومية الخاصة بالموقع المحدد وسيتم حساب تخفيض الوجبة على أساس مستويات معدلات المصروفات اليومية.</span><span class="sxs-lookup"><span data-stu-id="dab2c-120">The amount will be calculated based on the per diem rates for the selected location and meal reduction will be calculated based on the per diem rate tiers.</span></span>
