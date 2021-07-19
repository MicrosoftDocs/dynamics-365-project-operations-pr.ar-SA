---
title: نظرة عامة على شروط التعاقد المستندة إلى المشروع
description: يقدم هذا الموضوع معلومات حول العمل مع شروط التعاقد القائمة على المشروع.
author: rumant
ms.date: 10/28/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 22e8ff927c5ff6c3748a35031e7703e3fcfe0dab
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369900"
---
# <a name="project-based-contract-lines-overview"></a><span data-ttu-id="971c2-103">نظرة عامة على شروط التعاقد المستندة إلى المشروع</span><span class="sxs-lookup"><span data-stu-id="971c2-103">Project-based contract lines overview</span></span>

<span data-ttu-id="971c2-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="971c2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="971c2-105">تم تصميم شروط التعاقد القائمة على المشروع في Dynamics 365 Project Operations لاحتواء اتفاقيات التقديرات والفوترة لمكونات معينة من عمل المشروع على التزام معين.</span><span class="sxs-lookup"><span data-stu-id="971c2-105">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="971c2-106">يتم تمديد البنية الخاصة بشروط التعاقد المستندة إلى المشروع لتقديرات المشاريع وسيناريوهات الفوترة ذات المفاهيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="971c2-106">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="971c2-107">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="971c2-107">Billing method</span></span>
- <span data-ttu-id="971c2-108">تعيين المشاريع والمهام</span><span class="sxs-lookup"><span data-stu-id="971c2-108">Project and task mapping</span></span>
- <span data-ttu-id="971c2-109">فئات الحركات المضمنة</span><span class="sxs-lookup"><span data-stu-id="971c2-109">Included transaction classes</span></span>
- <span data-ttu-id="971c2-110">حد يجب عدم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="971c2-110">Not-to-exceed limit</span></span>
- <span data-ttu-id="971c2-111">إعداد الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="971c2-111">Chargeability setup</span></span>
- <span data-ttu-id="971c2-112">التقديرات باستخدام تفاصيل شروط التعاقد</span><span class="sxs-lookup"><span data-stu-id="971c2-112">Estimates using contract line details</span></span>
- <span data-ttu-id="971c2-113">عملاء شروط التعاقد</span><span class="sxs-lookup"><span data-stu-id="971c2-113">Contract line customers</span></span>

<span data-ttu-id="971c2-114">يتضمن الجدول التالي الحقول الموجودة في علامة التبويب **عام** الخاصة بشروط التعاقد القائمة على المشروع والتي تساعد في إعداد الأساس لتقدير تفصيلي وشامل وترتيبات الفوترة للعمل القائم على المشروع.‬</span><span class="sxs-lookup"><span data-stu-id="971c2-114">The following table includes the fields on the **General** tab of project–based contract lines that help set up the basis for a detailed, ground–up estimate and billing arrangements for project–based work.</span></span>

