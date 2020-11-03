---
title: إنشاء حقول وكيانات مخصصة كأبعاد تسعير
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء مجموعات الخيارات أو الكيانات المخصصة.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9dd43be79f8e906298578911b3bff03e66c2f1e5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070682"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="8ffdc-103">إنشاء حقول وكيانات مخصصة كأبعاد تسعير</span><span class="sxs-lookup"><span data-stu-id="8ffdc-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="8ffdc-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="8ffdc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8ffdc-105">أكمل الخطوات التالية في أي وقت تريد فيه إنشاء مجموعة خيارات مخصصة أو كيان مخصص.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-105">Complete the following steps any time that you want to create a custom option set or entity.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8ffdc-106">ومن المستحسن أن تقوم بإجراء كافة تغييرات أبعاد التسعير المخصصة في حل منفصل.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="8ffdc-107">يوفر هذه الممارسة الجيدة المهمة المرونة في المستقبل لتحديث التغييرات أو إزالتها حسب الحاجة، والتي تساعد في إعادة استخدام عملك، وتسهل نقل هذه التغييرات إلى مثيل آخر.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="8ffdc-108">بعد إجراء كافة التغييرات المطلوبة، قم بتصدير هذا الحل **كحل مُدار** واستيراده إلى المثيلات الأخرى لإعادة استخدام إعداد التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="8ffdc-109">إنشاء حل مخصص لأبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="8ffdc-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="8ffdc-110">انتقل إلى **الإعدادات** > **الحلول** ، ثم حدد **جديد** لإنشاء حل جديد.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-110">Go to **Settings** > **Solutions** , and then select **New** to create a new solution.</span></span> 
2. <span data-ttu-id="8ffdc-111">قم بتسميه الحل، **\<your organization name> أبعاد التسعير** ، وأدخل المعلومات المطلوبة المتبقية، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-111">Name the solution, **\<your organization name> pricing dimensions** , enter the remaining required information, and then select **Save**.</span></span>
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="8ffdc-112">إنشاء حقول مخصصة ومجموعات خيارات في حل بُعد التسعير</span><span class="sxs-lookup"><span data-stu-id="8ffdc-112">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="8ffdc-113">قد يكون بُعد التسعير مجموعة خيارات أو كيان.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-113">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="8ffdc-114">يجب إنشاء كلاهما في حل التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-114">Both must be created in your pricing solution.</span></span> <span data-ttu-id="8ffdc-115">توضح الخطوات الواردة في هذا الإجراء كيفية إنشاء أبعاد تستند إلى الكيان وأبعاد تستند إلى مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-115">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="8ffdc-116">الأبعاد المستندة إلى الكيان</span><span class="sxs-lookup"><span data-stu-id="8ffdc-116">Entity-based dimensions</span></span>

1. <span data-ttu-id="8ffdc-117">انتقل إلى **إعدادات** > **حلول** ، وانقر نقرًا مزدوجًا فوق **\<your organization name> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-117">Go to **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="8ffdc-118">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-118">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="8ffdc-119">حدد **جديد** لإنشاء كيان جديد يسمي **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-119">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="8ffdc-120">أدخل المعلومات المتبقية المطلوبة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-120">Enter the remaining required information, and then select **Save**.</span></span>


