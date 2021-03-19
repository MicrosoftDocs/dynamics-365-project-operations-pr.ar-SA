---
title: نظرة عامة على بنود عرض الأسعار القائم على المشروع - خفيف
description: يقدم هذا الموضوع معلومات حول استخدام بنود عروض الأسعار المستندة إلى المشروع لعمل المشروع. (احترافي)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4865c06691fba09eacf5fe6449adfaf542444520
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272957"
---
# <a name="project-based-quote-lines-overview---lite"></a><span data-ttu-id="c4abb-104">نظرة عامة على بنود عرض الأسعار القائم على المشروع - خفيف</span><span class="sxs-lookup"><span data-stu-id="c4abb-104">Project-based quote lines overview - lite</span></span>

<span data-ttu-id="c4abb-105">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="c4abb-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c4abb-106">تم تصميم بنود عرض الأسعار المستندة إلى المشروع للمساعدة في تقدير عمل المشروع بأحد المشاركات.</span><span class="sxs-lookup"><span data-stu-id="c4abb-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="c4abb-107">يتم توسيع بنية سطر عرض الأسعار المستند إلى المشروع لتقديرات المشروع بالمفاهيم التالية:</span><span class="sxs-lookup"><span data-stu-id="c4abb-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="c4abb-108">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="c4abb-108">Billing Method</span></span>
- <span data-ttu-id="c4abb-109">تعيين المشروع والمهمة</span><span class="sxs-lookup"><span data-stu-id="c4abb-109">Project and Task Mapping</span></span>
- <span data-ttu-id="c4abb-110">فئات الحركات المضمنة</span><span class="sxs-lookup"><span data-stu-id="c4abb-110">Included Transaction classes</span></span>
- <span data-ttu-id="c4abb-111">حد يجب عدم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="c4abb-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="c4abb-112">إعداد الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="c4abb-112">Chargeability setup</span></span>
- <span data-ttu-id="c4abb-113">التقدير باستخدام تفاصيل بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="c4abb-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="c4abb-114">عملاء بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="c4abb-114">Quote line Customers</span></span>

