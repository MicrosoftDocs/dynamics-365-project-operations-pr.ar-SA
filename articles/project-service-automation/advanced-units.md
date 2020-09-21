---
title: مجموعات الوحدات والوحدات
description: يقدم هذا الموضوع معلومات حول مجموعات الوحدات والوحدات.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: b5422be3-5bfc-4ee2-b19a-4eca68813ff2
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: fc2dde2d9471f8585c190a65f3ad9b32de75af86
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748758"
---
# <a name="unit-groups-and-units"></a><span data-ttu-id="fe041-103">مجموعات الوحدات والوحدات</span><span class="sxs-lookup"><span data-stu-id="fe041-103">Unit groups and units</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="fe041-104">وتعتبر مجموعات الوحدات والوحدات كيانات أساسية في Microsoft Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="fe041-104">Unit groups and units are basic entities in Microsoft Dynamics 365.</span></span> <span data-ttu-id="fe041-105">تمثل الوحدة وحدة قياس فردية، ويمكن تجميع وحدات متعددة في مجموعات الوحدات.</span><span class="sxs-lookup"><span data-stu-id="fe041-105">A unit is a single unit of measure, and multiple units can be grouped into unit groups.</span></span> <span data-ttu-id="fe041-106">تتم الإشارة في بعض الأحيان إلى مجموعة الوحدات على أنها جدول وحدات في واجهه مستخدم Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="fe041-106">A unit group is sometimes referred to as a unit schedule in the Dynamics 365 user interface (UI).</span></span> 

<span data-ttu-id="fe041-107">واليك بعض الأمثلة عن الوحدات ومجموعات الوحدات:</span><span class="sxs-lookup"><span data-stu-id="fe041-107">Here are some examples of units and unit groups:</span></span>
 
- <span data-ttu-id="fe041-108">**مجموعة وحدات**: المسافة</span><span class="sxs-lookup"><span data-stu-id="fe041-108">**Unit group**: Distance</span></span> 
    - <span data-ttu-id="fe041-109">**الوحدات**: الميل، والكيلومتر، وهكذا.</span><span class="sxs-lookup"><span data-stu-id="fe041-109">**Units**: Mile, Kilometer, and so on.</span></span>
- <span data-ttu-id="fe041-110">**مجموعة وحدات**: الوقت</span><span class="sxs-lookup"><span data-stu-id="fe041-110">**Unit group**: Time</span></span>
    - <span data-ttu-id="fe041-111">**الوحدات**: ساعة ويوم وأسبوع وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="fe041-111">**Units**: Hour, day, week, and so on.</span></span> 

<span data-ttu-id="fe041-112">عندما تقوم بإعداد وحدات متعددة في مجموعه الوحدات، يجب عليك أيضا إعداد عامل تحويل بينهما من خلال تعيين الوحدة الأولى التي تقوم بإعدادها كوحدة افتراضية أو أساسية لمجموعة الوحدات.</span><span class="sxs-lookup"><span data-stu-id="fe041-112">When you set up multiple units in a unit group, you must also set up a conversion factor between them by designating the first unit that you set up as the default or primary unit for the unit group.</span></span> 

<span data-ttu-id="fe041-113">على سبيل المثال، في مجموعه وحدات **الوقت**، إذا قمت باعداد **الساعة** كوحدة أولى، فإن النظام يعين **الساعة** كوحدة افتراضية.</span><span class="sxs-lookup"><span data-stu-id="fe041-113">For example, in a **Time** unit group, if you set up **Hour** as the first unit, the system designates **Hour** as the default unit.</span></span> <span data-ttu-id="fe041-114">إذا كانت الوحدة التالية التي تقوم بإعدادها هي **اليوم**، فيجب عليك إعداد معامل تحويل من **يوم** إلى **ساعة**.</span><span class="sxs-lookup"><span data-stu-id="fe041-114">If the next unit that you set up is **Day**, you must set up a conversion factor for **Day** to **Hour**.</span></span> <span data-ttu-id="fe041-115">إذا أضفت بعد ذلك **الأسبوع** كوحدة ثالثة، فيجب عليك إعداد معامل تحويل **للأسبوع** في ضوء **اليوم** أو **الساعة**.</span><span class="sxs-lookup"><span data-stu-id="fe041-115">If you then add **Week** as a third unit, you must set up a conversion factor for **Week** in terms of **Day** or **Hour**.</span></span> 

