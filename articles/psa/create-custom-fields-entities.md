---
title: إنشاء حقول وكيانات مخصصة
description: يوضح هذا الموضوع كيفية إنشاء مجموعات الخيارات والكيانات في الحل الخاص بك في نظام Power Apps الأساسي.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 442ff9cf2206bec307cea7ff30b9266502d8f77b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070713"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="19e4c-103">إنشاء حقول وكيانات مخصصة</span><span class="sxs-lookup"><span data-stu-id="19e4c-103">Create custom fields and entities</span></span> 

<span data-ttu-id="19e4c-104">أكمل الخطوات التالية في أي وقت تريد فيه إنشاء مجموعة خيارات مخصصة أو كيان مخصص على نظام Power Apps الأساسي.</span><span class="sxs-lookup"><span data-stu-id="19e4c-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="19e4c-105">ينبغي إكمال الإجراءات الواردة في هذا الموضوع باستخدام واجهة ويب Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="19e4c-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="19e4c-106">ومن المستحسن أن تقوم بإجراء كافة تغييرات أبعاد التسعير المخصصة في حل منفصل.</span><span class="sxs-lookup"><span data-stu-id="19e4c-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="19e4c-107">يوفر هذه الممارسة الجيدة المهمة المرونة في المستقبل لتحديث التغييرات أو إزالتها حسب الحاجة، والتي تساعد في إعادة استخدام عملك، وتسهل نقل هذه التغييرات إلى مثيل آخر.</span><span class="sxs-lookup"><span data-stu-id="19e4c-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="19e4c-108">بعد إجراء كافة التغييرات المطلوبة، قم بتصدير هذا الحل **كحل مُدار** واستيراده إلى المثيلات الأخرى لإعادة استخدام إعداد التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="19e4c-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="19e4c-109">إنشاء حقول مخصصة ومجموعات خيارات في حل بُعد التسعير</span><span class="sxs-lookup"><span data-stu-id="19e4c-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="19e4c-110">قد يكون بُعد التسعير مجموعة خيارات أو كيان.</span><span class="sxs-lookup"><span data-stu-id="19e4c-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="19e4c-111">يجب إنشاء كلاهما في حل التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="19e4c-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="19e4c-112">توضح الخطوات الواردة في هذا الإجراء كيفية إنشاء أبعاد تستند إلى الكيان وأبعاد تستند إلى مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="19e4c-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="19e4c-113">الأبعاد المستندة إلى الكيان</span><span class="sxs-lookup"><span data-stu-id="19e4c-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="19e4c-114">في PSA، انقر فوق **الإعدادات** > **الحلول** ، ثم انقر نقرًا مزدوجًا فوق **\<your organization name> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-114">In PSA, click **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="19e4c-115">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="19e4c-116">انقر فوق **جديد** لإنشاء كيان جديد يسمي **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="19e4c-117">أدخل المعلومات المتبقية المطلوبة، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![تعريف كيان العنوان القياسي](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="19e4c-119">الأبعاد المستندة إلى مجموعة الخيارات</span><span class="sxs-lookup"><span data-stu-id="19e4c-119">Option set-based dimensions</span></span> 
<span data-ttu-id="19e4c-120">يمكنك إنشاء بعدين يستندان إلى مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="19e4c-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="19e4c-121">استخدام **موقع عمل المورد** لتعقب سعر الموقع **بالمنزل** والعمل **في الموقع** واستخدم **ساعات عمل المورد** مع القيم **العادية** و **الوقت الإضافي** لتطبيق رفع السعر عند اكتمال العمل.</span><span class="sxs-lookup"><span data-stu-id="19e4c-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="19e4c-122">في PSA، انقر فوق **الإعدادات** > **الحلول** ، ثم انقر نقرًا مزدوجًا فوق **\<your organization name> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-122">In PSA, click **Settings** > **Solutions** , and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="19e4c-123">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **مجموعات الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="19e4c-124">انقر فوق **جديد** لإنشاء مجموعة خيارات جديدة، وادخل المعلومات المطلوبة المتبقية، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="19e4c-125">بعد التسعير المعتمد على مجموعة الخيارات يسمى موقع عمل المورد</span><span class="sxs-lookup"><span data-stu-id="19e4c-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="19e4c-126">بعد التسعير المعتمد على مجموعة الخيارات يسمى ساعات عمل المورد</span><span class="sxs-lookup"><span data-stu-id="19e4c-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="19e4c-127">إنشاء بيانات للأبعاد المستندة إلى الكيانات</span><span class="sxs-lookup"><span data-stu-id="19e4c-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="19e4c-128">يمكنك إنشاء بيانات للأبعاد المستندة إلى الكيانات يدويًا، أو باستخدام الاستيراد أو استدعاءات الخدمة في Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="19e4c-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="19e4c-129">استخدم الخطوات الواردة في هذا الإجراء لإنشاء عنوانين قياسيين **مهندس أنظمة** و **مهندس أنظمة متمرس** من البعد المستند إلى كيان **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="19e4c-130">إذا كانت البيانات التي تريد إنشائها صغيرهة، كما هو موضح في المثال التالي، يمكنك استخدام نموذج قياسي.</span><span class="sxs-lookup"><span data-stu-id="19e4c-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="19e4c-131">في PSA، انقر فوق **بحث متقدم**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="19e4c-132">حدد كيان **العنوان القياسي** ثم انقر فوق **النتائج**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="19e4c-133">سيتم عرض كافة الصفوف الموجودة في كيان **العنوان القياسي**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="19e4c-134">انقر فوق **جديد**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-134">Click **New**.</span></span> <span data-ttu-id="19e4c-135">في حقل **الاسم** ، أدخل "مهندس الأنظمة" ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="19e4c-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="19e4c-136">أغلق النموذج.</span><span class="sxs-lookup"><span data-stu-id="19e4c-136">Close the form.</span></span> 
4. <span data-ttu-id="19e4c-137">كرر الخطوات 1-3 لإنشاء عنوان قياسي آخر لـ "مهندس الأنظمة المتمرس".</span><span class="sxs-lookup"><span data-stu-id="19e4c-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="19e4c-138">نموذج بيانات لكيان العنوان القياسي</span><span class="sxs-lookup"><span data-stu-id="19e4c-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)


