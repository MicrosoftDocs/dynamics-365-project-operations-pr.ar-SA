---
title: تكوين إدارة المصروفات
description: توضح هذه المقالة الاعتبارات والقرارات التي يجب اتخاذها أثناء عملية التخطيط قبل تكوين إدارة المصروفات في Microsoft Dynamics 365 Finance.
author: KimANelson
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 52538946c7260fad4076a64e8dc34fecf08b90cf
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005370"
---
# <a name="configure-expense-management"></a><span data-ttu-id="91010-103">تكوين إدارة المصروفات</span><span class="sxs-lookup"><span data-stu-id="91010-103">Configure expense management</span></span>

<span data-ttu-id="91010-104">يصف هذا الموضوع الاعتبارات والقرارات التي يجب اتخاذها أثناء عملية التخطيط قبل تكوين إدارة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="91010-104">This topic describes the considerations and the decisions that you must make during the planning process before you configure Expense management.</span></span> <span data-ttu-id="91010-105">في إدارة المصروفات، يمكنك تخزين معلومات حول طرق الدفع وطلبات السفر وتقارير المصروفات والسياسات وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="91010-105">In Expense management, you can store information about payment methods, travel requisitions, expense reports, policies, and so on.</span></span>

<span data-ttu-id="91010-106">لأن الكثير من القرارات التي تتخذها عندما تخطط لتكوين إدارة المصروفات تستند إلى التدرج الهرمي والبنية المالية لمؤسستك، يجب عليك الرجوع إلى مستندات التخطيط الخاصة بهذه النواحي.</span><span class="sxs-lookup"><span data-stu-id="91010-106">Because many of the decisions that you make when you plan your configuration for Expense management are based on your organization’s hierarchy and financial structure, you must refer to the planning documents for those areas.</span></span>

## <a name="intercompany-expenses"></a><span data-ttu-id="91010-107">المصروفات بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="91010-107">Intercompany expenses</span></span>

<span data-ttu-id="91010-108">عندما تقوم بتمكين المصروفات بين الشركات الشقيقة، فأنت تتيح للكيانات القانونية والموظفين بتحمل المصروفات نيابة عن كيان قانوني آخر، وتحصيل المدفوعات من الكيان القانوني الخاص بالتوظيف داخل مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="91010-108">When you enable intercompany expenses, you allow legal entities and employees to incur expenses on behalf of another legal entity, and collect payment from the legal entity of employment within your organization.</span></span> <span data-ttu-id="91010-109">على سبيل المثال، يقوم موظف في الكيان القانوني A بإكمال مشروع للكيان القانوني B، ويتحمل المشروع المصروفات المرتبطة بالسفر.</span><span class="sxs-lookup"><span data-stu-id="91010-109">For example, an employee in legal entity A completes a project for legal entity B, and the project incurs travel related expenses.</span></span> <span data-ttu-id="91010-110">إذا تم تمكين المصروفات بين الشركات الشقيقة، يمكن للموظف بعد ذلك إنشاء تقرير مصروفات يقوم بترحيل المصروفات إلى الكيان القانوني B، ويجب بعد ذلك دفع المصروفات من خلال الكيان القانوني A. إذا لم تكن مؤسستك تشتمل على العديد من الكيانات القانونية، فلست بحاجة إلى تمكين المصروفات بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="91010-110">If intercompany expenses are enabled, the employee can then file an expense report that will post the expense to legal entity B, and the expense must then be paid by legal entity A. If your organization doesn’t have multiple legal entities, you don’t have to enable intercompany expenses.</span></span>

<span data-ttu-id="91010-111">**القرار:** هل تريد تمكين المصروفات بين الشركات الشقيقة؟</span><span class="sxs-lookup"><span data-stu-id="91010-111">**Decision:** Do you want to enable intercompany expenses?</span></span>

## <a name="financial-management"></a><span data-ttu-id="91010-112">الإدارة المالية</span><span class="sxs-lookup"><span data-stu-id="91010-112">Financial management</span></span>