<span data-ttu-id="fe041-116">تظهر الصورة التالية مثال إعداد لوحدة **اليوم**، حيث يُظهر حقل **الكمية** عدد الساعات الموجودة في يوم و**الأسبوع**، حيث يظهر حقل **الكمية**  عدد الأيام في الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="fe041-116">The following image shows an example setup for the **Day** unit, where the **Quantity** field shows the number of hours that are in a day, and **Week**, where the **Quantity** field show the number of days that are in a week.</span></span>

> ![مجموعة الوحدات: صفحة المعلومات](media/advanced-2.png)

## <a name="using-units-and-unit-groups"></a><span data-ttu-id="fe041-118">استخدام الوحدات ومجموعات الوحدات</span><span class="sxs-lookup"><span data-stu-id="fe041-118">Using units and unit groups</span></span>

<span data-ttu-id="fe041-119">يستخدم Dynamics 365 Project Service Automation الوحدات ومجموعات الوحدات لمعالجة التقديرات والإدخالات لكل من المصروفات والوقت.</span><span class="sxs-lookup"><span data-stu-id="fe041-119">Dynamics 365 Project Service Automation uses units and unit groups to process estimates and entries for both expenses and time.</span></span> 

<span data-ttu-id="fe041-120">بالنسبة للمصروفات، تشتمل كل فئة مصروفات على مجموعة وحدات افتراضية ووحدة افتراضية.</span><span class="sxs-lookup"><span data-stu-id="fe041-120">For expenses, each expense category has a default unit group and unit.</span></span> <span data-ttu-id="fe041-121">يتم إدخال هذه القيم كقيم افتراضية في إدخالات قائمة الأسعار لفئات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="fe041-121">These values are entered as default values on price list entries for expense categories.</span></span> 

<span data-ttu-id="fe041-122">علي سبيل المثال، لديك فئة مصروفات تسمي **تعويض السفر بالميل**.</span><span class="sxs-lookup"><span data-stu-id="fe041-122">For example, you have an expense category that is named **Mileage**.</span></span> <span data-ttu-id="fe041-123">وهي تحتوي علي مجموعة وحدات تسمى **المسافة** والوحدة الافتراضية تسمى **الميل**.</span><span class="sxs-lookup"><span data-stu-id="fe041-123">It has a unit group that is named **Distance** and a default unit that is named **Mile**.</span></span> <span data-ttu-id="fe041-124">إذا قمت بإعداد مجموعة وحدات **المسافة** بحيث تحتوي علي وحدتين(**الميل** **والكيلومتر**)، فيمكنك تعيين سعرين للفئة **تعويض السفر بالميل**  في قائمة أسعار واحدة: السعر لكل ميل وسعر لكل كيلومتر.</span><span class="sxs-lookup"><span data-stu-id="fe041-124">If you set up the **Distance** unit group so that it has two units (**Mile** and **Kilometer**), you can set two prices for the **Mileage** category on one price list: price per mile and price per kilometer.</span></span>

