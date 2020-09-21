---
title: إنشاء حقول وكيانات مخصصة
description: يوضح هذا الموضوع كيفية إنشاء مجموعات الخيارات والكيانات في الحل الخاص بك في نظام Power Apps الأساسي.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748720"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="ce124-103">إنشاء حقول وكيانات مخصصة</span><span class="sxs-lookup"><span data-stu-id="ce124-103">Create custom fields and entities</span></span> 

<span data-ttu-id="ce124-104">أكمل الخطوات التالية في أي وقت تريد فيه إنشاء مجموعة خيارات مخصصة أو كيان مخصص على نظام Power Apps الأساسي.</span><span class="sxs-lookup"><span data-stu-id="ce124-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="ce124-105">ينبغي إكمال الإجراءات الواردة في هذا الموضوع باستخدام واجهة ويب Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="ce124-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ce124-106">ومن المستحسن أن تقوم بإجراء كافة تغييرات أبعاد التسعير المخصصة في حل منفصل.</span><span class="sxs-lookup"><span data-stu-id="ce124-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="ce124-107">يوفر هذه الممارسة الجيدة المهمة المرونة في المستقبل لتحديث التغييرات أو إزالتها حسب الحاجة، والتي تساعد في إعادة استخدام عملك، وتسهل نقل هذه التغييرات إلى مثيل آخر.</span><span class="sxs-lookup"><span data-stu-id="ce124-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="ce124-108">بعد إجراء كافة التغييرات المطلوبة، قم بتصدير هذا الحل **كحل مُدار** واستيراده إلى المثيلات الأخرى لإعادة استخدام إعداد التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="ce124-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="ce124-109">إنشاء حل مخصص لأبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="ce124-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="ce124-110">في PSA ، انقر فوق **الإعدادات** > **الحلول**، ثم انقر فوق **جديد** لإنشاء حل جديد.</span><span class="sxs-lookup"><span data-stu-id="ce124-110">In PSA, click **Settings** > **Solutions**, and then click **New** to create a new solution.</span></span> 
2. <span data-ttu-id="ce124-111">قم بتسميه الحل، **\<اسم المؤسسة الخاصة بك > أبعاد التسعير**، وأدخل المعلومات المطلوبة المتبقية، ثم انقر فوق **حفظ.**</span><span class="sxs-lookup"><span data-stu-id="ce124-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then click **Save**.</span></span>