| <span data-ttu-id="971c2-115">الحقل</span><span class="sxs-lookup"><span data-stu-id="971c2-115">Field</span></span> | <span data-ttu-id="971c2-116">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="971c2-116">Description</span></span> | <span data-ttu-id="971c2-117">تأثير لاحق</span><span class="sxs-lookup"><span data-stu-id="971c2-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="971c2-118">**الاسم**</span><span class="sxs-lookup"><span data-stu-id="971c2-118">**Name**</span></span> | <span data-ttu-id="971c2-119">اسم شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="971c2-119">Name of the contract line.</span></span> <span data-ttu-id="971c2-120">يحدد شرط التعاقد هذا المكون المنفصل للعقد الجاري تقديره.</span><span class="sxs-lookup"><span data-stu-id="971c2-120">This identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="971c2-121">بالنسبة لعقد مشروع تم إنشاؤه من عرض أسعار، يتم نسخ هذه القيمة من قيمة مقابلة لبند عرض أسعار قائم على المشروع.</span><span class="sxs-lookup"><span data-stu-id="971c2-121">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="971c2-122">الاسم المنسوخ على بند فاتورة المشروع الذي تم إنشاؤه من شرط التعاقد هذا عند إنشاء الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="971c2-122">The name copied over to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="971c2-123">**أسلوب الفوترة**</span><span class="sxs-lookup"><span data-stu-id="971c2-123">**Billing Method**</span></span> | <span data-ttu-id="971c2-124">على عقد مشروع تم إنشاؤه من عرض أسعار، يتم نسخ هذه القيمة من الحقل المقابل على بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="971c2-124">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="971c2-125">هذه مجموعة خيارات تمثل نموذجي التعاقد الرئيسيين المدعومين من Project Operations:</span><span class="sxs-lookup"><span data-stu-id="971c2-125">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="971c2-126">- **سعر ثابت**</span><span class="sxs-lookup"><span data-stu-id="971c2-126">- **Fixed Price**</span></span></br><span data-ttu-id="971c2-127">- **الوقت والمادة**</span><span class="sxs-lookup"><span data-stu-id="971c2-127">- **Time and Material**</span></span> | <span data-ttu-id="971c2-128">بالاستناد إلى أسلوب الفوترة لشرط التعاقد المشار إليه، ستتم معالجة الحركة الفعلية.</span><span class="sxs-lookup"><span data-stu-id="971c2-128">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="971c2-129">إذا كان شرط التعاقد الذي تشير إليه القيمة الفعلية يتضمن أسلوب فوترة الوقت والمواد، سيتم إنشاء سجلات القيمة الفعلية للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="971c2-129">If the contract line referenced by the actual has a time and material billing method, cost and unbilled sales actual records are created.</span></span> <span data-ttu-id="971c2-130">إذا كان شرط التعاقد الذي تشير إليه القيمة الفعلية يتضمن أسلوب فوترة بسعر ثابت، سيتم إنشاء قيمة فعلية للتكلفة فقط.</span><span class="sxs-lookup"><span data-stu-id="971c2-130">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="971c2-131">**Project**</span><span class="sxs-lookup"><span data-stu-id="971c2-131">**Project**</span></span> | <span data-ttu-id="971c2-132">استخدم هذا الحقل لتحديد المشروع الذي سيتم استخدامه لتقديم العمل على هذا الالتزام.</span><span class="sxs-lookup"><span data-stu-id="971c2-132">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="971c2-133">سيتم استخدام هذه القيمة مع **المهام المضمنة** و **فئات الحركات المضمنة** لحل مرجع شروط التعاقد حول سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="971c2-133">This value will be used in conjunction with **Included Tasks** and **Included Transaction Classes** to resolve the contract line reference on an actual or estimate line record.</span></span> |
| <span data-ttu-id="971c2-134">**المهام المضمنة**</span><span class="sxs-lookup"><span data-stu-id="971c2-134">**Included Tasks**</span></span> | <span data-ttu-id="971c2-135">تشير إلى ما إذا كان بند التعاقد هذا يتضمن كافة مهام المشروع الخاصة بالمشروع المحدد أو مجموعة فرعية من المهام فقط.</span><span class="sxs-lookup"><span data-stu-id="971c2-135">Indicates if this contract line includes all project tasks for the selected project or only a subset of the tasks.</span></span> <span data-ttu-id="971c2-136">إنها مجموعة خيارات تتضمن القيم الممكنة التالية:</span><span class="sxs-lookup"><span data-stu-id="971c2-136">This is an option set that has the following possible values:</span></span></br><span data-ttu-id="971c2-137">- **كل مهام المشروع**</span><span class="sxs-lookup"><span data-stu-id="971c2-137">- **All Project Tasks**</span></span></br><span data-ttu-id="971c2-138">- **مهام المشروع المحددة فقط**.</span><span class="sxs-lookup"><span data-stu-id="971c2-138">- **Selected Project Tasks Only**.</span></span> <span data-ttu-id="971c2-139">القيمة الفارغة في هذا الحقل تساوي تحديد **كل مهام المشروع‬**.</span><span class="sxs-lookup"><span data-stu-id="971c2-139">A blank value in this field is equal to selecting **All Project Tasks**.</span></span> | <span data-ttu-id="971c2-140">إذا كان الخيار **المهام المحددة فقط** محددًا، فيمكنك تحديد مهام معينة وربطها بشرط التعاقد هذا في علامة التبويب **إعداد فوترة المهام‬** في صفحة **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="971c2-140">If **Selected Tasks Only** is selected, you can select specific tasks and associate them to this contract line on the **Task Billing Setup** tab on the **Project** page.</span></span> <span data-ttu-id="971c2-141">سيتم استخدام القيمة بالتزامن مع فئتي **المشروع** و **الحركة المضمنة** لحل مرجع شروط التعاقد في سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="971c2-141">The value will be used in conjunction with **Project** and **Included Transaction** classes to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="971c2-142">**تضمين الوقت**</span><span class="sxs-lookup"><span data-stu-id="971c2-142">**Include Time**</span></span> | <span data-ttu-id="971c2-143">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين حركات الوقت أو تكاليف العمالة على المشروع المحدد في التقدير على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-143">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="971c2-144">تشير القيمة **لا** إلى أنه لن يتم تضمين حركات الوقت أو تكاليف العمالة على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-144">A **No** value indicates that the time transactions or labor cost will not be included on this contract line.</span></span> <span data-ttu-id="971c2-145">تشير القيمة **نعم** إلى تضمينها.</span><span class="sxs-lookup"><span data-stu-id="971c2-145">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="971c2-146">وتستخدم هذه القيمة مع المشروع لحل مرجع شروط التعاقد حول سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="971c2-146">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="971c2-147">**يتضمن المصروفات**</span><span class="sxs-lookup"><span data-stu-id="971c2-147">**Include Expense**</span></span> | <span data-ttu-id="971c2-148">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين تكاليف المصروفات على المشروع المحدد في التقدير على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-148">A **Yes**/**No** value indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="971c2-149">تشير القيمة **لا** إلى أنه لن يتم تضمين تكاليف المصروفات على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-149">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="971c2-150">تشير القيمة **نعم** إلى تضمينها.</span><span class="sxs-lookup"><span data-stu-id="971c2-150">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="971c2-151">وتستخدم هذه القيمة مع المشروع لحل مرجع شروط التعاقد حول سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="971c2-151">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="971c2-152">**تضمين المواد**</span><span class="sxs-lookup"><span data-stu-id="971c2-152">**Include Materials**</span></span> | <span data-ttu-id="971c2-153">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين تكاليف المواد على المشروع المحدد في التقدير على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-153">A **Yes**/**No** value indicates if material costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="971c2-154">تشير القيمة **نعم** إلى أنه لن يتم تضمين تكاليف المواد في التقدير على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-154">A **No** value indicates that the material costs will not be included on this contract line.</span></span> <span data-ttu-id="971c2-155">تشير القيمة **نعم** إلى تضمينها.</span><span class="sxs-lookup"><span data-stu-id="971c2-155">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="971c2-156">وتستخدم هذه القيمة مع المشروع لحل مرجع شروط التعاقد حول سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="971c2-156">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="971c2-157">**تضمين الرسوم**</span><span class="sxs-lookup"><span data-stu-id="971c2-157">**Include Fee**</span></span> | <span data-ttu-id="971c2-158">تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين الرسوم على المشروع المحدد في التقدير على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-158">A **Yes**/**No** value indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="971c2-159">تشير القيمة **لا** إلى أنه لن يتم تضمين الرسوم على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-159">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="971c2-160">تشير القيمة **نعم** إلى تضمينها.</span><span class="sxs-lookup"><span data-stu-id="971c2-160">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="971c2-161">وتستخدم هذه القيمة مع المشروع لحل مرجع شروط التعاقد حول سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="971c2-161">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="971c2-162">**المبلغ المتعاقد عليه**</span><span class="sxs-lookup"><span data-stu-id="971c2-162">**Contracted Amount**</span></span> | <span data-ttu-id="971c2-163">على شرط تعاقد بسعر ثابت، هذا المبلغ هو القيمة المتفق عليها التي ستتم فوترتها على العميل لكافة مكونات العمل المقترنة بشرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-163">On a fixed price contract line, this amount is the agreed-on value that will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="971c2-164">على شرط تعاقد الوقت والمواد، هذا المبلغ هو قيمة مقدرة لما ستتم فوترته على العميل لكافة مكونات العمل المقترنة بشرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="971c2-164">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="971c2-165">على عقد مشروع تم إنشاؤه من عرض أسعار، يتم نسخ هذه القيمة من الحقل المقابل على بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="971c2-165">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="971c2-166">عندما يتضمن شرط تعاقد قائم على المشروع تفاصيل البند، يتم تأمين هذا الحقل للتحرير ويتم تلخيصه من المبلغ على تفاصيل شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="971c2-166">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="971c2-167">عندما يتضمن شرط التعاقد تفاصيل البند، يمكن تعديل هذه القيمة عن طريق تغيير المبالغ على تفاصيل البند.</span><span class="sxs-lookup"><span data-stu-id="971c2-167">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="971c2-168">على شرط تعاقد بسعر ثابت، يتم استخدام هذه القيمة لإنشاء المبلغ قبل الضريبة على المراحل الرئيسية للفوترة الدورية.</span><span class="sxs-lookup"><span data-stu-id="971c2-168">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="971c2-169">**الضريبة المقدرة**</span><span class="sxs-lookup"><span data-stu-id="971c2-169">**Estimated Tax**</span></span> | <span data-ttu-id="971c2-170">يمكن للمستخدم تحرير هذا الحقل لإدخال مبلغ الضريبة المقدرة في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="971c2-170">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="971c2-171">عندما يتضمن شرط تعاقد قائم على المشروع تفاصيل البند، يتم تأمين هذا الحقل للتحرير ويتم تلخيصه من مبلغ الضريبة على تفاصيل شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="971c2-171">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="971c2-172">عندما يتضمن شرط التعاقد تفاصيل البند، يمكن تعديل هذه القيمة عن طريق تغيير مبالغ الضريبة على تفاصيل البند.</span><span class="sxs-lookup"><span data-stu-id="971c2-172">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="971c2-173">على شرط تعاقد بسعر ثابت، يتم استخدام هذه القيمة لإنشاء الضريبة على المراحل الرئيسية للفوترة الدورية.</span><span class="sxs-lookup"><span data-stu-id="971c2-173">On a fixed price contract line, this value is used to generate the tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="971c2-174">**‏‫المبلغ المتعاقد عليه‬ بعد الضريبة**</span><span class="sxs-lookup"><span data-stu-id="971c2-174">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="971c2-175">‏‫مبلغ شرط التعاقد‬ بعد الضريبة.</span><span class="sxs-lookup"><span data-stu-id="971c2-175">The contract line amount after tax.</span></span> <span data-ttu-id="971c2-176">هذا الحقل للقراءة فقط ويتم حسابه على أنه **مبلغ متعاقد عليه + ضريبة**.</span><span class="sxs-lookup"><span data-stu-id="971c2-176">This field is read only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="971c2-177">على شرط تعاقد بسعر ثابت، يتم استخدام هذه القيمة لإنشاء المراحل الرئيسية للفوترة الدورية.</span><span class="sxs-lookup"><span data-stu-id="971c2-177">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="971c2-178">**حد يجب عدم تجاوزه**</span><span class="sxs-lookup"><span data-stu-id="971c2-178">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="971c2-179">يمكن للمستخدم تحرير هذا الحقل ويكون متاحًا فقط في شروط التعاقد القائمة على المشروع والتي تم تعيين أسلوب الفوترة لها على أنه الوقت والمواد.</span><span class="sxs-lookup"><span data-stu-id="971c2-179">The user can edit this field and it is only available on project-based contract lines that have the billing method set as time and material.</span></span> | <span data-ttu-id="971c2-180">يمكن للمستخدم تحرير هذا الحقل.</span><span class="sxs-lookup"><span data-stu-id="971c2-180">The user can edit this field.</span></span> <span data-ttu-id="971c2-181">عندما تشير قيمة فعلية للوقت والمواد إلى شرط التعاقد هذا للوقت والمواد، يتم تقييم المبلغ على القيمة الفعلية مقابل الحد الذي يجب عدم تجاوزه على شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="971c2-181">When an actual for time and material references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on the contract line.</span></span> <span data-ttu-id="971c2-182">تكتمل عملية التقييم هذه بعد حساب المبالغ التي تمت إنفاقها والالتزام بها.</span><span class="sxs-lookup"><span data-stu-id="971c2-182">This evaluation is completed after  the already spent and committed amounts are accounted for.</span></span> |
| <span data-ttu-id="971c2-183">**موازنة العميل**</span><span class="sxs-lookup"><span data-stu-id="971c2-183">**Customer Budget**</span></span> | <span data-ttu-id="971c2-184">هذا الحقل قابل للتحرير ويتم نسخه من الحقل المقابل على بند عرض الأسعار، إذا تم إنشاء العقد من عرض أسعار.</span><span class="sxs-lookup"><span data-stu-id="971c2-184">This field is editable and is copied from the corresponding field on the quote line if the contract was created from a quote.</span></span> | <span data-ttu-id="971c2-185">يُستخدم هذا الحقل للمعلومات فقط ولا يتضمن أي دلالة لاحقة.</span><span class="sxs-lookup"><span data-stu-id="971c2-185">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="971c2-186">قواعد التحقق من الصحة للخيارات الموجودة في علامة التبويب "عام" في شروط التعاقد القائمة على المشروع</span><span class="sxs-lookup"><span data-stu-id="971c2-186">Validation rules for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="971c2-187">القاعدة 1: إذا كان حقل **المهام المضمنة** فارغًا أو تم تعيينه إلى **كل مهام المشروع**، يتم تضمين كافة المهام الخاصة بالمشروع في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="971c2-187">Rule 1: If the **Included Tasks** field is blank or set to **All Project Tasks**, all tasks of the project are included on the contract line.</span></span>