| <span data-ttu-id="fe041-125">فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="fe041-125">Expense category</span></span>  | <span data-ttu-id="fe041-126">مجموعة الوحدات</span><span class="sxs-lookup"><span data-stu-id="fe041-126">Unit group</span></span>  | <span data-ttu-id="fe041-127">الوحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-127">Unit</span></span>      | <span data-ttu-id="fe041-128">أسلوب التسعير</span><span class="sxs-lookup"><span data-stu-id="fe041-128">Pricing method</span></span>  | <span data-ttu-id="fe041-129">السعر لكل وحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-129">Price per unit</span></span>  |
|-------------------|---------------|-----------|-------------------|-------------------|
| <span data-ttu-id="fe041-130">تعويض السفر بالميل</span><span class="sxs-lookup"><span data-stu-id="fe041-130">Mileage</span></span>           | <span data-ttu-id="fe041-131">المسافة</span><span class="sxs-lookup"><span data-stu-id="fe041-131">Distance</span></span>      | <span data-ttu-id="fe041-132">ميل</span><span class="sxs-lookup"><span data-stu-id="fe041-132">Mile</span></span>      | <span data-ttu-id="fe041-133">السعر لكل وحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-133">Price per unit</span></span>    | <span data-ttu-id="fe041-134">10 دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="fe041-134">10 USD</span></span>            |
| <span data-ttu-id="fe041-135">تعويض سفر بالميل</span><span class="sxs-lookup"><span data-stu-id="fe041-135">Mileage</span></span>           | <span data-ttu-id="fe041-136">المسافة</span><span class="sxs-lookup"><span data-stu-id="fe041-136">Distance</span></span>      | <span data-ttu-id="fe041-137">كيلومتر</span><span class="sxs-lookup"><span data-stu-id="fe041-137">Kilometer</span></span> | <span data-ttu-id="fe041-138">السعر لكل وحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-138">Price per unit</span></span>    |  <span data-ttu-id="fe041-139">6 دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="fe041-139">6 USD</span></span>            |

<span data-ttu-id="fe041-140">عندما تقوم بإدخال مصروفات في مشروع، يحدد النظام السعر من خلال جمع الفئة والوحدة في المصروفات.</span><span class="sxs-lookup"><span data-stu-id="fe041-140">When you enter an expense on a project, the system determines the price through the combination of the category and the unit on the expense.</span></span> 

| <span data-ttu-id="fe041-141">وصف المصروفات</span><span class="sxs-lookup"><span data-stu-id="fe041-141">Expense description</span></span>        | <span data-ttu-id="fe041-142">فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="fe041-142">Expense category</span></span>  | <span data-ttu-id="fe041-143">الوحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-143">Unit</span></span>  | <span data-ttu-id="fe041-144">الكمية</span><span class="sxs-lookup"><span data-stu-id="fe041-144">Quantity</span></span>  | <span data-ttu-id="fe041-145">سعر الوحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-145">Unit price</span></span>   |
|----------------------------|---------------------|-------|-----------|----------------|
| <span data-ttu-id="fe041-146">القيادة إلى موقع العميل</span><span class="sxs-lookup"><span data-stu-id="fe041-146">Drive to client location</span></span> | <span data-ttu-id="fe041-147">تعويض سفر بالميل</span><span class="sxs-lookup"><span data-stu-id="fe041-147">Mileage</span></span>             | <span data-ttu-id="fe041-148">ميل</span><span class="sxs-lookup"><span data-stu-id="fe041-148">Mile</span></span>  | <span data-ttu-id="fe041-149">10</span><span class="sxs-lookup"><span data-stu-id="fe041-149">10</span></span>        | <span data-ttu-id="fe041-150">10 دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="fe041-150">10 USD</span></span>         |

<span data-ttu-id="fe041-151">بالنسبة للوقت، يكون لكل رأس قائمة أسعار حقل **وحدة الزمن الافتراضية** .</span><span class="sxs-lookup"><span data-stu-id="fe041-151">For time, each price list header has a **Default Time Unit** field.</span></span> <span data-ttu-id="fe041-152">ويتم تعيين القيمة عند إنشاء رأس قائمه الأسعار.</span><span class="sxs-lookup"><span data-stu-id="fe041-152">The value is set when you create the price list header.</span></span> <span data-ttu-id="fe041-153">ويتم استخدام هذه الوحدة بعد ذلك لتعيين كافة الأسعار المستندة إلى الأدوار في قائمة الأسعار هذه.</span><span class="sxs-lookup"><span data-stu-id="fe041-153">This unit is then used to set all role-based prices on that price list.</span></span>

