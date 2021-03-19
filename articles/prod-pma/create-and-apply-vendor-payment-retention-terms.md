---
title: إنشاء شروط احتجاز دفع المورّد وتطبيقها
description: يقدم هذا الموضوع معلومات حول كيفية إعداد شروط احتجاز دفع المورّد والاحتفاظ بها.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: e6f6424b983f76a96825d76e1b4b81b54dc84b84
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270929"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a><span data-ttu-id="27aa9-103">إنشاء شروط احتجاز دفع المورّد وتطبيقها</span><span class="sxs-lookup"><span data-stu-id="27aa9-103">Create and apply vendor payment retention terms</span></span>

[!include [banner](../includes/banner.md)] 

<span data-ttu-id="27aa9-104">يعتبر إعداد شروط احتجاز دفع المورّد لمشروع ما مفيدًا عندما تريد المؤسسة الاحتفاظ بجزء من الدفعات التي يتم تسديدها للمورّد.</span><span class="sxs-lookup"><span data-stu-id="27aa9-104">Setting up vendor payment retention terms for a project is useful when your organization wants to retain part of the payments made to a vendor.</span></span> <span data-ttu-id="27aa9-105">على سبيل المثال، عندما تريد احتجاز دفعة للمورّد حتى تلبي المنتجات التي يتم تسليمها توقعاتك.</span><span class="sxs-lookup"><span data-stu-id="27aa9-105">For example, when you want to hold payment to a vendor until the products delivered meet your expectations.</span></span> <span data-ttu-id="27aa9-106">يمكن تحديد شروط احتجاز دفع المورّد عندما تفاوض بشأن عقد المورّد.</span><span class="sxs-lookup"><span data-stu-id="27aa9-106">Vendor payment retention terms can be specified when you negotiate a vendor contract.</span></span>

## <a name="create-vendor-payment-retention-terms"></a><span data-ttu-id="27aa9-107">إنشاء شروط احتجاز دفع المورّد</span><span class="sxs-lookup"><span data-stu-id="27aa9-107">Create vendor payment retention terms</span></span>

<span data-ttu-id="27aa9-108">يمكنك إدخال النسبة المئوية لدفعة المورّد التي تريد احتجازها والنسبة المئوية من المبالغ التي سبق أن تم احتجازها والتي يجب تحريرها.</span><span class="sxs-lookup"><span data-stu-id="27aa9-108">You can enter the percentage of vendor payment for retention and the percentage of the previously retained amounts to be released.</span></span> <span data-ttu-id="27aa9-109">يتم بشكل تلقائي احتجاز المبالغ على فواتير المورّد حتى يصل العقد إلى حالة الاكتمال المحددة.</span><span class="sxs-lookup"><span data-stu-id="27aa9-109">Amounts are automatically retained on vendor invoices until the contract reaches the specified state of completion.</span></span> <span data-ttu-id="27aa9-110">بعد إعداد شروط الاحتجاز، يمكنك تطبيقها على أي مشروع لهذا المورّد.</span><span class="sxs-lookup"><span data-stu-id="27aa9-110">After you set up the retention terms, you can apply them to any project for that vendor.</span></span>

<span data-ttu-id="27aa9-111">استخدم الخطوات التالية لإعداد شروط احتجاز دفع المورّد والاحتفاظ بها.</span><span class="sxs-lookup"><span data-stu-id="27aa9-111">Use the following steps to set up and maintain retention terms for vendor payments.</span></span> 

