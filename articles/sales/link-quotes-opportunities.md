---
title: إنشاء عروض أسعار المشروع من الفرص
description: يقدم هذا الموضوع معلومات حول إنشاء عرض أسعار المشروع من فرصة.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 606098473db479d0015e3a7a3c01a3d3b6de9db1
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070556"
---
# <a name="create-project-quotes-from-opportunities"></a><span data-ttu-id="34dc8-103">إنشاء عروض أسعار المشروع من الفرص</span><span class="sxs-lookup"><span data-stu-id="34dc8-103">Create project quotes from opportunities</span></span>

<span data-ttu-id="34dc8-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="34dc8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="34dc8-105">يمكن إنشاء عروض الأسعار من فرص المشروع بالطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="34dc8-105">Quotes can be created from project opportunities in the following ways:</span></span>

- <span data-ttu-id="34dc8-106">من علامة التبويب **عروض الأسعار** في صفحة **فرصة المشروع**</span><span class="sxs-lookup"><span data-stu-id="34dc8-106">From the **Quotes** tab on the **Project Opportunity** page</span></span>
- <span data-ttu-id="34dc8-107">من سير مهام عملية مبيعات الفرصة</span><span class="sxs-lookup"><span data-stu-id="34dc8-107">From the Opportunity sales process flow</span></span>
- <span data-ttu-id="34dc8-108">من خلال تحديث مرجع الفرصة على عرض أسعار موجود</span><span class="sxs-lookup"><span data-stu-id="34dc8-108">By updating the opportunity reference on an existing quote</span></span>

## <a name="from-the-quotes-tab-of-the-project-opportunity-page"></a><span data-ttu-id="34dc8-109">من علامة التبويب عروض الأسعار في صفحة فرصة المشروع</span><span class="sxs-lookup"><span data-stu-id="34dc8-109">From the Quotes tab of the Project Opportunity page</span></span>

<span data-ttu-id="34dc8-110">لإنشاء عرض أسعار مشروع من فرصة، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="34dc8-110">To create a project quote from an opportunity, complete the following steps.</span></span>

1. <span data-ttu-id="34dc8-111">افتح صفحة **فرصة المشروع** ، وحدد علامة التبويب **عروض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="34dc8-111">Open the **Project Opportunity** page and select the **Quotes** tab.</span></span> 
2. <span data-ttu-id="34dc8-112">على الشبكة الفرعية **عروض الأسعار** ، حدد **+** لإنشاء عرض أسعار مشروع جديد استنادًا إلى الفرصة.</span><span class="sxs-lookup"><span data-stu-id="34dc8-112">On the **Quotes** sub-grid, select the **+** to create a new project quote based on the opportunity.</span></span> <span data-ttu-id="34dc8-113">يتم نسخ جميع بنود الفرصة وقوائم أسعار المشروع ذات الصلة إلى عرض الأسعار الجديد من الفرصة.</span><span class="sxs-lookup"><span data-stu-id="34dc8-113">All of the opportunity lines and related Project price lists are copied to the new quote from the opportunity.</span></span>

## <a name="from-the-opportunity-sales-process-flow"></a><span data-ttu-id="34dc8-114">من سير مهام عملية مبيعات الفرصة</span><span class="sxs-lookup"><span data-stu-id="34dc8-114">From the Opportunity sales process flow</span></span>

<span data-ttu-id="34dc8-115">لإنشاء عرض أسعار مشروع من سير مهام عملية مبيعات الفرصة‬، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="34dc8-115">To create a quote from the Opportunity sales process flow, complete the following steps.</span></span>