<span data-ttu-id="971c2-188">القاعدة 2: عندما يكون حقل **المهام المضمنة** فارغًا أو تم تعيينه بشكل واضح إلى **كل مهام المشروع**، يمكن تضمين مشروع وفئة حركات معينة فقط في شرط تعاقد واحد قائم على مشروع في عقد.</span><span class="sxs-lookup"><span data-stu-id="971c2-188">Rule 2: When the **Included Tasks** field is blank or explicitly set to **All Project Tasks**, a project and a certain transaction class can only be included on one project-based contract line of a contract.</span></span>

<span data-ttu-id="971c2-189">القاعدة 3: عندما يكون حقل **المهام المضمنة** معينًا إلى **مهام المشروع المحددة فقط**، يمكن تضمين مشروع وفئة حركات معينة فقط في شروط تعاقد متعددة قائمة على مشروع في عقد.</span><span class="sxs-lookup"><span data-stu-id="971c2-189">Rule 3: When the **Included Tasks** field is set to **Selected Project Tasks Only**, a project and a certain transaction class can be included on multiple project-based contract lines of a contract.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p><span data-ttu-id="971c2-190">
                    <strong>‏‏عقد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-190">
                    <strong>Contract</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="971c2-191">
                    <strong>شروط التعاقد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-191">
                    <strong>Contract line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="971c2-192">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-192">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="67" valign="top">
                <p><span data-ttu-id="971c2-193">
                    <strong>المهام المضمنة</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-193">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="971c2-194">
                    <strong>تضمين الوقت</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-194">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="971c2-195">
                    <strong>يتضمن المصروفات</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-195">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="971c2-196">
                    <strong>تضمين المواد</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-196">
                    <strong>Include Materials</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="971c2-197">
                    <strong>تضمين</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-197">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="971c2-198">
                    <strong>رسوم</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-198">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="53" valign="top">
                <p><span data-ttu-id="971c2-199">
                    <strong>صالح/غير صالح</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-199">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="250" valign="top">
                <p><span data-ttu-id="971c2-200">
                    <strong>سبب</strong>
                </span><span class="sxs-lookup"><span data-stu-id="971c2-200">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-201">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-201">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-202">CL1</span><span class="sxs-lookup"><span data-stu-id="971c2-202">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-203">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-203">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-204">فارغ</span><span class="sxs-lookup"><span data-stu-id="971c2-204">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-205">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-205">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-206">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-206">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-207">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-207">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-208">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-208">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-209">غير صالح</span><span class="sxs-lookup"><span data-stu-id="971c2-209">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-210">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="971c2-210">Violation of Rule #2.</span></span> <span data-ttu-id="971c2-211">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في شرطي التعاقد CL1 و CL2.</span><span class="sxs-lookup"><span data-stu-id="971c2-211">Time, Expense, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-212">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-212">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-213">CL2</span><span class="sxs-lookup"><span data-stu-id="971c2-213">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-214">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-214">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-215">فارغ</span><span class="sxs-lookup"><span data-stu-id="971c2-215">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-216">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-216">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-217">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-217">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-218">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-218">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-219">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-219">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-220">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-220">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-221">CL1</span><span class="sxs-lookup"><span data-stu-id="971c2-221">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-222">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-222">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-223">فارغ</span><span class="sxs-lookup"><span data-stu-id="971c2-223">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-224">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-224">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-225">لا </span><span class="sxs-lookup"><span data-stu-id="971c2-225">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-226">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-226">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-227">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-227">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-228">غير صالح</span><span class="sxs-lookup"><span data-stu-id="971c2-228">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-229">انتهاك القاعدة #2.</span><span class="sxs-lookup"><span data-stu-id="971c2-229">Violation of Rule #2.</span></span> <span data-ttu-id="971c2-230">يتم تضمين الوقت والمواد والرسوم في المشروع P1 في شرطي التعاقد CL1 و CL2.</span><span class="sxs-lookup"><span data-stu-id="971c2-230">Time, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-231">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-231">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-232">CL2</span><span class="sxs-lookup"><span data-stu-id="971c2-232">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-233">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-233">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-234">فارغ</span><span class="sxs-lookup"><span data-stu-id="971c2-234">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-235">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-235">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-236">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-236">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-237">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-237">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-238">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-238">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-239">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-239">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-240">CL1</span><span class="sxs-lookup"><span data-stu-id="971c2-240">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-241">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-241">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-242">فارغ</span><span class="sxs-lookup"><span data-stu-id="971c2-242">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-243">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-243">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-244">لا </span><span class="sxs-lookup"><span data-stu-id="971c2-244">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-245">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-245">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-246">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-246">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-247">صالح</span><span class="sxs-lookup"><span data-stu-id="971c2-247">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-248">يتم تضمين الوقت والمواد والرسوم في المشروع P1 على CL1.</span><span class="sxs-lookup"><span data-stu-id="971c2-248">Time, Materials, and Fees on P1 project are included on CL1.</span></span>
                </p>
                <ul>
                    <li>
