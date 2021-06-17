---
title: نظرة عامة على بنود عرض الأسعار القائم على المشروع
description: يقدم هذا الموضوع معلومات حول استخدام بنود عروض الأسعار المستندة إلى المشروع لعمل المشروع.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32337b05f09ef7c5b84fdff9870744d6367e2693
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994840"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="96144-103">نظرة عامة على بنود عرض الأسعار القائم على المشروع</span><span class="sxs-lookup"><span data-stu-id="96144-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="96144-104">_**ينطبق على:** نشر خفيف - التعامل مع الفواتير الأولية‬، Project Operations لسيناريوهات الموارد/المنتجات غير المخزنة_</span><span class="sxs-lookup"><span data-stu-id="96144-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="96144-105">تم تصميم بنود عرض الأسعار المستندة إلى المشروع للمساعدة في تقدير عمل المشروع بأحد المشاركات.</span><span class="sxs-lookup"><span data-stu-id="96144-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="96144-106">يتم توسيع بنية سطر عرض الأسعار المستند إلى المشروع لتقديرات المشروع بالمفاهيم التالية:</span><span class="sxs-lookup"><span data-stu-id="96144-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="96144-107">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="96144-107">Billing Method</span></span>
- <span data-ttu-id="96144-108">تعيين المشروع والمهمة</span><span class="sxs-lookup"><span data-stu-id="96144-108">Project and Task Mapping</span></span>
- <span data-ttu-id="96144-109">فئات الحركات المضمنة</span><span class="sxs-lookup"><span data-stu-id="96144-109">Included Transaction classes</span></span>
- <span data-ttu-id="96144-110">حد يجب عدم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="96144-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="96144-111">إعداد الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="96144-111">Chargeability setup</span></span>
- <span data-ttu-id="96144-112">التقدير باستخدام تفاصيل بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="96144-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="96144-113">عملاء بند عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="96144-113">Quote line Customers</span></span>