1. <span data-ttu-id="34dc8-116">من سير مهام عملية مبيعات الفرصة‬، افتح الفرصة.</span><span class="sxs-lookup"><span data-stu-id="34dc8-116">From the Opportunity sales process flow, open the Opportunity.</span></span>
2. <span data-ttu-id="34dc8-117">حدد مرحلة **التأهيل**.</span><span class="sxs-lookup"><span data-stu-id="34dc8-117">Select the **Qualify** stage.</span></span> 
3. <span data-ttu-id="34dc8-118">حدد **التالي** ، ثم حدد **+ إنشاء** لإنشاء عرض أسعار جديد.</span><span class="sxs-lookup"><span data-stu-id="34dc8-118">Select **Next** and then select **+ Create** to create a new quote.</span></span> <span data-ttu-id="34dc8-119">ستكون معظم المعلومات الموجودة في علامة التبويب **الملخص** لعرض الأسعار الجديد هذا معلومات افتراضية من الفرصة.</span><span class="sxs-lookup"><span data-stu-id="34dc8-119">Most of the information on the **Summary** tab for this new quote will have defaulted from the opportunity.</span></span> 
4. <span data-ttu-id="34dc8-120">أدخل أي معلومات مطلوبة مفقودة، أو قم بتحديث القيم الافتراضية حسب الضرورة في علامة التبويب **الملخص**.</span><span class="sxs-lookup"><span data-stu-id="34dc8-120">Enter in any required information that is missing, or update defaulted values as necessary on the **Summary** tab,</span></span>
5. <span data-ttu-id="34dc8-121">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="34dc8-121">Select **Save**.</span></span> <span data-ttu-id="34dc8-122">يتم إنشاء عرض الأسعار الجديد ويتم ربطه بالفرصة.</span><span class="sxs-lookup"><span data-stu-id="34dc8-122">The new quote is created and associated to the opportunity.</span></span> <span data-ttu-id="34dc8-123">يمكنك الآن عرض معلومات عرض الأسعار على علامة التبويب **عروض الأسعار** في صفحة **الفرصة**.</span><span class="sxs-lookup"><span data-stu-id="34dc8-123">You can now view the quote information on the **Quotes** tab of the **Opportunity** page.</span></span> 

   <span data-ttu-id="34dc8-124">تنتقل عملية مبيعات الفرصة إلى المرحلة التالية، **اقتراح**.</span><span class="sxs-lookup"><span data-stu-id="34dc8-124">The Opportunity sales process moves to the next stage, **Propose**.</span></span>


## <a name="by-updating-the-opportunity-reference-on-an-existing-quote"></a><span data-ttu-id="34dc8-125">من خلال تحديث مرجع الفرصة على عرض أسعار موجود</span><span class="sxs-lookup"><span data-stu-id="34dc8-125">By updating the opportunity reference on an existing quote</span></span>

<span data-ttu-id="34dc8-126">يمكن ربط عرض أسعار موجود بفرصة.</span><span class="sxs-lookup"><span data-stu-id="34dc8-126">An existing quote can be linked to an Opportunity.</span></span> <span data-ttu-id="34dc8-127">أكمل الخطوات التالية لتحديث معلومات الفرصة في عرض أسعار موجود.</span><span class="sxs-lookup"><span data-stu-id="34dc8-127">Complete the following steps to update the Opportunity information on an existing quote.</span></span>

1. <span data-ttu-id="34dc8-128">افتح صفحة **عرض الأسعار** ، وحدد علامة التبويب **الملخص**.</span><span class="sxs-lookup"><span data-stu-id="34dc8-128">Open the **Quote** page and select the **Summary** tab.</span></span>
2. <span data-ttu-id="34dc8-129">في حقل **الفرصة** ، حدد الفرصة التي ترغب في ربطها بعرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="34dc8-129">In the **Opportunity** field, select the opportunity that you want to link to the quote.</span></span> <span data-ttu-id="34dc8-130">يمكنك رؤية عرض الأسعار في شبكة **عروض الأسعار** الخاصة بالفرصة.</span><span class="sxs-lookup"><span data-stu-id="34dc8-130">You can see the quote in the **Quotes** grid of the Opportunity.</span></span> 
3. <span data-ttu-id="34dc8-131">باستخدام عملية مبيعات الفرصة، يمكن نقل الفرصة إلى المرحلة التالية، **اقتراح**.</span><span class="sxs-lookup"><span data-stu-id="34dc8-131">Using the Opportunity sales process, the opportunity can be moved to the next stage, **Propose**.</span></span> 

   <span data-ttu-id="34dc8-132">عند نقل الفرصة إلى هذه المرحلة، يمكنك تحديد عرض الأسعار هذا من قائمة عروض الأسعار المقترنة بهذه الفرصة.</span><span class="sxs-lookup"><span data-stu-id="34dc8-132">When you move an opportunity to this stage, you can select this quote from a list of quotes associated with this opportunity.</span></span> <span data-ttu-id="34dc8-133">يشير تحديد عرض الأسعار هذا إلى أنك تنتقل إلى المرحلة التالية معه.</span><span class="sxs-lookup"><span data-stu-id="34dc8-133">Selecting this quote indicates that you're moving forward with it.</span></span>

   <span data-ttu-id="34dc8-134">ستظل كافة عروض الأسعار الأخرى المقترنة بالفرصة متوفرة ونشطة إلى أن يتم الفوز بإحداها.</span><span class="sxs-lookup"><span data-stu-id="34dc8-134">All the other quotes associated with the Opportunity will still be available and active until one of them is won.</span></span> <span data-ttu-id="34dc8-135">يمكنك نقل عملية المبيعات مره أخرى إلى المرحلة السابقة **تأهيل** ، واختيار عرض أسعار آخر للانتقال معه إلى المرحلة التالية.</span><span class="sxs-lookup"><span data-stu-id="34dc8-135">You can move the sales process back to the previous stage **Qualify** , and pick another quote to move forward with.</span></span>
