---
title: إنشاء حل لأبعاد التسعير المخصصة
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء حلول لأبعاد التسعير المخصصة.
author: Rumant
manager: tfehr
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3e3f688b0147974ef252a0ee00be20c4669d7165
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278402"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="552ee-103">إنشاء حل لأبعاد التسعير المخصصة</span><span class="sxs-lookup"><span data-stu-id="552ee-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="552ee-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="552ee-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="552ee-105">يجب أن تكون كافة تغييرات أبعاد التسعير المخصصة في حل منفصل.</span><span class="sxs-lookup"><span data-stu-id="552ee-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="552ee-106">تتيح أفضل الممارسات المهمة هذه المرونة في تحديث التغييرات أو إزالتها حسب الحاجة، وتساعد في إعادة استخدام عملك، وتسهل نقل التغييرات إلى حالات أخرى.</span><span class="sxs-lookup"><span data-stu-id="552ee-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="552ee-107">بعد إجراء التغييرات المطلوبة، قم بتصدير هذا الحل كحل **مُدار**، ثم قم باستيراده إلى مثيلات أخرى لإعادة استخدامها.</span><span class="sxs-lookup"><span data-stu-id="552ee-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="552ee-108">إنشاء حل لأبعاد التسعير المخصصة</span><span class="sxs-lookup"><span data-stu-id="552ee-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="552ee-109">حدد **الإعدادات** > **الحلول**، ثم حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="552ee-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="552ee-110">قم بتسمية الحل، *أبعاد أسعار <your organization name>*.</span><span class="sxs-lookup"><span data-stu-id="552ee-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="552ee-111">أدخل المعلومات المتبقية المطلوبة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="552ee-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![إنشاء حل أبعاد التسعير المخصص](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="552ee-113">إضافة جميع الكيانات المطلوبة والمكونات ذات الصلة إلى حل أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="552ee-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="552ee-114">قم باضافه كيانات Project Service التالية إلى حل التسعير الخاص بك لاجراء تغييرات علي المخطط في حل التسعير.</span><span class="sxs-lookup"><span data-stu-id="552ee-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="552ee-115">بعد الانتهاء من هذا الاجراء، ستتعرف الكيانات علي ابعاد التسعير الجديدة.</span><span class="sxs-lookup"><span data-stu-id="552ee-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="552ee-116">حدد **الإعدادات** > **الحلول**، ثم انقر نقرًا مزدوجًا فوق **<*اسم مؤسستك*> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="552ee-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="552ee-117">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **إضافة الموجود** > **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="552ee-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="552ee-118">في مربع حوار **مكونات الحل**، حدد الكيانات التالية:</span><span class="sxs-lookup"><span data-stu-id="552ee-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="552ee-119">**فعلي**</span><span class="sxs-lookup"><span data-stu-id="552ee-119">**Actual**</span></span>
   - <span data-ttu-id="552ee-120">**المورد القابل للحجز**</span><span class="sxs-lookup"><span data-stu-id="552ee-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="552ee-121">**سطر التقدير**</span><span class="sxs-lookup"><span data-stu-id="552ee-121">**Estimate Line**</span></span>
   - <span data-ttu-id="552ee-122">**مهمة المشروع**</span><span class="sxs-lookup"><span data-stu-id="552ee-122">**Project Task**</span></span>
   - <span data-ttu-id="552ee-123">**تفاصيل بند الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="552ee-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="552ee-124">**سطر دفتر اليومية**</span><span class="sxs-lookup"><span data-stu-id="552ee-124">**Journal Line**</span></span>
   - <span data-ttu-id="552ee-125">**تفاصيل بنود عقد المشروع**</span><span class="sxs-lookup"><span data-stu-id="552ee-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="552ee-126">**عضو فريق المشروع**</span><span class="sxs-lookup"><span data-stu-id="552ee-126">**Project Team Member**</span></span>
   - <span data-ttu-id="552ee-127">**تفاصيل بند عرض الأسعار‬**</span><span class="sxs-lookup"><span data-stu-id="552ee-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="552ee-128">**رفع سعر الدور**</span><span class="sxs-lookup"><span data-stu-id="552ee-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="552ee-129">**سعر الدور**</span><span class="sxs-lookup"><span data-stu-id="552ee-129">**Role Price**</span></span>
   - <span data-ttu-id="552ee-130">**إدخال الوقت**</span><span class="sxs-lookup"><span data-stu-id="552ee-130">**Time Entry**</span></span>
 
   ![أضف حل بُعد التسعير المخصص للكيانات الحالية](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="552ee-132">بالنسبة لكل كيان، قم بمراجعه المكونات التي تتم اضافتها والقائمة النهائية لأصول الكيانات لكل كيان.</span><span class="sxs-lookup"><span data-stu-id="552ee-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="552ee-133">قم بتضمين كافة النماذج وطرق العرض لكل من الكيانات المحددة.</span><span class="sxs-lookup"><span data-stu-id="552ee-133">Include all forms and views for each of the selected entities.</span></span>

  ![تمت إضافة الكيانات](./media/solution-component-selection.png)


5.  <span data-ttu-id="552ee-135">عند المطالبة بتضمين أي كيانات تابعه للكيانات المحددة، حدد **لا، لا تقم بتضمين المكونات المطلوبة.**</span><span class="sxs-lookup"><span data-stu-id="552ee-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![تضمين الكيانات التابعة](./media/Do-not-include-required.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]