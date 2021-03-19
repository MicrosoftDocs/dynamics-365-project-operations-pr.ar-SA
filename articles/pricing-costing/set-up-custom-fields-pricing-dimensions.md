---
title: 'إعداد الحقول المخصصة كأبعاد تسعير '
description: يقدم هذا الموضوع معلومات حول إعداد أبعاد التسعير باستخدام الحقول المخصصة.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1468c3396a01c1bee1bc0f47eac1ee8b44eaa459
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274847"
---
# <a name="set-up-custom-fields-as-pricing-dimensions"></a><span data-ttu-id="8e053-103">إعداد الحقول المخصصة كأبعاد تسعير </span><span class="sxs-lookup"><span data-stu-id="8e053-103">Set up custom fields as pricing dimensions</span></span>

<span data-ttu-id="8e053-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="8e053-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8e053-105">قبل البدء، يفترض هذا الموضوع أنك أكملت الإجراءات الموجودة في المواضيع، [إنشاء الحقول والكيانات المخصصة](create-custom-fields-entities-pricing-dimensions.md)و [إضافة حقول مخصصة إلى إعداد الأسعار وكيانات المعاملات](add-custom-fields-price-setup-transactional-entities.md).</span><span class="sxs-lookup"><span data-stu-id="8e053-105">Before you begin, this topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities-pricing-dimensions.md) and [Add required custom fields to price setup and transactional entities](add-custom-fields-price-setup-transactional-entities.md).</span></span> <span data-ttu-id="8e053-106">إذا لم تقم بإكمال هذه الإجراءات، فقم بالرجوع إلى الحالة السابقة وإكمالها ثم عد إلى هذا الموضوع.</span><span class="sxs-lookup"><span data-stu-id="8e053-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span> 

<span data-ttu-id="8e053-107">يقدم هذا الموضوع معلومات حول إعداد أبعاد التسعير المخصصة.</span><span class="sxs-lookup"><span data-stu-id="8e053-107">This topic provides information about setting up custom pricing dimensions.</span></span> <span data-ttu-id="8e053-108">في صفحة **المعلمات** تعرض علامة التبويب **أبعاد التسعير القائمة على المبلغ** السجلات في كيانات أبعاد التسعير.</span><span class="sxs-lookup"><span data-stu-id="8e053-108">On the **Parameters** page, the **Amount-Based Pricing Dimensions** tab shows the records in the pricing dimension entities.</span></span> <span data-ttu-id="8e053-109">وبشكل افتراضي، يوجد صفين في الشبكة على علامة التبويب هذه:</span><span class="sxs-lookup"><span data-stu-id="8e053-109">By default, there are two rows in the grid on this tab:</span></span>

- <span data-ttu-id="8e053-110">**msdyn_resourcecategory** (الدور)</span><span class="sxs-lookup"><span data-stu-id="8e053-110">**msdyn_resourcecategory** (Role)</span></span>
- <span data-ttu-id="8e053-111">**msdyn_OrganizationalUnit** (الوحدة التنظيمية)</span><span class="sxs-lookup"><span data-stu-id="8e053-111">**msdyn_OrganizationalUnit** (Organizational Unit)</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8e053-112">لا تحذف هذه الصفوف.</span><span class="sxs-lookup"><span data-stu-id="8e053-112">Do not delete these rows.</span></span> <span data-ttu-id="8e053-113">ومع ذلك، إذا لم تكن بحاجة إليها، فيمكنك جعلها غير قابلة للتطبيق في سياق محدد من خلال تعيين **قابل للتطبيق للتكلفة**، و **قابل للتطبيق للمبيعات**، و **قابل للتطبيق للشراء** جميعًا إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="8e053-113">However, if you do not need them, you can make them not applicable in a specific context by setting **Applicable to Cost**, **Applicable to Sales**, and **Applicable to Purchase** all to **No**.</span></span> <span data-ttu-id="8e053-114">ولتعيين قيم السمات هذه إلى **لا** نفس تأثير عدم وجود الحقل كبعد تسعير.</span><span class="sxs-lookup"><span data-stu-id="8e053-114">Setting these attribute values to **No** has the same effect of not having the field as a pricing dimension.</span></span>

