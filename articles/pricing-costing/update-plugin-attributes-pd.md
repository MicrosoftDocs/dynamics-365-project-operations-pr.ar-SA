---
title: تحديث سمات المكونات الإضافية لتشمل أبعاد التسعير الجديدة
description: يقدم هذا الموضوع معلومات حول كيفية تحديث سمات الوظيفة الإضافيه لأبعاد التسعير.
author: rumant
manager: Annbe
ms.date: 11/18/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7999c003a0cf670d586ebf4445901e106fbee39f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274667"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a><span data-ttu-id="811ec-103">تحديث سمات المكونات الإضافية لتشمل أبعاد التسعير الجديدة</span><span class="sxs-lookup"><span data-stu-id="811ec-103">Update plug-in attributes with new pricing dimensions</span></span>

<span data-ttu-id="811ec-104">يقدم هذا الموضوع معلومات حول كيفية تحديث سمات الوظيفة الإضافيه لأبعاد التسعير.</span><span class="sxs-lookup"><span data-stu-id="811ec-104">This topic provides information about how to update plug-in attributes for pricing dimensions.</span></span>

> [!NOTE]
> <span data-ttu-id="811ec-105">لا ينطبق موضوع هذا إلا على عرض الأسعار وميزات العقد الموجودة في Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="811ec-105">This topic is only applicable to the quote and contract features in Dynamics 365 Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="811ec-106">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="811ec-106">Prerequisites</span></span>
<span data-ttu-id="811ec-107">قبل إكمال الخطوات الواردة في هذه الموضوع ، يجب ان تكمل الإجراءات الموجودة في الموضوعات التالية:</span><span class="sxs-lookup"><span data-stu-id="811ec-107">Before you complete the steps in this topic, you must have completed the procedures in the following topics:</span></span>

  - [<span data-ttu-id="811ec-108">إنشاء حقول وكيانات مخصصة</span><span class="sxs-lookup"><span data-stu-id="811ec-108">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md) 
  - [<span data-ttu-id="811ec-109">إضافة حقول مخصصة إلى إعداد الأسعار وكيانات الحركات </span><span class="sxs-lookup"><span data-stu-id="811ec-109">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
  - <span data-ttu-id="811ec-110">[إعداد الحقول المخصصة كأبعاد تسعير](set-up-custom-fields-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="811ec-110">[Set up custom fields as pricing dimensions](set-up-custom-fields-pricing-dimensions.md).</span></span> 
  
<span data-ttu-id="811ec-111">إذا لم تكن قد أكملت هذه الإجراءات، فأكملها ثم عد إلى هذا الموضوع.</span><span class="sxs-lookup"><span data-stu-id="811ec-111">If you haven't completed those procedures, complete them and then return to this topic.</span></span>

## <a name="register-a-plug-in"></a><span data-ttu-id="811ec-112">تسجيل مكون إضافي</span><span class="sxs-lookup"><span data-stu-id="811ec-112">Register a plug-in</span></span>
<span data-ttu-id="811ec-113">عندما يتم إنشاء تفصيل بند عرض الأسعار في صفحة **بند عرض الأسعار** لبند عرض أسعار المشروع، يقوم النظام بإنشاء بندين للتقدير.</span><span class="sxs-lookup"><span data-stu-id="811ec-113">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines.</span></span> <span data-ttu-id="811ec-114">ويعتبر بند واحد هو الخاص بجانب التكلفة للتقدير ويكون البند الآخر خاصا بالنسبة لمبيعات الجانب.</span><span class="sxs-lookup"><span data-stu-id="811ec-114">One line is for the cost side of the estimate and the other line is for sales the side.</span></span> <span data-ttu-id="811ec-115">هذا هو نفس الشيء بالنسبة لبنود عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="811ec-115">This is the same  for project contract lines.</span></span>

<span data-ttu-id="811ec-116">عندما تقوم بإجراء تغيير على الكمية أو الحقل في جانب التكلفة، يتم أيضًا إجراء هذا التغيير لجانب المبيعات.</span><span class="sxs-lookup"><span data-stu-id="811ec-116">When you make a change to the quantity or a field on the cost side, that change is also made on the sales side.</span></span> <span data-ttu-id="811ec-117">هذا ممكن لأن المكونات الإضافية PreOperation في كيانات تفاصيل Quotelined وContractline تربط سمات معينة على جانب التكلفة بجانب المبيعات من الحركة.</span><span class="sxs-lookup"><span data-stu-id="811ec-117">This is possible because the PreOperation plug-ins on Quotelinedetail and contractline detail entities connect specific attributes on the cost side to the sales side of the transaction.</span></span> <span data-ttu-id="811ec-118">إذا كنت بحاجة إلى إجراء تغييرات على قيم أبعاد التسعير في جانب المبيعات ليتم إجراؤها أيضًا على جانب التكلفة ، فيجب إعادة تسجيل المكونات الإضافية التالية بعد إجراء تغييرات على بُعد التسعير.</span><span class="sxs-lookup"><span data-stu-id="811ec-118">If you need changes made to the pricing dimension values on the sales side to also be made on the cost side, the following plug-ins must be re-registered after making changes to a pricing dimension.</span></span>

<span data-ttu-id="811ec-119">هذه هي المكونات الاضافيه لتحديثها وأعاده تسجيلها:</span><span class="sxs-lookup"><span data-stu-id="811ec-119">These are the plug-ins to update and re-register:</span></span>

- <span data-ttu-id="811ec-120">PreOperationContractLineDetailUpdate - **تحديث msdyn_orderlinetransaction**</span><span class="sxs-lookup"><span data-stu-id="811ec-120">PreOperationContractLineDetailUpdate - **Update msdyn_orderlinetransaction**</span></span>
- <span data-ttu-id="811ec-121">PreOperationQuoteLineDetailUpdate - **تحديثات msdyn_quotelinetransaction**</span><span class="sxs-lookup"><span data-stu-id="811ec-121">PreOperationQuoteLineDetailUpdate - **Updates msdyn_quotelinetransaction**</span></span>

<span data-ttu-id="811ec-122">أكمل الخطوات التالية لتحديث المكونات الاضافيه وأعاده تسجيلها.</span><span class="sxs-lookup"><span data-stu-id="811ec-122">Complete the following steps to update and re-register the plug-ins.</span></span>

1. <span data-ttu-id="811ec-123">افتح **PluginRegistrationTool** وقم بالاتصال ببيئة Dataverse لـ Project Operations لديك.</span><span class="sxs-lookup"><span data-stu-id="811ec-123">Open **PluginRegistrationTool** and connect to your Project Operations Dataverse environment.</span></span>
2. <span data-ttu-id="811ec-124">حدد **بحث**، واكتب الأحرف الاولي من المكون الإضافي الذي سيتم تحديثه.</span><span class="sxs-lookup"><span data-stu-id="811ec-124">Select **Search**, and type in the first few letters of the plug-in to be updated.</span></span>
3. <span data-ttu-id="811ec-125">بعد العثور على المكون الإضافي، حدده ثم حدد **تحديد في النموذج الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="811ec-125">After the plug-in is found, select it, and then select **Select on Main Form**.</span></span>
4. <span data-ttu-id="811ec-126">حدد خطوة **Update msdyn_orderlinetransaction**، وانقر بزر الماوس الأيمن، ثم حدد **تحديث**.</span><span class="sxs-lookup"><span data-stu-id="811ec-126">Select the **Update msdyn_orderlinetransaction** step, right-click, and then select **Update**.</span></span>
5. <span data-ttu-id="811ec-127">في صفحة مربع الحوار **تحديث**، حدد علامة القطع (**...**) في سمات التصفية.</span><span class="sxs-lookup"><span data-stu-id="811ec-127">In the **Update** dialog page, select the ellipsis (**...**) in the filtering attributes.</span></span>
6. <span data-ttu-id="811ec-128">يتم فتح النافذة سمات التصفية ويوفر قائمه بكافة السمات الموجودة في الكيان وابعاد التسعير.</span><span class="sxs-lookup"><span data-stu-id="811ec-128">The filtering attributes window opens and provides a list of all attributes in the entity and the pricing dimensions.</span></span> <span data-ttu-id="811ec-129">حدد خانات الاختيار الخاصة بسمات ابعاد التسعير.</span><span class="sxs-lookup"><span data-stu-id="811ec-129">Select the check boxes for the pricing dimension attributes.</span></span>
7. <span data-ttu-id="811ec-130">حدد **موافق** لإغلاق الصفحة، ثم حدد **تحديث الخطوة**.</span><span class="sxs-lookup"><span data-stu-id="811ec-130">Select **OK** to close the page, and then select **Update Step**.</span></span>
8. <span data-ttu-id="811ec-131">كرر الخطوات من 2 إلى 7 للمكون الإضافي الثاني، **PreOperationQuoteLineDetail**.</span><span class="sxs-lookup"><span data-stu-id="811ec-131">Repeat steps 2-7 for the second plug-in, **PreOperationQuoteLineDetail**.</span></span> <span data-ttu-id="811ec-132">بالنسبة لهذا المكون الإضافي، يلزمك تحديث خطوة **تحديث msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="811ec-132">For this plug-in, you need to update the **Update of msdyn_quotelinetransaction** step.</span></span>
9. <span data-ttu-id="811ec-133">أغلق **PluginRegistrationTool**.</span><span class="sxs-lookup"><span data-stu-id="811ec-133">Close **PluginRegistrationTool**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]