<span data-ttu-id="fe041-154">يمكن التعبير عن البنود المقدرة لحقل **لوقت في عرض الأسعار** بأي وحدة زمنية.</span><span class="sxs-lookup"><span data-stu-id="fe041-154">Estimate lines for the **Time on Quote** field can be expressed in any unit of time.</span></span> <span data-ttu-id="fe041-155">ومع ذلك، يمكن أن تستخدم البنود التقديرية في المشروعات والإدخالات الزمنية للمشاريع الوحدة الزمنية **للساعة** فقط.</span><span class="sxs-lookup"><span data-stu-id="fe041-155">However, estimate lines on projects and time entries for projects can use only the **Hour** unit of time.</span></span> <span data-ttu-id="fe041-156">إذا كانت الوحدة الموجودة في الإدخال الزمني أو بند التقدير لا تطابق الوحدة الموجودة في بند قائمة الأسعار لهذا الدور، سيقوم النظام بتحويل السعر إلى الوحدات المحددة في تقدير المشروع أو الحركة الفعلية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="fe041-156">If the unit on the time entry or estimate line doesn't match the unit on the price list line for that role, the system converts the price to the units that are defined in the project estimate or the project actual transaction.</span></span>

<span data-ttu-id="fe041-157">يوضح المثال التالي كيفية استخدام PSA لمجموعات الوحدات والوحدات وعوامل التحويل.</span><span class="sxs-lookup"><span data-stu-id="fe041-157">The following example shows how PSA uses the unit group, units, and conversion factors.</span></span>
- <span data-ttu-id="fe041-158">الوحدات</span><span class="sxs-lookup"><span data-stu-id="fe041-158">Units</span></span>

   - <span data-ttu-id="fe041-159">**مجموعة وحدات**: الوقت</span><span class="sxs-lookup"><span data-stu-id="fe041-159">**Unit group**: Time</span></span> 
   - <span data-ttu-id="fe041-160">**الوحدات**: الساعة</span><span class="sxs-lookup"><span data-stu-id="fe041-160">**Units**: Hour</span></span> 
    
    - <span data-ttu-id="fe041-161">**اليوم** عمل التحويل: 8 ساعات</span><span class="sxs-lookup"><span data-stu-id="fe041-161">**Day** - Conversion factor: 8 hours</span></span>       
    - <span data-ttu-id="fe041-162">**الأسبوع** عمل التحويل: 40 ساعة</span><span class="sxs-lookup"><span data-stu-id="fe041-162">**Week** - Conversion factor: 40 hours</span></span>  
        
- <span data-ttu-id="fe041-163">اعداد قائمة الأسعار في المشروع أ:</span><span class="sxs-lookup"><span data-stu-id="fe041-163">Price list setup on Project A:</span></span>

    - <span data-ttu-id="fe041-164">**الاسم**: أسعار مبيعات المملكة المتحدة 2016</span><span class="sxs-lookup"><span data-stu-id="fe041-164">**Name**: UK sales prices 2016</span></span> 
    - <span data-ttu-id="fe041-165">**وحدة الوقت الافتراضية**: اليوم</span><span class="sxs-lookup"><span data-stu-id="fe041-165">**Default time unit**: Day</span></span> 
    - <span data-ttu-id="fe041-166">**العملة**: جنية إسترليني</span><span class="sxs-lookup"><span data-stu-id="fe041-166">**Currency**: GBP</span></span>

| <span data-ttu-id="fe041-167">الدور</span><span class="sxs-lookup"><span data-stu-id="fe041-167">Role</span></span>      | <span data-ttu-id="fe041-168">مجموعة الوحدات</span><span class="sxs-lookup"><span data-stu-id="fe041-168">Unit group</span></span> | <span data-ttu-id="fe041-169">الوحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-169">Unit</span></span> | <span data-ttu-id="fe041-170">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="fe041-170">Organizational unit</span></span> | <span data-ttu-id="fe041-171">السعر</span><span class="sxs-lookup"><span data-stu-id="fe041-171">Price</span></span>   |
|-----------|------------|------|---------------------|---------|
| <span data-ttu-id="fe041-172">المطور</span><span class="sxs-lookup"><span data-stu-id="fe041-172">Developer</span></span> | <span data-ttu-id="fe041-173">Time</span><span class="sxs-lookup"><span data-stu-id="fe041-173">Time</span></span>       | <span data-ttu-id="fe041-174">Day</span><span class="sxs-lookup"><span data-stu-id="fe041-174">Day</span></span>  | <span data-ttu-id="fe041-175">شركة حسني البريطانية</span><span class="sxs-lookup"><span data-stu-id="fe041-175">Contoso UK</span></span>          | <span data-ttu-id="fe041-176">800 جنية إسترليني</span><span class="sxs-lookup"><span data-stu-id="fe041-176">800 GBP</span></span> |