<span data-ttu-id="91010-113">تتكامل إدارة المصروفات بشكل محكم مع الإدارة المالية لمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="91010-113">Expense management is tightly integrated with the financial management of your organization.</span></span> <span data-ttu-id="91010-114">سيستند عدد كبير من تكوينات إدارة المصروفات إلى القرارات التي اتخذتها حول الشؤون المالية لمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="91010-114">Lots of your configuration for Expense management will be based on the decisions that you’ve made about your organization’s finances.</span></span> <span data-ttu-id="91010-115">تصف الأقسام التالية النواحي المختلفة التي تتطلب التخطيط والقرارات، استنادًا إلى القرارات المالية لمؤسستك وإرشادات من فريق القيادة.</span><span class="sxs-lookup"><span data-stu-id="91010-115">The following sections describe the various areas that require planning and decisions, based on your organization’s financial decisions and guidance from your leadership team.</span></span>

### <a name="per-diems"></a><span data-ttu-id="91010-116">المصروفات اليومية</span><span class="sxs-lookup"><span data-stu-id="91010-116">Per diems</span></span>

<span data-ttu-id="91010-117">يجب تحديد الموظف لكل المصروفات اليومية التي توفرها مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="91010-117">You must define the employee per diems that your organization provides.</span></span> <span data-ttu-id="91010-118">نظرًا لاستخدام المصروفات اليومية عادةً لتغطية المصروفات مثل الوجبات والإقامة وبعض المصروفات العرضية الأخرى، يمكنك إنشاء قواعد لبدلات المصروفات اليومية التي تقدمها مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="91010-118">Because per diems are typically used to cover expenses such as meals, lodging, and other incidental expenses, you can create rules for the per diem allowances that your organization offers.</span></span> <span data-ttu-id="91010-119">بإمكان معدلات المصروفات اليومية أن تستند إلى الوقت من السنة أو موقع السفر أو كليهما.</span><span class="sxs-lookup"><span data-stu-id="91010-119">per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="91010-120">عندما تحدد قاعدة للمصروفات اليومية، يمكنك تحديد أنه سيتم اقتطاع نسبة مئوية لمعدل المصروفات اليومية إذا تلقى العام وجبات أو خدمات مجانية.</span><span class="sxs-lookup"><span data-stu-id="91010-120">When you define a per diem rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="91010-121">يمكنك أيضا تعيين معدل المصروفات اليومية لتعيين الحد الأدنى والحد الأقصى لعدد الساعات التي يمكن لكل معدل مصروفات يومية يمكن تطبيقه على سفر العامل.</span><span class="sxs-lookup"><span data-stu-id="91010-121">You can also define per diem rate tiers to set the minimum and maximum number of hours that the per diem rate can be applied to a worker’s travel.</span></span>

<span data-ttu-id="91010-122">**القرارات:**</span><span class="sxs-lookup"><span data-stu-id="91010-122">**Decisions:**</span></span>

- <span data-ttu-id="91010-123">قواعد المصروفات اليومية الافتراضية لليومين الأول والأخير:</span><span class="sxs-lookup"><span data-stu-id="91010-123">Default per diem rules for the first and last days:</span></span>

    - <span data-ttu-id="91010-124">ما هو الحد الأدنى لعدد الساعات التي يمكن لأحد الموظفين المطالبة بها ليوم ما واستمرار استلام المصروف اليومي؟</span><span class="sxs-lookup"><span data-stu-id="91010-124">What is the minimum number of hours that an employee can claim for a day and still receive a per diem?</span></span>
    - <span data-ttu-id="91010-125">هل هناك تخفيض في المبلغ المقدم لوجبات الطعام لليومين الأول والأخير؟</span><span class="sxs-lookup"><span data-stu-id="91010-125">Is there a reduction in the amount that is offered for meals for the first day and last day?</span></span> <span data-ttu-id="91010-126">في حاله وجود تخفيض، ما النسبة المئوية للتخفيض؟</span><span class="sxs-lookup"><span data-stu-id="91010-126">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="91010-127">هل هناك تخفيض في المبلغ المقدم للفندق لليومين الأول والأخير؟</span><span class="sxs-lookup"><span data-stu-id="91010-127">Is there a reduction in the amount that is offered for a hotel for the first day and last day?</span></span> <span data-ttu-id="91010-128">في حاله وجود تخفيض، ما النسبة المئوية للتخفيض؟</span><span class="sxs-lookup"><span data-stu-id="91010-128">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="91010-129">هل هناك تخفيض في المبلغ المقدم للمصروفات الأخرى التي يتم تحملها لليومين الأول والأخير؟</span><span class="sxs-lookup"><span data-stu-id="91010-129">Is there a reduction in the amount that is offered for other expenses that are incurred on the first day and last day?</span></span> <span data-ttu-id="91010-130">في حاله وجود تخفيض، ما النسبة المئوية للتخفيض؟</span><span class="sxs-lookup"><span data-stu-id="91010-130">If there is a reduction, what is the percentage of the reduction?</span></span>

