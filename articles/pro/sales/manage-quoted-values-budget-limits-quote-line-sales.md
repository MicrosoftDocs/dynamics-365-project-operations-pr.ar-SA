---
title: نظرة عامة على بنود عرض الأسعار القائم على المشروع
description: يقدم هذا الموضوع معلومات حول استخدام بنود عروض الأسعار المستندة إلى المشروع لعمل المشروع.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: b7076a4b9280472f8c30d0b58c3aa9b9bc86d651
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369855"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="c847f-103">نظرة عامة على بنود عرض الأسعار القائم على المشروع</span><span class="sxs-lookup"><span data-stu-id="c847f-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="c847f-104">_**ينطبق على:** نشر خفيف - التعامل مع الفواتير الأولية‬، Project Operations لسيناريوهات الموارد/المنتجات غير المخزنة_</span><span class="sxs-lookup"><span data-stu-id="c847f-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c847f-105">تم تصميم بنود عرض الأسعار المستندة إلى المشروع للمساعدة في تقدير عمل المشروع بأحد المشاركات.</span><span class="sxs-lookup"><span data-stu-id="c847f-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="c847f-106">يتم توسيع بنية سطر عرض الأسعار المستند إلى المشروع لتقديرات المشروع بالمفاهيم التالية:</span><span class="sxs-lookup"><span data-stu-id="c847f-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="c847f-107">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="c847f-107">Billing Method</span></span>
- <span data-ttu-id="c847f-108">تعيين المشروع والمهمة</span><span class="sxs-lookup"><span data-stu-id="c847f-108">Project and Task Mapping</span></span>
- <span data-ttu-id="c847f-109">فئات الحركات المضمنة</span><span class="sxs-lookup"><span data-stu-id="c847f-109">Included Transaction classes</span></span>
- <span data-ttu-id="c847f-110">حد يجب عدم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="c847f-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="c847f-111">إعداد الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="c847f-111">Chargeability setup</span></span>
- <span data-ttu-id="c847f-112">التقدير باستخدام تفاصيل بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="c847f-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="c847f-113">عملاء بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="c847f-113">Quote line Customers</span></span>