<span data-ttu-id="8e053-115">ولكي يصبح الحقل بعد تسعير، يجب أن يكون:</span><span class="sxs-lookup"><span data-stu-id="8e053-115">For a field to become a pricing dimension, it must be:</span></span>

- <span data-ttu-id="8e053-116">تم إنشاؤه كحقل في كياني **سعر الدور** و **رفع سعر الدور**.</span><span class="sxs-lookup"><span data-stu-id="8e053-116">Created as a field in the **Role Price** and **Role Price markup** entities.</span></span> <span data-ttu-id="8e053-117">لمزيد من المعلومات حول كيفية القيام بهذا، راجع [إضافة الحقول المخصصة إلى كيانات المعاملات وإعداد الأسعار](add-custom-fields-price-setup-transactional-entities.md).</span><span class="sxs-lookup"><span data-stu-id="8e053-117">For more information on how to do this, see [Add custom fields to price setup and transactional entities](add-custom-fields-price-setup-transactional-entities.md).</span></span>

- <span data-ttu-id="8e053-118">تم إنشاؤه كصف في جدول **بعد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="8e053-118">Created as a row in the **Pricing Dimension** table.</span></span> <span data-ttu-id="8e053-119">على سبيل المثال، أضف صفوف أبعاد التسعير كما هو موضح في الرسم التالي.</span><span class="sxs-lookup"><span data-stu-id="8e053-119">For example, add pricing dimension rows as shown in the following graphic.</span></span> 

![صفوف أبعاد التسعير المستندة إلى المبلغ](media/Amt-based-PD.png)

<span data-ttu-id="8e053-121">تمت إضافة ساعات عمل المورد (**msdyn_resourceworkhours**) كبعد يستند مستند إلى رفع السعر وتمت إضافتها إلى الشبكة في علامة التبويب **بعد التسعير المستند إلى رفع السعر**.</span><span class="sxs-lookup"><span data-stu-id="8e053-121">Resource Work hours (**msdyn_resourceworkhours**) is added as a markup-based dimension and has been added to the grid on the **Markup Based Pricing Dimension** tab.</span></span>

![صفوف أبعاد التسعير المستندة إلى رفع السعر](media/Markup-based-PD.png)


> [!IMPORTANT]
> <span data-ttu-id="8e053-123">يتم نشر أي تغييرات على بيانات أبعاد التسعير الموجودة في هذا الجدول الحالي أو الجديد لمنطق التسعير فقد بعد تحديث ذاكرة التخزين المؤقت.</span><span class="sxs-lookup"><span data-stu-id="8e053-123">Any change to pricing dimension data in this table, existing or new, is propagated to the pricing business logic only after the cache is refreshed.</span></span> <span data-ttu-id="8e053-124">قد يستغرق وقت تحديث ذاكرة التخزين المؤقت حتى 10 دقائق.</span><span class="sxs-lookup"><span data-stu-id="8e053-124">The cache refresh time may take up to 10 minutes.</span></span> <span data-ttu-id="8e053-125">اسمح لطول المدة بمشاهدة التغييرات في منطق افتراض الأسعار الذي يجب أن ينتج عن التغييرات في بيانات بُعد التسعير.</span><span class="sxs-lookup"><span data-stu-id="8e053-125">Allow that length of time to see the changes in price defaulting logic that must result from changes to the Pricing Dimension data.</span></span>


## <a name="attributes-of-the-pricing-dimensions-table"></a><span data-ttu-id="8e053-126">سمات جدول أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="8e053-126">Attributes of the Pricing Dimensions table</span></span>
<span data-ttu-id="8e053-127">توفر الأقسام التالية معلومات عن السمات المختلفة في جدول **أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="8e053-127">The following sections provide information about the different attributes in the **Pricing Dimensions** table.</span></span>