- <span data-ttu-id="91010-131">قواعد المصروفات اليومية الافتراضية:</span><span class="sxs-lookup"><span data-stu-id="91010-131">Default per diem rules:</span></span>

    - <span data-ttu-id="91010-132">هل هناك نسبة تخفيض في بدل المصروفات اليومية لكل وجبة إذا كانت الوجبة مجانية على سبيل المثال؟</span><span class="sxs-lookup"><span data-stu-id="91010-132">Is there a percentage reduction in the per diem allowance for each meal if, for example, the meal is complimentary?</span></span> <span data-ttu-id="91010-133">في حاله وجود تخفيض، ما النسبة المئوية للتخفيض لكل وجبة؟</span><span class="sxs-lookup"><span data-stu-id="91010-133">If there is a reduction, what is the reduction percentage for each meal?</span></span>
    - <span data-ttu-id="91010-134">هل يتم احتساب تخفيض الوجبات لكل يوم أو لكل رحلة أو حسب عدد الوجبات في اليوم؟</span><span class="sxs-lookup"><span data-stu-id="91010-134">Is the meal reduction calculated per day, per trip, or by the number of meals per day?</span></span>
    - <span data-ttu-id="91010-135">هل يتعين تقريب مبالغ المصروفات اليومية بالطريقة العادية أم تقريبها لأعلى؟</span><span class="sxs-lookup"><span data-stu-id="91010-135">Should per diem amounts be rounded in the regular manner or rounded up?</span></span>
    - <span data-ttu-id="91010-136">هل يتم احتساب المصروفات اليومية استنادًا إلى فترة 24 ساعة أو يوم تقويم؟</span><span class="sxs-lookup"><span data-stu-id="91010-136">Are per diems calculated on a 24-hour period or on a calendar day?</span></span>

- <span data-ttu-id="91010-137">قواعد المصروفات اليومية التي تستند إلى الموقع:</span><span class="sxs-lookup"><span data-stu-id="91010-137">Per diem rules that are based on location:</span></span>

    - <span data-ttu-id="91010-138">هل تختلف معدلات المصروفات اليومية وفقًا للموقع؟</span><span class="sxs-lookup"><span data-stu-id="91010-138">Do per diem rates vary according to location?</span></span> <span data-ttu-id="91010-139">ما المواقع المضمنة؟</span><span class="sxs-lookup"><span data-stu-id="91010-139">What locations are included?</span></span>
    - <span data-ttu-id="91010-140">إذا اختلفت معدلات المصروفات اليومية وفقًا للموقع، لكل موقع، ما مبلغ النسبة المئوية الذي يتم توفرها لأنواع المصروفات التالية:</span><span class="sxs-lookup"><span data-stu-id="91010-140">If per diem rates vary according to location, for each location, what percentage amount is provided for the following types of expenses:</span></span>

        - <span data-ttu-id="91010-141">الوجبات</span><span class="sxs-lookup"><span data-stu-id="91010-141">Meals</span></span>
        - <span data-ttu-id="91010-142">فندق</span><span class="sxs-lookup"><span data-stu-id="91010-142">Hotel</span></span>
        - <span data-ttu-id="91010-143">مصروفات أخرى</span><span class="sxs-lookup"><span data-stu-id="91010-143">Other expenses</span></span>

### <a name="expense-management-journals-and-accounts"></a><span data-ttu-id="91010-144">حسابات ودفاتر يومية إدارة المصروفات</span><span class="sxs-lookup"><span data-stu-id="91010-144">Expense management journals and accounts</span></span>

<span data-ttu-id="91010-145">تتطلب إدارة المصروفات استخدام العديد من دفاتر اليومية والحسابات.</span><span class="sxs-lookup"><span data-stu-id="91010-145">Expense management requires that you use multiple journals and accounts.</span></span> <span data-ttu-id="91010-146">يجب أن تقرر، على سبيل المثال، ما إذا كان سيتم استخدام الحساب نفسه للسلف النقدية ونزاعات بطاقات الائتمان.</span><span class="sxs-lookup"><span data-stu-id="91010-146">You must decide, for example, whether the same account is used for cash advances and credit card disputes.</span></span>