<span data-ttu-id="971c2-249">يتم تضمين المصروفات في المشروع P1 في CL2.</span><span class="sxs-lookup"><span data-stu-id="971c2-249">Expense on P1 project is included on CL2.</span></span>
                    </li>
                </ul>
                <p>
<span data-ttu-id="971c2-250">لا يوجد تداخل في ما يتم تضمينه في كل شرط تعاقد وهو بالتالي صالح.</span><span class="sxs-lookup"><span data-stu-id="971c2-250">No overlap in what is being included on each Contract line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-251">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-251">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-252">CL2</span><span class="sxs-lookup"><span data-stu-id="971c2-252">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-253">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-253">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-254">فارغ</span><span class="sxs-lookup"><span data-stu-id="971c2-254">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-255">لا </span><span class="sxs-lookup"><span data-stu-id="971c2-255">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-256">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-257">لا </span><span class="sxs-lookup"><span data-stu-id="971c2-257">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-258">لا </span><span class="sxs-lookup"><span data-stu-id="971c2-258">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-259">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-259">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-260">CL1</span><span class="sxs-lookup"><span data-stu-id="971c2-260">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-261">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-261">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-262">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="971c2-262">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-263">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-263">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-264">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-264">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-265">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-266">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-266">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-267">غير صالح</span><span class="sxs-lookup"><span data-stu-id="971c2-267">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-268">انتهاك القاعدة رقم 2</span><span class="sxs-lookup"><span data-stu-id="971c2-268">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="971c2-269">يتضمن C1 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1.</span><span class="sxs-lookup"><span data-stu-id="971c2-269">C1 includes Time, Materials, Expenses and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="971c2-270">يتضمن CL2 الوقت والمواد والمصروفات لمشروع P1 بكامله وبالتالي يتداخل مع ما يتضمنه C1.</span><span class="sxs-lookup"><span data-stu-id="971c2-270">CL2 includes Time, Materials, Expenses and Fees for the whole project P1 and therefore overlaps with what is included on C1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-271">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-271">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-272">CL2</span><span class="sxs-lookup"><span data-stu-id="971c2-272">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-273">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-273">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-274">فارغ</span><span class="sxs-lookup"><span data-stu-id="971c2-274">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-275">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-275">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-276">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-276">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-277">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-278">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-278">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-279">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-279">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-280">CL1</span><span class="sxs-lookup"><span data-stu-id="971c2-280">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-281">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-281">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-282">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="971c2-282">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-283">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-283">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-284">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-284">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-285">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-285">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-286">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-286">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-287">صالح</span><span class="sxs-lookup"><span data-stu-id="971c2-287">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="971c2-288">حسب القاعدة 3</span><span class="sxs-lookup"><span data-stu-id="971c2-288">Per Rule #3</span></span> </p>
                <p>
