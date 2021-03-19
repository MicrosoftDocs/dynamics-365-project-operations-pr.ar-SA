---
title: استعلام جدول نفقات المكافآت الفيدرالية
description: يقدم هذا الموضوع معلومات حول استعلام جدول نفقات المكافآت الفيدرالية.
author: velofog
manager: Ann Beebe
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: 70dff12c106723dda801668412cfd084c462db4b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288948"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="28109-103">استعلام جدول نفقات المكافآت الفيدرالية</span><span class="sxs-lookup"><span data-stu-id="28109-103">Schedule of Expenditures of Federal Awards inquiry</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="28109-104">وفقًا لما ورد في Office of Management and Budget Circular A-133، تخضع الوكالات التي تتلقى المنح الفيدرالية لمتطلبات التدقيق، المعروفة أيضًا بعمليات التدقيق الفردية.</span><span class="sxs-lookup"><span data-stu-id="28109-104">According to Office of Management and Budget Circular A-133, agencies that receive federal funds are subject to audit requirements, which are also known as single audits.</span></span> <span data-ttu-id="28109-105">يتم استخدام عملية التدقيق للإبلاغ عن إيرادات ونفقات المنح الفيدرالية على أساس متكرر.</span><span class="sxs-lookup"><span data-stu-id="28109-105">The audit process is used to report on the revenues and expenditures of federal grants on a recurring basis.</span></span> <span data-ttu-id="28109-106">يشتمل جزء من تقرير التدقيق الفردي على جدول نفقات المكافآت الفيدرالية (SEFA).</span><span class="sxs-lookup"><span data-stu-id="28109-106">Part of the single audit report includes the Schedule of Expenditures of Federal Awards (SEFA).</span></span>

<span data-ttu-id="28109-107">يتضمن جدول نفقات المكافآت الفيدرالية عنوان ورقم كتالوج المساعدة المحلية الفيدرالية (CFDA) ورقم المنحة وسنة المنحة واسم الوكالة الفيدرالية التي توفر الأموال واسم الكيان العابر.</span><span class="sxs-lookup"><span data-stu-id="28109-107">The Schedule of Expenditures of Federal Awards inquiry includes the Catalog of Federal Domestic Assistance (CFDA) title and number, the grant number, the year of the grant, the name of the federal agency that provides the funds, and the name of the pass-through entity.</span></span> <span data-ttu-id="28109-108">يتعلق الاستعلام بفترة محددة.</span><span class="sxs-lookup"><span data-stu-id="28109-108">The inquiry is for a specific period.</span></span> <span data-ttu-id="28109-109">تكون هذه الفترة عادةً هي نفسها فترة البيان المالي، وهو سنة مالية.</span><span class="sxs-lookup"><span data-stu-id="28109-109">Typically, that period is the same as the financial statement period, which is a fiscal year.</span></span>

<span data-ttu-id="28109-110">يتضمن الاستعلام المنح التي لديها تواريخ توقع في نطاق التاريخ المحدد.</span><span class="sxs-lookup"><span data-stu-id="28109-110">The inquiry includes grants that have projection dates in the selected date range.</span></span> <span data-ttu-id="28109-111">يعرض عمود **الوكالة المانحة** للاستعلام عميل المنحة، أو الوكالة المانحة إذا تعلق الأمر بمنحة عابرة.</span><span class="sxs-lookup"><span data-stu-id="28109-111">The **Grantor agency** column of the inquiry shows the grant customer or, for a pass-through grant, the grantor agency.</span></span> <span data-ttu-id="28109-112">بالنسبة إلى المنحة العابرة، يُظهر عمود **الوكالة العابرة** عميل المنحة.</span><span class="sxs-lookup"><span data-stu-id="28109-112">For a pass-through grant, the **Pass-through agency** column shows the grant customer.</span></span> <span data-ttu-id="28109-113">إذا لم تكن المنحة عبارة عن منحة عابرة، فسيكون عمود **الوكالة العابرة** فارغًا.</span><span class="sxs-lookup"><span data-stu-id="28109-113">If the grant isn't a pass-through grant, the **Pass-through agency** column is blank.</span></span>

## <a name="set-up-the-cfda-clusters"></a><span data-ttu-id="28109-114">إعداد مجموعات CFDA</span><span class="sxs-lookup"><span data-stu-id="28109-114">Set up the CFDA clusters</span></span>