<span data-ttu-id="91010-147">**القرارات:**</span><span class="sxs-lookup"><span data-stu-id="91010-147">**Decisions:**</span></span>

- <span data-ttu-id="91010-148">ما دفتر يومية دفتر الأستاذ حيث يتم ترحيل تقارير المصروفات الموافق عليها؟</span><span class="sxs-lookup"><span data-stu-id="91010-148">Which ledger journal are approved expense reports posted to?</span></span>
- <span data-ttu-id="91010-149">ما الحساب المستخدم للسلف النقدية؟</span><span class="sxs-lookup"><span data-stu-id="91010-149">Which account is used for cash advances?</span></span>
- <span data-ttu-id="91010-150">هل سيتم ترحيل السلف النقدية على الفور؟</span><span class="sxs-lookup"><span data-stu-id="91010-150">Should cash advances be posted immediately?</span></span>

### <a name="payment-methods"></a><span data-ttu-id="91010-151">طرق الدفع</span><span class="sxs-lookup"><span data-stu-id="91010-151">Payment methods</span></span>

<span data-ttu-id="91010-152">عندما تسمح للموظفين بتحمل المصروفات نيابة عن شركاتك، يتعين عليك تحديد طرق الدفع المسموح للموظفين باستخدامها.</span><span class="sxs-lookup"><span data-stu-id="91010-152">When you allow employees to incur expenses on behalf of your business, you must define the payment methods that employees are allowed to use.</span></span> <span data-ttu-id="91010-153">على سبيل المثال، قد تسمح للموظفين باستخدام النقد أو بطاقة ائتمان الشركة.</span><span class="sxs-lookup"><span data-stu-id="91010-153">For example, you might allow employees to use cash or a corporate credit card.</span></span> <span data-ttu-id="91010-154">كما يمكنك السماح للموظفين باستخدام بطاقات الائتمان الشخصية، ثم تعويض الموظفين.</span><span class="sxs-lookup"><span data-stu-id="91010-154">You might also allow employees to use personal credit cards, and then reimburse the employees.</span></span> <span data-ttu-id="91010-155">يجب اتخاذ القرارات التالية لكل طريقة دفع تسمح لك بذلك.</span><span class="sxs-lookup"><span data-stu-id="91010-155">You must make the following decisions for each payment method that you allow.</span></span>

<span data-ttu-id="91010-156">**القرارات:**</span><span class="sxs-lookup"><span data-stu-id="91010-156">**Decisions:**</span></span>

- <span data-ttu-id="91010-157">ما هي طرق الدفع المسموح بها؟</span><span class="sxs-lookup"><span data-stu-id="91010-157">What payment methods are allowed?</span></span>
- <span data-ttu-id="91010-158">من الذي يمتلك مصروفات طريقة الدفع؟</span><span class="sxs-lookup"><span data-stu-id="91010-158">Who owns the payment method expenses?</span></span>
- <span data-ttu-id="91010-159">هل هناك نوع حساب مقابل؟</span><span class="sxs-lookup"><span data-stu-id="91010-159">Is there an offset account type?</span></span> <span data-ttu-id="91010-160">إذا كان هناك نوع حساب مقابل، فما هو؟</span><span class="sxs-lookup"><span data-stu-id="91010-160">If there is an offset account type, what is it?</span></span>
- <span data-ttu-id="91010-161">إذا كان هناك حساب مقابل، فما هو الحساب؟</span><span class="sxs-lookup"><span data-stu-id="91010-161">If there is an offset account, what is the account?</span></span>
- <span data-ttu-id="91010-162">إذا كانت طريقه الدفع بطاقة ائتمان، هل يتعين استخدام طريقة الدفع فقط مع الحركات المستوردة؟</span><span class="sxs-lookup"><span data-stu-id="91010-162">If the payment method is a credit card, should the payment method be used only with imported transactions?</span></span>

### <a name="expense-categories-and-shared-categories"></a><span data-ttu-id="91010-163">فئات المصروفات والفئات المشتركة</span><span class="sxs-lookup"><span data-stu-id="91010-163">Expense categories and shared categories</span></span>

