---
title: تحديث سمات المكونات الإضافية لتشمل أبعاد التسعير الجديدة
description: يقدم هذا الموضوع معلومات حول تحديث سمات الوظيفة الإضافيه لأبعاد التسعير.
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: project-operations
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: c42e5fda79d51430f4dedf46037e11c86a38c474
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121832"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a><span data-ttu-id="c77fc-103">تحديث سمات المكونات الإضافية لتشمل أبعاد التسعير الجديدة</span><span class="sxs-lookup"><span data-stu-id="c77fc-103">Update plug-in attributes to include new pricing dimensions</span></span>

> [!NOTE]
> <span data-ttu-id="c77fc-104">إذا لم تكن تستخدم ميزات التعاقد وعروض الأسعار في Project Service Automation (PSA)، يمكنك تخطي هذه الموضوع.</span><span class="sxs-lookup"><span data-stu-id="c77fc-104">If you are not using the Project Service Automation (PSA) Quoting and Contracting features, you can skip this topic.</span></span>

<span data-ttu-id="c77fc-105">يفترض هذا الموضوع أنك أكملت الإجراءات الموجودة في المواضيع، و[إنشاء الحقول والكيانات المخصصة](create-custom-fields-entities.md)، و[إضافة حقول مخصصة إلى إعداد الأسعار وكيانات المعاملات](field-references.md)، و[إعداد الحقول المخصصة كأبعاد تسعير](set-up-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="c77fc-105">This topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md), [Add custom fields to price setup and transactional entities](field-references.md), and [Set up custom fields as pricing dimensions](set-up-pricing-dimensions.md).</span></span> <span data-ttu-id="c77fc-106">إذا لم تقم بإكمال هذه الإجراءات، فقم بالرجوع إلى الحالة السابقة وإكمالها ثم عد إلى هذا الموضوع.</span><span class="sxs-lookup"><span data-stu-id="c77fc-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span>

<span data-ttu-id="c77fc-107">عند إنشاء تفصيل بند عرض الأسعار في صفحة **بند عرض الأسعار** لبند عرض أسعار المشروع، يقوم النظام بإنشاء بندين للتقدير في الخلفية -- بند لجانب التكلفة للتقدير والآخر لجانب المبيعات.</span><span class="sxs-lookup"><span data-stu-id="c77fc-107">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines in the background -- one line for the cost side of the estimate and one for sales side.</span></span> <span data-ttu-id="c77fc-108">هذا هو نفس الشيء بالنسبة لبنود عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="c77fc-108">This is the same  for project contract lines.</span></span>

<span data-ttu-id="c77fc-109">عندما تقوم بإجراء تغيير على الكمية أو الحقل في جانب التكلفة، يتم نشر هذا التغيير لجانب المبيعات.</span><span class="sxs-lookup"><span data-stu-id="c77fc-109">When you make a change to the quantity or a field on the cost side, that change is propagated to the sales side.</span></span> <span data-ttu-id="c77fc-110">ويعد ذلك ممكنًا بسبب المكونات الاضافيه التالية التي يجب إعاده تسجيلها بعد التغيير إلى أبعاد التسعير.</span><span class="sxs-lookup"><span data-stu-id="c77fc-110">This is possible because of the following plug-ins that must be re-registered after a change to pricing dimensions.</span></span>

- <span data-ttu-id="c77fc-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="c77fc-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span></span>
- <span data-ttu-id="c77fc-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="c77fc-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span></span>

<span data-ttu-id="c77fc-113">توضح الخطوات التالية عملية تسجيل المكونات الاضافيه.</span><span class="sxs-lookup"><span data-stu-id="c77fc-113">The following steps walk you through the process of registering the plug-ins.</span></span>

1. <span data-ttu-id="c77fc-114">افتح **PluginRegistrationTool** وقم بالاتصال بالمثيل الخاص بك على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="c77fc-114">Open the **PluginRegistrationTool** and connect to your online instance.</span></span>
2. <span data-ttu-id="c77fc-115">انقر فوق **بحث**، وابحث عن المكون الإضافي المراد تحديثه.</span><span class="sxs-lookup"><span data-stu-id="c77fc-115">Click **Search** and search for the plug-in to be updated.</span></span>

 ![لقطة شاشة لشجرة البحث](media/PRT-1.png)

3. <span data-ttu-id="c77fc-117">بعد العثور على المكون الإضافي، حدده ثم انقر فوق **تحديد في النموذج الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="c77fc-117">After the plug-in is found, select it and then click **Select on Main Form**.</span></span>

4. <span data-ttu-id="c77fc-118">حدد خطوة المكون الإضافي المراد تحديثها، وانقر بزر الماوس الأيمن، ثم حدد **تحديث**.</span><span class="sxs-lookup"><span data-stu-id="c77fc-118">Select the step of the plug-in to be updated, right-click, and then select **Update**.</span></span>

 ![لقطة شاشة للمكون الإضافي المراد تحديثه](media/PRT-2.png)
 
5. <span data-ttu-id="c77fc-120">في نافذة التحديث، انقر فوق علامة القطع (**...**) في سمات التصفية.</span><span class="sxs-lookup"><span data-stu-id="c77fc-120">In the update window, click the ellipsis (**...**) in the filtering attributes.</span></span>

 ![لقطة شاشة لمعلومات تكوين الخطوة الحالية للتحديث](media/PRT-3.png)
 
6. <span data-ttu-id="c77fc-122">حدد خانات اختيار سمات التسعير.</span><span class="sxs-lookup"><span data-stu-id="c77fc-122">Select the pricing attribute check boxes.</span></span>

 ![لقطة شاشة تظهر تحديد خانة الاختيار لسمات التسعير](media/PRT-4.png)

7. <span data-ttu-id="c77fc-124">انقر فوق **موافق** لإغلاق الصفحة، ثم حدد **تحديث الخطوة**.</span><span class="sxs-lookup"><span data-stu-id="c77fc-124">Click **OK** to close the page and then select **Update Step**.</span></span>

 ![لقطة شاشة تظهر زر "تحديث الخطوة"](media/PRT-5.png)
 
8. <span data-ttu-id="c77fc-126">كرر هذه العملية للمكون الإضافي الثاني، **PreOperationQuoteLineDetail - تحديث msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="c77fc-126">Repeat this process for the second plug-in, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span></span>

9. <span data-ttu-id="c77fc-127">أغلق أداة تسجيل المكون الإضافي.</span><span class="sxs-lookup"><span data-stu-id="c77fc-127">Close the plug-in registration tool.</span></span>