> ![إنشاء حل مخصص لأبعاد التسعير](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="ce124-113">إنشاء حقول مخصصة ومجموعات خيارات في حل بُعد التسعير</span><span class="sxs-lookup"><span data-stu-id="ce124-113">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="ce124-114">قد يكون بُعد التسعير مجموعة خيارات أو كيان.</span><span class="sxs-lookup"><span data-stu-id="ce124-114">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="ce124-115">يجب إنشاء كلاهما في حل التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="ce124-115">Both must be created in your pricing solution.</span></span> <span data-ttu-id="ce124-116">توضح الخطوات الواردة في هذا الإجراء كيفية إنشاء أبعاد تستند إلى الكيان وأبعاد تستند إلى مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="ce124-116">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="ce124-117">الأبعاد المستندة إلى الكيان</span><span class="sxs-lookup"><span data-stu-id="ce124-117">Entity-based dimensions</span></span>

1. <span data-ttu-id="ce124-118">في PSA ، انقر فوق **الإعدادات** > **الحلول**، ثم انقر نقرا مزدوجا فوق **\<اسم المؤسسة الخاصة بك> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="ce124-118">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="ce124-119">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="ce124-119">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="ce124-120">انقر فوق **جديد** لإنشاء كيان جديد يسمي **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="ce124-120">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="ce124-121">أدخل المعلومات المتبقية المطلوبة، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ce124-121">Enter the remaining required information, and then click **Save**.</span></span>

> ![تعريف كيان العنوان القياسي](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="ce124-123">الأبعاد المستندة إلى مجموعة الخيارات</span><span class="sxs-lookup"><span data-stu-id="ce124-123">Option set-based dimensions</span></span> 
<span data-ttu-id="ce124-124">يمكنك إنشاء بعدين يستندان إلى مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="ce124-124">You can create two option set-based dimensions.</span></span> <span data-ttu-id="ce124-125">استخدام **موقع عمل المورد** لتعقب سعر الموقع **بالمنزل** والعمل **في الموقع** واستخدم**ساعات عمل المورد** مع القيم **العادية** و**الوقت الإضافي** لتطبيق رفع السعر عند اكتمال العمل.</span><span class="sxs-lookup"><span data-stu-id="ce124-125">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="ce124-126">في PSA ، انقر فوق **الإعدادات** > **الحلول**، ثم انقر نقرا مزدوجا فوق **\<اسم المؤسسة الخاصة بك> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="ce124-126">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="ce124-127">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **مجموعات الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="ce124-127">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="ce124-128">انقر فوق **جديد** لإنشاء مجموعة خيارات جديدة، وادخل المعلومات المطلوبة المتبقية، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ce124-128">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="ce124-129">بعد التسعير المعتمد على مجموعة الخيارات يسمى موقع عمل المورد</span><span class="sxs-lookup"><span data-stu-id="ce124-129">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="ce124-130">بعد التسعير المعتمد على مجموعة الخيارات يسمى ساعات عمل المورد</span><span class="sxs-lookup"><span data-stu-id="ce124-130">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="ce124-131">إنشاء بيانات للأبعاد المستندة إلى الكيانات</span><span class="sxs-lookup"><span data-stu-id="ce124-131">Create data for entity-based dimensions</span></span>

<span data-ttu-id="ce124-132">يمكنك إنشاء بيانات للأبعاد المستندة إلى الكيانات يدويًا، أو باستخدام الاستيراد أو استدعاءات الخدمة في Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="ce124-132">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="ce124-133">استخدم الخطوات الواردة في هذا الاجراء لإنشاء عنوانين قياسيين **مهندس أنظمة** و**مهندس أنظمة متمرس**من البعد المستند إلى كيان **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="ce124-133">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="ce124-134">إذا كانت البيانات التي تريد إنشائها صغيرهة، كما هو موضح في المثال التالي، يمكنك استخدام نموذج قياسي.</span><span class="sxs-lookup"><span data-stu-id="ce124-134">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="ce124-135">في PSA، انقر فوق **بحث متقدم**.</span><span class="sxs-lookup"><span data-stu-id="ce124-135">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="ce124-136">حدد كيان **العنوان القياسي** ثم انقر فوق **النتائج**.</span><span class="sxs-lookup"><span data-stu-id="ce124-136">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="ce124-137">سيتم عرض كافة الصفوف الموجودة في كيان **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="ce124-137">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="ce124-138">انقر فوق **جديد**.</span><span class="sxs-lookup"><span data-stu-id="ce124-138">Click **New**.</span></span> <span data-ttu-id="ce124-139">في حقل **الاسم**، أدخل "مهندس الأنظمة" ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ce124-139">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="ce124-140">أغلق النموذج.</span><span class="sxs-lookup"><span data-stu-id="ce124-140">Close the form.</span></span> 
4. <span data-ttu-id="ce124-141">كرر الخطوات 1-3 لإنشاء عنوان قياسي آخر لـ "مهندس الأنظمة المتمرس".</span><span class="sxs-lookup"><span data-stu-id="ce124-141">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="ce124-142">نموذج بيانات لكيان العنوان القياسي</span><span class="sxs-lookup"><span data-stu-id="ce124-142">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="ce124-143">إضافة جميع كيانات PSA المطلوبة والمكونات ذات الصلة إلى حل بُعد التسعير</span><span class="sxs-lookup"><span data-stu-id="ce124-143">Add all required PSA entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="ce124-144">ستحتاج إلى إضافة كيانات Project Service التالية إلى حل التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="ce124-144">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="ce124-145">استخدم الخطوات الواردة في هذا الإجراء لإجراء بعض التغييرات الهامة في المخطط في حل التسعير لكي تصبح الكيانات على علم بأبعاد التسعير الجديدة.</span><span class="sxs-lookup"><span data-stu-id="ce124-145">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="ce124-146">في PSA ، انقر فوق **الإعدادات** > **الحلول**، ثم انقر نقرا مزدوجا فوق **\<اسم المؤسسة الخاصة بك> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="ce124-146">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="ce124-147">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **إضافة الموجود** > **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="ce124-147">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="ce124-148">في مربع حوار **مكونات الحل**، حدد الكيانات التالية:</span><span class="sxs-lookup"><span data-stu-id="ce124-148">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="ce124-149">فعلي</span><span class="sxs-lookup"><span data-stu-id="ce124-149">Actual</span></span>
- <span data-ttu-id="ce124-150">مورد قابل للحجز</span><span class="sxs-lookup"><span data-stu-id="ce124-150">Bookable Resource</span></span>
- <span data-ttu-id="ce124-151">سطر التقدير</span><span class="sxs-lookup"><span data-stu-id="ce124-151">Estimate Line</span></span>
- <span data-ttu-id="ce124-152">تفاصيل بند الفاتورة</span><span class="sxs-lookup"><span data-stu-id="ce124-152">Invoice Line Detail</span></span>
- <span data-ttu-id="ce124-153">سطر دفتر اليومية</span><span class="sxs-lookup"><span data-stu-id="ce124-153">Journal Line</span></span>
- <span data-ttu-id="ce124-154">تفاصيل بنود عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="ce124-154">Project Contract Line Detail</span></span>
- <span data-ttu-id="ce124-155">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="ce124-155">Project Team Member</span></span>
- <span data-ttu-id="ce124-156">تفاصيل بند عرض الأسعار‬</span><span class="sxs-lookup"><span data-stu-id="ce124-156">Quote Line Detail</span></span>
- <span data-ttu-id="ce124-157">رفع سعر الدور</span><span class="sxs-lookup"><span data-stu-id="ce124-157">Role Price Markup</span></span>
- <span data-ttu-id="ce124-158">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="ce124-158">Role Price</span></span> 
- <span data-ttu-id="ce124-159">إدخال الوقت</span><span class="sxs-lookup"><span data-stu-id="ce124-159">Time Entry</span></span> 

> ![إضافة الكيانات الموجودة إلى حل أبعاد التسعير](media/Existing-entities-to-PD-solution.png)

> ![حدد مكونات الحل](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="ce124-162">تأكد من تضمين كافة النماذج وطرق العرض لكل من الكيانات المحددة.</span><span class="sxs-lookup"><span data-stu-id="ce124-162">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="ce124-163">عند المطالبة بتضمين أية كيانات تابعة للكيانات المحددة أعلاه ، انقر فوق **لا**.</span><span class="sxs-lookup"><span data-stu-id="ce124-163">When prompted to include any dependent entities for the entities selected above, click **No**.</span></span>

> ![لا تقم بتضمين كافة المكونات ذات الصلة.](media/Do-not-include-required.png)