<span data-ttu-id="91010-164">عندما يقوم الموظفون بإنشاء تقرير مصروفات، يجب أن يكون كل بند مصروفات يتم تسجيله مقترنًا بفئة مصروفات.</span><span class="sxs-lookup"><span data-stu-id="91010-164">When employees create an expense report, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="91010-165">يتم اشتقاق فئات المصروفات من الفئات المشتركة التي يمكن مشاركتها عبر الكيانات القانونية في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="91010-165">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="91010-166">يمكن أيضًا مشاركة هذه الفئات في إدارة المشروعات والمحاسبة، وذلك وفقًا للطريقة التي يتم بها تعريف مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="91010-166">These categories can also be shared in Project management and accounting, depending on the way that your organization is defined.</span></span> <span data-ttu-id="91010-167">وتبعًا لتعريف مؤسستك والإرشادات من فريق التنفيذ، يجب عليك تحديد ما إذا كان سيتم استخدام الفئات المستخدمة في إدارة المصروفات فقط في إدارة المصروفات أم يجب مشاركتها بين إدارة المشاريع والمحاسبة‬ وإدارة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="91010-167">Based on the definition of your organization and guidance from the implementation team, determine whether the categories that are used in Expense management will be used only in Expense management, or whether they should be shared between Project management and accounting and Expense management.</span></span> <span data-ttu-id="91010-168">لاحظ أنه يمكن مشاركة هذه الفئات بين إدارة المشروع والمصروفات أو المشروع والإنتاج وليس بين المصروفات والإنتاج.</span><span class="sxs-lookup"><span data-stu-id="91010-168">Note that these categories can be shared between Project and Expense or Project and Production, but not between Expense and Production.</span></span> <span data-ttu-id="91010-169">يجب اتخاذ القرارات التالية لكل فئة من فئات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="91010-169">You must make the following decisions for each expense category.</span></span>

<span data-ttu-id="91010-170">**القرارات:**</span><span class="sxs-lookup"><span data-stu-id="91010-170">**Decisions:**</span></span>

- <span data-ttu-id="91010-171">ما هي فئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-171">What is the expense category?</span></span> <span data-ttu-id="91010-172">وتتضمن الأمثلة فئات رحلات الطيران أو الفنادق أو الأميال.</span><span class="sxs-lookup"><span data-stu-id="91010-172">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="91010-173">هل يمكن أيضا استخدام فئة المصروفات في إدارة المشروع والمحاسبة؟</span><span class="sxs-lookup"><span data-stu-id="91010-173">Can the expense category also be used in Project management and accounting?</span></span>
- <span data-ttu-id="91010-174">ما هو نوع المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-174">What is the expense type?</span></span>
- <span data-ttu-id="91010-175">ما هي طريقة الدفع الافتراضية لفئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-175">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="91010-176">هل يجب تفصيل بنود المصروفات في فئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-176">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="91010-177">ما هو الحساب الرئيسي الافتراضي لفئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-177">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="91010-178">ما هي مجموعة ضريبة مبيعات الصنف الافتراضية لفئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-178">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="91010-179">هل يتم السماح بطرق دفع إضافية لفئة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-179">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="91010-180">عند وجود طرق دفع إضافية مسموحة، فما هي؟</span><span class="sxs-lookup"><span data-stu-id="91010-180">If additional payment methods are allowed, what are they?</span></span>
- <span data-ttu-id="91010-181">هل يوجد هناك فئات فرعية في فئة المصروفات هذه؟</span><span class="sxs-lookup"><span data-stu-id="91010-181">Are there subcategories in this expense category?</span></span> <span data-ttu-id="91010-182">إذا كان هناك فئات فرعية، فيجب أيضًا أن تحسم أمرك بشأن القرارات التالية:</span><span class="sxs-lookup"><span data-stu-id="91010-182">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="91010-183">هل يتم استبعاد أي من الفئات الفرعية من استرداد الضريبة؟</span><span class="sxs-lookup"><span data-stu-id="91010-183">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="91010-184">ما هي مجموعة ضريبة مبيعات الصنف للفئات الفرعية؟</span><span class="sxs-lookup"><span data-stu-id="91010-184">What is the item sales tax group of the subcategories?</span></span>