<span data-ttu-id="28109-115">يجب عليك إعداد مجموعات CFDA التي يمكن ربطها بأرقام CFDA في استعلام جدول نفقات المكافآت الفيدرالية.</span><span class="sxs-lookup"><span data-stu-id="28109-115">You must set up the CFDA clusters that can be associated with CFDA numbers in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="28109-116">انتقل إلى **إدارة المشاريع والمحاسبة \> الإعداد \> المنح \> كتالوج مجموعات المساعدة المحلية الفيدرالية**.</span><span class="sxs-lookup"><span data-stu-id="28109-116">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance clusters**.</span></span>
2. <span data-ttu-id="28109-117">حدد **جديد** لإنشاء مجموعة CFDA.</span><span class="sxs-lookup"><span data-stu-id="28109-117">Select **New** to create a CFDA cluster.</span></span>
3. <span data-ttu-id="28109-118">أدخل اسم المجموعة.</span><span class="sxs-lookup"><span data-stu-id="28109-118">Enter the cluster name.</span></span>
4. <span data-ttu-id="28109-119">حدد **حفظ** لتطبيق التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="28109-119">Select **Save** to save your changes.</span></span>

## <a name="set-up-cfda-numbers"></a><span data-ttu-id="28109-120">إعداد أرقام CFDA</span><span class="sxs-lookup"><span data-stu-id="28109-120">Set up CFDA numbers</span></span>

<span data-ttu-id="28109-121">يجب عليك إعداد أرقام CFDA التي يمكن إضافتها إلى المنح وتضمينها في استعلام جدول نفقات المكافآت الفيدرالية.</span><span class="sxs-lookup"><span data-stu-id="28109-121">You must set up CFDA numbers that can be added to grants and included in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="28109-122">انتقل إلى **إدارة المشاريع والمحاسبة \> الإعداد \> المنح \> أرقام كتالوجات المساعدة المحلية الفيدرالية**.</span><span class="sxs-lookup"><span data-stu-id="28109-122">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance numbers**.</span></span>
2. <span data-ttu-id="28109-123">حدد **جديد** لإنشاء رقم CFDA.</span><span class="sxs-lookup"><span data-stu-id="28109-123">Select **New** to create a CFDA number.</span></span>
3. <span data-ttu-id="28109-124">في عمود **الرقم**، أدخل رقم CFDA.</span><span class="sxs-lookup"><span data-stu-id="28109-124">In the **Number** column, enter the CFDA number.</span></span>
4. <span data-ttu-id="28109-125">اضغط على المفتاح **Tab**.</span><span class="sxs-lookup"><span data-stu-id="28109-125">Press the **Tab** key.</span></span>
5. <span data-ttu-id="28109-126">في عمود **الوصف**، أدخل عنوان CFDA.</span><span class="sxs-lookup"><span data-stu-id="28109-126">In the **Description** column, enter the CFDA title.</span></span>
6. <span data-ttu-id="28109-127">اضغط على المفتاح **Tab**.</span><span class="sxs-lookup"><span data-stu-id="28109-127">Press the **Tab** key.</span></span>
7. <span data-ttu-id="28109-128">اختياري: في الحقل **مجموعة البرامج**، أضف مجموعة CFDA المناسبة.</span><span class="sxs-lookup"><span data-stu-id="28109-128">Optional: In the **Program cluster** field, add the appropriate CFDA cluster.</span></span>
8. <span data-ttu-id="28109-129">حدد **حفظ** لتطبيق التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="28109-129">Select **Save** to save your changes.</span></span>

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="28109-130">إعداد المنح للإبلاغ عن استعلام جدول نفقات المكافآت الفيدرالية‬</span><span class="sxs-lookup"><span data-stu-id="28109-130">Set up grants to report for the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="28109-131">انتقل إلى **إدارة المشاريع والمحاسبة \> المنح \> المنح**، وحدد منحة موجودة.</span><span class="sxs-lookup"><span data-stu-id="28109-131">Go to **Project management and accounting \> Grants \> Grants**, and select an existing grant.</span></span>
2. <span data-ttu-id="28109-132">على علامة التبويب السريع **الإعداد**، في حقل **كتالوج المساعدة المحلية الفيدرالية**، عيّن رقم CFDA.</span><span class="sxs-lookup"><span data-stu-id="28109-132">On the **Setup** FastTab, in the **Catalog of Federal Domestic Assistance** field, assign the CFDA number.</span></span> <span data-ttu-id="28109-133">يحدد رقم CFDA على المنحة مجموعة CFDA لإعداد التقارير.</span><span class="sxs-lookup"><span data-stu-id="28109-133">The CFDA number on the grant determines the CFDA cluster for reporting.</span></span>
3. <span data-ttu-id="28109-134">على علامة التبويب السريعة **معلومات الاتصال**، أدخل معلومات المانح عن طريق اتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="28109-134">On **Contact information** FastTab, enter the grantor information by following these steps:</span></span>

    1. <span data-ttu-id="28109-135">في الحقل **عميل المنحة**، أدخل اسم العميل المسؤول عن المنحة.</span><span class="sxs-lookup"><span data-stu-id="28109-135">In the **Grant customer** field, enter the customer who is responsible for the grant.</span></span> <span data-ttu-id="28109-136">بالنسبة إلى منحة موجودة، من المحتمل أن تكون هذه المعلومات مدخلة بالفعل.</span><span class="sxs-lookup"><span data-stu-id="28109-136">For an existing grant, this information might already be entered.</span></span>
    2. <span data-ttu-id="28109-137">حدد ما إذا كان عميل المنحة هو المموّل.</span><span class="sxs-lookup"><span data-stu-id="28109-137">Indicate whether the grant customer is the funder.</span></span> <span data-ttu-id="28109-138">إذا كان العميل المانح هو المموّل، فاترك خانة الاختيار **عابر** من دون تحديد.</span><span class="sxs-lookup"><span data-stu-id="28109-138">If the grant customer is the funder, leave the **Pass-through** check box cleared.</span></span> <span data-ttu-id="28109-139">إذا كان المموّل عميل آخر، والعميل المانح مسؤول عن إنفاق المال وتعقبه، فحدد خانة الاختيار **عابر**.</span><span class="sxs-lookup"><span data-stu-id="28109-139">If another customer is the funder, and the grant customer is responsible for spending and tracking the money, select the **Pass-through** check box.</span></span>