### <a name="option-set-based-dimensions"></a><span data-ttu-id="8ffdc-121">الأبعاد المستندة إلى مجموعة الخيارات</span><span class="sxs-lookup"><span data-stu-id="8ffdc-121">Option set-based dimensions</span></span> 
<span data-ttu-id="8ffdc-122">يمكنك إنشاء بعدين يستندان إلى مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-122">You can create two option set-based dimensions.</span></span> <span data-ttu-id="8ffdc-123">استخدام **موقع عمل المورد** لتعقب سعر الموقع **بالمنزل** والعمل **في الموقع** واستخدم **ساعات عمل المورد** مع القيم **العادية** و **الوقت الإضافي** لتطبيق رفع السعر عند اكتمال العمل.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="8ffdc-124">انتقل إلى **إعدادات** > **حلول** ، وانقر نقرًا مزدوجًا فوق  **\<your organization name> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-124">Go to **Settings** > **Solutions** , and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="8ffdc-125">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **مجموعات الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-125">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="8ffdc-126">حدد **جديد** لإنشاء مجموعة خيارات جديدة، وادخل المعلومات المطلوبة المتبقية، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-126">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="8ffdc-127">إنشاء بيانات للأبعاد المستندة إلى الكيانات</span><span class="sxs-lookup"><span data-stu-id="8ffdc-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="8ffdc-128">يمكنك إنشاء بيانات للأبعاد المستندة إلى الكيانات يدويًا، أو باستخدام الاستيراد أو استدعاءات الخدمة في Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="8ffdc-129">استخدم الخطوات الواردة في هذا الإجراء لإنشاء عنوانين قياسيين **مهندس أنظمة** و **مهندس أنظمة متمرس** من البعد المستند إلى كيان **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="8ffdc-130">إذا كانت البيانات التي تريد إنشائها صغيرهة، كما هو موضح في المثال التالي، يمكنك استخدام نموذج قياسي.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="8ffdc-131">حدد **بحث متقدم** ، حدد **العنوان القياسي** للكيان، ثم حدد **النتائج**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-131">Select **Advanced Find** , select the entity **Standard Title** , and then select **Results**.</span></span> <span data-ttu-id="8ffdc-132">سيتم عرض كافة الصفوف الموجودة في كيان **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-132">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="8ffdc-133">حدد **جديد** ، وفي حقل **الاسم** ، أدخل "مهندس الأنظمة" ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-133">Select **New** , and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
3. <span data-ttu-id="8ffdc-134">إغلاق النموذج.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-134">Close the form.</span></span> 
4. <span data-ttu-id="8ffdc-135">كرر الخطوات 1-3 لإنشاء عنوان قياسي آخر لـ "مهندس الأنظمة المتمرس".</span><span class="sxs-lookup"><span data-stu-id="8ffdc-135">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="8ffdc-136">إضافة جميع الكيانات المطلوبة والمكونات ذات الصلة إلى حل بُعد التسعير</span><span class="sxs-lookup"><span data-stu-id="8ffdc-136">Add all required entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="8ffdc-137">ستحتاج إلى إضافة الكيانات التالية إلى حل التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-137">You will need to add the following entities to your pricing solution.</span></span> <span data-ttu-id="8ffdc-138">استخدم الخطوات الواردة في هذا الإجراء لإجراء بعض التغييرات الهامة في المخطط في حل التسعير لكي تصبح الكيانات على علم بأبعاد التسعير الجديدة.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-138">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="8ffdc-139">حدد **إعدادات** > **حلول** ، وانقر نقرًا مزدوجًا فوق **\<your organization name> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-139">Select **Settings** > **Solutions** , and double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="8ffdc-140">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **إضافة الموجود** > **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-140">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="8ffdc-141">في مربع حوار **مكونات الحل** ، حدد الكيانات التالية:</span><span class="sxs-lookup"><span data-stu-id="8ffdc-141">In the **Solution Components** dialog box, select the following entities:</span></span>

  - <span data-ttu-id="8ffdc-142">فعلي</span><span class="sxs-lookup"><span data-stu-id="8ffdc-142">Actual</span></span>
  - <span data-ttu-id="8ffdc-143">مورد قابل للحجز</span><span class="sxs-lookup"><span data-stu-id="8ffdc-143">Bookable Resource</span></span>
  - <span data-ttu-id="8ffdc-144">سطر التقدير</span><span class="sxs-lookup"><span data-stu-id="8ffdc-144">Estimate Line</span></span>
  - <span data-ttu-id="8ffdc-145">تفاصيل بند الفاتورة</span><span class="sxs-lookup"><span data-stu-id="8ffdc-145">Invoice Line Detail</span></span>
  - <span data-ttu-id="8ffdc-146">سطر دفتر اليومية</span><span class="sxs-lookup"><span data-stu-id="8ffdc-146">Journal Line</span></span>
  - <span data-ttu-id="8ffdc-147">تفاصيل بنود عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="8ffdc-147">Project Contract Line Detail</span></span>
  - <span data-ttu-id="8ffdc-148">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="8ffdc-148">Project Team Member</span></span>
  - <span data-ttu-id="8ffdc-149">تفاصيل بند عرض الأسعار‬</span><span class="sxs-lookup"><span data-stu-id="8ffdc-149">Quote Line Detail</span></span>
  - <span data-ttu-id="8ffdc-150">رفع سعر الدور</span><span class="sxs-lookup"><span data-stu-id="8ffdc-150">Role Price Markup</span></span>
  - <span data-ttu-id="8ffdc-151">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="8ffdc-151">Role Price</span></span> 
  - <span data-ttu-id="8ffdc-152">إدخال الوقت</span><span class="sxs-lookup"><span data-stu-id="8ffdc-152">Time Entry</span></span> 


> [!NOTE]
> <span data-ttu-id="8ffdc-153">تأكد من تضمين كافة النماذج وطرق العرض لكل من الكيانات المحددة.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-153">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="8ffdc-154">عند المطالبة بتضمين أية كيانات تابعة للكيانات المحددة أعلاه ، حدد **لا**.</span><span class="sxs-lookup"><span data-stu-id="8ffdc-154">When prompted to include any dependent entities for the entities selected above, select **No**.</span></span>