1. <span data-ttu-id="27aa9-112">انتقل إلى **إدارة المشاريع والمحاسبة‬** > **الاحتجاز** > **شروط احتجاز دفع المورّد**.</span><span class="sxs-lookup"><span data-stu-id="27aa9-112">Go to **Project management and accounting** > **Retention** > **Vendor payment retention terms**.</span></span>
2. <span data-ttu-id="27aa9-113">حدد **جديد** لإضافة شرط جديد من شروط احتجاز دفع المورّد.</span><span class="sxs-lookup"><span data-stu-id="27aa9-113">Select **New** to add a new vendor retention term.</span></span> <span data-ttu-id="27aa9-114">يتم إدخال قيمة **معرف القاعدة** للشرط الجديد بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="27aa9-114">The **Rule ID** value for the new term is automatically entered.</span></span> 
3. <span data-ttu-id="27aa9-115">أدخل وصفًا موجزًا في حقل **الوصف**، وعلى علامة التبويب السريعة **الشروط**، حدد **إضافة بند** لإدخال قيم الشروط لما يلي:</span><span class="sxs-lookup"><span data-stu-id="27aa9-115">Enter a brief description in the **Description** field, and on the **Terms** FastTab, select **Add line** to enter term values for the following:</span></span>

   - <span data-ttu-id="27aa9-116">**النسبة المئوية للوحدات التي تم تسليمها**: أدخل نسبة اكتمال الشرط.</span><span class="sxs-lookup"><span data-stu-id="27aa9-116">**Percentage of units delivered**: Enter a percentage of completion for the term.</span></span> <span data-ttu-id="27aa9-117">يتم بشكل تلقائي احتجاز المبالغ على فواتير المورّد حتى تصبح مرحلة اكتمال المشروع مساوية للنسبة المئوية.</span><span class="sxs-lookup"><span data-stu-id="27aa9-117">Amounts are automatically retained on vendor invoices until the project stage of completion is equal to the specified percentage.</span></span> <span data-ttu-id="27aa9-118">على سبيل المثال، إذا قمت بإدخال 50.00، يتم احتجاز المبالغ حتى اكتمال المشروع بنسبة 50%.</span><span class="sxs-lookup"><span data-stu-id="27aa9-118">For example, if you enter 50.00, amounts are retained until the project is 50 percent completed.</span></span>
   - <span data-ttu-id="27aa9-119">**النسبة المئوية لاحتجازها**: أدخل نسبة مئوية لمبلغ فاتورة المورّد التي يجب احتجازها.</span><span class="sxs-lookup"><span data-stu-id="27aa9-119">**Percentage to retain**: Enter a percentage of the vendor invoice amount to be retained.</span></span> <span data-ttu-id="27aa9-120">على سبيل المثال ، إذا قمت بإدخال 10.00، فسيتم احتجاز 10 بالمئة من المبلغ على فاتورة المورّد حتى يصل المشروع إلى النسبة المئوية للاكتمال كما تم تعيينها في الحقل **النسبة المئوية لعدد الوحدات التي تم تسليمها**.</span><span class="sxs-lookup"><span data-stu-id="27aa9-120">For example, if you enter 10.00, then 10 percent of the amount on a vendor invoice is retained until the project reaches the percentage of completion as set in the **Percentage of units delivered field**.</span></span>
   - <span data-ttu-id="27aa9-121">**النسبة المئوية لتحريرها**: حدد **إضافة بند** لإدخال نسبة مئوية من أي مبالغ تم احتجازها في الاسبق ويجب تحريرها للمستوى المحدد من اكتمال المشروع.</span><span class="sxs-lookup"><span data-stu-id="27aa9-121">**Percentage to release**: Select **Add line** to enter a percentage of any previously retained amounts to be released for the selected level of project completion.</span></span>

> [!NOTE]
> <span data-ttu-id="27aa9-122">إذا كان لديك أكثر من مرحلة رئيسية واحدة لمستويات إكمال المشروع المختلفة، فأدخل بندًا منفصلاً لشروط احتجاز دفع المورّد لكل قاعدة احتجاز.</span><span class="sxs-lookup"><span data-stu-id="27aa9-122">If you have more than one milestone for different levels of project completion, enter a separate vendor retention term line for each retention rule.</span></span> <span data-ttu-id="27aa9-123">يمكن لكل بند تحديد نسبة احتجاز مختلفة ونسبة تحرير مختلفة لكل مستوى معين من اكتمال المشروع.</span><span class="sxs-lookup"><span data-stu-id="27aa9-123">Each line can specify a different retention percentage and a different release percentage for each designated level of project completion.</span></span>

