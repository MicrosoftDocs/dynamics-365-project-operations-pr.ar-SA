---
title: العمل مع شروط التعاقد القائمة على المشروع
description: يقدم هذا الموضوع معلومات حول شروط التعاقد القائمة على المشروع.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 14d880eccd5547c122ebe37b63022e64fa2fb6fe
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181670"
---
# <a name="work-with-projectbased-contract-lines"></a><span data-ttu-id="18e5e-103">العمل مع شروط التعاقد القائمة على المشروع</span><span class="sxs-lookup"><span data-stu-id="18e5e-103">Work with project–based contract lines</span></span>

<span data-ttu-id="18e5e-104">تم تصميم شروط التعاقد القائمة على المشروع في Dynamics 365 Project Operations لاحتواء اتفاقيات التقديرات والفوترة لمكونات معينة من عمل المشروع على التزام معين.</span><span class="sxs-lookup"><span data-stu-id="18e5e-104">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="18e5e-105">يتم توسيع بنية شروط التعاقد القائمة على المشروع لتقديرات المشروع وسيناريوهات الفوترة بواسطة المفاهيم التالية:</span><span class="sxs-lookup"><span data-stu-id="18e5e-105">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="18e5e-106">أسلوب الفوترة</span><span class="sxs-lookup"><span data-stu-id="18e5e-106">Billing method</span></span>
- <span data-ttu-id="18e5e-107">تعيين المشروع والمهمة</span><span class="sxs-lookup"><span data-stu-id="18e5e-107">Project and task mapping</span></span>
- <span data-ttu-id="18e5e-108">فئات الحركات المضمنة</span><span class="sxs-lookup"><span data-stu-id="18e5e-108">Included transaction classes</span></span>
- <span data-ttu-id="18e5e-109">حد يجب عدم تجاوزه</span><span class="sxs-lookup"><span data-stu-id="18e5e-109">Not-to-exceed limit</span></span>
- <span data-ttu-id="18e5e-110">إعداد الخضوع للرسوم</span><span class="sxs-lookup"><span data-stu-id="18e5e-110">Chargeability setup</span></span>
- <span data-ttu-id="18e5e-111">التقديرات باستخدام تفاصيل شروط التعاقد</span><span class="sxs-lookup"><span data-stu-id="18e5e-111">Estimates using contract line details</span></span>
- <span data-ttu-id="18e5e-112">عملاء شروط التعاقد</span><span class="sxs-lookup"><span data-stu-id="18e5e-112">Contract line customers</span></span>

<span data-ttu-id="18e5e-113">تم تضمين الحقول التالية في علامة التبويب **عام** لشروط التعاقد القائمة على المشروع.</span><span class="sxs-lookup"><span data-stu-id="18e5e-113">The following fields are included on the **General** tab of project–based contract lines.</span></span> <span data-ttu-id="18e5e-114">تساعد هذه الحقول على إعداد أساس لتقدير تفصيلي وشامل وترتيبات الفوترة للعمل القائم على المشروع.</span><span class="sxs-lookup"><span data-stu-id="18e5e-114">These fields help to set up the basis for a detailed, ground–up estimate and the billing arrangements for project–based work.</span></span>