### <a name="time-entry"></a><span data-ttu-id="fe041-177">إدخال الوقت</span><span class="sxs-lookup"><span data-stu-id="fe041-177">Time entry</span></span>

<span data-ttu-id="fe041-178">يوضح الجدول التالي الحركة الناتجة بجانب المبيعات التي تم إنشاؤها بواسطة PSA لمشروع ثلاث ساعات.</span><span class="sxs-lookup"><span data-stu-id="fe041-178">The following table shows the resulting sales-side transaction created by PSA for a three hour project.</span></span>


| <span data-ttu-id="fe041-179">المشروع</span><span class="sxs-lookup"><span data-stu-id="fe041-179">Project</span></span>   | <span data-ttu-id="fe041-180">مهمة</span><span class="sxs-lookup"><span data-stu-id="fe041-180">Task</span></span>    | <span data-ttu-id="fe041-181">الدور</span><span class="sxs-lookup"><span data-stu-id="fe041-181">Role</span></span>      | <span data-ttu-id="fe041-182">الكمية</span><span class="sxs-lookup"><span data-stu-id="fe041-182">Quantity</span></span> | <span data-ttu-id="fe041-183">الوحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-183">Unit</span></span>  | <span data-ttu-id="fe041-184">سعر الوحدة</span><span class="sxs-lookup"><span data-stu-id="fe041-184">Unit price</span></span> | <span data-ttu-id="fe041-185">مبلغ المبيعات غير المفوترة</span><span class="sxs-lookup"><span data-stu-id="fe041-185">Unbilled sales amount</span></span> |
|-----------|---------|-----------|----------|-------|------------|-----------------------|
| <span data-ttu-id="fe041-186">المشروع أ</span><span class="sxs-lookup"><span data-stu-id="fe041-186">Project A</span></span> | <span data-ttu-id="fe041-187">تصميم</span><span class="sxs-lookup"><span data-stu-id="fe041-187">Design</span></span>  | <span data-ttu-id="fe041-188">المطور</span><span class="sxs-lookup"><span data-stu-id="fe041-188">Developer</span></span> | <span data-ttu-id="fe041-189">3</span><span class="sxs-lookup"><span data-stu-id="fe041-189">3</span></span>        | <span data-ttu-id="fe041-190">Hour‬</span><span class="sxs-lookup"><span data-stu-id="fe041-190">Hour</span></span>  | <span data-ttu-id="fe041-191">100 جنية إسترليني</span><span class="sxs-lookup"><span data-stu-id="fe041-191">100 GBP</span></span>    | <span data-ttu-id="fe041-192">300 جنية إسترليني</span><span class="sxs-lookup"><span data-stu-id="fe041-192">300 GBP</span></span>               |

## <a name="time-unit-faq"></a><span data-ttu-id="fe041-193">الاسئلة الشائعة للوحدة الزمنية</span><span class="sxs-lookup"><span data-stu-id="fe041-193">Time unit FAQ</span></span>

### <a name="does-psa-convert-to-different-units-in-the-case-of-expenses"></a><span data-ttu-id="fe041-194">هل يقوم PSA بالتحويل إلى وحدات مختلفة في حالة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="fe041-194">Does PSA convert to different units in the case of expenses?</span></span>
<span data-ttu-id="fe041-195">‏‏لا.</span><span class="sxs-lookup"><span data-stu-id="fe041-195">No.</span></span> <span data-ttu-id="fe041-196">لا يعمل تحويل الوحدة إلا على الوقت فقط.</span><span class="sxs-lookup"><span data-stu-id="fe041-196">Unit conversion works only for time.</span></span> <span data-ttu-id="fe041-197">بالنسبة للمصروفات، إذا لم يتمكن النظام من إيجاد سعر لمجموعة المصروفات والوحدة، سيتم تعيين السعر إلى 0.00 بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="fe041-197">For expenses, if the system can't find a price for the combination of the expense category and unit, the price is set to 0.00 by default.</span></span>

