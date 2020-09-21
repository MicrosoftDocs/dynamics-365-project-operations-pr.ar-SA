---
title: تكوين فواتير المشاريع بين الشركات الشقيقة
description: يوضح هذا الموضوع كيفية إعداد فواتير المشروع بين شركتين في مؤسستك.
author: KimANelson
manager: AnnBe
ms.date: 07/29/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendTable, InterCompanyTradingRelationSetupVendor, SysDataAreaSelectLookup, ProjParameters, ProjPosting, ProjTransferPrice
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.assetid: 72d6c257-f2d3-483b-8ff2-445263796963
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 7b199c85736f6268bc5914fddaa10e4cabd44ef1
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748613"
---
# <a name="configure-intercompany-project-invoicing"></a><span data-ttu-id="5a3a0-103">تكوين فواتير المشاريع بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="5a3a0-103">Configure intercompany project invoicing</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="5a3a0-104">يوضح هذا الموضوع كيفية إعداد فواتير المشروع بين شركتين في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-104">This topic shows how to set up project invoicing between two companies in your organization.</span></span> <span data-ttu-id="5a3a0-105">تستخدم هذه المهمة مجموعة بيانات USSI.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="5a3a0-106">في جزء التنقل، انتقل إلى **الوحدات > الحسابات الدائنة > الموردون > جميع الموردين**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-106">In the navigation pane, go to **Modules > Accounts payable > Vendors > All vendors**.</span></span>
2. <span data-ttu-id="5a3a0-107">في قائمة **جميع الموردين**، ابحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-107">In the **All vendors** list, find and select the desired record.</span></span>
3. <span data-ttu-id="5a3a0-108">في جزء الإجراءات، حدد **عام**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-108">On the Action Pane, select **General**.</span></span>
4. <span data-ttu-id="5a3a0-109">حدد **بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-109">Select **Intercompany**.</span></span>
5. <span data-ttu-id="5a3a0-110">قم بتعيين **نشط** إلى **نعم** لتمكين التجارة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-110">Set **Active** to **Yes** to enable intercompany trading.</span></span>
6. <span data-ttu-id="5a3a0-111">في حقل **شركة العميل**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-111">In the **Customer company** field, enter or select a value.</span></span>
7. <span data-ttu-id="5a3a0-112">في حقل **حسابي**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-112">In the **My account** field, enter or select a value.</span></span>
8. <span data-ttu-id="5a3a0-113">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-113">Select **Save**.</span></span>
9. <span data-ttu-id="5a3a0-114">أغلق الصفحات للعودة إلى الصفحة الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-114">Close the pages to return to the home page.</span></span>
10. <span data-ttu-id="5a3a0-115">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > إعداد > معلمات المشاريع ومحاسبتها**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-115">In the navigation pane, go to **Modules > Project management and accounting > Setup > Project management and accounting parameters**.</span></span>
11. <span data-ttu-id="5a3a0-116">حدد علامة التبويب **بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-116">Select the **Intercompany** tab.</span></span>
12. <span data-ttu-id="5a3a0-117">حرك شريط التمرير إلى **نعم** لتمكين جدولة الموارد والجداول الزمنيه بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-117">Move the slider to **Yes** to enable intercompany resource scheduling and timesheets.</span></span>
13. <span data-ttu-id="5a3a0-118">في القائمة، ضع علامة على الصف المحدد.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-118">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="5a3a0-119">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-119">Select **New**.</span></span>
15. <span data-ttu-id="5a3a0-120">في حقل **استعارة الكيان القانوني**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-120">In the **Borrowing legal entity** field, enter or select a value.</span></span>
16. <span data-ttu-id="5a3a0-121">انقر فوق خانة الاختيار **تراكم الإيراد**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-121">Select the **Accrue revenue** check box.</span></span>
17. <span data-ttu-id="5a3a0-122">في حقل **فئة الجدول الزمني الافتراضية**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-122">In the **Default timesheet category** field, enter or select a value.</span></span>
18. <span data-ttu-id="5a3a0-123">في حقل **فئة المصروفات الافتراضية**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-123">In the **Default expense category** field, enter or select a value.</span></span>
19. <span data-ttu-id="5a3a0-124">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-124">Select **Save**.</span></span>
20. <span data-ttu-id="5a3a0-125">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-125">Close the page.</span></span>
21. <span data-ttu-id="5a3a0-126">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > إعداد > نشر > إعداد نشر دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-126">In the navigation pane, go to **Modules > Project management and accounting > Setup > Posting > Ledger posting setup**.</span></span>
22. <span data-ttu-id="5a3a0-127">في حقل **أنواع حساب دفتر الأستاذ**، حدد أحد الخيارات.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-127">In the **Ledger account types** field, select an option.</span></span>
23. <span data-ttu-id="5a3a0-128">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-128">Select **New**.</span></span>
24. <span data-ttu-id="5a3a0-129">في حقل **الحساب الرئيسي** للصف الجديد، حدد القيم المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-129">In the **Main account** field of the new row, specify the desired values.</span></span>
25. <span data-ttu-id="5a3a0-130">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-130">Select **Save**.</span></span>
26. <span data-ttu-id="5a3a0-131">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-131">Close the page.</span></span>
27. <span data-ttu-id="5a3a0-132">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > إعداد > الأسعار > سعر النقل**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-132">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Transfer price**.</span></span>
28. <span data-ttu-id="5a3a0-133">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-133">Select **New**.</span></span>
29. <span data-ttu-id="5a3a0-134">في حقل **تاريخ السريان**، وأدخل تاريخًا.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-134">In the **Effective date** field, enter a date.</span></span>
30. <span data-ttu-id="5a3a0-135">في حقل **استعارة الكيان القانوني**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-135">In the **Borrowing legal entity** field, enter or select a value.</span></span>
31. <span data-ttu-id="5a3a0-136">في حقل **نموذج سعر التحويل**، حدد أحد الخيارات.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-136">In the **Transfer price model** field, select an option.</span></span>
32. <span data-ttu-id="5a3a0-137">في حقل **الأسعار**، حدد رقمًا.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-137">In the **Pricing** field, enter a number.</span></span>
33. <span data-ttu-id="5a3a0-138">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5a3a0-138">Select **Save**.</span></span>