<span data-ttu-id="27aa9-124">بعد إنشاء شروط احتجاز دفع المورّد لمورّد، يمكنك تطبيقها على مشروع.</span><span class="sxs-lookup"><span data-stu-id="27aa9-124">After you create vendor retention terms for a vendor, you can apply the terms to a project.</span></span>

## <a name="apply-vendor-retention-terms-to-a-project"></a><span data-ttu-id="27aa9-125">تطبيق شروط احتجاز دفع المورّد على مشروع</span><span class="sxs-lookup"><span data-stu-id="27aa9-125">Apply vendor retention terms to a project</span></span>

1. <span data-ttu-id="27aa9-126">انتقل إلى **إدارة المشاريع والمحاسبة‬** > **المشاريع** > **جميع المشاريع** وافتح مشروعًا من صفحة قائمة المشاريع.</span><span class="sxs-lookup"><span data-stu-id="27aa9-126">Go to **Project management and accounting** > **Projects** > **All projects** and open a project from the project list page.</span></span>
2. <span data-ttu-id="27aa9-127">على علامة التبويب السريعة **اتفاقيات المورّد**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="27aa9-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="27aa9-128">في **حقل كود الحساب**، حدد أحد الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="27aa9-128">In the **Account code field**, select one of the following options:</span></span> 

   - <span data-ttu-id="27aa9-129">**الجدول**: تنطبق شروط احتجاز دفع المورّد على مورّد واحد.</span><span class="sxs-lookup"><span data-stu-id="27aa9-129">**Table**: The vendor retention terms apply to a single vendor.</span></span>
   - <span data-ttu-id="27aa9-130">**المجموعة**: تنطبق شروط احتجاز دفع المورّد على جميع المورّدين في مجموعة مورّدين.</span><span class="sxs-lookup"><span data-stu-id="27aa9-130">**Group**: The vendor retention terms apply to all vendors in a vendor group.</span></span>
   - <span data-ttu-id="27aa9-131">**الكل**: تنطبق شروط احتجاز دفع المورّد على جميع المورّدين.</span><span class="sxs-lookup"><span data-stu-id="27aa9-131">**All**: The vendor retention terms apply to all vendors.</span></span>

4. <span data-ttu-id="27aa9-132">في **حقل المورّد/مجموعة المورّدين**، حدد المورّد أو مجموعة المورّدين التي تنطبق عليها شروط احتجاز دفع المورّد.</span><span class="sxs-lookup"><span data-stu-id="27aa9-132">In the **Vendor/Vendor group field**, select the vendor or vendor group to which the vendor retention terms apply.</span></span> <span data-ttu-id="27aa9-133">إذا حددت **الكل** في الخطوة السابقة، لن يكون هذا الحقل متوفرًا.</span><span class="sxs-lookup"><span data-stu-id="27aa9-133">If you selected **All** in the previous step, this field is unavailable.</span></span>
5. <span data-ttu-id="27aa9-134">في الحقل **شروط احتجاز المورّد**، حدد شروط الاحتجاز التي أنشأتها في الإجراء السابق.</span><span class="sxs-lookup"><span data-stu-id="27aa9-134">In the **Vendor retention terms** field, select the retention terms that you created in the previous procedure.</span></span>
6. <span data-ttu-id="27aa9-135">إذا تم إعداد شروط الدفع عند استلام الدفع في المشروع للمورّد، فأدخل النسبة المئوية للحد في المشروع في حقل **النسبة المئوية لحد الدفع عند استلام الدفع**.</span><span class="sxs-lookup"><span data-stu-id="27aa9-135">If the project also has pay-when-paid (PWP) terms set up for the vendor, enter the threshold percentage for the project in the **PWP threshold percentage** field.</span></span>

<span data-ttu-id="27aa9-136">تظهر أيضًا شروط احتجاز دفع المورّد في أوامر الشراء التي تقوم بإنشائها للمورّد.</span><span class="sxs-lookup"><span data-stu-id="27aa9-136">The vendor retention terms are also displayed on purchase orders that you create for the vendor.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]