### <a name="pricing-dimension-name"></a><span data-ttu-id="8e053-128">اسم بُعد التسعير</span><span class="sxs-lookup"><span data-stu-id="8e053-128">Pricing Dimension Name</span></span>
<span data-ttu-id="8e053-129">يجب أن تكون هذه القيمة مطابقه لاسم المخطط الخاص بالحقل الذي تمت إضافته إلى جدول **سعر الدور** لأبعاد التسعير المخصصة.</span><span class="sxs-lookup"><span data-stu-id="8e053-129">This value should be the exact same as the schema name of the field that is added to the **Role Price** table for custom pricing dimensions.</span></span> <span data-ttu-id="8e053-130">لمزيد من المعلومات حول إضافة الحقول إلى جدول **سعر الدور**، راجع [إضافة حقول مخصصة إلى كيانات المعاملات وإعداد الأسعار](add-custom-fields-price-setup-transactional-entities.md).</span><span class="sxs-lookup"><span data-stu-id="8e053-130">For more information about adding fields to the **Role Price** table, see [Add custom fields to price setup and transactional entities](add-custom-fields-price-setup-transactional-entities.md).</span></span>

### <a name="type-of-dimension"></a><span data-ttu-id="8e053-131">نوع البُعد</span><span class="sxs-lookup"><span data-stu-id="8e053-131">Type of dimension</span></span>
<span data-ttu-id="8e053-132">هناك نوعان من أبعاد التسعير:</span><span class="sxs-lookup"><span data-stu-id="8e053-132">There are two types of pricing dimensions:</span></span>
  
  - <span data-ttu-id="8e053-133">**الأبعاد المستندة إلى المبلغ**: تتم مطابقه قيم الأبعاد من سياق الإدخال بقيم الأبعاد الموجودة في بند **سعر الدور** ويتم تعيين السعر/التكلفة افتراضيا مباشرةً من جدول **سعر الدور**.</span><span class="sxs-lookup"><span data-stu-id="8e053-133">**Amount-based dimensions**: The dimension values from the input context are matched to the dimension values on **Role Price** line and the price/cost is defaulted directly from the **Role Price** table.</span></span>
  - <span data-ttu-id="8e053-134">**الأبعاد المستندة إلى رفع السعر**: هذه هي الأبعاد التي ستُستخدم فيها العملية التالية المكونة من ثلاثة خطوات للحصول على السعر/التكلفة:</span><span class="sxs-lookup"><span data-stu-id="8e053-134">**Markup-based dimensions**: These are dimensions where the following three-step process to get the price/cost is used:</span></span>
 
    1. <span data-ttu-id="8e053-135">تتطابق قيم الأبعاد المستندة إلى غير رفع الأسعار من سياق الإدخال مع بند سعر الدور للحصول على السعر الأساسي.</span><span class="sxs-lookup"><span data-stu-id="8e053-135">The non-markup-based dimension values from the input context are matched to the Role Price line to get the base rate.</span></span>
    2. <span data-ttu-id="8e053-136">تتطابق قيم الأبعاد من سياق الإدخال ببند **رفع سعر الدور** للحصول على نسبة مئوية لرفع السعر.</span><span class="sxs-lookup"><span data-stu-id="8e053-136">The dimension values from the input context are matched to the **Role Price Markup** line to get a markup percentage.</span></span>
    3. <span data-ttu-id="8e053-137">تطبق النسبة المئوية لرفع السعر من الخطوة الثانية على السعر الأساسي الذي تم الحصول عليه من جدول **سعر الدور** في الخطوة الأولى للوصول إلى السعر/التكلفة النهائية.</span><span class="sxs-lookup"><span data-stu-id="8e053-137">The markup percentage from the second step is applied to the base rate obtained from the **Role Price** table in the first step to arrive at final price/cost.</span></span>
   
   <span data-ttu-id="8e053-138">يوضح الجدول التالي حساب عمليات رفع الأسعار.</span><span class="sxs-lookup"><span data-stu-id="8e053-138">The following table illustrates the calculation of price markups.</span></span>
  
