---
title: إنشاء حل لأبعاد التسعير المخصصة
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء حلول لأبعاد التسعير المخصصة.
author: Rumant
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 86f4cd2c26ebfca621d1b226b571d220d3b2441e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010320"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="644c5-103">إنشاء حل لأبعاد التسعير المخصصة</span><span class="sxs-lookup"><span data-stu-id="644c5-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="644c5-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="644c5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="644c5-105">يجب أن تكون كافة تغييرات أبعاد التسعير المخصصة في حل منفصل.</span><span class="sxs-lookup"><span data-stu-id="644c5-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="644c5-106">تتيح أفضل الممارسات المهمة هذه المرونة في تحديث التغييرات أو إزالتها حسب الحاجة، وتساعد في إعادة استخدام عملك، وتسهل نقل التغييرات إلى حالات أخرى.</span><span class="sxs-lookup"><span data-stu-id="644c5-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="644c5-107">بعد إجراء التغييرات المطلوبة، قم بتصدير هذا الحل كحل **مُدار**، ثم قم باستيراده إلى مثيلات أخرى لإعادة استخدامها.</span><span class="sxs-lookup"><span data-stu-id="644c5-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="644c5-108">إنشاء حل لأبعاد التسعير المخصصة</span><span class="sxs-lookup"><span data-stu-id="644c5-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="644c5-109">حدد **الإعدادات** > **الحلول**، ثم حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="644c5-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="644c5-110">قم بتسمية الحل، *أبعاد أسعار <your organization name>*.</span><span class="sxs-lookup"><span data-stu-id="644c5-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="644c5-111">أدخل المعلومات المتبقية المطلوبة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="644c5-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![إنشاء حل أبعاد التسعير المخصص](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="644c5-113">إضافة جميع الكيانات المطلوبة والمكونات ذات الصلة إلى حل أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="644c5-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="644c5-114">قم باضافه كيانات Project Service التالية إلى حل التسعير الخاص بك لاجراء تغييرات علي المخطط في حل التسعير.</span><span class="sxs-lookup"><span data-stu-id="644c5-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="644c5-115">بعد الانتهاء من هذا الاجراء، ستتعرف الكيانات علي ابعاد التسعير الجديدة.</span><span class="sxs-lookup"><span data-stu-id="644c5-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="644c5-116">حدد **الإعدادات** > **الحلول**، ثم انقر نقرًا مزدوجًا فوق **<*اسم مؤسستك*> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="644c5-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="644c5-117">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **إضافة الموجود** > **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="644c5-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="644c5-118">في مربع حوار **مكونات الحل**، حدد الكيانات التالية:</span><span class="sxs-lookup"><span data-stu-id="644c5-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="644c5-119">**فعلي**</span><span class="sxs-lookup"><span data-stu-id="644c5-119">**Actual**</span></span>
   - <span data-ttu-id="644c5-120">**المورد القابل للحجز**</span><span class="sxs-lookup"><span data-stu-id="644c5-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="644c5-121">**سطر التقدير**</span><span class="sxs-lookup"><span data-stu-id="644c5-121">**Estimate Line**</span></span>
   - <span data-ttu-id="644c5-122">**مهمة المشروع**</span><span class="sxs-lookup"><span data-stu-id="644c5-122">**Project Task**</span></span>
   - <span data-ttu-id="644c5-123">**تفاصيل بند الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="644c5-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="644c5-124">**سطر دفتر اليومية**</span><span class="sxs-lookup"><span data-stu-id="644c5-124">**Journal Line**</span></span>
   - <span data-ttu-id="644c5-125">**تفاصيل بنود عقد المشروع**</span><span class="sxs-lookup"><span data-stu-id="644c5-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="644c5-126">**عضو فريق المشروع**</span><span class="sxs-lookup"><span data-stu-id="644c5-126">**Project Team Member**</span></span>
   - <span data-ttu-id="644c5-127">**تفاصيل بند عرض الأسعار‬**</span><span class="sxs-lookup"><span data-stu-id="644c5-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="644c5-128">**رفع سعر الدور**</span><span class="sxs-lookup"><span data-stu-id="644c5-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="644c5-129">**سعر الدور**</span><span class="sxs-lookup"><span data-stu-id="644c5-129">**Role Price**</span></span>
   - <span data-ttu-id="644c5-130">**إدخال الوقت**</span><span class="sxs-lookup"><span data-stu-id="644c5-130">**Time Entry**</span></span>
 
   ![أضف حل بُعد التسعير المخصص للكيانات الحالية](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="644c5-132">بالنسبة لكل كيان، قم بمراجعه المكونات التي تتم اضافتها والقائمة النهائية لأصول الكيانات لكل كيان.</span><span class="sxs-lookup"><span data-stu-id="644c5-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="644c5-133">قم بتضمين كافة النماذج وطرق العرض لكل من الكيانات المحددة.</span><span class="sxs-lookup"><span data-stu-id="644c5-133">Include all forms and views for each of the selected entities.</span></span>

  ![تمت إضافة الكيانات](./media/solution-component-selection.png)


5.  <span data-ttu-id="644c5-135">عند المطالبة بتضمين أي كيانات تابعه للكيانات المحددة، حدد **لا، لا تقم بتضمين المكونات المطلوبة.**</span><span class="sxs-lookup"><span data-stu-id="644c5-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![تضمين الكيانات التابعة](./media/Do-not-include-required.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]