<span data-ttu-id="971c2-289">يتضمن C1 الوقت والمصروفات والمواد والرسوم في مجموعة فرعية من المهام في المشروع P1.</span><span class="sxs-lookup"><span data-stu-id="971c2-289">C1 includes Time, Expenses, Materials, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="971c2-290">يتضمن CL2 الوقت والمصروفات والمواد والرسوم في مجموعة فرعية من المهام في المشروع P1.</span><span class="sxs-lookup"><span data-stu-id="971c2-290">CL2 includes Time, Expenses, Materials, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="971c2-291">التحقق الإضافي الوحيد هو حول المجموعة الفرعية من المهام على CL1 التي تختلف عن المجموعة الفرعية للمهام في CL2 لضمان عدم وجود تداخل.</span><span class="sxs-lookup"><span data-stu-id="971c2-291">The only additional validation is around the subset of tasks on CL1 is different from the subset of tasks on CL2 to ensure that there are no overlaps there.</span></span> <span data-ttu-id="971c2-292">يتم ذلك بواسطة النظام عند اقتران المهام.</span><span class="sxs-lookup"><span data-stu-id="971c2-292">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="971c2-293">C1</span><span class="sxs-lookup"><span data-stu-id="971c2-293">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="971c2-294">CL2</span><span class="sxs-lookup"><span data-stu-id="971c2-294">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-295">P1</span><span class="sxs-lookup"><span data-stu-id="971c2-295">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="971c2-296">المهام المحددة فقط</span><span class="sxs-lookup"><span data-stu-id="971c2-296">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-297">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-297">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="971c2-298">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-298">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-299">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-299">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="971c2-300">نعم </span><span class="sxs-lookup"><span data-stu-id="971c2-300">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