| <span data-ttu-id="8e053-139">الدور</span><span class="sxs-lookup"><span data-stu-id="8e053-139">Role</span></span>        | <span data-ttu-id="8e053-140">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="8e053-140">Org Unit</span></span>    |<span data-ttu-id="8e053-141">موقع العمل</span><span class="sxs-lookup"><span data-stu-id="8e053-141">Work Location</span></span>      |<span data-ttu-id="8e053-142">العنوان القياسي</span><span class="sxs-lookup"><span data-stu-id="8e053-142">Standard Title</span></span>      |<span data-ttu-id="8e053-143">ساعات عمل الموارد</span><span class="sxs-lookup"><span data-stu-id="8e053-143">Resource Work Hours</span></span>      |  <span data-ttu-id="8e053-144">رفع السعر</span><span class="sxs-lookup"><span data-stu-id="8e053-144">Mark Up</span></span>|
| ------------|-------------|-------------------|--------------------|-------------------------|--------:|
|             | <span data-ttu-id="8e053-145">شركة حسني بالهند</span><span class="sxs-lookup"><span data-stu-id="8e053-145">Contoso India</span></span>|<span data-ttu-id="8e053-146">في الموقع</span><span class="sxs-lookup"><span data-stu-id="8e053-146">Onsite</span></span>            |                    |<span data-ttu-id="8e053-147">العمل الإضافي</span><span class="sxs-lookup"><span data-stu-id="8e053-147">Overtime</span></span>                 |<span data-ttu-id="8e053-148">15</span><span class="sxs-lookup"><span data-stu-id="8e053-148">15</span></span>     |
|             | <span data-ttu-id="8e053-149">شركة حسني بالهند</span><span class="sxs-lookup"><span data-stu-id="8e053-149">Contoso India</span></span>|<span data-ttu-id="8e053-150">محلي</span><span class="sxs-lookup"><span data-stu-id="8e053-150">Local</span></span>             |                    |<span data-ttu-id="8e053-151">العمل الإضافي</span><span class="sxs-lookup"><span data-stu-id="8e053-151">Overtime</span></span>                 |<span data-ttu-id="8e053-152">10</span><span class="sxs-lookup"><span data-stu-id="8e053-152">10</span></span>     |
|             | <span data-ttu-id="8e053-153">Contoso US</span><span class="sxs-lookup"><span data-stu-id="8e053-153">Contoso US</span></span>   |<span data-ttu-id="8e053-154">محلي</span><span class="sxs-lookup"><span data-stu-id="8e053-154">Local</span></span>             |                    |<span data-ttu-id="8e053-155">العمل الإضافي</span><span class="sxs-lookup"><span data-stu-id="8e053-155">Overtime</span></span>                 |<span data-ttu-id="8e053-156">20</span><span class="sxs-lookup"><span data-stu-id="8e053-156">20</span></span>     |


<span data-ttu-id="8e053-157">إذا كان هناك مورد من شركة حسني بالهند والذي يبلغ سعره الأساسي 100 دولار أمريكي يعمل في الموقع، ويقوم بتسجيل 8 ساعات من الوقت العادي وساعتين من الوقت الإضافي عند الدخول، فسوف يستخدم محرك التسعير السعر الأساسي 100 لمدة 8 ساعات لتسجيل 800 دولار.</span><span class="sxs-lookup"><span data-stu-id="8e053-157">If a resource from Contoso India whose base rate is 100 USD is working onsite, and they log 8 hours of Regular time and 2 hours of overtime on the time entry, the pricing engine will use the base rate of 100 for the 8 hours to record 800 USD.</span></span> <span data-ttu-id="8e053-158">خلال ساعتي العمل الإضافيتين، سيتم تطبيق رفع سعر بنسبة 15٪ على السعر الأساسي 100 للحصول على سعر الوحدة البالغ 115 دولارًا أمريكيًا وسيسجل تكلفة إجمالية قدرها 230 دولارًا أمريكيًا.</span><span class="sxs-lookup"><span data-stu-id="8e053-158">For the 2 hours overtime, a markup of 15% will be applied to the base rate of 100 to get a unit price of 115 USD and will record a total cost of 230 USD.</span></span>

### <a name="applicable-to-cost"></a><span data-ttu-id="8e053-159">قابل للتطبيق على التكلفة</span><span class="sxs-lookup"><span data-stu-id="8e053-159">Applicable to Cost</span></span> 
<span data-ttu-id="8e053-160">إذا تم تعيين هذا إلى **نعم**، فإنه يشير إلى أن قيمة البعد من سياق الإدخال يجب استخدامها لمطابقة **سعر الدور** و **رفع سعر الدور** عند استرداد أسعار التكلفة ورفع السعر.</span><span class="sxs-lookup"><span data-stu-id="8e053-160">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the cost and markup rates.</span></span>