<span data-ttu-id="c4abb-115">يوفر الجدول التالي معلومات حول الحقول الموجودة في علامة التبويب **عام** في بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="c4abb-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="c4abb-116">وتساعد هذه الحقول في إعداد الأساس لتقدير تفصيلي من القاعدة إلى القمة لعمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="c4abb-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="c4abb-117">**الحقل**</span><span class="sxs-lookup"><span data-stu-id="c4abb-117">**Field**</span></span> | <span data-ttu-id="c4abb-118">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="c4abb-118">**Description**</span></span> | <span data-ttu-id="c4abb-119">**تأثير لاحق**</span><span class="sxs-lookup"><span data-stu-id="c4abb-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="c4abb-120">اسم</span><span class="sxs-lookup"><span data-stu-id="c4abb-120">Name</span></span> | <span data-ttu-id="c4abb-121">اسم بند عرض الأسعار الذي ينبغي أن يساعدك في تحديد المكون المنفصل لعرض الأسعار الذي يتم تقديره.</span><span class="sxs-lookup"><span data-stu-id="c4abb-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="c4abb-122">يتم نسخه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-123">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="c4abb-123">Billing Method</span></span> | <span data-ttu-id="c4abb-124">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل المقابل في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="c4abb-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="c4abb-125">يتضمن هذا الحقل نموذجين أساسيين للتعاقد يدعمهما Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="c4abb-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="c4abb-126">- سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="c4abb-126">- Fixed price</span></span></br><span data-ttu-id="c4abb-127">- الوقت والمادة.</span><span class="sxs-lookup"><span data-stu-id="c4abb-127">- Time and material.</span></span>| <span data-ttu-id="c4abb-128">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-129">Project</span><span class="sxs-lookup"><span data-stu-id="c4abb-129">Project</span></span> | <span data-ttu-id="c4abb-130">استخدم هذا الحقل الاختياري لتحديد المشروع الذي سيتم استخدامه لتسليم العمل في هذه المشاركة.</span><span class="sxs-lookup"><span data-stu-id="c4abb-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="c4abb-131">عندما يتم تعيين مشروع إلى بند عرض الأسعار، فإنه يساعد في إعداد المهام الخاضعة للرسوم وكذلك يساعد في إحضار التقديرات المستندة إلى المشروع لبند عرض الأسعار كتفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="c4abb-132">عند عدم تعيين مشروع لبند عرض أسعار يستند إلى مشروع، يتعين إنشاء التقدير يدويًا عن طريق إنشاء كل تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="c4abb-133">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="c4abb-134">المهام المضمنة</span><span class="sxs-lookup"><span data-stu-id="c4abb-134">Included Tasks</span></span> | <span data-ttu-id="c4abb-135">يشير إلى ما إذا كان يتم استخدام بند عرض الأسعار لكافة مهام المشروع أو بعضها للمشروع المحدد.</span><span class="sxs-lookup"><span data-stu-id="c4abb-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="c4abb-136">يحتوي هذا الحقل على القيم الممكنة التالية:</span><span class="sxs-lookup"><span data-stu-id="c4abb-136">This field has the following possible values:</span></span></br><span data-ttu-id="c4abb-137">- كل مهام المشروع</span><span class="sxs-lookup"><span data-stu-id="c4abb-137">- All project tasks</span></span></br><span data-ttu-id="c4abb-138">- مهام المشروع المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="c4abb-138">- Selected project tasks only</span></span></br><span data-ttu-id="c4abb-139">القيمة الفارغة في هذا الحقل تكافئ خيار **كافة مهام المشروع**.</span><span class="sxs-lookup"><span data-stu-id="c4abb-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="c4abb-140">عند اختيار **مهام المشروع المحددة فقط**، عندئذ في صفحة المشروع، تسمح علامة التبويب **إعداد فوترة المهمة** لك بتحديد مهام معينة لإقرانها ببند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="c4abb-141">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-142">تضمين الوقت</span><span class="sxs-lookup"><span data-stu-id="c4abb-142">Include Time</span></span> | <span data-ttu-id="c4abb-143">تشير علامة **نعم**/**لا** إلى ما إذا كان حركات الوقت أو تكاليف العمالة في المشروع المحدد مضمنة في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c4abb-144">تشير علامة **لا** إلى أن حركات الوقت أو تكلفة العمالة لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c4abb-145">تشير علامة **نعم** إلى أن حركات الوقت أو تكلفة العمالة سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c4abb-146">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-147">يتضمن المصروفات</span><span class="sxs-lookup"><span data-stu-id="c4abb-147">Include Expense</span></span> | <span data-ttu-id="c4abb-148">تشير علامة **نعم**/**لا** إلى ما إذا كانت تكاليف المصروفات في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c4abb-149">تشير علامة **لا** إلى أن تكلفة المصروفات لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c4abb-150">تشير علامة **نعم** إلى أن تكلفة المصروفات سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c4abb-151">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-152">تضمين الرسوم</span><span class="sxs-lookup"><span data-stu-id="c4abb-152">Include Fee</span></span> | <span data-ttu-id="c4abb-153">تشير علامة **نعم**/**لا** إلى ما إذا كانت الرسوم في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c4abb-154">تشير علامة **لا** إلى أن الرسوم لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c4abb-155">تشير علامة **نعم** إلى أن الرسوم سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c4abb-156">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-157">المبلغ المعروض</span><span class="sxs-lookup"><span data-stu-id="c4abb-157">Quoted Amount</span></span> | <span data-ttu-id="c4abb-158">هذا هو المبلغ الذي سيتم وضعه في التسعير للعميل لكل العمل المتوقع في بند عرض الأسعار المستند إلى المشروع هذا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="c4abb-159">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل **ميزانية العميل** في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="c4abb-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="c4abb-160">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من المبلغ الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="c4abb-161">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-162">الضريبة المقدرة</span><span class="sxs-lookup"><span data-stu-id="c4abb-162">Estimated Tax</span></span> | <span data-ttu-id="c4abb-163">هذا حقل قابل للتحرير لكي يقوم المستخدم بإضافة مبلغ الضريبة المقدرة في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="c4abb-164">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من مبلغ الضريبة الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="c4abb-165">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-166">‏‫المبلغ المعروض‬ بعد الضريبة</span><span class="sxs-lookup"><span data-stu-id="c4abb-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="c4abb-167">هذا الحقل هو مبلغ بند عرض الأسعار بعد الضريبة وهو للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="c4abb-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="c4abb-168">يتم حساب المبلغ الموجود في هذا الحقل *كمبلغ معروض + الضريبة*.</span><span class="sxs-lookup"><span data-stu-id="c4abb-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="c4abb-169">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-170">حد ما يجب ألا يتم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="c4abb-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="c4abb-171">ويكون هذا الحقل قابلا للتحرير ويكون متاحا فقط في بنود عروض الأسعار المستندة إلى المشروع والتي لها أسلوب فوترة **الوقت والمادة**.</span><span class="sxs-lookup"><span data-stu-id="c4abb-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="c4abb-172">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c4abb-173">موازنة العميل</span><span class="sxs-lookup"><span data-stu-id="c4abb-173">Customer Budget</span></span> | <span data-ttu-id="c4abb-174">يكون هذا الحقل قابلا للتحرير ويتم نسخه من الحقل المقابل في بند الفرصة إذا تم إنشاء عرض الأسعار من إحدى الفرص.</span><span class="sxs-lookup"><span data-stu-id="c4abb-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="c4abb-175">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="c4abb-176">قواعد التحقق من الصحة للحقول في علامة التبويب عام لبنود عرض الأسعار المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="c4abb-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="c4abb-177">**القاعدة 1**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه على **جميع مهام المشروع**، فسيتم تضمين المشروع في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="c4abb-178">**القاعدة 2**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه إلى **كافة مهام المشروع**، فيمكن تضمين مشروع وفئة حركة معينة فقط في بند عرض أسعار واحد يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="c4abb-179">**القاعدة 3**: إذا تم تعيين حقل **المهام المضمنة** إلى **مهام المشروع المحددة فقط**، فيمكن تضمين مشروع وفئة حركة معينة فقط في عدة بنود عرض أسعار يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c4abb-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="c4abb-180">**القاعدة 4**: إذا كانت الفرصة تحتوي على عدة عروض أسعار، فيمكن أن يكون هناك بنود عرض أسعار مختلفة والتي تشير إلى نفس المشروع وتتضمن نفس فئة الحركات.</span><span class="sxs-lookup"><span data-stu-id="c4abb-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="c4abb-181">**القاعدة 5**: إذا لم تكن عروض الأسعار تنتمي إلى نفس الفرصة، فلا يمكن أن تتضمن نفس فئة المشروع والحركات.</span><span class="sxs-lookup"><span data-stu-id="c4abb-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="c4abb-182">
                    <strong>الفرصة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="c4abb-183">
                    <strong>اقتباس</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="c4abb-184">
                    <strong>بند عرض الأسعار</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="c4abb-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="c4abb-186">
                    <strong>المهام المضمنة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="c4abb-187">
                    <strong>تضمين الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="c4abb-188">
                    <strong>يتضمن المصروفات</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="c4abb-189">
                    <strong>تضمين</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="c4abb-190">
                    <strong>رسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="c4abb-191">
                    <strong>صالح/غير صالح</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="c4abb-192">
                    <strong>سبب</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c4abb-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-193">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-194">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-195">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-196">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-197">فارغ</span><span class="sxs-lookup"><span data-stu-id="c4abb-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-198">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-199">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-200">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-201">غير صالح</span><span class="sxs-lookup"><span data-stu-id="c4abb-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-202">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="c4abb-202">Violation of Rule #2.</span></span> <span data-ttu-id="c4abb-203">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في بنود عرض الأسعار QL1 و QL2.</span><span class="sxs-lookup"><span data-stu-id="c4abb-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-204">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-205">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-206">QL2</span><span class="sxs-lookup"><span data-stu-id="c4abb-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-207">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-208">فارغ</span><span class="sxs-lookup"><span data-stu-id="c4abb-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-209">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-210">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-211">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-211">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="c4abb-212">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-213">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-214">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-215">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-216">فارغ</span><span class="sxs-lookup"><span data-stu-id="c4abb-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-217">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-218">Yes</span><span class="sxs-lookup"><span data-stu-id="c4abb-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-219">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-220">غير صالح</span><span class="sxs-lookup"><span data-stu-id="c4abb-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-221">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="c4abb-221">Violation of Rule #2.</span></span> <span data-ttu-id="c4abb-222">يتم تضمين الوقت والرسوم في المشروع P1 في بنود عرض الأسعار QL1 و QL2.</span><span class="sxs-lookup"><span data-stu-id="c4abb-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-223">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-224">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-225">QL2</span><span class="sxs-lookup"><span data-stu-id="c4abb-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-226">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-227">فارغ</span><span class="sxs-lookup"><span data-stu-id="c4abb-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-228">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-229">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-230">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-230">Yes</span></span> </p>
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
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-231">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-232">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-233">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-234">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-235">فارغ</span><span class="sxs-lookup"><span data-stu-id="c4abb-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-236">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-237">Yes</span><span class="sxs-lookup"><span data-stu-id="c4abb-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-238">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-239">صالح</span><span class="sxs-lookup"><span data-stu-id="c4abb-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="c4abb-240">يتم تضمين الوقت والرسوم على المشروع P1 في QL1.</span><span class="sxs-lookup"><span data-stu-id="c4abb-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="c4abb-241">يتم تضمين المصروفات في المشروع P1 في QL2.</span><span class="sxs-lookup"><span data-stu-id="c4abb-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="c4abb-242">لا يكون هناك تداخل في ما يتم تضمينه في كل بند عرض الأسعار ويكون صالحًا.</span><span class="sxs-lookup"><span data-stu-id="c4abb-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-243">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-244">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-245">QL2</span><span class="sxs-lookup"><span data-stu-id="c4abb-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-246">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-247">فارغ</span><span class="sxs-lookup"><span data-stu-id="c4abb-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-248">Yes</span><span class="sxs-lookup"><span data-stu-id="c4abb-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-249">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-250">Yes</span><span class="sxs-lookup"><span data-stu-id="c4abb-250">No</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="c4abb-251">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-252">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-253">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-254">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-255">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="c4abb-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-256">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-257">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-258">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-259">غير صالح</span><span class="sxs-lookup"><span data-stu-id="c4abb-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-260">انتهاك القاعدة #2 السابقة</span><span class="sxs-lookup"><span data-stu-id="c4abb-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="c4abb-261">يتضمن Q1 الوقت والمصروفات والرسوم على مجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="c4abb-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="c4abb-262">يتضمن QL2 الوقت والمصروفات والرسوم للمشروع P1 بالكامل ويتداخل مع ما تم تضمينه في Q1.</span><span class="sxs-lookup"><span data-stu-id="c4abb-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-263">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-264">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-265">QL2</span><span class="sxs-lookup"><span data-stu-id="c4abb-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-266">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-267">فارغ</span><span class="sxs-lookup"><span data-stu-id="c4abb-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-268">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-269">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-270">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-270">Yes</span></span> </p>
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
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-271">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-272">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-273">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-274">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-275">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="c4abb-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-276">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-277">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-278">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-279">صالح</span><span class="sxs-lookup"><span data-stu-id="c4abb-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-280">لكل قاعدة #3 أعلاه،</span><span class="sxs-lookup"><span data-stu-id="c4abb-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="c4abb-281">يتضمن Q1 الوقت والمصروفات والرسوم على مجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="c4abb-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="c4abb-282">يتضمن QL2 الوقت والمصروفات والرسوم لمجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="c4abb-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="c4abb-283">يتعلق التحقق الإضافي الوحيد بمجموعة المهام الفرعية في QL1 والتي تختلف عن مجموعة المهام الفرعية في QL2.</span><span class="sxs-lookup"><span data-stu-id="c4abb-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="c4abb-284">وهذا يضمن عدم وجود تداخلات.</span><span class="sxs-lookup"><span data-stu-id="c4abb-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="c4abb-285">يتم ذلك بواسطة النظام عند اقتران المهام.</span><span class="sxs-lookup"><span data-stu-id="c4abb-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-286">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-287">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-288">QL2</span><span class="sxs-lookup"><span data-stu-id="c4abb-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-289">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-290">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="c4abb-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-291">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-292">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-293">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-293">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="c4abb-294">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-295">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-296">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-297">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-298">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="c4abb-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-299">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-300">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-301">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="c4abb-302">صالح</span><span class="sxs-lookup"><span data-stu-id="c4abb-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-303">بناء على القاعد #5، فإن Q1 و Q2 يمثلان عرضا أسعار في نفس الفرصة، لذا يمكنهم التقدير لنفس المكونات الخاصة بأحد المشروعات.</span><span class="sxs-lookup"><span data-stu-id="c4abb-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-304">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-305">ربع السنة الثاني</span><span class="sxs-lookup"><span data-stu-id="c4abb-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-306">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-307">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-308">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="c4abb-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-309">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-310">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-311">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-311">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="c4abb-312">O1</span><span class="sxs-lookup"><span data-stu-id="c4abb-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-313">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-314">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-315">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-316">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="c4abb-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-317">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-318">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-319">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="c4abb-320">صالح</span><span class="sxs-lookup"><span data-stu-id="c4abb-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c4abb-321">بناء على القاعد #4، فإن Q1 و Q2 يمثلان عرضا أسعار لفرص مختلفة، لذا لا يمكنهم التقدير لنفس المكونات الخاصة بنفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="c4abb-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="c4abb-322">O2</span><span class="sxs-lookup"><span data-stu-id="c4abb-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c4abb-323">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c4abb-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-324">QL1</span><span class="sxs-lookup"><span data-stu-id="c4abb-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-325">P1</span><span class="sxs-lookup"><span data-stu-id="c4abb-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="c4abb-326">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="c4abb-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-327">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="c4abb-328">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="c4abb-329">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="c4abb-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="c4abb-330">غير صالح</span><span class="sxs-lookup"><span data-stu-id="c4abb-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]