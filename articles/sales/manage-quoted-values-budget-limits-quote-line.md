---
title: نظرة عامة على بنود عرض الأسعار القائم على المشروع
description: يقدم هذا الموضوع معلومات حول استخدام بنود عروض الأسعار المستندة إلى المشروع لعمل المشروع.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ea54d83b1e26d1ee3520dbfab9ba56ffd1191dc9
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181841"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="95347-103">نظرة عامة على بنود عرض الأسعار القائم على المشروع</span><span class="sxs-lookup"><span data-stu-id="95347-103">Project-based quote lines overview</span></span>

<span data-ttu-id="95347-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="95347-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="95347-105">تم تصميم بنود عرض الأسعار المستندة إلى المشروع للمساعدة في تقدير عمل المشروع بأحد المشاركات.</span><span class="sxs-lookup"><span data-stu-id="95347-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="95347-106">يتم توسيع بنية سطر عرض الأسعار المستند إلى المشروع لتقديرات المشروع بالمفاهيم التالية:</span><span class="sxs-lookup"><span data-stu-id="95347-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="95347-107">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="95347-107">Billing Method</span></span>
- <span data-ttu-id="95347-108">تعيين المشروع</span><span class="sxs-lookup"><span data-stu-id="95347-108">Project Mapping</span></span>
- <span data-ttu-id="95347-109">فئات الحركات المضمنة</span><span class="sxs-lookup"><span data-stu-id="95347-109">Included Transaction classes</span></span>
- <span data-ttu-id="95347-110">حد يجب عدم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="95347-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="95347-111">إعداد الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="95347-111">Chargeability setup</span></span>
- <span data-ttu-id="95347-112">التقدير باستخدام تفاصيل بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="95347-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="95347-113">عملاء بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="95347-113">Quote line Customers</span></span>

