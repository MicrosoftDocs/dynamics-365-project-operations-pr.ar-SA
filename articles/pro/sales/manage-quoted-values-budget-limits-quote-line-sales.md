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
ms.openlocfilehash: be1663c0d226fa19fe4b9df566e16d215f1fc08e
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181076"
---
# <a name="project-based-quote-lines-overview---lite"></a><span data-ttu-id="74480-104">نظرة عامة على بنود عرض الأسعار القائم على المشروع - خفيف</span><span class="sxs-lookup"><span data-stu-id="74480-104">Project-based quote lines overview - lite</span></span>

<span data-ttu-id="74480-105">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="74480-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="74480-106">تم تصميم بنود عرض الأسعار المستندة إلى المشروع للمساعدة في تقدير عمل المشروع بأحد المشاركات.</span><span class="sxs-lookup"><span data-stu-id="74480-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="74480-107">يتم توسيع بنية سطر عرض الأسعار المستند إلى المشروع لتقديرات المشروع بالمفاهيم التالية:</span><span class="sxs-lookup"><span data-stu-id="74480-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="74480-108">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="74480-108">Billing Method</span></span>
- <span data-ttu-id="74480-109">تعيين المشروع والمهمة</span><span class="sxs-lookup"><span data-stu-id="74480-109">Project and Task Mapping</span></span>
- <span data-ttu-id="74480-110">فئات الحركات المضمنة</span><span class="sxs-lookup"><span data-stu-id="74480-110">Included Transaction classes</span></span>
- <span data-ttu-id="74480-111">حد يجب عدم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="74480-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="74480-112">إعداد الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="74480-112">Chargeability setup</span></span>
- <span data-ttu-id="74480-113">التقدير باستخدام تفاصيل بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="74480-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="74480-114">عملاء بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="74480-114">Quote line Customers</span></span>

