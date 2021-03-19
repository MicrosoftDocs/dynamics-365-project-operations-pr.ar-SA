---
title: إنشاء حلول مخصصة لأبعاد التسعير
description: يشرح هذا الموضوع كيفية إنشاء حل مخصص عند إنشاء أبعاد تسعير مخصصة.
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
ms.openlocfilehash: 1d8117d6f6bcedc97264401fc941470f34efb1ae
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284972"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="a5724-103">إنشاء حلول مخصصة لأبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="a5724-103">Create custom solutions for pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> <span data-ttu-id="a5724-104">يجب أن تكون كافة تغييرات أبعاد التسعير المخصصة في حل منفصل.</span><span class="sxs-lookup"><span data-stu-id="a5724-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="a5724-105">يوفر هذه الممارسة الجيدة المهمة المرونة في المستقبل لتحديث التغييرات أو إزالتها حسب الحاجة، والتي تساعد في إعادة استخدام عملك، وتسهل نقل هذه التغييرات إلى مثيل آخر.</span><span class="sxs-lookup"><span data-stu-id="a5724-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="a5724-106">بعد إجراء كافة التغييرات المطلوبة، يمكنك تصدير هذا الحل **كحل مُدار** واستيراده إلى مثيلات أخرى لإعادة استخدام إعداد تسعيرك.</span><span class="sxs-lookup"><span data-stu-id="a5724-106">After you make the required changes, export this solution as a **Managed solution**, and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="a5724-107">حدد **الإعدادات** > **الحلول**، ثم حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a5724-107">Select **Settings** > **Solutions**, and then select **New**.</span></span> 
2. <span data-ttu-id="a5724-108">قم بتسميه الحل، **\<your organization name> أبعاد التسعير**، وأدخل المعلومات المطلوبة المتبقية، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a5724-108">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>

> ![إنشاء حل مخصص لأبعاد التسعير](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="a5724-110">إضافة جميع الكيانات المطلوبة والمكونات ذات الصلة إلى حل أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="a5724-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="a5724-111">ستحتاج إلى إضافة كيانات Project Service التالية إلى حل التسعير الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="a5724-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="a5724-112">أكمل الخطوات الواردة في هذا الإجراء لإجراء بعض التغييرات الهامة في المخطط في حل التسعير لكي تصبح الكيانات على علم بأبعاد التسعير الجديدة.</span><span class="sxs-lookup"><span data-stu-id="a5724-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="a5724-113">حدد **الإعدادات** > **حلول**، وانقر نقرًا مزدوجًا فوق **\<your organization name> أبعاد التسعير**.</span><span class="sxs-lookup"><span data-stu-id="a5724-113">Select **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="a5724-114">في مستكشف الحلول، في جزء التنقل الأيسر، حدد **إضافة الموجود** > **الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="a5724-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="a5724-115">في مربع حوار **مكونات الحل**، حدد الكيانات التالية:</span><span class="sxs-lookup"><span data-stu-id="a5724-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="a5724-116">فعلي</span><span class="sxs-lookup"><span data-stu-id="a5724-116">Actual</span></span>
- <span data-ttu-id="a5724-117">المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="a5724-117">Bookable Resource</span></span>
- <span data-ttu-id="a5724-118">سطر التقدير</span><span class="sxs-lookup"><span data-stu-id="a5724-118">Estimate Line</span></span>
- <span data-ttu-id="a5724-119">مهمة المشروع</span><span class="sxs-lookup"><span data-stu-id="a5724-119">Project Task</span></span>
- <span data-ttu-id="a5724-120">تفاصيل بند الفاتورة</span><span class="sxs-lookup"><span data-stu-id="a5724-120">Invoice Line Detail</span></span>
- <span data-ttu-id="a5724-121">سطر دفتر اليومية</span><span class="sxs-lookup"><span data-stu-id="a5724-121">Journal Line</span></span>
- <span data-ttu-id="a5724-122">تفاصيل بنود عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="a5724-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="a5724-123">عضو فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="a5724-123">Project Team Member</span></span>
- <span data-ttu-id="a5724-124">تفاصيل بند عرض الأسعار‬</span><span class="sxs-lookup"><span data-stu-id="a5724-124">Quote Line Detail</span></span>
- <span data-ttu-id="a5724-125">رفع سعر الدور</span><span class="sxs-lookup"><span data-stu-id="a5724-125">Role Price Markup</span></span>
- <span data-ttu-id="a5724-126">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="a5724-126">Role Price</span></span> 
- <span data-ttu-id="a5724-127">إدخال الوقت</span><span class="sxs-lookup"><span data-stu-id="a5724-127">Time Entry</span></span> 

> ![إضافة الكيانات الموجودة إلى حل أبعاد التسعير](media/Existing-entities-to-PD-solution.png)

> ![حدد مكونات الحل](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="a5724-130">تأكد من تضمين كافة النماذج وطرق العرض لكل من الكيانات المحددة.</span><span class="sxs-lookup"><span data-stu-id="a5724-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="a5724-131">عند مطالبتك بتضمين أية كيانات تابعة للكيانات المحددة، حدد **لا**.</span><span class="sxs-lookup"><span data-stu-id="a5724-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![لا تقم بتضمين كافة المكونات ذات الصلة.](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]