<span data-ttu-id="c847f-114">يوفر الجدول التالي معلومات حول الحقول الموجودة في علامة التبويب **عام** في بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="c847f-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="c847f-115">وتساعد هذه الحقول في إعداد الأساس لتقدير تفصيلي من القاعدة إلى القمة لعمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="c847f-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="c847f-116">**الحقل**</span><span class="sxs-lookup"><span data-stu-id="c847f-116">**Field**</span></span> | <span data-ttu-id="c847f-117">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="c847f-117">**Description**</span></span> | <span data-ttu-id="c847f-118">**تأثير لاحق**</span><span class="sxs-lookup"><span data-stu-id="c847f-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="c847f-119">الاسم </span><span class="sxs-lookup"><span data-stu-id="c847f-119">Name</span></span> | <span data-ttu-id="c847f-120">اسم بند عرض الأسعار الذي يساعدك في تحديد المكون المنفصل لعرض الأسعار الجاري تقديره.</span><span class="sxs-lookup"><span data-stu-id="c847f-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="c847f-121">يتم نسخه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-122">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="c847f-122">Billing Method</span></span> | <span data-ttu-id="c847f-123">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل المقابل في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="c847f-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="c847f-124">يتضمن هذا الحقل نموذجين أساسيين للتعاقد يدعمهما Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="c847f-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="c847f-125">- سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="c847f-125">- Fixed price</span></span></br><span data-ttu-id="c847f-126">- الوقت والمادة.</span><span class="sxs-lookup"><span data-stu-id="c847f-126">- Time and material.</span></span>| <span data-ttu-id="c847f-127">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-128">Project</span><span class="sxs-lookup"><span data-stu-id="c847f-128">Project</span></span> | <span data-ttu-id="c847f-129">استخدم هذا الحقل الاختياري لتحديد المشروع الذي سيتم استخدامه لتسليم العمل في هذه المشاركة.</span><span class="sxs-lookup"><span data-stu-id="c847f-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="c847f-130">عندما يتم تعيين مشروع إلى بند عرض الأسعار، فإنه يساعد في إعداد المهام الخاضعة للرسوم وكذلك يساعد في إحضار التقديرات المستندة إلى المشروع لبند عرض الأسعار كتفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="c847f-131">عند عدم تعيين مشروع لبند عرض أسعار يستند إلى مشروع، يتعين إنشاء التقدير يدويًا عن طريق إنشاء كل تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="c847f-132">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="c847f-133">المهام المضمنة</span><span class="sxs-lookup"><span data-stu-id="c847f-133">Included Tasks</span></span> | <span data-ttu-id="c847f-134">يشير إلى ما إذا كان يتم استخدام بند عرض الأسعار لكافة مهام المشروع أو بعضها للمشروع المحدد.</span><span class="sxs-lookup"><span data-stu-id="c847f-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="c847f-135">يحتوي هذا الحقل على القيم الممكنة التالية:</span><span class="sxs-lookup"><span data-stu-id="c847f-135">This field has the following possible values:</span></span></br><span data-ttu-id="c847f-136">- كل مهام المشروع</span><span class="sxs-lookup"><span data-stu-id="c847f-136">- All project tasks</span></span></br><span data-ttu-id="c847f-137">- مهام المشروع المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="c847f-137">- Selected project tasks only</span></span></br><span data-ttu-id="c847f-138">القيمة الفارغة في هذا الحقل تكافئ خيار **كافة مهام المشروع**.</span><span class="sxs-lookup"><span data-stu-id="c847f-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="c847f-139">عند تحديد الخيار **مهام المشروع المحددة فقط‬** على صفحة المشروع، تسمح لك علامة التبويب **إعداد فوترة المهام** تحديد مهام معينة لربطها ببند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="c847f-140">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-141">تضمين الوقت</span><span class="sxs-lookup"><span data-stu-id="c847f-141">Include Time</span></span> | <span data-ttu-id="c847f-142">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين حركات الوقت أو تكاليف العمالة على المشروع المحدد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c847f-143">تشير علامة **لا** إلى أن حركات الوقت أو تكلفة العمالة لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c847f-144">تشير علامة **نعم** إلى أن حركات الوقت أو تكلفة العمالة سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c847f-145">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-146">يتضمن المصروفات</span><span class="sxs-lookup"><span data-stu-id="c847f-146">Include Expense</span></span> | <span data-ttu-id="c847f-147">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين تكاليف المصروفات على المشروع المحدد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c847f-148">تشير علامة **لا** إلى أن تكلفة المصروفات لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c847f-149">تشير علامة **نعم** إلى أن تكلفة المصروفات سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c847f-150">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-151">تضمين المواد</span><span class="sxs-lookup"><span data-stu-id="c847f-151">Include Material</span></span> | <span data-ttu-id="c847f-152">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين تكاليف المواد على المشروع المحدد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c847f-153">تشير القيمة **نعم** إلى أنه لن يتم تضمين تكاليف المواد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c847f-154">تشير القيمة **نعم** إلى أنه سيتم تضمين تكاليف المواد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c847f-155">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-156">تضمين الرسوم</span><span class="sxs-lookup"><span data-stu-id="c847f-156">Include Fee</span></span> | <span data-ttu-id="c847f-157">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين الرسوم على المشروع المحدد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c847f-158">تشير القيمة **لا** إلى أنه لن يتم تضمين الرسوم في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c847f-159">تشير القيمة **نعم** إلى أنه سيتم تضمين الرسوم في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="c847f-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c847f-160">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-161">المبلغ المعروض</span><span class="sxs-lookup"><span data-stu-id="c847f-161">Quoted Amount</span></span> | <span data-ttu-id="c847f-162">هذا هو المبلغ الذي سيتم إدراجه في عرض الأسعار للعميل لكل العمل المتوقع في شرط التعاقد القائم على هذا المشروع.</span><span class="sxs-lookup"><span data-stu-id="c847f-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="c847f-163">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل **ميزانية العميل** في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="c847f-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="c847f-164">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من المبلغ الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="c847f-165">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-166">الضريبة المقدرة</span><span class="sxs-lookup"><span data-stu-id="c847f-166">Estimated Tax</span></span> | <span data-ttu-id="c847f-167">هذا حقل قابل للتحرير لكي يقوم المستخدم بإضافة مبلغ الضريبة المقدرة في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="c847f-168">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من مبلغ الضريبة الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="c847f-169">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-170">‏‫المبلغ المعروض‬ بعد الضريبة</span><span class="sxs-lookup"><span data-stu-id="c847f-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="c847f-171">هذا الحقل هو مبلغ بند عرض الأسعار بعد الضريبة وهو للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="c847f-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="c847f-172">يتم حساب المبلغ الموجود في هذا الحقل *كمبلغ معروض + الضريبة*.</span><span class="sxs-lookup"><span data-stu-id="c847f-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="c847f-173">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-174">حد ما يجب ألا يتم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="c847f-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="c847f-175">ويكون هذا الحقل قابلا للتحرير ويكون متاحا فقط في بنود عروض الأسعار المستندة إلى المشروع والتي لها أسلوب فوترة **الوقت والمادة**.</span><span class="sxs-lookup"><span data-stu-id="c847f-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="c847f-176">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c847f-177">موازنة العميل</span><span class="sxs-lookup"><span data-stu-id="c847f-177">Customer Budget</span></span> | <span data-ttu-id="c847f-178">يكون هذا الحقل قابلا للتحرير ويتم نسخه من الحقل المقابل في بند الفرصة إذا تم إنشاء عرض الأسعار من إحدى الفرص.</span><span class="sxs-lookup"><span data-stu-id="c847f-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="c847f-179">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="c847f-180">قواعد التحقق من الصحة للحقول في علامة التبويب عام لبنود عرض الأسعار المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="c847f-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="c847f-181">**القاعدة 1**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه على **جميع مهام المشروع**، فسيتم تضمين المشروع في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="c847f-182">**القاعدة 2**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه إلى **كافة مهام المشروع**، فيمكن تضمين مشروع وفئة حركة معينة فقط في بند عرض أسعار واحد يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="c847f-183">**القاعدة 3**: إذا تم تعيين حقل **المهام المضمنة** إلى **مهام المشروع المحددة فقط**، فيمكن تضمين مشروع وفئة حركة معينة فقط في عدة بنود عرض أسعار يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="c847f-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="c847f-184">**القاعدة 4**: إذا كانت الفرصة تحتوي على عدة عروض أسعار، فيمكن أن يكون هناك بنود عرض أسعار مختلفة والتي تشير إلى نفس المشروع وتتضمن نفس فئة الحركات.</span><span class="sxs-lookup"><span data-stu-id="c847f-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="c847f-185">**القاعدة 5**: إذا لم تكن عروض الأسعار تنتمي إلى نفس الفرصة، فلا يمكن أن تتضمن نفس فئة المشروع والحركات.</span><span class="sxs-lookup"><span data-stu-id="c847f-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="c847f-186">
                    <strong>الفرصة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="c847f-187">
                    <strong>اقتباس</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="c847f-188">
                    <strong>بند عرض الأسعار</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="c847f-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="c847f-190">
                    <strong>المهام المضمنة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="c847f-191">
                    <strong>تضمين الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="c847f-192">
                    <strong>يتضمن المصروفات</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="c847f-193">
                    <strong>تضمين المواد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="c847f-194">
                    <strong>تضمين</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="c847f-195">
                    <strong>رسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="c847f-196">
                    <strong>صالح/غير صالح</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="c847f-197">
                    <strong>سبب</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c847f-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-198">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-199">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-200">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-201">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-202">فارغ</span><span class="sxs-lookup"><span data-stu-id="c847f-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-203">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-204">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-205">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-206">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-207">غير صالح</span><span class="sxs-lookup"><span data-stu-id="c847f-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-208">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="c847f-208">Violation of Rule #2.</span></span> <span data-ttu-id="c847f-209">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في بنود عرض الأسعار QL1 وQL2.</span><span class="sxs-lookup"><span data-stu-id="c847f-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-210">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-211">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-212">QL2</span><span class="sxs-lookup"><span data-stu-id="c847f-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-213">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-214">فارغ</span><span class="sxs-lookup"><span data-stu-id="c847f-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-215">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-216">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-217">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-218">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-218">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-219">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-220">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-221">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-222">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-223">فارغ</span><span class="sxs-lookup"><span data-stu-id="c847f-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-224">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-225">لا </span><span class="sxs-lookup"><span data-stu-id="c847f-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-226">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-227">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-228">غير صالح</span><span class="sxs-lookup"><span data-stu-id="c847f-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-229">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="c847f-229">Violation of Rule #2.</span></span> <span data-ttu-id="c847f-230">يتم تضمين الوقت والمواد والرسوم في المشروع P1 في بنود عرض الأسعار QL1 وQL2.</span><span class="sxs-lookup"><span data-stu-id="c847f-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-231">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-232">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-233">QL2</span><span class="sxs-lookup"><span data-stu-id="c847f-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-234">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-235">فارغ</span><span class="sxs-lookup"><span data-stu-id="c847f-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-236">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-237">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-238">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-239">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-239">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-240">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-241">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-242">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-243">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-244">فارغ</span><span class="sxs-lookup"><span data-stu-id="c847f-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-245">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-246">لا </span><span class="sxs-lookup"><span data-stu-id="c847f-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-247">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-248">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-249">صالح</span><span class="sxs-lookup"><span data-stu-id="c847f-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-250">يتم تضمين الوقت والمواد والرسوم في المشروع P1 على QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="c847f-251">يتم تضمين المصروفات في المشروع P1 في QL2.</span><span class="sxs-lookup"><span data-stu-id="c847f-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="c847f-252">لا يوجد تداخل في ما يتم تضمينه في كل بند عرض أسعار وهو بالتالي صالح.</span><span class="sxs-lookup"><span data-stu-id="c847f-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-253">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-254">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-255">QL2</span><span class="sxs-lookup"><span data-stu-id="c847f-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-256">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-257">فارغ</span><span class="sxs-lookup"><span data-stu-id="c847f-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-258">لا </span><span class="sxs-lookup"><span data-stu-id="c847f-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-259">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-260">لا </span><span class="sxs-lookup"><span data-stu-id="c847f-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-261">لا </span><span class="sxs-lookup"><span data-stu-id="c847f-261">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-262">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-263">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-264">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-265">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-266">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="c847f-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-267">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-268">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-269">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-270">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-271">غير صالح</span><span class="sxs-lookup"><span data-stu-id="c847f-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-272">انتهاك القاعدة رقم 2</span><span class="sxs-lookup"><span data-stu-id="c847f-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="c847f-273">يتضمن Q1 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1</span><span class="sxs-lookup"><span data-stu-id="c847f-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="c847f-274">يتضمن QL2 الوقت والمصروفات والرسوم لمشروع P1 بكامله وبالتالي يتداخل مع ما يتضمنه Q1.</span><span class="sxs-lookup"><span data-stu-id="c847f-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-275">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-276">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-277">QL2</span><span class="sxs-lookup"><span data-stu-id="c847f-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-278">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-279">فارغ</span><span class="sxs-lookup"><span data-stu-id="c847f-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-280">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-281">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-282">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-283">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-283">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-284">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-285">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-286">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-287">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-288">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="c847f-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-289">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-290">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-291">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-292">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-293">صالح</span><span class="sxs-lookup"><span data-stu-id="c847f-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-294">حسب القاعدة 3</span><span class="sxs-lookup"><span data-stu-id="c847f-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="c847f-295">يتضمن Q1 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1.</span><span class="sxs-lookup"><span data-stu-id="c847f-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="c847f-296">يتضمن QL2 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1.</span><span class="sxs-lookup"><span data-stu-id="c847f-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="c847f-297">التحقق الإضافي الوحيد هو حول المجموعة الفرعية من المهام على QL1 التي تختلف عن المجموعة الفرعية للمهام في QL2 لضمان عدم وجود تداخل.</span><span class="sxs-lookup"><span data-stu-id="c847f-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="c847f-298">يتم ذلك بواسطة النظام عند اقتران المهام.</span><span class="sxs-lookup"><span data-stu-id="c847f-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-299">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-300">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-301">QL2</span><span class="sxs-lookup"><span data-stu-id="c847f-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-302">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-303">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="c847f-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-304">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-305">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-306">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-307">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-307">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-308">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-309">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-310">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-311">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-312">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="c847f-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-313">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-314">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-315">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-316">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-317">صالح</span><span class="sxs-lookup"><span data-stu-id="c847f-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-318">بحسب القاعدة 5، Q1 وQ2 عبارة عن عرضي أسعار في نفس الفرصة، وبالتالي يقدران المكونات نفسها لمشروع</span><span class="sxs-lookup"><span data-stu-id="c847f-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-319">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-320">ربع السنة الثاني</span><span class="sxs-lookup"><span data-stu-id="c847f-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-321">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-322">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-323">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="c847f-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-324">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-325">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-326">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-327">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-327">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-328">O1</span><span class="sxs-lookup"><span data-stu-id="c847f-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-329">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-330">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-331">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-332">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="c847f-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-333">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-334">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-335">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-336">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-337">غير صالح</span><span class="sxs-lookup"><span data-stu-id="c847f-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c847f-338">بحسب القاعدة 4، Q1 وQ2 عبارة عن عرضي أسعار في فرص مختلفة، وبالتالي لا يمكنهما تقدير المكونات نفسها للمشروع نفسه.</span><span class="sxs-lookup"><span data-stu-id="c847f-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c847f-339">O2</span><span class="sxs-lookup"><span data-stu-id="c847f-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c847f-340">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="c847f-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c847f-341">QL1</span><span class="sxs-lookup"><span data-stu-id="c847f-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-342">P1</span><span class="sxs-lookup"><span data-stu-id="c847f-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c847f-343">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="c847f-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c847f-344">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c847f-345">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c847f-346">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c847f-347">نعم </span><span class="sxs-lookup"><span data-stu-id="c847f-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