<span data-ttu-id="91010-185">إذا كانت فئة المصروفات مستخدمة أيضًا في إدارة المشاريع والمحاسبة، فأجب على الأسئلة المتبقية.</span><span class="sxs-lookup"><span data-stu-id="91010-185">If the expense category is also used in Project management and accounting, answer the remaining questions.</span></span> <span data-ttu-id="91010-186">وإلا، فانتقل إلى القسم التالي.</span><span class="sxs-lookup"><span data-stu-id="91010-186">Otherwise, move on to the next section.</span></span>

- <span data-ttu-id="91010-187">ما هي حسابات التكلفة التي سيتم استخدامها للمصروفات التالية؟</span><span class="sxs-lookup"><span data-stu-id="91010-187">Which cost accounts will be used for the following expenses?</span></span>

    - <span data-ttu-id="91010-188">التكلفة</span><span class="sxs-lookup"><span data-stu-id="91010-188">Cost</span></span>
    - <span data-ttu-id="91010-189">توزيع كشف الرواتب</span><span class="sxs-lookup"><span data-stu-id="91010-189">Payroll allocation</span></span>
    - <span data-ttu-id="91010-190">الأعمال قيد التنفيذ (WIP)-قيمة التكلفة</span><span class="sxs-lookup"><span data-stu-id="91010-190">WIP-cost value</span></span>
    - <span data-ttu-id="91010-191">عنصر التكلفة</span><span class="sxs-lookup"><span data-stu-id="91010-191">Cost-item</span></span>
    - <span data-ttu-id="91010-192">الأعمال قيد التنفيذ (WIP) - عنصر قيمة التكلفة</span><span class="sxs-lookup"><span data-stu-id="91010-192">WIP-cost value-item</span></span>
    - <span data-ttu-id="91010-193">الخسارة المتكبدة</span><span class="sxs-lookup"><span data-stu-id="91010-193">Accrued loss</span></span>
    - <span data-ttu-id="91010-194">الأعمال قيد التنفيذ (WIP) - الخسارة المتكبدة</span><span class="sxs-lookup"><span data-stu-id="91010-194">WIP-accrued loss</span></span>

- <span data-ttu-id="91010-195">ما هي حسابات الإيرادات التي سيتم استخدامها للعناصر التالية؟</span><span class="sxs-lookup"><span data-stu-id="91010-195">Which revenue accounts will be used for the following?</span></span>

    - <span data-ttu-id="91010-196">الإيرادات المفوترة</span><span class="sxs-lookup"><span data-stu-id="91010-196">Invoiced revenue</span></span>
    - <span data-ttu-id="91010-197">الإيرادات المستحقة - قيمة المبيعات</span><span class="sxs-lookup"><span data-stu-id="91010-197">Accrued revenue-sales value</span></span>
    - <span data-ttu-id="91010-198">الأعمال قيد التنفيذ (WIP) - قيمة المبيعات</span><span class="sxs-lookup"><span data-stu-id="91010-198">WIP-sales value</span></span>
    - <span data-ttu-id="91010-199">الإيراد المستحق-الإنتاج</span><span class="sxs-lookup"><span data-stu-id="91010-199">Accrued revenue-production</span></span>
    - <span data-ttu-id="91010-200">الأعمال قيد التنفيذ (WIP) - الإنتاج</span><span class="sxs-lookup"><span data-stu-id="91010-200">WIP-production</span></span>
    - <span data-ttu-id="91010-201">الإيراد المستحق - الربح</span><span class="sxs-lookup"><span data-stu-id="91010-201">Accrued revenue-profit</span></span>
    - <span data-ttu-id="91010-202">الأعمال قيد التنفيذ (WIP) - الربح</span><span class="sxs-lookup"><span data-stu-id="91010-202">WIP-profit</span></span>
    - <span data-ttu-id="91010-203">الإيراد المستحق - الاشتراك</span><span class="sxs-lookup"><span data-stu-id="91010-203">Accrued revenue-subscription</span></span>
    - <span data-ttu-id="91010-204">الأعمال قيد التنفيذ (WIP) - الاشتراك</span><span class="sxs-lookup"><span data-stu-id="91010-204">WIP-subscription</span></span>

### <a name="taxes"></a><span data-ttu-id="91010-205">الضرائب</span><span class="sxs-lookup"><span data-stu-id="91010-205">Taxes</span></span>

<span data-ttu-id="91010-206">بالنسبة للضرائب المرتبطة بالمصروفات، يجب عليك تحديد ما تم تضمينه أو تمكينه في تقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="91010-206">For expense-related taxes, you must determine what is included or enabled on expense reports.</span></span>