### <a name="applicable-to-sales"></a><span data-ttu-id="8e053-161">قابل للتطبيق على المبيعات</span><span class="sxs-lookup"><span data-stu-id="8e053-161">Applicable to Sales</span></span>
<span data-ttu-id="8e053-162">إذا تم تعيين هذا إلى **نعم**، فإنه يشير إلى أن قيمة البعد من سياق الإدخال يجب استخدامها لمطابقة **سعر الدور** و **رفع سعر الدور** عند استرداد أسعار الفاتورة ورفع السعر.</span><span class="sxs-lookup"><span data-stu-id="8e053-162">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the bill and markup rates.</span></span>

### <a name="applicable-to-purchase"></a><span data-ttu-id="8e053-163">قابل للتطبيق على الشراء</span><span class="sxs-lookup"><span data-stu-id="8e053-163">Applicable to Purchase</span></span>
<span data-ttu-id="8e053-164">إذا تم تعيين هذا إلى **نعم**، فإنه يشير إلى أن قيمة البعد من سياق الإدخال يجب استخدامها لمطابقة **سعر الدور** و **رفع سعر الدور** عند استرداد سعر الشراء.</span><span class="sxs-lookup"><span data-stu-id="8e053-164">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the purchase price.</span></span> <span data-ttu-id="8e053-165">سيناريوهات التعاقد من الباطن غير مدعومة، بالتالي لا يتم استخدام هذا الحقل.</span><span class="sxs-lookup"><span data-stu-id="8e053-165">Subcontracting scenarios are not supported, so this field is not used.</span></span> 

### <a name="priority"></a><span data-ttu-id="8e053-166">الأولوية</span><span class="sxs-lookup"><span data-stu-id="8e053-166">Priority</span></span>
<span data-ttu-id="8e053-167">يساعد تعيين أولوية البعد التسعير على تقديم سعر حتى إذا لم يتمكن من العثور على مطابقة تامة بين قيم أبعاد الإدخالات والقيم الواردة من جدول **سعر الدور** أو **رفع سعر الدور**.</span><span class="sxs-lookup"><span data-stu-id="8e053-167">Setting the dimension priority helps pricing produce a price even when it can't find an exact match between the input dimension values and the values from the **Role Price** or **Role Price Markup** tables.</span></span> <span data-ttu-id="8e053-168">في هذا السيناريو، ستستخدم القيم الخالية لقيم الأبعاد غير المتطابقة عن طريق وزن الأبعاد حسب أولوياتها.</span><span class="sxs-lookup"><span data-stu-id="8e053-168">In this scenario, null values are used for unmatched dimension values by weighing the dimensions in order of their priority.</span></span>

- <span data-ttu-id="8e053-169">**أولوية التكلفة**: ستشير قيمة أولوية تكلفة البعد إلى الوزن الخاص بهذا البعد عند إجراء المطابقة مقابل إعداد أسعار التكلفة.</span><span class="sxs-lookup"><span data-stu-id="8e053-169">**Cost Priority**: The value of a dimension's cost priority will indicate the weight of that dimension when matching against the setup of cost prices.</span></span> <span data-ttu-id="8e053-170">يجب أن تكون قيمة **أولوية التكلفة** فريدة عبر الأبعاد **القابلة للتطبيق على التكلفة**.</span><span class="sxs-lookup"><span data-stu-id="8e053-170">The value of **Cost Priority** must be unique across dimensions that are **Applicable to Cost**.</span></span>
- <span data-ttu-id="8e053-171">**أولوية المبيعات**: ستشير قيمة أولوية مبيعات البعد إلى الوزن الخاص بهذا البعد عند إجراء المطابقة مقابل إعداد أسعار المبيعات أو أسعار الفواتير.</span><span class="sxs-lookup"><span data-stu-id="8e053-171">**Sales Priority**: The value of dimension's sales priority will indicate the weight of that dimension when matching against the setup of sales prices or bill rates.</span></span> <span data-ttu-id="8e053-172">يجب أن تكون قيمة **أولوية المبيعات** فريدة عبر الأبعاد **القابلة للتطبيق على المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="8e053-172">The value of **Sales Priority** must be unique across dimensions that are **Applicable to Sales**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]