4. <span data-ttu-id="28109-140">إذا قمت بتحديد خانة الاختيار **عابر** في الخطوة السابقة، فأدخل اسم العميل الذي قدم المنحة في حقل **الوكالة المانحة**.</span><span class="sxs-lookup"><span data-stu-id="28109-140">If you selected the **Pass-through** check box in the previous step, in the **Grantor agency** field, enter the customer who provided the grant.</span></span> <span data-ttu-id="28109-141">لا يمكن أن يشير خيار الوكالة المانحة والعميل المانح إلى العميل نفسه.</span><span class="sxs-lookup"><span data-stu-id="28109-141">The grantor agency and the grant customer can't be the same customer.</span></span>

<span data-ttu-id="28109-142">فيما يلي مثال عن منحة عابرة:</span><span class="sxs-lookup"><span data-stu-id="28109-142">Here is an example of a pass-through grant:</span></span>

<span data-ttu-id="28109-143">قامت الحكومة الفيدرالية بتمويل مشروع بنية أساسية في ولاية.</span><span class="sxs-lookup"><span data-stu-id="28109-143">The federal government funded an infrastructure project for a state.</span></span> <span data-ttu-id="28109-144">قدمت الحكومة الفيدرالية للولاية الأموال المطلوب إنفاقها.</span><span class="sxs-lookup"><span data-stu-id="28109-144">The federal government gave the money to the state to spend.</span></span> <span data-ttu-id="28109-145">وفي هذه الحالة، تكون الحكومة الفيدرالية الوكالة المانحة، والولاية هي العميل المانح.</span><span class="sxs-lookup"><span data-stu-id="28109-145">In this case, the federal government is the grantor agency, and the state is the grant customer.</span></span>

> [!NOTE] 
> <span data-ttu-id="28109-146">عند تشغيل الميزة للمرة الأولى، سيتم إدخال أرقام CFDA باستخدام الأرقام الموجودة على المنح.</span><span class="sxs-lookup"><span data-stu-id="28109-146">When you first turn on the feature, initial CFDA numbers will be entered by using the existing numbers on grants.</span></span>

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a><span data-ttu-id="28109-147">استبعاد المنح من تقارير SEFA المستندة إلى نوع المنحة</span><span class="sxs-lookup"><span data-stu-id="28109-147">Exclude grants from SEFA reporting based on the grant type</span></span>