<span data-ttu-id="74480-115">يوفر الجدول التالي معلومات حول الحقول الموجودة في علامة التبويب **عام** في بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="74480-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="74480-116">وتساعد هذه الحقول في إعداد الأساس لتقدير تفصيلي من القاعدة إلى القمة لعمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="74480-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="74480-117">**الحقل**</span><span class="sxs-lookup"><span data-stu-id="74480-117">**Field**</span></span> | <span data-ttu-id="74480-118">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="74480-118">**Description**</span></span> | <span data-ttu-id="74480-119">**تأثير لاحق**</span><span class="sxs-lookup"><span data-stu-id="74480-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="74480-120">اسم</span><span class="sxs-lookup"><span data-stu-id="74480-120">Name</span></span> | <span data-ttu-id="74480-121">اسم بند عرض الأسعار الذي ينبغي أن يساعدك في تحديد المكون المنفصل لعرض الأسعار الذي يتم تقديره.</span><span class="sxs-lookup"><span data-stu-id="74480-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="74480-122">يتم نسخه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-123">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="74480-123">Billing Method</span></span> | <span data-ttu-id="74480-124">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل المقابل في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="74480-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="74480-125">يتضمن هذا الحقل اثنين من نماذج التعاقد الرئيسية المدعومة من Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="74480-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="74480-126">- سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="74480-126">- Fixed price</span></span></br><span data-ttu-id="74480-127">- الوقت والمادة.</span><span class="sxs-lookup"><span data-stu-id="74480-127">- Time and material.</span></span>| <span data-ttu-id="74480-128">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-129">Project</span><span class="sxs-lookup"><span data-stu-id="74480-129">Project</span></span> | <span data-ttu-id="74480-130">استخدم هذا الحقل الاختياري لتحديد المشروع الذي سيتم استخدامه لتسليم العمل في هذه المشاركة.</span><span class="sxs-lookup"><span data-stu-id="74480-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="74480-131">عندما يتم تعيين مشروع إلى بند عرض الأسعار، فإنه يساعد في إعداد المهام الخاضعة للرسوم وكذلك يساعد في إحضار التقديرات المستندة إلى المشروع لبند عرض الأسعار كتفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="74480-132">عند عدم تعيين مشروع لبند عرض أسعار يستند إلى مشروع، يتعين إنشاء التقدير يدويًا عن طريق إنشاء كل تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="74480-133">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="74480-134">المهام المضمنة</span><span class="sxs-lookup"><span data-stu-id="74480-134">Included Tasks</span></span> | <span data-ttu-id="74480-135">يشير إلى ما إذا كان يتم استخدام بند عرض الأسعار لكافة مهام المشروع أو بعضها للمشروع المحدد.</span><span class="sxs-lookup"><span data-stu-id="74480-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="74480-136">يحتوي هذا الحقل على القيم الممكنة التالية:</span><span class="sxs-lookup"><span data-stu-id="74480-136">This field has the following possible values:</span></span></br><span data-ttu-id="74480-137">- كل مهام المشروع</span><span class="sxs-lookup"><span data-stu-id="74480-137">- All project tasks</span></span></br><span data-ttu-id="74480-138">- مهام المشروع المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="74480-138">- Selected project tasks only</span></span></br><span data-ttu-id="74480-139">القيمة الفارغة في هذا الحقل تكافئ خيار **كافة مهام المشروع**.</span><span class="sxs-lookup"><span data-stu-id="74480-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="74480-140">عند اختيار **مهام المشروع المحددة فقط**، عندئذ في صفحة المشروع، تسمح علامة التبويب **إعداد فوترة المهمة** لك بتحديد مهام معينة لإقرانها ببند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="74480-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="74480-141">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-142">تضمين الوقت</span><span class="sxs-lookup"><span data-stu-id="74480-142">Include Time</span></span> | <span data-ttu-id="74480-143">تشير علامة **نعم**/**لا** إلى ما إذا كان حركات الوقت أو تكاليف العمالة في المشروع المحدد مضمنة في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="74480-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="74480-144">تشير علامة **لا** إلى أن حركات الوقت أو تكلفة العمالة لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="74480-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="74480-145">تشير علامة **نعم** إلى أن حركات الوقت أو تكلفة العمالة سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="74480-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="74480-146">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-147">يتضمن المصروفات</span><span class="sxs-lookup"><span data-stu-id="74480-147">Include Expense</span></span> | <span data-ttu-id="74480-148">تشير علامة **نعم**/**لا** إلى ما إذا كانت تكاليف المصروفات في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="74480-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="74480-149">تشير علامة **لا** إلى أن تكلفة المصروفات لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="74480-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="74480-150">تشير علامة **نعم** إلى أن تكلفة المصروفات سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="74480-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="74480-151">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-152">تضمين الرسوم</span><span class="sxs-lookup"><span data-stu-id="74480-152">Include Fee</span></span> | <span data-ttu-id="74480-153">تشير علامة **نعم**/**لا** إلى ما إذا كانت الرسوم في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا.</span><span class="sxs-lookup"><span data-stu-id="74480-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="74480-154">تشير علامة **لا** إلى أن الرسوم لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="74480-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="74480-155">تشير علامة **نعم** إلى أن الرسوم سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="74480-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="74480-156">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-157">المبلغ المعروض</span><span class="sxs-lookup"><span data-stu-id="74480-157">Quoted Amount</span></span> | <span data-ttu-id="74480-158">هذا هو المبلغ الذي سيتم وضعه في التسعير للعميل لكل العمل المتوقع في بند عرض الأسعار المستند إلى المشروع هذا.</span><span class="sxs-lookup"><span data-stu-id="74480-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="74480-159">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل **ميزانية العميل** في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="74480-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="74480-160">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من المبلغ الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="74480-161">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-162">الضريبة المقدرة</span><span class="sxs-lookup"><span data-stu-id="74480-162">Estimated Tax</span></span> | <span data-ttu-id="74480-163">هذا حقل قابل للتحرير لكي يقوم المستخدم بإضافة مبلغ الضريبة المقدرة في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="74480-164">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من مبلغ الضريبة الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="74480-165">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-166">‏‫المبلغ المعروض‬ بعد الضريبة</span><span class="sxs-lookup"><span data-stu-id="74480-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="74480-167">هذا الحقل هو مبلغ بند عرض الأسعار بعد الضريبة وهو للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="74480-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="74480-168">يتم حساب المبلغ الموجود في هذا الحقل *كمبلغ معروض + الضريبة*.</span><span class="sxs-lookup"><span data-stu-id="74480-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="74480-169">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-170">حد ما يجب ألا يتم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="74480-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="74480-171">ويكون هذا الحقل قابلا للتحرير ويكون متاحا فقط في بنود عروض الأسعار المستندة إلى المشروع والتي لها أسلوب فوترة **الوقت والمادة**.</span><span class="sxs-lookup"><span data-stu-id="74480-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="74480-172">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="74480-173">موازنة العميل</span><span class="sxs-lookup"><span data-stu-id="74480-173">Customer Budget</span></span> | <span data-ttu-id="74480-174">يكون هذا الحقل قابلا للتحرير ويتم نسخه من الحقل المقابل في بند الفرصة إذا تم إنشاء عرض الأسعار من إحدى الفرص.</span><span class="sxs-lookup"><span data-stu-id="74480-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="74480-175">يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="74480-176">قواعد التحقق من الصحة للحقول في علامة التبويب عام لبنود عرض الأسعار المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="74480-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="74480-177">**القاعدة 1**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه على **جميع مهام المشروع**، فسيتم تضمين المشروع في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="74480-178">**القاعدة 2**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه إلى **كافة مهام المشروع**، فيمكن تضمين مشروع وفئة حركة معينة فقط في بند عرض أسعار واحد يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="74480-179">**القاعدة 3**: إذا تم تعيين حقل **المهام المضمنة** إلى **مهام المشروع المحددة فقط**، فيمكن تضمين مشروع وفئة حركة معينة فقط في عدة بنود عرض أسعار يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="74480-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="74480-180">**القاعدة 4**: إذا كانت الفرصة تحتوي على عدة عروض أسعار، فيمكن أن يكون هناك بنود عرض أسعار مختلفة والتي تشير إلى نفس المشروع وتتضمن نفس فئة الحركات.</span><span class="sxs-lookup"><span data-stu-id="74480-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="74480-181">**القاعدة 5**: إذا لم تكن عروض الأسعار تنتمي إلى نفس الفرصة، فلا يمكن أن تتضمن نفس فئة المشروع والحركات.</span><span class="sxs-lookup"><span data-stu-id="74480-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="74480-182">
                    <strong>الفرصة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="74480-183">
                    <strong>اقتباس</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="74480-184">
                    <strong>بند عرض الأسعار</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="74480-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="74480-186">
                    <strong>المهام المضمنة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="74480-187">
                    <strong>تضمين الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="74480-188">
                    <strong>يتضمن المصروفات</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="74480-189">
                    <strong>تضمين</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="74480-190">
                    <strong>رسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="74480-191">
                    <strong>صالح/غير صالح</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="74480-192">
                    <strong>سبب</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74480-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="74480-193">O1</span><span class="sxs-lookup"><span data-stu-id="74480-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-194">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-195">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-196">P1</span><span class="sxs-lookup"><span data-stu-id="74480-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-197">فارغ</span><span class="sxs-lookup"><span data-stu-id="74480-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-198">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-199">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-200">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-201">غير صالح</span><span class="sxs-lookup"><span data-stu-id="74480-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-202">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="74480-202">Violation of Rule #2.</span></span> <span data-ttu-id="74480-203">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في بنود عرض الأسعار QL1 و QL2.</span><span class="sxs-lookup"><span data-stu-id="74480-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="74480-204">O1</span><span class="sxs-lookup"><span data-stu-id="74480-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-205">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-206">QL2</span><span class="sxs-lookup"><span data-stu-id="74480-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-207">P1</span><span class="sxs-lookup"><span data-stu-id="74480-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-208">فارغ</span><span class="sxs-lookup"><span data-stu-id="74480-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-209">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-210">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-211">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-211">Yes</span></span> </p>
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
<span data-ttu-id="74480-212">O1</span><span class="sxs-lookup"><span data-stu-id="74480-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-213">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-214">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-215">P1</span><span class="sxs-lookup"><span data-stu-id="74480-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-216">فارغ</span><span class="sxs-lookup"><span data-stu-id="74480-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-217">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-218">Yes</span><span class="sxs-lookup"><span data-stu-id="74480-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-219">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-220">غير صالح</span><span class="sxs-lookup"><span data-stu-id="74480-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-221">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="74480-221">Violation of Rule #2.</span></span> <span data-ttu-id="74480-222">يتم تضمين الوقت والرسوم في المشروع P1 في بنود عرض الأسعار QL1 و QL2.</span><span class="sxs-lookup"><span data-stu-id="74480-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="74480-223">O1</span><span class="sxs-lookup"><span data-stu-id="74480-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-224">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-225">QL2</span><span class="sxs-lookup"><span data-stu-id="74480-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-226">P1</span><span class="sxs-lookup"><span data-stu-id="74480-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-227">فارغ</span><span class="sxs-lookup"><span data-stu-id="74480-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-228">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-229">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-230">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-230">Yes</span></span> </p>
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
<span data-ttu-id="74480-231">O1</span><span class="sxs-lookup"><span data-stu-id="74480-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-232">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-233">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-234">P1</span><span class="sxs-lookup"><span data-stu-id="74480-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-235">فارغ</span><span class="sxs-lookup"><span data-stu-id="74480-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-236">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-237">Yes</span><span class="sxs-lookup"><span data-stu-id="74480-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-238">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-239">صالح</span><span class="sxs-lookup"><span data-stu-id="74480-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="74480-240">يتم تضمين الوقت والرسوم على المشروع P1 في QL1.</span><span class="sxs-lookup"><span data-stu-id="74480-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="74480-241">يتم تضمين المصروفات في المشروع P1 في QL2.</span><span class="sxs-lookup"><span data-stu-id="74480-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="74480-242">لا يكون هناك تداخل في ما يتم تضمينه في كل بند عرض الأسعار ويكون صالحًا.</span><span class="sxs-lookup"><span data-stu-id="74480-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="74480-243">O1</span><span class="sxs-lookup"><span data-stu-id="74480-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-244">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-245">QL2</span><span class="sxs-lookup"><span data-stu-id="74480-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-246">P1</span><span class="sxs-lookup"><span data-stu-id="74480-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-247">فارغ</span><span class="sxs-lookup"><span data-stu-id="74480-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-248">Yes</span><span class="sxs-lookup"><span data-stu-id="74480-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-249">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-250">Yes</span><span class="sxs-lookup"><span data-stu-id="74480-250">No</span></span> </p>
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
<span data-ttu-id="74480-251">O1</span><span class="sxs-lookup"><span data-stu-id="74480-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-252">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-253">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-254">P1</span><span class="sxs-lookup"><span data-stu-id="74480-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-255">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="74480-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-256">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-257">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-258">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-259">غير صالح</span><span class="sxs-lookup"><span data-stu-id="74480-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-260">انتهاك القاعدة #2 السابقة</span><span class="sxs-lookup"><span data-stu-id="74480-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="74480-261">يتضمن Q1 الوقت والمصروفات والرسوم على مجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="74480-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="74480-262">يتضمن QL2 الوقت والمصروفات والرسوم للمشروع P1 بالكامل ويتداخل مع ما تم تضمينه في Q1.</span><span class="sxs-lookup"><span data-stu-id="74480-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="74480-263">O1</span><span class="sxs-lookup"><span data-stu-id="74480-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-264">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-265">QL2</span><span class="sxs-lookup"><span data-stu-id="74480-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-266">P1</span><span class="sxs-lookup"><span data-stu-id="74480-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-267">فارغ</span><span class="sxs-lookup"><span data-stu-id="74480-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-268">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-269">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-270">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-270">Yes</span></span> </p>
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
<span data-ttu-id="74480-271">O1</span><span class="sxs-lookup"><span data-stu-id="74480-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-272">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-273">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-274">P1</span><span class="sxs-lookup"><span data-stu-id="74480-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-275">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="74480-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-276">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-277">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-278">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-279">صالح</span><span class="sxs-lookup"><span data-stu-id="74480-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-280">لكل قاعدة #3 أعلاه،</span><span class="sxs-lookup"><span data-stu-id="74480-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="74480-281">يتضمن Q1 الوقت والمصروفات والرسوم على مجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="74480-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="74480-282">يتضمن QL2 الوقت والمصروفات والرسوم لمجموعة فرعية من المهام في مشروع P1.</span><span class="sxs-lookup"><span data-stu-id="74480-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="74480-283">يتعلق التحقق الإضافي الوحيد بمجموعة المهام الفرعية في QL1 والتي تختلف عن مجموعة المهام الفرعية في QL2.</span><span class="sxs-lookup"><span data-stu-id="74480-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="74480-284">وهذا يضمن عدم وجود تداخلات.</span><span class="sxs-lookup"><span data-stu-id="74480-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="74480-285">يتم ذلك بواسطة النظام عند اقتران المهام.</span><span class="sxs-lookup"><span data-stu-id="74480-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="74480-286">O1</span><span class="sxs-lookup"><span data-stu-id="74480-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-287">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-288">QL2</span><span class="sxs-lookup"><span data-stu-id="74480-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-289">P1</span><span class="sxs-lookup"><span data-stu-id="74480-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-290">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="74480-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-291">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-292">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-293">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-293">Yes</span></span> </p>
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
<span data-ttu-id="74480-294">O1</span><span class="sxs-lookup"><span data-stu-id="74480-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-295">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-296">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-297">P1</span><span class="sxs-lookup"><span data-stu-id="74480-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-298">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="74480-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-299">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-300">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-301">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="74480-302">صالح</span><span class="sxs-lookup"><span data-stu-id="74480-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-303">بناء على القاعد #5، فإن Q1 و Q2 يمثلان عرضا أسعار في نفس الفرصة، لذا يمكنهم التقدير لنفس المكونات الخاصة بأحد المشروعات.</span><span class="sxs-lookup"><span data-stu-id="74480-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="74480-304">O1</span><span class="sxs-lookup"><span data-stu-id="74480-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-305">ربع السنة الثاني</span><span class="sxs-lookup"><span data-stu-id="74480-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-306">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-307">P1</span><span class="sxs-lookup"><span data-stu-id="74480-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-308">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="74480-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-309">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-310">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-311">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-311">Yes</span></span> </p>
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
<span data-ttu-id="74480-312">O1</span><span class="sxs-lookup"><span data-stu-id="74480-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-313">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-314">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-315">P1</span><span class="sxs-lookup"><span data-stu-id="74480-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-316">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="74480-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-317">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-318">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-319">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="74480-320">صالح</span><span class="sxs-lookup"><span data-stu-id="74480-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74480-321">بناء على القاعد #4، فإن Q1 و Q2 يمثلان عرضا أسعار لفرص مختلفة، لذا لا يمكنهم التقدير لنفس المكونات الخاصة بنفس المشروع.</span><span class="sxs-lookup"><span data-stu-id="74480-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="74480-322">O2</span><span class="sxs-lookup"><span data-stu-id="74480-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="74480-323">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="74480-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-324">QL1</span><span class="sxs-lookup"><span data-stu-id="74480-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-325">P1</span><span class="sxs-lookup"><span data-stu-id="74480-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="74480-326">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="74480-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-327">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="74480-328">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="74480-329">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="74480-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="74480-330">غير صالح</span><span class="sxs-lookup"><span data-stu-id="74480-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