<span data-ttu-id="96144-114">يوفر الجدول التالي معلومات حول الحقول الموجودة في علامة التبويب **عام** في بند عرض الأسعار المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="96144-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="96144-115">وتساعد هذه الحقول في إعداد الأساس لتقدير تفصيلي من القاعدة إلى القمة لعمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="96144-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="96144-116">**الحقل**</span><span class="sxs-lookup"><span data-stu-id="96144-116">**Field**</span></span> | <span data-ttu-id="96144-117">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="96144-117">**Description**</span></span> | <span data-ttu-id="96144-118">**تأثير لاحق**</span><span class="sxs-lookup"><span data-stu-id="96144-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="96144-119">الاسم </span><span class="sxs-lookup"><span data-stu-id="96144-119">Name</span></span> | <span data-ttu-id="96144-120">اسم بند عرض الأسعار الذي يساعدك في تحديد المكون المنفصل لعرض الأسعار الجاري تقديره.</span><span class="sxs-lookup"><span data-stu-id="96144-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="96144-121">يتم نسخه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-122">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="96144-122">Billing Method</span></span> | <span data-ttu-id="96144-123">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل المقابل في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="96144-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="96144-124">يتضمن هذا الحقل نموذجين أساسيين للتعاقد يدعمهما Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="96144-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="96144-125">- سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="96144-125">- Fixed price</span></span></br><span data-ttu-id="96144-126">- الوقت والمادة.</span><span class="sxs-lookup"><span data-stu-id="96144-126">- Time and material.</span></span>| <span data-ttu-id="96144-127">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-128">Project</span><span class="sxs-lookup"><span data-stu-id="96144-128">Project</span></span> | <span data-ttu-id="96144-129">استخدم هذا الحقل الاختياري لتحديد المشروع الذي سيتم استخدامه لتسليم العمل في هذه المشاركة.</span><span class="sxs-lookup"><span data-stu-id="96144-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="96144-130">عندما يتم تعيين مشروع إلى بند عرض الأسعار، فإنه يساعد في إعداد المهام الخاضعة للرسوم وكذلك يساعد في إحضار التقديرات المستندة إلى المشروع لبند عرض الأسعار كتفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="96144-131">عند عدم تعيين مشروع لبند عرض أسعار يستند إلى مشروع، يتعين إنشاء التقدير يدويًا عن طريق إنشاء كل تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="96144-132">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="96144-133">المهام المضمنة</span><span class="sxs-lookup"><span data-stu-id="96144-133">Included Tasks</span></span> | <span data-ttu-id="96144-134">يشير إلى ما إذا كان يتم استخدام بند عرض الأسعار لكافة مهام المشروع أو بعضها للمشروع المحدد.</span><span class="sxs-lookup"><span data-stu-id="96144-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="96144-135">يحتوي هذا الحقل على القيم الممكنة التالية:</span><span class="sxs-lookup"><span data-stu-id="96144-135">This field has the following possible values:</span></span></br><span data-ttu-id="96144-136">- كل مهام المشروع</span><span class="sxs-lookup"><span data-stu-id="96144-136">- All project tasks</span></span></br><span data-ttu-id="96144-137">- مهام المشروع المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="96144-137">- Selected project tasks only</span></span></br><span data-ttu-id="96144-138">القيمة الفارغة في هذا الحقل تكافئ خيار **كافة مهام المشروع**.</span><span class="sxs-lookup"><span data-stu-id="96144-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="96144-139">عند تحديد الخيار **مهام المشروع المحددة فقط‬** على صفحة المشروع، تسمح لك علامة التبويب **إعداد فوترة المهام** تحديد مهام معينة لربطها ببند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="96144-140">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-141">تضمين الوقت</span><span class="sxs-lookup"><span data-stu-id="96144-141">Include Time</span></span> | <span data-ttu-id="96144-142">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين حركات الوقت أو تكاليف العمالة على المشروع المحدد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="96144-143">تشير علامة **لا** إلى أن حركات الوقت أو تكلفة العمالة لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="96144-144">تشير علامة **نعم** إلى أن حركات الوقت أو تكلفة العمالة سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="96144-145">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-146">يتضمن المصروفات</span><span class="sxs-lookup"><span data-stu-id="96144-146">Include Expense</span></span> | <span data-ttu-id="96144-147">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين تكاليف المصروفات على المشروع المحدد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="96144-148">تشير علامة **لا** إلى أن تكلفة المصروفات لن يتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="96144-149">تشير علامة **نعم** إلى أن تكلفة المصروفات سيتم تضمينها في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="96144-150">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-151">تضمين المواد</span><span class="sxs-lookup"><span data-stu-id="96144-151">Include Material</span></span> | <span data-ttu-id="96144-152">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين تكاليف المواد على المشروع المحدد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="96144-153">تشير القيمة **نعم** إلى أنه لن يتم تضمين تكاليف المواد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="96144-154">تشير القيمة **نعم** إلى أنه سيتم تضمين تكاليف المواد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="96144-155">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-156">تضمين الرسوم</span><span class="sxs-lookup"><span data-stu-id="96144-156">Include Fee</span></span> | <span data-ttu-id="96144-157">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين الرسوم على المشروع المحدد في التقدير على بند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="96144-158">تشير القيمة **لا** إلى أنه لن يتم تضمين الرسوم في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="96144-159">تشير القيمة **نعم** إلى أنه سيتم تضمين الرسوم في التقدير لبند عرض الأسعار هذا.</span><span class="sxs-lookup"><span data-stu-id="96144-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="96144-160">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-161">المبلغ المعروض</span><span class="sxs-lookup"><span data-stu-id="96144-161">Quoted Amount</span></span> | <span data-ttu-id="96144-162">هذا هو المبلغ الذي سيتم إدراجه في عرض الأسعار للعميل لكل العمل المتوقع في شرط التعاقد القائم على هذا المشروع.</span><span class="sxs-lookup"><span data-stu-id="96144-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="96144-163">في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل **ميزانية العميل** في بند الفرصة.</span><span class="sxs-lookup"><span data-stu-id="96144-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="96144-164">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من المبلغ الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="96144-165">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-166">الضريبة المقدرة</span><span class="sxs-lookup"><span data-stu-id="96144-166">Estimated Tax</span></span> | <span data-ttu-id="96144-167">هذا حقل قابل للتحرير لكي يقوم المستخدم بإضافة مبلغ الضريبة المقدرة في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="96144-168">عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من مبلغ الضريبة الموجود في تفاصيل بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="96144-169">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-170">‏‫المبلغ المعروض‬ بعد الضريبة</span><span class="sxs-lookup"><span data-stu-id="96144-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="96144-171">هذا الحقل هو مبلغ بند عرض الأسعار بعد الضريبة وهو للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="96144-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="96144-172">يتم حساب المبلغ الموجود في هذا الحقل *كمبلغ معروض + الضريبة*.</span><span class="sxs-lookup"><span data-stu-id="96144-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="96144-173">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-174">حد ما يجب ألا يتم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="96144-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="96144-175">ويكون هذا الحقل قابلا للتحرير ويكون متاحا فقط في بنود عروض الأسعار المستندة إلى المشروع والتي لها أسلوب فوترة **الوقت والمادة**.</span><span class="sxs-lookup"><span data-stu-id="96144-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="96144-176">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="96144-177">موازنة العميل</span><span class="sxs-lookup"><span data-stu-id="96144-177">Customer Budget</span></span> | <span data-ttu-id="96144-178">يكون هذا الحقل قابلا للتحرير ويتم نسخه من الحقل المقابل في بند الفرصة إذا تم إنشاء عرض الأسعار من إحدى الفرص.</span><span class="sxs-lookup"><span data-stu-id="96144-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="96144-179">يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="96144-180">قواعد التحقق من الصحة للحقول في علامة التبويب عام لبنود عرض الأسعار المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="96144-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="96144-181">**القاعدة 1**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه على **جميع مهام المشروع**، فسيتم تضمين المشروع في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="96144-182">**القاعدة 2**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه إلى **كافة مهام المشروع**، فيمكن تضمين مشروع وفئة حركة معينة فقط في بند عرض أسعار واحد يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="96144-183">**القاعدة 3**: إذا تم تعيين حقل **المهام المضمنة** إلى **مهام المشروع المحددة فقط**، فيمكن تضمين مشروع وفئة حركة معينة فقط في عدة بنود عرض أسعار يستند إلى مشروع في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="96144-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="96144-184">**القاعدة 4**: إذا كانت الفرصة تحتوي على عدة عروض أسعار، فيمكن أن يكون هناك بنود عرض أسعار مختلفة والتي تشير إلى نفس المشروع وتتضمن نفس فئة الحركات.</span><span class="sxs-lookup"><span data-stu-id="96144-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="96144-185">**القاعدة 5**: إذا لم تكن عروض الأسعار تنتمي إلى نفس الفرصة، فلا يمكن أن تتضمن نفس فئة المشروع والحركات.</span><span class="sxs-lookup"><span data-stu-id="96144-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="96144-186">
                    <strong>الفرصة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="96144-187">
                    <strong>اقتباس</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="96144-188">
                    <strong>بند عرض الأسعار</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="96144-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="96144-190">
                    <strong>المهام المضمنة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="96144-191">
                    <strong>تضمين الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="96144-192">
                    <strong>يتضمن المصروفات</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="96144-193">
                    <strong>تضمين المواد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="96144-194">
                    <strong>تضمين</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="96144-195">
                    <strong>رسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="96144-196">
                    <strong>صالح/غير صالح</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="96144-197">
                    <strong>سبب</strong>
                </span><span class="sxs-lookup"><span data-stu-id="96144-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="96144-198">O1</span><span class="sxs-lookup"><span data-stu-id="96144-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-199">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-200">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-201">P1</span><span class="sxs-lookup"><span data-stu-id="96144-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-202">فارغ</span><span class="sxs-lookup"><span data-stu-id="96144-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-203">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-204">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-205">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-206">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-207">غير صالح</span><span class="sxs-lookup"><span data-stu-id="96144-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-208">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="96144-208">Violation of Rule #2.</span></span> <span data-ttu-id="96144-209">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في بنود عرض الأسعار QL1 وQL2.</span><span class="sxs-lookup"><span data-stu-id="96144-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="96144-210">O1</span><span class="sxs-lookup"><span data-stu-id="96144-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-211">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-212">QL2</span><span class="sxs-lookup"><span data-stu-id="96144-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-213">P1</span><span class="sxs-lookup"><span data-stu-id="96144-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-214">فارغ</span><span class="sxs-lookup"><span data-stu-id="96144-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-215">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-216">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-217">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-218">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-218">Yes</span></span> </p>
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
<span data-ttu-id="96144-219">O1</span><span class="sxs-lookup"><span data-stu-id="96144-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-220">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-221">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-222">P1</span><span class="sxs-lookup"><span data-stu-id="96144-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-223">فارغ</span><span class="sxs-lookup"><span data-stu-id="96144-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-224">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-225">لا </span><span class="sxs-lookup"><span data-stu-id="96144-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-226">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-227">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-228">غير صالح</span><span class="sxs-lookup"><span data-stu-id="96144-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-229">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="96144-229">Violation of Rule #2.</span></span> <span data-ttu-id="96144-230">يتم تضمين الوقت والمواد والرسوم في المشروع P1 في بنود عرض الأسعار QL1 وQL2.</span><span class="sxs-lookup"><span data-stu-id="96144-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="96144-231">O1</span><span class="sxs-lookup"><span data-stu-id="96144-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-232">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-233">QL2</span><span class="sxs-lookup"><span data-stu-id="96144-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-234">P1</span><span class="sxs-lookup"><span data-stu-id="96144-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-235">فارغ</span><span class="sxs-lookup"><span data-stu-id="96144-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-236">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-237">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-238">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-239">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-239">Yes</span></span> </p>
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
<span data-ttu-id="96144-240">O1</span><span class="sxs-lookup"><span data-stu-id="96144-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-241">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-242">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-243">P1</span><span class="sxs-lookup"><span data-stu-id="96144-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-244">فارغ</span><span class="sxs-lookup"><span data-stu-id="96144-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-245">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-246">لا </span><span class="sxs-lookup"><span data-stu-id="96144-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-247">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-248">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-249">صالح</span><span class="sxs-lookup"><span data-stu-id="96144-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-250">يتم تضمين الوقت والمواد والرسوم في المشروع P1 على QL1</span><span class="sxs-lookup"><span data-stu-id="96144-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="96144-251">يتم تضمين المصروفات في المشروع P1 في QL2.</span><span class="sxs-lookup"><span data-stu-id="96144-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="96144-252">لا يوجد تداخل في ما يتم تضمينه في كل بند عرض أسعار وهو بالتالي صالح.</span><span class="sxs-lookup"><span data-stu-id="96144-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="96144-253">O1</span><span class="sxs-lookup"><span data-stu-id="96144-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-254">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-255">QL2</span><span class="sxs-lookup"><span data-stu-id="96144-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-256">P1</span><span class="sxs-lookup"><span data-stu-id="96144-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-257">فارغ</span><span class="sxs-lookup"><span data-stu-id="96144-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-258">لا </span><span class="sxs-lookup"><span data-stu-id="96144-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-259">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-260">لا </span><span class="sxs-lookup"><span data-stu-id="96144-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-261">لا </span><span class="sxs-lookup"><span data-stu-id="96144-261">No</span></span> </p>
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
<span data-ttu-id="96144-262">O1</span><span class="sxs-lookup"><span data-stu-id="96144-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-263">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-264">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-265">P1</span><span class="sxs-lookup"><span data-stu-id="96144-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-266">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="96144-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-267">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-268">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-269">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-270">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-271">غير صالح</span><span class="sxs-lookup"><span data-stu-id="96144-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-272">انتهاك القاعدة رقم 2</span><span class="sxs-lookup"><span data-stu-id="96144-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="96144-273">يتضمن Q1 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1</span><span class="sxs-lookup"><span data-stu-id="96144-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="96144-274">يتضمن QL2 الوقت والمصروفات والرسوم لمشروع P1 بكامله وبالتالي يتداخل مع ما يتضمنه Q1.</span><span class="sxs-lookup"><span data-stu-id="96144-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="96144-275">O1</span><span class="sxs-lookup"><span data-stu-id="96144-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-276">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-277">QL2</span><span class="sxs-lookup"><span data-stu-id="96144-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-278">P1</span><span class="sxs-lookup"><span data-stu-id="96144-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-279">فارغ</span><span class="sxs-lookup"><span data-stu-id="96144-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-280">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-281">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-282">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-283">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-283">Yes</span></span> </p>
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
<span data-ttu-id="96144-284">O1</span><span class="sxs-lookup"><span data-stu-id="96144-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-285">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-286">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-287">P1</span><span class="sxs-lookup"><span data-stu-id="96144-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-288">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="96144-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-289">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-290">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-291">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-292">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-293">صالح</span><span class="sxs-lookup"><span data-stu-id="96144-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-294">حسب القاعدة 3</span><span class="sxs-lookup"><span data-stu-id="96144-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="96144-295">يتضمن Q1 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1.</span><span class="sxs-lookup"><span data-stu-id="96144-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="96144-296">يتضمن QL2 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1.</span><span class="sxs-lookup"><span data-stu-id="96144-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="96144-297">التحقق الإضافي الوحيد هو حول المجموعة الفرعية من المهام على QL1 التي تختلف عن المجموعة الفرعية للمهام في QL2 لضمان عدم وجود تداخل.</span><span class="sxs-lookup"><span data-stu-id="96144-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="96144-298">يتم ذلك بواسطة النظام عند اقتران المهام.</span><span class="sxs-lookup"><span data-stu-id="96144-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="96144-299">O1</span><span class="sxs-lookup"><span data-stu-id="96144-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-300">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-301">QL2</span><span class="sxs-lookup"><span data-stu-id="96144-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-302">P1</span><span class="sxs-lookup"><span data-stu-id="96144-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-303">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="96144-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-304">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-305">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-306">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-307">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-307">Yes</span></span> </p>
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
<span data-ttu-id="96144-308">O1</span><span class="sxs-lookup"><span data-stu-id="96144-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-309">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-310">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-311">P1</span><span class="sxs-lookup"><span data-stu-id="96144-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-312">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="96144-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-313">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-314">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-315">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-316">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-317">صالح</span><span class="sxs-lookup"><span data-stu-id="96144-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-318">بحسب القاعدة 5، Q1 وQ2 عبارة عن عرضي أسعار في نفس الفرصة، وبالتالي يقدران المكونات نفسها لمشروع</span><span class="sxs-lookup"><span data-stu-id="96144-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="96144-319">O1</span><span class="sxs-lookup"><span data-stu-id="96144-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-320">ربع السنة الثاني</span><span class="sxs-lookup"><span data-stu-id="96144-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-321">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-322">P1</span><span class="sxs-lookup"><span data-stu-id="96144-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-323">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="96144-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-324">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-325">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-326">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-327">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-327">Yes</span></span> </p>
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
<span data-ttu-id="96144-328">O1</span><span class="sxs-lookup"><span data-stu-id="96144-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-329">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-330">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-331">P1</span><span class="sxs-lookup"><span data-stu-id="96144-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-332">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="96144-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-333">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-334">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-335">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-336">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-337">غير صالح</span><span class="sxs-lookup"><span data-stu-id="96144-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="96144-338">بحسب القاعدة 4، Q1 وQ2 عبارة عن عرضي أسعار في فرص مختلفة، وبالتالي لا يمكنهما تقدير المكونات نفسها للمشروع نفسه.</span><span class="sxs-lookup"><span data-stu-id="96144-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="96144-339">O2</span><span class="sxs-lookup"><span data-stu-id="96144-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="96144-340">ربع السنة الأول</span><span class="sxs-lookup"><span data-stu-id="96144-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="96144-341">QL1</span><span class="sxs-lookup"><span data-stu-id="96144-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-342">P1</span><span class="sxs-lookup"><span data-stu-id="96144-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="96144-343">كافة مهام المشروع أو فارغة</span><span class="sxs-lookup"><span data-stu-id="96144-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="96144-344">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="96144-345">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="96144-346">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="96144-347">نعم </span><span class="sxs-lookup"><span data-stu-id="96144-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
