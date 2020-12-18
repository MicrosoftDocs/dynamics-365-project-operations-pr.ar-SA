---
title: إنشاء حقول وكيانات مخصصة كأبعاد تسعير
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء مجموعات الخيارات أو الكيانات المخصصة.
author: rumant
manager: AnnBe
ms.date: 11/18/2020
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: fc5917856b8f28d36dc55593a68eba7823a00b36
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642797"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="55b28-103">إنشاء حقول وكيانات مخصصة كأبعاد تسعير</span><span class="sxs-lookup"><span data-stu-id="55b28-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="55b28-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="55b28-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="55b28-105">أكمل الخطوات التالية عندما تريد إنشاء كيان أو مجموعة خيارات مخصصة لاستخدامها كبُعد تسعير.</span><span class="sxs-lookup"><span data-stu-id="55b28-105">Complete the following steps when you want to create a custom option set or entity for using it as a pricing dimension.</span></span> <span data-ttu-id="55b28-106">للاطلاع على مزيد من المعلومات، راجع [نظرة عامة على أبعاد الأسعار](pricing-dimensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="55b28-106">For more information, see [Pricing dimensions overview](pricing-dimensions-overview.md).</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="55b28-107">ومن المستحسن أن تقوم بإجراء كافة تغييرات أبعاد التسعير المخصصة في حل منفصل.</span><span class="sxs-lookup"><span data-stu-id="55b28-107">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="55b28-108">توفر هذه الممارسة الأفضل الهامة المرونة في المستقبل لتحديث أو إزالة التغييرات حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="55b28-108">This important best practice provides flexibility in the future to update or remove changes as needed.</span></span> <span data-ttu-id="55b28-109">سيساعد هذا أيضًا في إعادة استخدام عملك وتسهيل تنفيذ هذه التغييرات إلى مثيل آخر بعد إجراء كافة التغييرات المطلوبة، قم بتصدير هذا الحل كـ **حل مُدار** واستيراده إلى مثيلات أخرى لإعادة استخدام إعداد التسعير.</span><span class="sxs-lookup"><span data-stu-id="55b28-109">This will also help with re-use of your work and make it easier to port these changes to another instance After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="55b28-110">إنشاء حقول مخصصة ومجموعات خيارات في حل بُعد التسعير</span><span class="sxs-lookup"><span data-stu-id="55b28-110">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="55b28-111">قد يكون بُعد التسعير مجموعة خيارات أو كيان.</span><span class="sxs-lookup"><span data-stu-id="55b28-111">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="55b28-112">يجب إنشاء كلاهما في حل التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="55b28-112">Both must be created in your pricing solution.</span></span> <span data-ttu-id="55b28-113">توضح الخطوات الواردة في هذا الإجراء كيفية إنشاء أبعاد تستند إلى الكيان وأبعاد تستند إلى مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="55b28-113">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="55b28-114">الأبعاد المستندة إلى الكيان</span><span class="sxs-lookup"><span data-stu-id="55b28-114">Entity-based dimensions</span></span>
<span data-ttu-id="55b28-115">لإنشاء أبعاد تستند إلى الكيان، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="55b28-115">To create entity-based dimensions, follow these steps:</span></span>

1. <span data-ttu-id="55b28-116">انتقل إلى **إعدادات** > **حلول**، وانقر نقرًا مزدوجًا فوق **\<your organization name> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="55b28-116">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="55b28-117">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="55b28-117">In Solution Explorer, in the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="55b28-118">حدد **جديد** لإنشاء كيان جديد يسمي **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="55b28-118">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="55b28-119">أدخل المعلومات المتبقية المطلوبة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="55b28-119">Enter the remaining required information, and then select **Save**.</span></span>

> ![تعريف كيان العنوان القياسي](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a><span data-ttu-id="55b28-121">الأبعاد المستندة إلى مجموعة الخيارات</span><span class="sxs-lookup"><span data-stu-id="55b28-121">Option set-based dimensions</span></span> 
<span data-ttu-id="55b28-122">يمكنك إنشاء بعدين يستندان إلى مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="55b28-122">You can create two option set-based dimensions.</span></span> 

- <span data-ttu-id="55b28-123">استخدم **موقع عمل الموارد** لتعقب سعر العمل في الموقع **الرئيسي** والعمل **في الموقع**.</span><span class="sxs-lookup"><span data-stu-id="55b28-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work.</span></span> 
- <span data-ttu-id="55b28-124">استخدم **ساعات عمل الموارد** مع القيم **منتظمة** و **الوقت الإضافي** لاستخدام ترميز عند اكتمال العمل.</span><span class="sxs-lookup"><span data-stu-id="55b28-124">Use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when the work is complete.</span></span>

<span data-ttu-id="55b28-125">يوفر الرسم التالي طريقة عرض بعد **موقع عمل الموارد**.</span><span class="sxs-lookup"><span data-stu-id="55b28-125">The following graphic provides a view of the **Resource Work Location** dimension.</span></span> 

> ![بعد التسعير المعتمد على مجموعة الخيارات يسمى موقع عمل المورد](media/Option-set-PD-called-Resource-Work-Location.png)

<span data-ttu-id="55b28-127">يوفر الرسم التالي طريقة عرض بعد **ساعات عمل الموارد**.</span><span class="sxs-lookup"><span data-stu-id="55b28-127">The following graphic provides a view of the **Resource Work Hours** dimension.</span></span> 

> ![بعد التسعير المعتمد على مجموعة الخيارات يسمى ساعات عمل المورد](media/Option-set-PD-called-Resource-Work-Hours.png)

1. <span data-ttu-id="55b28-129">انتقل إلى **إعدادات** > **حلول**، وانقر نقرًا مزدوجًا فوق  **\<your organization name> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="55b28-129">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="55b28-130">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **مجموعات الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="55b28-130">In Solution Explorer, in the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="55b28-131">حدد **جديد** لإنشاء مجموعة خيارات جديدة، وادخل المعلومات المطلوبة المتبقية، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="55b28-131">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="55b28-132">إنشاء بيانات للأبعاد المستندة إلى الكيانات</span><span class="sxs-lookup"><span data-stu-id="55b28-132">Create data for entity-based dimensions</span></span>

<span data-ttu-id="55b28-133">يمكنك إنشاء بيانات للأبعاد المستندة إلى الكيانات يدويًا، أو باستخدام الاستيراد أو استدعاءات الخدمة في Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="55b28-133">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="55b28-134">استخدم الخطوات الواردة في هذا الإجراء لإنشاء عنوانين قياسيين **مهندس أنظمة** و **مهندس أنظمة متمرس** من البعد المستند إلى كيان **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="55b28-134">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="55b28-135">إذا كانت البيانات التي تريد إنشائها صغيرهة، كما هو موضح في المثال التالي، يمكنك استخدام نموذج قياسي.</span><span class="sxs-lookup"><span data-stu-id="55b28-135">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="55b28-136">حدد **البحث المتقدم**.</span><span class="sxs-lookup"><span data-stu-id="55b28-136">Select **Advanced Find**.</span></span>
2. <span data-ttu-id="55b28-137">حدد كيان **العنوان القياسي**، ثم حدد **النتائج**.</span><span class="sxs-lookup"><span data-stu-id="55b28-137">Select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="55b28-138">سيتم عرض كافة الصفوف الموجودة في كيان **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="55b28-138">All of the rows in the **Standard Title** entity will be shown.</span></span>
3. <span data-ttu-id="55b28-139">حدد **جديد**، وفي حقل **الاسم** ، أدخل "مهندس الأنظمة" ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="55b28-139">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
4. <span data-ttu-id="55b28-140">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="55b28-140">Close the page.</span></span> 
5. <span data-ttu-id="55b28-141">كرر الخطوات 1-3 لإنشاء عنوان قياسي آخر لـ "مهندس الأنظمة المتمرس".</span><span class="sxs-lookup"><span data-stu-id="55b28-141">Repeat steps 1-3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![نموذج بيانات لكيان العنوان القياسي](media/ST-data.png)