<span data-ttu-id="95347-114">يوفر الجدول التالي معلومات حول الحقول الموجودة في علامة التبويب **عام** في بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="95347-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="95347-115">وتساعد هذه الحقول في إعداد الأساس لتقدير تفصيلي من القاعدة إلى القمة لعمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="95347-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="95347-116">**الحقل**</span><span class="sxs-lookup"><span data-stu-id="95347-116">**Field**</span></span> | <span data-ttu-id="95347-117">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="95347-117">**Description**</span></span> | <span data-ttu-id="95347-118">**تأثير لاحق**</span><span class="sxs-lookup"><span data-stu-id="95347-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="95347-119">اسم</span><span class="sxs-lookup"><span data-stu-id="95347-119">Name</span></span> | <span data-ttu-id="95347-120">اسم بند عرض الأسعار الذي ينبغي أن يساعدك في تحديد المكون المنفصل لعرض الأسعار الذي يتم تقديره.</span><span class="sxs-lookup"><span data-stu-id="95347-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="95347-121">يتم نسخه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-122">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="95347-122">Billing Method</span></span> | <span data-ttu-id="95347-123">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل المقابل في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="95347-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="95347-124">يتضمن هذا الحقل اثنين من نماذج التعاقد الرئيسية المدعومة من Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="95347-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="95347-125">- سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="95347-125">- Fixed price</span></span></br><span data-ttu-id="95347-126">- الوقت والمادة.</span><span class="sxs-lookup"><span data-stu-id="95347-126">- Time and material.</span></span>| <span data-ttu-id="95347-127">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-128">Project</span><span class="sxs-lookup"><span data-stu-id="95347-128">Project</span></span> | <span data-ttu-id="95347-129">استخدم هذا الحقل الاختياري لتحديد المشروع الذي سيتم استخدامه لتسليم العمل في هذه المشاركة.</span><span class="sxs-lookup"><span data-stu-id="95347-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="95347-130">عندما يتم تعيين مشروع إلى بند عرض الأسعار، فإنه يساعد في إعداد المهام الخاضعة للرسوم وكذلك يساعد في إحضار التقديرات المستندة إلى المشروع لبند عرض الأسعار كتفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="95347-131">عند عدم تعيين مشروع لبند عرض أسعار يستند إلى مشروع، يتعين إنشاء التقدير يدويًا عن طريق إنشاء كل تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="95347-132">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-133">تضمين الوقت</span><span class="sxs-lookup"><span data-stu-id="95347-133">Include Time</span></span> | <span data-ttu-id="95347-134">تشير علامة **نعم**/**لا** إلى ما إذا كان حركات الوقت أو تكاليف العمالة في المشروع المحدد مضمنة في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="95347-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="95347-135">تشير علامة **لا** إلى أن حركات الوقت أو تكلفة العمالة لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="95347-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="95347-136">تشير علامة **نعم** إلى أن حركات الوقت أو تكلفة العمالة سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="95347-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="95347-137">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-138">يتضمن المصروفات</span><span class="sxs-lookup"><span data-stu-id="95347-138">Include Expense</span></span> | <span data-ttu-id="95347-139">تشير علامة **نعم**/**لا** إلى ما إذا كانت تكاليف المصروفات في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="95347-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="95347-140">تشير علامة **لا** إلى أن تكلفة المصروفات لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="95347-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="95347-141">تشير علامة **نعم** إلى أن تكلفة المصروفات سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="95347-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="95347-142">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-143">تضمين الرسوم</span><span class="sxs-lookup"><span data-stu-id="95347-143">Include Fee</span></span> | <span data-ttu-id="95347-144">تشير علامة **نعم**/**لا** إلى ما إذا كانت الرسوم في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="95347-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="95347-145">تشير علامة **لا** إلى أن الرسوم لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="95347-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="95347-146">تشير علامة **نعم** إلى أن الرسوم سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="95347-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="95347-147">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-148">المبلغ المعروض</span><span class="sxs-lookup"><span data-stu-id="95347-148">Quoted Amount</span></span> | <span data-ttu-id="95347-149">هذا هو المبلغ الذي سيتم وضعه في التسعير للعميل لكل العمل المتوقع في بند عرض الأسعار المستند إلى المشروع هذا.</span><span class="sxs-lookup"><span data-stu-id="95347-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="95347-150">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل **ميزانية العميل** في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="95347-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="95347-151">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من المبلغ الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="95347-152">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-153">الضريبة المقدرة</span><span class="sxs-lookup"><span data-stu-id="95347-153">Estimated Tax</span></span> | <span data-ttu-id="95347-154">هذا حقل قابل للتحرير لكي يقوم المستخدم بإضافة مبلغ الضريبة المقدرة في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="95347-155">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من مبلغ الضريبة الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="95347-156">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-157">‏‫المبلغ المعروض‬ بعد الضريبة</span><span class="sxs-lookup"><span data-stu-id="95347-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="95347-158">هذا الحقل هو مبلغ بند عرض الأسعار بعد الضريبة وهو للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="95347-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="95347-159">يتم حساب المبلغ الموجود في هذا الحقل *كمبلغ معروض + الضريبة*.</span><span class="sxs-lookup"><span data-stu-id="95347-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="95347-160">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-161">حد ما يجب ألا يتم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="95347-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="95347-162">ويكون هذا الحقل قابلا للتحرير ويكون متاحا فقط في بنود عروض الأسعار المستندة إلى المشروع والتي لها أسلوب فوترة **الوقت والمادة**.</span><span class="sxs-lookup"><span data-stu-id="95347-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="95347-163">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="95347-164">موازنة العميل</span><span class="sxs-lookup"><span data-stu-id="95347-164">Customer Budget</span></span> | <span data-ttu-id="95347-165">يكون هذا الحقل قابلا للتحرير ويتم نسخه من الحقل المقابل في بند الفرصة إذا تم إنشاء عرض الأسعار من إحدى الفرص.</span><span class="sxs-lookup"><span data-stu-id="95347-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="95347-166">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="95347-167">قواعد التحقق من الصحة للحقول في علامة التبويب عام لبنود عرض الأسعار المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="95347-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="95347-168">**القاعدة 1**: يمكن فقط تضمين فئة حركات معينة في المشروع المحدد في بند عرض أسعار واحد يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="95347-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="95347-169">**القاعدة 2**: إذا كانت الفرصة تحتوي على عدة عروض أسعار، فيمكن أن يكون هناك بنود عرض أسعار مختلفة والتي تشير إلى نفس المشروع وتتضمن نفس فئة الحركات.</span><span class="sxs-lookup"><span data-stu-id="95347-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="95347-170">**القاعدة 3**: إذا لم تكن عروض الأسعار تنتمي إلى نفس الفرصة، فلا يمكن أن تتضمن نفس فئة المشروع والحركات.</span><span class="sxs-lookup"><span data-stu-id="95347-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="95347-171">
                    <strong>الفرصة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="95347-172">
                    <strong>اقتباس</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="95347-173">
                    <strong>بند عرض الأسعار</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="95347-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="95347-175">
                    <strong>تضمين الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="95347-176">
                    <strong>تضمين المصروفات</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="95347-177">
                    <strong>تضمين</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="95347-178">
                    <strong>الرسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="95347-179">
                    <strong>صالح/غير صالح</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="95347-180">
                    <strong>سبب</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95347-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-181">O1</span><span class="sxs-lookup"><span data-stu-id="95347-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-182">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-183">QL1</span><span class="sxs-lookup"><span data-stu-id="95347-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-184">P1</span><span class="sxs-lookup"><span data-stu-id="95347-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-185">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-186">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-187">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-188">غير صالح</span><span class="sxs-lookup"><span data-stu-id="95347-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-189">انتهاك القاعدة #1.</span><span class="sxs-lookup"><span data-stu-id="95347-189">Violation of Rule #1.</span></span> <span data-ttu-id="95347-190">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في كل من بنود عرض الأسعار وQL1 و QL2.</span><span class="sxs-lookup"><span data-stu-id="95347-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-191">O1</span><span class="sxs-lookup"><span data-stu-id="95347-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-192">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-193">QL2</span><span class="sxs-lookup"><span data-stu-id="95347-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-194">P1</span><span class="sxs-lookup"><span data-stu-id="95347-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-195">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-196">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-197">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-197">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-198">O1</span><span class="sxs-lookup"><span data-stu-id="95347-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-199">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-200">QL1</span><span class="sxs-lookup"><span data-stu-id="95347-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-201">P1</span><span class="sxs-lookup"><span data-stu-id="95347-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-202">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-203">Yes</span><span class="sxs-lookup"><span data-stu-id="95347-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-204">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-205">غير صالح</span><span class="sxs-lookup"><span data-stu-id="95347-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-206">انتهاك القاعدة #1.</span><span class="sxs-lookup"><span data-stu-id="95347-206">Violation of Rule #1.</span></span> <span data-ttu-id="95347-207">يتم تضمين الوقت والرسوم في المشروع P1 في كل من بنود عرض الأسعار وQL1 و QL2.</span><span class="sxs-lookup"><span data-stu-id="95347-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-208">O1</span><span class="sxs-lookup"><span data-stu-id="95347-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-209">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-210">QL2</span><span class="sxs-lookup"><span data-stu-id="95347-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-211">P1</span><span class="sxs-lookup"><span data-stu-id="95347-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-212">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-213">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-214">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-214">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-215">O1</span><span class="sxs-lookup"><span data-stu-id="95347-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-216">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-217">QL1</span><span class="sxs-lookup"><span data-stu-id="95347-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-218">P1</span><span class="sxs-lookup"><span data-stu-id="95347-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-219">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-220">Yes</span><span class="sxs-lookup"><span data-stu-id="95347-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-221">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-222">صالح</span><span class="sxs-lookup"><span data-stu-id="95347-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="95347-223">يتم تضمين الوقت والرسوم على المشروع P1 في QL1.</span><span class="sxs-lookup"><span data-stu-id="95347-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="95347-224">يتم تضمين المصروفات في المشروع P1 في QL2.</span><span class="sxs-lookup"><span data-stu-id="95347-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="95347-225">لا يكون هناك تداخل في ما يتم تضمينه في كل بند عرض الأسعار لذا يكون صالحًا.</span><span class="sxs-lookup"><span data-stu-id="95347-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-226">O1</span><span class="sxs-lookup"><span data-stu-id="95347-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-227">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-228">QL2</span><span class="sxs-lookup"><span data-stu-id="95347-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-229">P1</span><span class="sxs-lookup"><span data-stu-id="95347-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-230">Yes</span><span class="sxs-lookup"><span data-stu-id="95347-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-231">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-232">Yes</span><span class="sxs-lookup"><span data-stu-id="95347-232">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-233">O1</span><span class="sxs-lookup"><span data-stu-id="95347-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-234">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-235">QL1</span><span class="sxs-lookup"><span data-stu-id="95347-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-236">P1</span><span class="sxs-lookup"><span data-stu-id="95347-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-237">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-238">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-239">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-240">غير صالح</span><span class="sxs-lookup"><span data-stu-id="95347-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-241">انتهاك القاعدة #1 السابقة</span><span class="sxs-lookup"><span data-stu-id="95347-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="95347-242">يتضمن Q1 الوقت والمصروفات والرسوم للمشروع P1 بالكامل.</span><span class="sxs-lookup"><span data-stu-id="95347-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="95347-243">يتضمن QL2 الوقت والمصروفات والرسوم للمشروع P1 بالكامل ويتداخل مع ما تم تضمينه في Q1.</span><span class="sxs-lookup"><span data-stu-id="95347-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-244">O1</span><span class="sxs-lookup"><span data-stu-id="95347-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-245">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-246">QL2</span><span class="sxs-lookup"><span data-stu-id="95347-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-247">P1</span><span class="sxs-lookup"><span data-stu-id="95347-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-248">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-249">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-250">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-250">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-251">O1</span><span class="sxs-lookup"><span data-stu-id="95347-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-252">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-253">QL1</span><span class="sxs-lookup"><span data-stu-id="95347-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-254">P1</span><span class="sxs-lookup"><span data-stu-id="95347-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-255">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-256">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-257">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="95347-258">صالح</span><span class="sxs-lookup"><span data-stu-id="95347-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-259">بناء على القاعد #2، فإن Q1 و Q2 يمثلان عرضا أسعار في نفس الفرصة، لذا يمكنهم التقدير لنفس المكونات الخاصة بأحد المشروعات.</span><span class="sxs-lookup"><span data-stu-id="95347-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-260">O1</span><span class="sxs-lookup"><span data-stu-id="95347-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-261">ربع السنة الثاني</span><span class="sxs-lookup"><span data-stu-id="95347-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-262">QL1 في Q2</span><span class="sxs-lookup"><span data-stu-id="95347-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-263">P1</span><span class="sxs-lookup"><span data-stu-id="95347-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-264">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-265">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-266">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-266">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-267">O1</span><span class="sxs-lookup"><span data-stu-id="95347-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-268">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-269">QL1</span><span class="sxs-lookup"><span data-stu-id="95347-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-270">P1</span><span class="sxs-lookup"><span data-stu-id="95347-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-271">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-272">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-273">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="95347-274">صالح</span><span class="sxs-lookup"><span data-stu-id="95347-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95347-275">بناء على القاعد #3، فإن Q1 و Q2 يمثلان عرضا أسعار لفرص مختلفة، لذا لا يمكنهم التقدير لنفس المكونات الخاصة بنفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="95347-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="95347-276">O2</span><span class="sxs-lookup"><span data-stu-id="95347-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="95347-277">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="95347-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-278">QL1</span><span class="sxs-lookup"><span data-stu-id="95347-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-279">P1</span><span class="sxs-lookup"><span data-stu-id="95347-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-280">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="95347-281">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="95347-282">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="95347-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="95347-283">غير صالح</span><span class="sxs-lookup"><span data-stu-id="95347-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