### <a name="why-does-psa-convert-time-units"></a><span data-ttu-id="fe041-198">لماذا يحول PSA الوحدات الزمنية؟</span><span class="sxs-lookup"><span data-stu-id="fe041-198">Why does PSA convert time units?</span></span>
<span data-ttu-id="fe041-199">في بعض البلدان أو المناطق، هناك متطلب قانوني بأن يتم إعداد معدل الفاتورة بالأيام.</span><span class="sxs-lookup"><span data-stu-id="fe041-199">In some countries or regions, there is a legal requirement that bill rates be set up in days.</span></span> <span data-ttu-id="fe041-200">يجري التفاوض على السعر والخصم خلال دورة عرض الأسعار باستخدام أسعار الأيام لكل دور قابل للفوترة.</span><span class="sxs-lookup"><span data-stu-id="fe041-200">Price negotiation and discounting during the quote cycle is done by using day rates for each billable role.</span></span> <span data-ttu-id="fe041-201">يتم إجراء تقدير الجدول وإدخال الوقت بالساعات.</span><span class="sxs-lookup"><span data-stu-id="fe041-201">Schedule estimation and time entry are done in hours.</span></span> <span data-ttu-id="fe041-202">لدعم هذا الاختلاف في وحدات الوقت، يقوم PSA بتحويل وحدات الزمنية.</span><span class="sxs-lookup"><span data-stu-id="fe041-202">To support this difference in time units, PSA converts time units.</span></span>

### <a name="can-time-units-be-changed-on-project-estimates"></a><span data-ttu-id="fe041-203">هل يمكن تغيير وحدات الوقت في تقديرات المشروع؟</span><span class="sxs-lookup"><span data-stu-id="fe041-203">Can time units be changed on project estimates?</span></span>
<span data-ttu-id="fe041-204">‏‏لا.</span><span class="sxs-lookup"><span data-stu-id="fe041-204">No.</span></span> <span data-ttu-id="fe041-205">يتم تقييد تقدير الجدول في الوقت الحالي إلى ساعات ولا يمكن تغييره.</span><span class="sxs-lookup"><span data-stu-id="fe041-205">Schedule estimation is currently restricted to hours and can’t be changed.</span></span>

### <a name="can-units-and-unit-groups-be-edited-deleted-and-added"></a><span data-ttu-id="fe041-206">هل يمكن تحرير الوحدات ومجموعات الوحدات وحذفها وإضافتها؟</span><span class="sxs-lookup"><span data-stu-id="fe041-206">Can units and unit groups be edited, deleted, and added?</span></span>
<span data-ttu-id="fe041-207">نعم.</span><span class="sxs-lookup"><span data-stu-id="fe041-207">Yes.</span></span> <span data-ttu-id="fe041-208">وباستثناء مجموعة واحدات  **الوقت** ووحدة**الساعة**، يمكن حذف جميع الوحدات أو تحريرها، ويمكن إضافة وحدات جديدة.</span><span class="sxs-lookup"><span data-stu-id="fe041-208">With exception of the **Time** unit group and the **Hour** unit, all units can be deleted or edited, and new units can be added.</span></span> <span data-ttu-id="fe041-209">في PSA ، لا يمكن حذف مجموعة وحدات **الوقت** ووحدة **الساعة**.</span><span class="sxs-lookup"><span data-stu-id="fe041-209">In PSA, the **Time** unit group and the **Hour** unit can't be deleted.</span></span> <span data-ttu-id="fe041-210">ومع ذلك، يمكن أن يتم تحديثها بنص مترجم لحقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="fe041-210">However, they can be updated with a translated text for the **Name** field.</span></span>