| <span data-ttu-id="18e5e-115">الحقل</span><span class="sxs-lookup"><span data-stu-id="18e5e-115">Field</span></span> | <span data-ttu-id="18e5e-116">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="18e5e-116">Description</span></span> | <span data-ttu-id="18e5e-117">تأثير لاحق</span><span class="sxs-lookup"><span data-stu-id="18e5e-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="18e5e-118">**الاسم**</span><span class="sxs-lookup"><span data-stu-id="18e5e-118">**Name**</span></span> | <span data-ttu-id="18e5e-119">اسم شرط التعاقد الذي يحدد المكون المنفصل للعقد الجاري تقديره.</span><span class="sxs-lookup"><span data-stu-id="18e5e-119">The name of the contract line that identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="18e5e-120">بالنسبة لعقد مشروع تم إنشاؤه من عرض أسعار، يتم نسخ هذه القيمة من قيمة مقابلة لبند عرض أسعار قائم على المشروع.</span><span class="sxs-lookup"><span data-stu-id="18e5e-120">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="18e5e-121">يتم نسخ قيمة الحقل هذه إلى بند فاتورة المشروع الذي تم إنشاؤه من شرط التعاقد هذا عند إنشاء الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-121">This field value is copied to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="18e5e-122">**أسلوب الفوترة**</span><span class="sxs-lookup"><span data-stu-id="18e5e-122">**Billing Method**</span></span> | <span data-ttu-id="18e5e-123">على عقد مشروع تم إنشاؤه من عرض أسعار، يتم نسخ هذه القيمة من الحقل المقابل على بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="18e5e-123">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="18e5e-124">هذه مجموعة خيارات تمثل نموذجي التعاقد الرئيسيين المدعومين من Project Operations:</span><span class="sxs-lookup"><span data-stu-id="18e5e-124">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="18e5e-125">- **سعر ثابت**</span><span class="sxs-lookup"><span data-stu-id="18e5e-125">- **Fixed Price**</span></span></br><span data-ttu-id="18e5e-126">- **الوقت والمادة**</span><span class="sxs-lookup"><span data-stu-id="18e5e-126">- **Time and Material**</span></span> | <span data-ttu-id="18e5e-127">بالاستناد إلى أسلوب الفوترة لشرط التعاقد المشار إليه، ستتم معالجة الحركة الفعلية.</span><span class="sxs-lookup"><span data-stu-id="18e5e-127">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="18e5e-128">إذا كان شرط التعاقد الذي تشير إليه القيمة الفعلية يتضمن أسلوب فوترة الوقت والمواد، سيتم إنشاء سجل القيمة الفعلية للتكلفة غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-128">If the contract line referenced by the actual has a time and material billing method, a cost and an unbilled sales actual record are created.</span></span> <span data-ttu-id="18e5e-129">إذا كان شرط التعاقد الذي تشير إليه القيمة الفعلية يتضمن أسلوب فوترة بسعر ثابت، سيتم إنشاء قيمة فعلية للتكلفة فقط.</span><span class="sxs-lookup"><span data-stu-id="18e5e-129">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="18e5e-130">**Project**</span><span class="sxs-lookup"><span data-stu-id="18e5e-130">**Project**</span></span> | <span data-ttu-id="18e5e-131">استخدم هذا الحقل لتحديد المشروع الذي سيتم استخدامه لتقديم العمل على هذا الالتزام.</span><span class="sxs-lookup"><span data-stu-id="18e5e-131">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="18e5e-132">يتم استخدام القيمة الموجودة في هذا الحقل بالتزامن مع الحقلين **المهام المضمنة** و **فئات الحركات المضمنة** لحل مرجع شروط التعاقد في سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="18e5e-132">The value in this field is used in conjunction with **Included Tasks** and **Included Transaction Classes** fields to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="18e5e-133">**تضمين الوقت**</span><span class="sxs-lookup"><span data-stu-id="18e5e-133">**Include Time**</span></span> | <span data-ttu-id="18e5e-134">تشير علامة إلى تضمين حركات الوقت أو تكاليف العمالة في المشروع المحدد على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="18e5e-134">A flag indicates if time transactions or labor costs on the selected project are included on this contract line.</span></span> <span data-ttu-id="18e5e-135">تشير القيمة **لا** إلى أنه لن يتم تضمين حركات الوقت أو تكاليف العمالة على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="18e5e-135">A **No** value indicates that the time transactions or labor costs will not be included on this contract line.</span></span> <span data-ttu-id="18e5e-136">تشير القيمة **نعم** إلى تضمينها.</span><span class="sxs-lookup"><span data-stu-id="18e5e-136">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="18e5e-137">يتم استخدام قيمة الحقل هذه بالتزامن مع المشروع لحل مرجع شروط التعاقد في سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="18e5e-137">This field value is used in conjunction with project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="18e5e-138">**يتضمن المصروفات**</span><span class="sxs-lookup"><span data-stu-id="18e5e-138">**Include Expense**</span></span> | <span data-ttu-id="18e5e-139">تشير علامة إلى تضمين تكاليف المصروفات في المشروع المحدد على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="18e5e-139">A flag indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="18e5e-140">تشير القيمة **لا** إلى أنه لن يتم تضمين تكاليف المصروفات على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="18e5e-140">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="18e5e-141">تشير القيمة **نعم** إلى تضمينها.</span><span class="sxs-lookup"><span data-stu-id="18e5e-141">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="18e5e-142">يتم استخدام قيمة الحقل هذه مع المشروع لحل مرجع شروط التعاقد في سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="18e5e-142">This field value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="18e5e-143">**تضمين الرسوم**</span><span class="sxs-lookup"><span data-stu-id="18e5e-143">**Include Fee**</span></span> | <span data-ttu-id="18e5e-144">تشير علامة إلى تضمين الرسوم في المشروع المحدد على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="18e5e-144">A flag indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="18e5e-145">تشير القيمة **لا** إلى أنه لن يتم تضمين الرسوم على شرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="18e5e-145">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="18e5e-146">تشير القيمة **نعم** إلى تضمينها.</span><span class="sxs-lookup"><span data-stu-id="18e5e-146">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="18e5e-147">يتم استخدام قيمة الحقل هذه مع المشروع لحل مرجع شروط التعاقد في سجل بند قيمة فعلية أو تقدير.</span><span class="sxs-lookup"><span data-stu-id="18e5e-147">This field value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="18e5e-148">**المبلغ المتعاقد عليه**</span><span class="sxs-lookup"><span data-stu-id="18e5e-148">**Contracted Amount**</span></span> | <span data-ttu-id="18e5e-149">على شرط تعاقد بسعر ثابت، هذه القيمة هي القيمة المتفق عليها التي ستتم فوترتها على العميل لكافة مكونات العمل المقترنة بشرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="18e5e-149">On a fixed price contract line, this is the agreed-on value that will be invoiced to the customer for all the work components associated with this contract line.</span></span> <span data-ttu-id="18e5e-150">على شرط تعاقد الوقت والمواد، هذا المبلغ هو قيمة مقدرة لما ستتم فوترته على العميل لكافة مكونات العمل المقترنة بشرط التعاقد هذا.</span><span class="sxs-lookup"><span data-stu-id="18e5e-150">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="18e5e-151">على عقد مشروع تم إنشاؤه من عرض أسعار، يتم نسخ هذه القيمة من الحقل المقابل على بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="18e5e-151">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="18e5e-152">عندما يتضمن شرط تعاقد قائم على المشروع تفاصيل البند، يتم تأمين هذا الحقل للتحرير ويتم تلخيصه من المبلغ على تفاصيل شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="18e5e-152">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="18e5e-153">عندما يتضمن شرط التعاقد تفاصيل البند، يمكن تعديل هذه القيمة عن طريق تغيير المبالغ على تفاصيل البند.</span><span class="sxs-lookup"><span data-stu-id="18e5e-153">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="18e5e-154">على شرط تعاقد بسعر ثابت، يتم استخدام هذه القيمة لإنشاء المبلغ قبل الضريبة على المراحل الرئيسية للفوترة الدورية.</span><span class="sxs-lookup"><span data-stu-id="18e5e-154">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="18e5e-155">**الضريبة المقدرة**</span><span class="sxs-lookup"><span data-stu-id="18e5e-155">**Estimated Tax**</span></span> | <span data-ttu-id="18e5e-156">يمكن للمستخدم تحرير هذا الحقل لإدخال مبلغ الضريبة المقدرة في شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="18e5e-156">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="18e5e-157">عندما يتضمن شرط تعاقد قائم على المشروع تفاصيل البند، يتم تأمين هذا الحقل للتحرير ويتم تلخيصه من مبلغ الضريبة على تفاصيل شرط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="18e5e-157">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="18e5e-158">عندما يتضمن شرط التعاقد تفاصيل البند، يمكن تعديل هذه القيمة عن طريق تغيير مبالغ الضريبة على تفاصيل البند.</span><span class="sxs-lookup"><span data-stu-id="18e5e-158">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="18e5e-159">على شرط تعاقد بسعر ثابت، يتم استخدام هذه القيمة لإنشاء الضريبة على المراحل الرئيسية للفوترة الدورية.</span><span class="sxs-lookup"><span data-stu-id="18e5e-159">On a fixed price contract line, this value is used to generate tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="18e5e-160">**‏‫المبلغ المتعاقد عليه‬ بعد الضريبة**</span><span class="sxs-lookup"><span data-stu-id="18e5e-160">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="18e5e-161">‏‫مبلغ شرط التعاقد‬ بعد الضريبة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-161">The contract line amount after tax.</span></span> <span data-ttu-id="18e5e-162">هذا الحقل للقراءة فقط ويتم حسابه على أنه **مبلغ متعاقد عليه + ضريبة**.</span><span class="sxs-lookup"><span data-stu-id="18e5e-162">This field is read-only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="18e5e-163">على شرط تعاقد بسعر ثابت، يتم استخدام هذه القيمة لإنشاء المراحل الرئيسية للفوترة الدورية.</span><span class="sxs-lookup"><span data-stu-id="18e5e-163">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="18e5e-164">**حد يجب عدم تجاوزه**</span><span class="sxs-lookup"><span data-stu-id="18e5e-164">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="18e5e-165">يمكن للمستخدم تحرير هذا الحقل ويكون متاحًا فقط في شروط التعاقد القائمة على المشروع والتي لها أسلوب فوترة الوقت والمواد.</span><span class="sxs-lookup"><span data-stu-id="18e5e-165">The user can edit this field and it is only available on project-based contract lines that have a time and material billing method.</span></span> | <span data-ttu-id="18e5e-166">يمكن للمستخدم تحرير هذا الحقل.</span><span class="sxs-lookup"><span data-stu-id="18e5e-166">The user can edit this field.</span></span> <span data-ttu-id="18e5e-167">عندما تشير قيمة فعلية للوقت أو المصروفات إلى شرط التعاقد هذا للوقت والمواد، يتم تقييم المبلغ على القيمة الفعلية مقابل الحد الذي يجب عدم تجاوزه في شرط التعاقد هذا بعد حساب للمبالغ التي تم إنفاقها والمبالغ الملتزم بها.</span><span class="sxs-lookup"><span data-stu-id="18e5e-167">When a time or expense actual references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on this contract line after accounting for the already spent and committed amounts.</span></span> |
| <span data-ttu-id="18e5e-168">**موازنة العميل**</span><span class="sxs-lookup"><span data-stu-id="18e5e-168">**Customer Budget**</span></span> | <span data-ttu-id="18e5e-169">هذا الحقل قابل للتحرير ويتم نسخه من الحقل المقابل على بند عرض الأسعار، إذا تم إنشاء العقد من عرض أسعار.</span><span class="sxs-lookup"><span data-stu-id="18e5e-169">This field is editable and is copied from the corresponding field on the quote line, if the contract was created from a quote.</span></span> | <span data-ttu-id="18e5e-170">يُستخدم هذا الحقل للمعلومات فقط ولا يتضمن أي دلالة لاحقة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-170">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rule-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="18e5e-171">قاعدة التحقق من الصحة للخيارات الموجودة في علامة التبويب "عام" في شروط التعاقد القائمة على المشروع</span><span class="sxs-lookup"><span data-stu-id="18e5e-171">Validation rule for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="18e5e-172">القاعدة: يمكن تضمين مشروع وفئة حركة معينة في شرط تعاقد واحد قائم على مشروع في عقد.</span><span class="sxs-lookup"><span data-stu-id="18e5e-172">Rule: A project and a certain transaction class can only be included on one project-based contract line in a contract.</span></span>