1. <span data-ttu-id="28109-148">انتقل إلى **إدارة المشاريع والمحاسبة \> الإعداد \> المنح‏‎ \> أنواع المنح‏‎**.</span><span class="sxs-lookup"><span data-stu-id="28109-148">Go to **Project management and accounting \> Setup \> Grants \> Grant types**.</span></span>
2. <span data-ttu-id="28109-149">على علامة التبويب السريع **المعلومات الافتراضية**، حدد خانة الاختيار **استبعاد من جدول نفقات المكافآت الفيدرالية**.</span><span class="sxs-lookup"><span data-stu-id="28109-149">On the **Default information** FastTab, select the **Exclude from Schedule of Expenditures of Federal Awards** check box.</span></span>
3. <span data-ttu-id="28109-150">حدد **حفظ** لتطبيق التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="28109-150">Select **Save** to save your changes.</span></span>

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="28109-151">تشغيل استعلام جدول نفقات المكافآت الفيدرالية</span><span class="sxs-lookup"><span data-stu-id="28109-151">Run the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="28109-152">انتقل إلى **إدارة المشاريع والمحاسبة \> الاستعلامات والتقارير \> استعلام المنحة \> جدول نفقات المكافآت الفيدرالية‬**.</span><span class="sxs-lookup"><span data-stu-id="28109-152">Go to **Project management and accounting \> Inquiries and reports \> Grant inquiry \> Schedule of Expenditures of Federal Awards**.</span></span>
2. <span data-ttu-id="28109-153">في قسم **المعلمات**، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="28109-153">In the **Parameters** section, follow these steps:</span></span>

    1. <span data-ttu-id="28109-154">في الحقل **الفاصل الزمني**، حدد الكود الخاص بالفترة الزمنية.</span><span class="sxs-lookup"><span data-stu-id="28109-154">In the **Date interval** field, select the code for the date interval.</span></span> <span data-ttu-id="28109-155">أو حدد الفاصل الزمني في الحقلين **تاريخ البدء** و **تاريخ الانتهاء**.</span><span class="sxs-lookup"><span data-stu-id="28109-155">Alternatively, in the **From date** and **To date** fields, define the date interval.</span></span>
    2. <span data-ttu-id="28109-156">اختياري: لتضمين الحركات المفوترة فقط كإيراد في الاستعلام، قم بتعيين الخيار **تضمين الإيرادات المفوترة فقط** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="28109-156">Optional: To include only billed transactions as revenue in the inquiry, set the **Include only billed revenues** option to **Yes**.</span></span>

## <a name="columns"></a><span data-ttu-id="28109-157">الأعمدة</span><span class="sxs-lookup"><span data-stu-id="28109-157">Columns</span></span>

<span data-ttu-id="28109-158">يتضمن استعلام جدول نفقات المكافآت الفيدرالية‬ الأعمدة التالية:</span><span class="sxs-lookup"><span data-stu-id="28109-158">The Schedule of Expenditures of Federal Awards inquiry includes the following columns:</span></span>

- <span data-ttu-id="28109-159">اسم مجموعة كتالوج المساعدة المحلية الفيدرالية</span><span class="sxs-lookup"><span data-stu-id="28109-159">Catalog of Federal Domestic Assistance cluster name</span></span>
- <span data-ttu-id="28109-160">الوكالة المانحة</span><span class="sxs-lookup"><span data-stu-id="28109-160">Grantor agency</span></span>
- <span data-ttu-id="28109-161">الوكالة العابرة</span><span class="sxs-lookup"><span data-stu-id="28109-161">Pass-through agency</span></span>
- <span data-ttu-id="28109-162">اسم المنحة</span><span class="sxs-lookup"><span data-stu-id="28109-162">Grant name</span></span>
- <span data-ttu-id="28109-163">معرف المنحة</span><span class="sxs-lookup"><span data-stu-id="28109-163">Grant ID</span></span>
- <span data-ttu-id="28109-164">معرف تطبيق المنحة</span><span class="sxs-lookup"><span data-stu-id="28109-164">Grant application ID</span></span>
- <span data-ttu-id="28109-165">كتالوج المساعدة المحلية الفيدرالية</span><span class="sxs-lookup"><span data-stu-id="28109-165">Catalog of Federal Domestic Assistance</span></span>
- <span data-ttu-id="28109-166">إيصالات</span><span class="sxs-lookup"><span data-stu-id="28109-166">Receipts</span></span>
- <span data-ttu-id="28109-167">النفقات</span><span class="sxs-lookup"><span data-stu-id="28109-167">Expenditures</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]