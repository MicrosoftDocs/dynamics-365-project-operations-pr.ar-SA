---
title: بنود عروض الأسعار المستندة إلى المشروع (احترافي)
description: يقدم هذا الموضوع معلومات حول استخدام بنود عروض الأسعار المستندة إلى المشروع لعمل المشروع. (احترافي)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907815"
---
# <a name="project-based-quote-lines-pro"></a><span data-ttu-id="59046-104">بنود عروض الأسعار المستندة إلى المشروع (احترافي)</span><span class="sxs-lookup"><span data-stu-id="59046-104">Project-based quote lines (Pro)</span></span>

<span data-ttu-id="59046-105">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="59046-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="59046-106">تم تصميم بنود عرض الأسعار المستندة إلى المشروع للمساعدة في تقدير عمل المشروع بأحد المشاركات.</span><span class="sxs-lookup"><span data-stu-id="59046-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="59046-107">يتم توسيع بنية سطر عرض الأسعار المستند إلى المشروع لتقديرات المشروع بالمفاهيم التالية:</span><span class="sxs-lookup"><span data-stu-id="59046-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="59046-108">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="59046-108">Billing Method</span></span>
- <span data-ttu-id="59046-109">تعيين المشروع والمهمة</span><span class="sxs-lookup"><span data-stu-id="59046-109">Project and Task Mapping</span></span>
- <span data-ttu-id="59046-110">فئات الحركات المضمنة</span><span class="sxs-lookup"><span data-stu-id="59046-110">Included Transaction classes</span></span>
- <span data-ttu-id="59046-111">حد يجب عدم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="59046-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="59046-112">إعداد الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="59046-112">Chargeability setup</span></span>
- <span data-ttu-id="59046-113">التقدير باستخدام تفاصيل بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="59046-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="59046-114">عملاء بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="59046-114">Quote line Customers</span></span>