| <span data-ttu-id="18e5e-173">عقد</span><span class="sxs-lookup"><span data-stu-id="18e5e-173">Contract</span></span> | <span data-ttu-id="18e5e-174">شروط التعاقد</span><span class="sxs-lookup"><span data-stu-id="18e5e-174">Contract line</span></span> | <span data-ttu-id="18e5e-175">Project</span><span class="sxs-lookup"><span data-stu-id="18e5e-175">Project</span></span> | <span data-ttu-id="18e5e-176">تضمين الوقت</span><span class="sxs-lookup"><span data-stu-id="18e5e-176">Include time</span></span> | <span data-ttu-id="18e5e-177">تضمين المصروفات</span><span class="sxs-lookup"><span data-stu-id="18e5e-177">Include expense</span></span> | <span data-ttu-id="18e5e-178">تضمين الرسوم</span><span class="sxs-lookup"><span data-stu-id="18e5e-178">Include fee</span></span> | <span data-ttu-id="18e5e-179">صالح/غير صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-179">Valid/not valid</span></span> | <span data-ttu-id="18e5e-180">السبب</span><span class="sxs-lookup"><span data-stu-id="18e5e-180">Reason</span></span>                                                                                                                                                                                                  |
|----------|---------------|---------|--------------|-----------------|-------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="18e5e-181">C1</span><span class="sxs-lookup"><span data-stu-id="18e5e-181">C1</span></span>       | <span data-ttu-id="18e5e-182">CL1</span><span class="sxs-lookup"><span data-stu-id="18e5e-182">CL1</span></span>           | <span data-ttu-id="18e5e-183">P1</span><span class="sxs-lookup"><span data-stu-id="18e5e-183">P1</span></span>      | <span data-ttu-id="18e5e-184">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-184">Yes</span></span>          | <span data-ttu-id="18e5e-185">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-185">Yes</span></span>             | <span data-ttu-id="18e5e-186">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-186">Yes</span></span>         | <span data-ttu-id="18e5e-187">غير صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-187">Not valid</span></span>       | <span data-ttu-id="18e5e-188">انتهاك القاعدة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-188">Violates the rule.</span></span> <span data-ttu-id="18e5e-189">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 على شرطي التعاقد، CL1 وCL2.</span><span class="sxs-lookup"><span data-stu-id="18e5e-189">Time,   expense, and fees on project P1 are included on both contract lines, CL1 and   CL2.</span></span>                                                                                       |
| <span data-ttu-id="18e5e-190">C1</span><span class="sxs-lookup"><span data-stu-id="18e5e-190">C1</span></span>       | <span data-ttu-id="18e5e-191">CL2</span><span class="sxs-lookup"><span data-stu-id="18e5e-191">CL2</span></span>           | <span data-ttu-id="18e5e-192">P1</span><span class="sxs-lookup"><span data-stu-id="18e5e-192">P1</span></span>      | <span data-ttu-id="18e5e-193">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-193">Yes</span></span>          | <span data-ttu-id="18e5e-194">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-194">Yes</span></span>             | <span data-ttu-id="18e5e-195">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-195">Yes</span></span>         | <span data-ttu-id="18e5e-196">غير صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-196">Not valid</span></span>       | <span data-ttu-id="18e5e-197">انتهاك القاعدة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-197">Violates the rule.</span></span> <span data-ttu-id="18e5e-198">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 على شرطي التعاقد، CL1 وCL2.</span><span class="sxs-lookup"><span data-stu-id="18e5e-198">Time,   expense, and fees on project P1 are included on both contract lines, CL1 and   CL2.</span></span>                                                                                       |
| <span data-ttu-id="18e5e-199">C1</span><span class="sxs-lookup"><span data-stu-id="18e5e-199">C1</span></span>       | <span data-ttu-id="18e5e-200">CL1</span><span class="sxs-lookup"><span data-stu-id="18e5e-200">CL1</span></span>           | <span data-ttu-id="18e5e-201">P1</span><span class="sxs-lookup"><span data-stu-id="18e5e-201">P1</span></span>      | <span data-ttu-id="18e5e-202">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-202">Yes</span></span>          | <span data-ttu-id="18e5e-203">Yes</span><span class="sxs-lookup"><span data-stu-id="18e5e-203">No</span></span>              | <span data-ttu-id="18e5e-204">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-204">Yes</span></span>         | <span data-ttu-id="18e5e-205">غير صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-205">Not valid</span></span>       | <span data-ttu-id="18e5e-206">انتهاك القاعدة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-206">Violates the rule.</span></span> <span data-ttu-id="18e5e-207">يتم تضمين الوقت والرسوم في المشروع P1 على شرطي التعاقد، CL1 وCL2.</span><span class="sxs-lookup"><span data-stu-id="18e5e-207">Time and   fees on project P1 are included on both contract lines, CL1 and CL2.</span></span>                                                                                                   |
| <span data-ttu-id="18e5e-208">C1</span><span class="sxs-lookup"><span data-stu-id="18e5e-208">C1</span></span>       | <span data-ttu-id="18e5e-209">CL2</span><span class="sxs-lookup"><span data-stu-id="18e5e-209">CL2</span></span>           | <span data-ttu-id="18e5e-210">P1</span><span class="sxs-lookup"><span data-stu-id="18e5e-210">P1</span></span>      | <span data-ttu-id="18e5e-211">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-211">Yes</span></span>          | <span data-ttu-id="18e5e-212">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-212">Yes</span></span>             | <span data-ttu-id="18e5e-213">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-213">Yes</span></span>         | <span data-ttu-id="18e5e-214">غير صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-214">Not valid</span></span>       | <span data-ttu-id="18e5e-215">انتهاك القاعدة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-215">Violates the rule.</span></span> <span data-ttu-id="18e5e-216">يتم تضمين الوقت والرسوم في المشروع P1 على شرطي التعاقد، CL1 وCL2.</span><span class="sxs-lookup"><span data-stu-id="18e5e-216">Time and   fees on project P1 are included on both contract lines, CL1 and CL2.</span></span>                                                                                                   |
| <span data-ttu-id="18e5e-217">C1</span><span class="sxs-lookup"><span data-stu-id="18e5e-217">C1</span></span>       | <span data-ttu-id="18e5e-218">CL1</span><span class="sxs-lookup"><span data-stu-id="18e5e-218">CL1</span></span>           | <span data-ttu-id="18e5e-219">P1</span><span class="sxs-lookup"><span data-stu-id="18e5e-219">P1</span></span>      | <span data-ttu-id="18e5e-220">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-220">Yes</span></span>          | <span data-ttu-id="18e5e-221">Yes</span><span class="sxs-lookup"><span data-stu-id="18e5e-221">No</span></span>              | <span data-ttu-id="18e5e-222">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-222">Yes</span></span>         | <span data-ttu-id="18e5e-223">صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-223">Valid</span></span>           | <span data-ttu-id="18e5e-224">يتم تضمين الوقت والرسوم في المشروع P1 على CL1.</span><span class="sxs-lookup"><span data-stu-id="18e5e-224">Time and fees on project P1 are   included on the CL1.</span></span> <span data-ttu-id="18e5e-225">يتم تضمين المصروفات في المشروع P1 على CL2.</span><span class="sxs-lookup"><span data-stu-id="18e5e-225">Expense on project P1 is included on CL2.</span></span> </br>   <span data-ttu-id="18e5e-226">لا يوجد تداخل بين ما تم تضمينه في كل شرط تعاقد، وبالتالي هو صالح.</span><span class="sxs-lookup"><span data-stu-id="18e5e-226">There is no overlap in what is being included on each contract line and is   therefore valid.</span></span>  |
| <span data-ttu-id="18e5e-227">C1</span><span class="sxs-lookup"><span data-stu-id="18e5e-227">C1</span></span>       | <span data-ttu-id="18e5e-228">CL2</span><span class="sxs-lookup"><span data-stu-id="18e5e-228">CL2</span></span>           | <span data-ttu-id="18e5e-229">P1</span><span class="sxs-lookup"><span data-stu-id="18e5e-229">P1</span></span>      | <span data-ttu-id="18e5e-230">Yes</span><span class="sxs-lookup"><span data-stu-id="18e5e-230">No</span></span>           | <span data-ttu-id="18e5e-231">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-231">Yes</span></span>             | <span data-ttu-id="18e5e-232">Yes</span><span class="sxs-lookup"><span data-stu-id="18e5e-232">No</span></span>          | <span data-ttu-id="18e5e-233">صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-233">Valid</span></span>           | <span data-ttu-id="18e5e-234">يتم تضمين الوقت والرسوم في المشروع P1 على CL1.</span><span class="sxs-lookup"><span data-stu-id="18e5e-234">Time and fees on project P1 are   included on the CL1.</span></span> <span data-ttu-id="18e5e-235">يتم تضمين المصروفات في المشروع P1 على CL2.</span><span class="sxs-lookup"><span data-stu-id="18e5e-235">Expense on project P1 is included on CL2.</span></span> </br>   <span data-ttu-id="18e5e-236">لا يوجد تداخل بين ما تم تضمينه في كل شرط تعاقد، وبالتالي هو صالح.</span><span class="sxs-lookup"><span data-stu-id="18e5e-236">There is no overlap in what is being included on each contract line and is   therefore valid.</span></span>  |
| <span data-ttu-id="18e5e-237">C1</span><span class="sxs-lookup"><span data-stu-id="18e5e-237">C1</span></span>       | <span data-ttu-id="18e5e-238">CL1</span><span class="sxs-lookup"><span data-stu-id="18e5e-238">CL1</span></span>           | <span data-ttu-id="18e5e-239">P1</span><span class="sxs-lookup"><span data-stu-id="18e5e-239">P1</span></span>      | <span data-ttu-id="18e5e-240">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-240">Yes</span></span>          | <span data-ttu-id="18e5e-241">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-241">Yes</span></span>             | <span data-ttu-id="18e5e-242">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-242">Yes</span></span>         | <span data-ttu-id="18e5e-243">غير صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-243">Not valid</span></span>       | <span data-ttu-id="18e5e-244">انتهاك القاعدة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-244">Violates the rule.</span></span> <span data-ttu-id="18e5e-245">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 على بنود عقدين.</span><span class="sxs-lookup"><span data-stu-id="18e5e-245">Time,   expense, and fees on project P1 are included on the lines of two contracts.</span></span>                                                                                               |
| <span data-ttu-id="18e5e-246">CL2</span><span class="sxs-lookup"><span data-stu-id="18e5e-246">CL2</span></span>      | <span data-ttu-id="18e5e-247">CL2</span><span class="sxs-lookup"><span data-stu-id="18e5e-247">CL2</span></span>           | <span data-ttu-id="18e5e-248">P1</span><span class="sxs-lookup"><span data-stu-id="18e5e-248">P1</span></span>      | <span data-ttu-id="18e5e-249">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-249">Yes</span></span>          | <span data-ttu-id="18e5e-250">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-250">Yes</span></span>             | <span data-ttu-id="18e5e-251">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="18e5e-251">Yes</span></span>         | <span data-ttu-id="18e5e-252">غير صالح</span><span class="sxs-lookup"><span data-stu-id="18e5e-252">Not valid</span></span>       | <span data-ttu-id="18e5e-253">انتهاك القاعدة.</span><span class="sxs-lookup"><span data-stu-id="18e5e-253">Violates the rule.</span></span> <span data-ttu-id="18e5e-254">يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 على بنود عقدين.</span><span class="sxs-lookup"><span data-stu-id="18e5e-254">Time,   expense, and fees on project P1 are included on the lines of two contracts.</span></span>                                                                                               |