<span data-ttu-id="91010-207">**القرارات:**</span><span class="sxs-lookup"><span data-stu-id="91010-207">**Decisions:**</span></span>

- <span data-ttu-id="91010-208">هل تم تضمين ضريبة المبيعات في مبالغ المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-208">Is sales tax included in the expense amounts?</span></span>
- <span data-ttu-id="91010-209">هل ينبغي تمكين استرداد الضرائب على المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-209">Should tax recovery be enabled on expenses?</span></span>

    > [!NOTE]
    > <span data-ttu-id="91010-210">عندما تقوم بتخطيط دفتر الأستاذ العام، إذا قررت تطبيق قواعد ضريبة المبيعات الأمريكية واستخدام قواعد الضرائب، فلا يمكنك تمكين استرداد الضرائب على المصروفات.</span><span class="sxs-lookup"><span data-stu-id="91010-210">When you were planning the general ledger, if you decided to apply U.S. sales tax and use tax rules, you can’t enable tax recovery on expenses.</span></span> <span data-ttu-id="91010-211">(لتطبيق قواعد ضريبة المبيعات الأمريكية واستخدام قواعد الضرائب، فعيّن الخيار **تطبيق قواعد ضريبة المبيعات** إلى **نعم**.)</span><span class="sxs-lookup"><span data-stu-id="91010-211">(To apply U.S. sales tax and use tax rules, set the **Apply sales tax taxations rules** option to **Yes**.)</span></span>

## <a name="policies"></a><span data-ttu-id="91010-212">السياسات</span><span class="sxs-lookup"><span data-stu-id="91010-212">Policies</span></span>

<span data-ttu-id="91010-213">ومن خلال إنشاء سياسات تقارير المصروفات، يمكنك مساعدة مؤسستك على توفير الوقت والمال عندما يتحمل الموظفون المصروفات بالنيابة عنها.</span><span class="sxs-lookup"><span data-stu-id="91010-213">By creating expense report policies, you can help your organization save time and money when employees incur expenses on its behalf.</span></span> <span data-ttu-id="91010-214">تساعد السياسات على ضمان بقاء الموظفين ضمن الميزانية، وتوفير كل المعلومات، وإنفاق الأموال فقط عندما يحتاجون إليها.</span><span class="sxs-lookup"><span data-stu-id="91010-214">Policies help guarantee that employees stay in budget, provide all required information, and spend money only as they require it.</span></span> <span data-ttu-id="91010-215">يجب اتخاذ القرارات التالية لكل سياسة تقرير مصروفات ولكل سياسة موافقة على تقرير المصروفات التي تقوم بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="91010-215">You must make the following decisions for each expense report policy and each expense report approval policy that you create.</span></span>

<span data-ttu-id="91010-216">**القرارات:**</span><span class="sxs-lookup"><span data-stu-id="91010-216">**Decisions:**</span></span>

- <span data-ttu-id="91010-217">ما هو اسم السياسة؟</span><span class="sxs-lookup"><span data-stu-id="91010-217">What is the name of the policy?</span></span>
- <span data-ttu-id="91010-218">ما هدف سياسة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="91010-218">What is the expense policy for?</span></span>
- <span data-ttu-id="91010-219">إذا قررت في وقت سابق تمكين المصروفات بين الشركات الشقيقة، فما الشركات الموجودة في مؤسستك التي سيتم تطبيق هذه السياسة عليها؟</span><span class="sxs-lookup"><span data-stu-id="91010-219">If you previously decided to enable intercompany expenses, which companies in your organization will this policy apply to?</span></span>
- <span data-ttu-id="91010-220">متى تصبح السياسة سارية المفعول؟</span><span class="sxs-lookup"><span data-stu-id="91010-220">When does the policy become effective?</span></span>
- <span data-ttu-id="91010-221">متى تنتهي صلاحية السياسة؟</span><span class="sxs-lookup"><span data-stu-id="91010-221">When does the policy expire?</span></span>
- <span data-ttu-id="91010-222">ما هي قاعدة السياسة؟</span><span class="sxs-lookup"><span data-stu-id="91010-222">What is the policy rule?</span></span>
- <span data-ttu-id="91010-223">ما هي نتيجة قاعدة السياسة؟</span><span class="sxs-lookup"><span data-stu-id="91010-223">What is the outcome of the policy rule?</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]