<span data-ttu-id="59046-115">يوفر الجدول التالي معلومات حول الحقول الموجودة في علامة التبويب **عام** في بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="59046-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="59046-116">وتساعد هذه الحقول في إعداد الأساس لتقدير تفصيلي من القاعدة إلى القمة لعمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="59046-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="59046-117">**الحقل**</span><span class="sxs-lookup"><span data-stu-id="59046-117">**Field**</span></span> | <span data-ttu-id="59046-118">**الصلة والغرض والإرشاد**</span><span class="sxs-lookup"><span data-stu-id="59046-118">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="59046-119">**تأثير لاحق**</span><span class="sxs-lookup"><span data-stu-id="59046-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="59046-120">اسم</span><span class="sxs-lookup"><span data-stu-id="59046-120">Name</span></span> | <span data-ttu-id="59046-121">اسم بند عرض الأسعار الذي ينبغي أن يساعدك في تحديد المكون المنفصل لعرض الأسعار الذي يتم تقديره.</span><span class="sxs-lookup"><span data-stu-id="59046-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="59046-122">يتم نسخه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-123">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="59046-123">Billing Method</span></span> | <span data-ttu-id="59046-124">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل المقابل في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="59046-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="59046-125">يتضمن هذا الحقل اثنين من نماذج التعاقد الرئيسية المدعومة من Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="59046-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="59046-126">- سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="59046-126">- Fixed price</span></span></br><span data-ttu-id="59046-127">- الوقت والمادة.</span><span class="sxs-lookup"><span data-stu-id="59046-127">- Time and material.</span></span>| <span data-ttu-id="59046-128">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-129">Project</span><span class="sxs-lookup"><span data-stu-id="59046-129">Project</span></span> | <span data-ttu-id="59046-130">استخدم هذا الحقل الاختياري لتحديد المشروع الذي سيتم استخدامه لتسليم العمل في هذه المشاركة.</span><span class="sxs-lookup"><span data-stu-id="59046-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="59046-131">عندما يتم تعيين مشروع إلى بند عرض الأسعار، فإنه يساعد في إعداد المهام الخاضعة للرسوم وكذلك يساعد في إحضار التقديرات المستندة إلى المشروع لبند عرض الأسعار كتفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="59046-132">عند عدم تعيين مشروع لبند عرض أسعار يستند إلى مشروع، يتعين إنشاء التقدير يدويًا عن طريق إنشاء كل تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="59046-133">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="59046-134">المهام المضمنة</span><span class="sxs-lookup"><span data-stu-id="59046-134">Included Tasks</span></span> | <span data-ttu-id="59046-135">يشير إلى ما إذا كان يتم استخدام بند عرض الأسعار لكافة مهام المشروع أو بعضها للمشروع المحدد.</span><span class="sxs-lookup"><span data-stu-id="59046-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="59046-136">يحتوي هذا الحقل على القيم الممكنة التالية:</span><span class="sxs-lookup"><span data-stu-id="59046-136">This field has the following possible values:</span></span></br><span data-ttu-id="59046-137">- كل مهام المشروع</span><span class="sxs-lookup"><span data-stu-id="59046-137">- All project tasks</span></span></br><span data-ttu-id="59046-138">- مهام المشروع المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="59046-138">- Selected project tasks only</span></span></br><span data-ttu-id="59046-139">القيمة الفارغة في هذا الحقل تكافئ خيار **كافة مهام المشروع**.</span><span class="sxs-lookup"><span data-stu-id="59046-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="59046-140">عند اختيار **مهام المشروع المحددة فقط**، عندئذ في صفحة المشروع، تسمح علامة التبويب **إعداد فوترة المهمة** لك بتحديد مهام معينة لإقرانها ببند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="59046-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="59046-141">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-142">تضمين الوقت</span><span class="sxs-lookup"><span data-stu-id="59046-142">Include Time</span></span> | <span data-ttu-id="59046-143">تشير علامة **نعم**/**لا** إلى ما إذا كان حركات الوقت أو تكاليف العمالة في المشروع المحدد مضمنة في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="59046-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="59046-144">تشير علامة **لا** إلى أن حركات الوقت أو تكلفة العمالة لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="59046-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="59046-145">تشير علامة **نعم** إلى أن حركات الوقت أو تكلفة العمالة سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="59046-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="59046-146">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-147">يتضمن المصروفات</span><span class="sxs-lookup"><span data-stu-id="59046-147">Include Expense</span></span> | <span data-ttu-id="59046-148">تشير علامة **نعم**/**لا** إلى ما إذا كانت تكاليف المصروفات في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="59046-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="59046-149">تشير علامة **لا** إلى أن تكلفة المصروفات لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="59046-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="59046-150">تشير علامة **نعم** إلى أن تكلفة المصروفات سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="59046-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="59046-151">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-152">تضمين الرسوم</span><span class="sxs-lookup"><span data-stu-id="59046-152">Include Fee</span></span> | <span data-ttu-id="59046-153">تشير علامة **نعم**/**لا** إلى ما إذا كانت الرسوم في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="59046-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="59046-154">تشير علامة **لا** إلى أن الرسوم لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="59046-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="59046-155">تشير علامة **نعم** إلى أن الرسوم سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="59046-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="59046-156">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-157">المبلغ المعروض</span><span class="sxs-lookup"><span data-stu-id="59046-157">Quoted Amount</span></span> | <span data-ttu-id="59046-158">هذا هو المبلغ الذي سيتم وضعه في التسعير للعميل لكل العمل المتوقع في بند عرض الأسعار المستند إلى المشروع هذا.</span><span class="sxs-lookup"><span data-stu-id="59046-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="59046-159">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل **ميزانية العميل** في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="59046-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="59046-160">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من المبلغ الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="59046-161">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-162">الضريبة المقدرة</span><span class="sxs-lookup"><span data-stu-id="59046-162">Estimated Tax</span></span> | <span data-ttu-id="59046-163">هذا حقل قابل للتحرير لكي يقوم المستخدم بإضافة مبلغ الضريبة المقدرة في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="59046-164">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من مبلغ الضريبة الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="59046-165">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-166">‏‫المبلغ المعروض‬ بعد الضريبة</span><span class="sxs-lookup"><span data-stu-id="59046-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="59046-167">هذا الحقل هو مبلغ بند عرض الأسعار بعد الضريبة وهو للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="59046-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="59046-168">يتم حساب المبلغ الموجود في هذا الحقل *كمبلغ معروض + الضريبة*.</span><span class="sxs-lookup"><span data-stu-id="59046-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="59046-169">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-170">حد ما يجب ألا يتم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="59046-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="59046-171">ويكون هذا الحقل قابلا للتحرير ويكون متاحا فقط في بنود عروض الأسعار المستندة إلى المشروع والتي لها أسلوب فوترة **الوقت والمادة**.</span><span class="sxs-lookup"><span data-stu-id="59046-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="59046-172">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="59046-173">موازنة العميل</span><span class="sxs-lookup"><span data-stu-id="59046-173">Customer Budget</span></span> | <span data-ttu-id="59046-174">يكون هذا الحقل قابلا للتحرير ويتم نسخه من الحقل المقابل في بند الفرصة إذا تم إنشاء عرض الأسعار من إحدى الفرص.</span><span class="sxs-lookup"><span data-stu-id="59046-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="59046-175">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="59046-176">قواعد التحقق من الصحة للحقول في علامة التبويب عام لبنود عرض الأسعار المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="59046-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="59046-177">**القاعدة 1**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه على **جميع مهام المشروع**، فسيتم تضمين المشروع في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="59046-178">**القاعدة 2**: إذا كان حقل **المهام المضمنة**فارغًا، أو إذا تم تعيينه إلى **كافة مهام المشروع**، فيمكن تضمين مشروع وفئة حركة معينة فقط في بند عرض أسعار واحد يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="59046-179">**القاعدة 3**: إذا تم تعيين حقل **المهام المضمنة** إلى **مهام المشروع المحددة فقط**، فيمكن تضمين مشروع وفئة حركة معينة فقط في عدة بنود عرض أسعار يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="59046-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="59046-180">**القاعدة 4**: إذا كانت الفرصة تحتوي على عدة عروض أسعار، فيمكن أن يكون هناك بنود عرض أسعار مختلفة والتي تشير إلى نفس المشروع وتتضمن نفس فئة الحركات.</span><span class="sxs-lookup"><span data-stu-id="59046-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="59046-181">**القاعدة 5**: إذا لم تكن عروض الأسعار تنتمي إلى نفس الفرصة، فلا يمكن أن تتضمن نفس فئة المشروع والحركات.</span><span class="sxs-lookup"><span data-stu-id="59046-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="59046-182">
                    <strong>الفرصة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="59046-183">
                    <strong>اقتباس</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="59046-184">
                    <strong>بند عرض الأسعار</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="59046-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="59046-186">
                    <strong>المهام المضمنة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="59046-187">
                    <strong>تضمين الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="59046-188">
                    <strong>يتضمن المصروفات</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="59046-189">
                    <strong>تضمين</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="59046-190">
                    <strong>رسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="59046-191">
                    <strong>صالح/غير صالح</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="59046-192">
                    <strong>سبب</strong>
                </span><span class="sxs-lookup"><span data-stu-id="59046-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="59046-193">O1</span><span class="sxs-lookup"><span data-stu-id="59046-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-194">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-195">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-196">P1</span><span class="sxs-lookup"><span data-stu-id="59046-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-197">فارغ</span><span class="sxs-lookup"><span data-stu-id="59046-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-198">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-199">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-200">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-201">غير صالح</span><span class="sxs-lookup"><span data-stu-id="59046-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-202">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="59046-202">Violation of Rule #2.</span></span> <span data-ttu-id="59046-203">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في بنود عرض الأسعار QL1 و QL2.</span><span class="sxs-lookup"><span data-stu-id="59046-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="59046-204">O1</span><span class="sxs-lookup"><span data-stu-id="59046-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-205">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-206">QL2</span><span class="sxs-lookup"><span data-stu-id="59046-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-207">P1</span><span class="sxs-lookup"><span data-stu-id="59046-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-208">فارغ</span><span class="sxs-lookup"><span data-stu-id="59046-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-209">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-210">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-211">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-211">Yes</span></span> </p>
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
<span data-ttu-id="59046-212">O1</span><span class="sxs-lookup"><span data-stu-id="59046-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-213">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-214">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-215">P1</span><span class="sxs-lookup"><span data-stu-id="59046-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-216">فارغ</span><span class="sxs-lookup"><span data-stu-id="59046-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-217">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-218">Yes</span><span class="sxs-lookup"><span data-stu-id="59046-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-219">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-220">غير صالح</span><span class="sxs-lookup"><span data-stu-id="59046-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-221">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="59046-221">Violation of Rule #2.</span></span> <span data-ttu-id="59046-222">يتم تضمين الوقت والرسوم في المشروع P1 في بنود عرض الأسعار QL1 و QL2.</span><span class="sxs-lookup"><span data-stu-id="59046-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="59046-223">O1</span><span class="sxs-lookup"><span data-stu-id="59046-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-224">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-225">QL2</span><span class="sxs-lookup"><span data-stu-id="59046-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-226">P1</span><span class="sxs-lookup"><span data-stu-id="59046-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-227">فارغ</span><span class="sxs-lookup"><span data-stu-id="59046-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-228">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-229">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-230">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-230">Yes</span></span> </p>
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
<span data-ttu-id="59046-231">O1</span><span class="sxs-lookup"><span data-stu-id="59046-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-232">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-233">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-234">P1</span><span class="sxs-lookup"><span data-stu-id="59046-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-235">فارغ</span><span class="sxs-lookup"><span data-stu-id="59046-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-236">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-237">Yes</span><span class="sxs-lookup"><span data-stu-id="59046-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-238">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-239">صالح</span><span class="sxs-lookup"><span data-stu-id="59046-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="59046-240">يتم تضمين الوقت والرسوم على المشروع P1 في QL1.</span><span class="sxs-lookup"><span data-stu-id="59046-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="59046-241">يتم تضمين المصروفات في المشروع P1 في QL2.</span><span class="sxs-lookup"><span data-stu-id="59046-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="59046-242">لا يكون هناك تداخل في ما يتم تضمينه في كل بند عرض الأسعار ويكون صالحًا.</span><span class="sxs-lookup"><span data-stu-id="59046-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="59046-243">O1</span><span class="sxs-lookup"><span data-stu-id="59046-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-244">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-245">QL2</span><span class="sxs-lookup"><span data-stu-id="59046-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-246">P1</span><span class="sxs-lookup"><span data-stu-id="59046-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-247">فارغ</span><span class="sxs-lookup"><span data-stu-id="59046-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-248">Yes</span><span class="sxs-lookup"><span data-stu-id="59046-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-249">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-250">Yes</span><span class="sxs-lookup"><span data-stu-id="59046-250">No</span></span> </p>
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
<span data-ttu-id="59046-251">O1</span><span class="sxs-lookup"><span data-stu-id="59046-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-252">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-253">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-254">P1</span><span class="sxs-lookup"><span data-stu-id="59046-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-255">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="59046-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-256">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-257">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-258">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-259">غير صالح</span><span class="sxs-lookup"><span data-stu-id="59046-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-260">انتهاك القاعدة #2 السابقة</span><span class="sxs-lookup"><span data-stu-id="59046-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="59046-261">يتضمن Q1 الوقت والمصروفات والرسوم على مجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="59046-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="59046-262">يتضمن QL2 الوقت والمصروفات والرسوم للمشروع P1 بالكامل ويتداخل مع ما تم تضمينه في Q1.</span><span class="sxs-lookup"><span data-stu-id="59046-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="59046-263">O1</span><span class="sxs-lookup"><span data-stu-id="59046-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-264">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-265">QL2</span><span class="sxs-lookup"><span data-stu-id="59046-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-266">P1</span><span class="sxs-lookup"><span data-stu-id="59046-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-267">فارغ</span><span class="sxs-lookup"><span data-stu-id="59046-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-268">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-269">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-270">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-270">Yes</span></span> </p>
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
<span data-ttu-id="59046-271">O1</span><span class="sxs-lookup"><span data-stu-id="59046-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-272">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-273">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-274">P1</span><span class="sxs-lookup"><span data-stu-id="59046-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-275">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="59046-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-276">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-277">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-278">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-279">صالح</span><span class="sxs-lookup"><span data-stu-id="59046-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-280">لكل قاعدة #3 أعلاه،</span><span class="sxs-lookup"><span data-stu-id="59046-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="59046-281">يتضمن Q1 الوقت والمصروفات والرسوم على مجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="59046-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="59046-282">يتضمن QL2 الوقت والمصروفات والرسوم لمجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="59046-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="59046-283">يتعلق التحقق الإضافي الوحيد بمجموعة المهام الفرعية في QL1 والتي تختلف عن مجموعة المهام الفرعية في QL2.</span><span class="sxs-lookup"><span data-stu-id="59046-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="59046-284">وهذا يضمن عدم وجود تداخلات.</span><span class="sxs-lookup"><span data-stu-id="59046-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="59046-285">يتم ذلك بواسطة النظام عند اقتران المهام.</span><span class="sxs-lookup"><span data-stu-id="59046-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="59046-286">O1</span><span class="sxs-lookup"><span data-stu-id="59046-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-287">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-288">QL2</span><span class="sxs-lookup"><span data-stu-id="59046-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-289">P1</span><span class="sxs-lookup"><span data-stu-id="59046-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-290">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="59046-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-291">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-292">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-293">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-293">Yes</span></span> </p>
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
<span data-ttu-id="59046-294">O1</span><span class="sxs-lookup"><span data-stu-id="59046-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-295">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-296">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-297">P1</span><span class="sxs-lookup"><span data-stu-id="59046-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-298">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="59046-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-299">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-300">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-301">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="59046-302">صالح</span><span class="sxs-lookup"><span data-stu-id="59046-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-303">بناء على القاعد #5، فإن Q1 و Q2 يمثلان عرضا أسعار في نفس الفرصة، لذا يمكنهم التقدير لنفس المكونات الخاصة بأحد المشروعات.</span><span class="sxs-lookup"><span data-stu-id="59046-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="59046-304">O1</span><span class="sxs-lookup"><span data-stu-id="59046-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-305">ربع السنة الثاني</span><span class="sxs-lookup"><span data-stu-id="59046-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-306">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-307">P1</span><span class="sxs-lookup"><span data-stu-id="59046-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-308">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="59046-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-309">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-310">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-311">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-311">Yes</span></span> </p>
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
<span data-ttu-id="59046-312">O1</span><span class="sxs-lookup"><span data-stu-id="59046-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-313">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-314">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-315">P1</span><span class="sxs-lookup"><span data-stu-id="59046-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-316">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="59046-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-317">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-318">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-319">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="59046-320">صالح</span><span class="sxs-lookup"><span data-stu-id="59046-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="59046-321">بناء على القاعد #4، فإن Q1 و Q2 يمثلان عرضا أسعار لفرص مختلفة، لذا لا يمكنهم التقدير لنفس المكونات الخاصة بنفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="59046-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="59046-322">O2</span><span class="sxs-lookup"><span data-stu-id="59046-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="59046-323">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="59046-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-324">QL1</span><span class="sxs-lookup"><span data-stu-id="59046-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-325">P1</span><span class="sxs-lookup"><span data-stu-id="59046-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="59046-326">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="59046-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-327">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="59046-328">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="59046-329">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="59046-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="59046-330">غير صالح</span><span class="sxs-lookup"><span data-stu-id="59046-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

