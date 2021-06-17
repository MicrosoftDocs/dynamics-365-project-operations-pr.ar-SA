---
title: القيم الفعلية
description: يوفر هذا الموضوع معلومات حول كيفية التعامل مع القيم الفعلية في Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 78c7a9486d0338adfd7770447f21d17509e654f7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996595"
---
# <a name="actuals"></a><span data-ttu-id="cd0d6-103">العمل الفعلي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-103">Actuals</span></span> 

<span data-ttu-id="cd0d6-104">_**ينطبق على:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="cd0d6-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cd0d6-105">تمثل القيم الفعلية تقدم الجدول والماليات الذي تمت مراجعته والموافقة عليه في أحد المشروعات.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="cd0d6-106">يتم إنشاؤها نتيجة للموافقة على إدخالات الوقت والمصروفات واستخدام المواد وإدخالات دفاتر اليومية والفواتير.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="cd0d6-107">إرسال أسطر دفتر اليومية والوقت</span><span class="sxs-lookup"><span data-stu-id="cd0d6-107">Journal lines and time submission</span></span>

<span data-ttu-id="cd0d6-108">لمزيد من المعلومات حول إدخال الوقت، راجع [نظرة عامة حول إدخال الوقت](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="cd0d6-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="cd0d6-109">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-109">Time and materials</span></span>

<span data-ttu-id="cd0d6-110">عندما يكون إدخال الوقت المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد الوقت والمواد، يقوم النظام بإنشاء بندين لدفتر اليومية، بند للتكلفة وبند للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="cd0d6-111">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="cd0d6-111">Fixed price</span></span>

<span data-ttu-id="cd0d6-112">عندما يكون إدخال الوقت المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد بسعر ثابت، يُنشئ النظام بند دفتر يومية للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="cd0d6-113">التسعير الافتراضي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-113">Default pricing</span></span>

<span data-ttu-id="cd0d6-114">يكمن منطق إنشاء الأسعار الافتراضية في دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="cd0d6-115">يتم نسخ قيم الحقول من إدخال الوقت إلى دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="cd0d6-116">تتضمن هذه القيم تاريخ الحركة وشروط التعاقد التي تم تعيين المشروع لهاـ وينتج عن العملة قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="cd0d6-117">تُستخدم الحقول التي تؤثر في الأسعار الافتراضية مثل **الدور** و **وحدة الموارد** لتحديد السعر المناسب في سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="cd0d6-118">يمكنك إضافة حقل مخصص في إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="cd0d6-119">إذا كنت ترغب في نشر قيمة الحقل على قيم فعلية، فأنشئ الحقل في الجدولين **القيم الفعلية** و **سطر دفتر اليومية**.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="cd0d6-120">استخدم التعليمات البرمجية المخصصة لنشر قيمة الحقل المحددة من "إدخال الوقت" إلى "القيم الفعلية" عبر سطر دفتر اليومية باستخدام أصول الحركة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="cd0d6-121">لمزيد من المعلومات حول أصول واتصالات الحركات، راجع [ربط القيم الفعلية بالسجلات الأصلية](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="cd0d6-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="cd0d6-122">إرسال أسطر دفتر اليومية والمصروفات الأساسية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="cd0d6-123">لمزيد من المعلومات حول إدخال المصروفات، راجع [نظرة عامة حول المصروفات](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="cd0d6-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="cd0d6-124">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-124">Time and materials</span></span>

<span data-ttu-id="cd0d6-125">عندما يكون إدخال المصروفات الأساسية المُرسل مرتبطًا بمشروع تم تعيينه إلى شروط تعاقد الوقت والمواد، يقوم النظام بإنشاء بندين لدفتر اليومية، بند للتكلفة وبند للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="cd0d6-126">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="cd0d6-126">Fixed price</span></span>

<span data-ttu-id="cd0d6-127">عند ربط إدخال مصروفات أساسي مرسل بمشروع تم تعيينه إلى شرط تعاقد ثابت السعر، ينشئ النظام سطر دفتر يومية واحدًا فقط للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="cd0d6-128">التسعير الافتراضي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-128">Default pricing</span></span>

<span data-ttu-id="cd0d6-129">يستند منطق إدخال الأسعار الافتراضية للمصروفات إلى فئة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="cd0d6-130">يتم استخدام تاريخ الحركة وشرط التعاقد الذي تم تعيين المشروع له والعملة جميعًا لتحديد قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="cd0d6-131">تُستخدم الحقول التي تؤثر في الأسعار الافتراضية مثل **فئة الحركة** و **الوحدة** لتحديد السعر المناسب في سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="cd0d6-132">ومع ذلك، لا يعمل هذا الإجراء إلا عندما تكون طريقة التسعير في قائمة الأسعار **السعر لكل وحدة**.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="cd0d6-133">إذا كانت طريقة التسعير **بتكلفة‬** أو **نسبة السعر إلى التكلفة**، يتم استخدام السعر الذي تم إدخاله عند إنشاء إدخال المصروفات للتكلفة ويتم حساب السعر على بند دفتر يومية المبيعات بالاستناد إلى طريقة التسعير.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="cd0d6-134">يمكنك إضافة حقل مخصص في إدخال مصروفات.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="cd0d6-135">إذا كنت ترغب في نشر قيمة الحقل على قيم فعلية، فأنشئ الحقل في الجدولين **القيم الفعلية** و **سطر دفتر اليومية**.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="cd0d6-136">استخدم التعليمات البرمجية المخصصة لنشر قيمة الحقل المحددة من "إدخال الوقت" إلى "القيم الفعلية" عبر سطر دفتر اليومية باستخدام أصول الحركة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="cd0d6-137">لمزيد من المعلومات حول أصول واتصالات الحركات، راجع [ربط القيم الفعلية بالسجلات الأصلية](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="cd0d6-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="cd0d6-138">إرسال بنود دفتر اليومية وسجل استخدام المواد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="cd0d6-139">لمزيد من المعلومات حول إدخال المصروفات، راجع [سجل استخدام المواد](../material/material-usage-log.md)المواد.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="cd0d6-140">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-140">Time and materials</span></span>

<span data-ttu-id="cd0d6-141">عند ربط إدخال سجل استخدام مواد مرسل بمشروع تم تعيينه إلى شرط تعاقد الوقت والمواد، ينشئ النظام سطرين لدفتر اليومية، أحدهما للتكلفة والآخر للمبيعات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="cd0d6-142">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="cd0d6-142">Fixed price</span></span>

<span data-ttu-id="cd0d6-143">عند ربط إدخال سجل استخدام مواد مرسل بمشروع تم تعيينه إلى شرط تعاقد ثابت السعر، ينشئ النظام سطر دفتر يومية واحدًا فقط للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="cd0d6-144">التسعير الافتراضي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-144">Default pricing</span></span>

<span data-ttu-id="cd0d6-145">يستند منطق إدخال الأسعار الافتراضية للمواد إلى مجموعة المنتج والوحدة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="cd0d6-146">يتم استخدام تاريخ الحركة وشرط التعاقد الذي تم تعيين المشروع له والعملة جميعًا لتحديد قائمة الأسعار المناسبة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="cd0d6-147">تُستخدم الحقول التي تؤثر في الأسعار الافتراضية مثل **معرف المنتج** و **والوحدة** لتحديد السعر المناسب في سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="cd0d6-148">ومع ذلك، يعمل هذا فقط مع منتجات الكتالوج.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-148">However, this only works for catalog products.</span></span> <span data-ttu-id="cd0d6-149">بالنسبة للمنتجات المدونة، يُستخدم السعر الذي يتم إدخاله عند إنشاء إدخال سجل استخدام المواد للتكلفة وسعر المبيعات على أسطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="cd0d6-150">يمكنك إضافة حقل مخصص في إدخال **سجل استخدام المواد**.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="cd0d6-151">إذا كنت ترغب في نشر قيمة الحقل على قيم فعلية، فأنشئ الحقل في الجدولين **القيم الفعلية** و **سطر دفتر اليومية**.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="cd0d6-152">استخدم التعليمات البرمجية المخصصة لنشر قيمة الحقل المحددة من "إدخال الوقت" إلى "القيم الفعلية" عبر سطر دفتر اليومية باستخدام أصول الحركة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="cd0d6-153">لمزيد من المعلومات حول أصول واتصالات الحركات، راجع [ربط القيم الفعلية بالسجلات الأصلية](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="cd0d6-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="cd0d6-154">استخدام دفاتر يومية الإدخالات لتسجيل التكاليف</span><span class="sxs-lookup"><span data-stu-id="cd0d6-154">Use entry journals to record costs</span></span>

<span data-ttu-id="cd0d6-155">يمكنك استخدام دفاتر يومية الإدخالات لتسجيل التكلفة أو الإيرادات في فئات المواد أو الرسوم أو الوقت أو المصروفات أو الحركات الضريبية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="cd0d6-156">يمكن استخدام دفاتر اليومية للأغراض التالية:</span><span class="sxs-lookup"><span data-stu-id="cd0d6-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="cd0d6-157">نقل القيم الفعلية للمعاملة من نظام آخر إلى Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="cd0d6-158">تسجيل التكاليف التي حدثت في نظام آخر.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="cd0d6-159">يمكن أن تتضمن هذه التكاليف تكاليف التدبير أو التعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cd0d6-160">لا يتحقق التطبيق من نوع أسطر دفتر اليومية أو التسعير ذي الصلة الذي تم إدخاله على سطر دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="cd0d6-161">وبالتالي، فإن المستخدم الذي يكون على دراية بالتأثير المحاسبي للقيم الفعلية على المشروع وهو وحده الذي يجب عليه أن يستخدم دفاتر يومية الإدخالات لإنشاء القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="cd0d6-162">بسبب تأثير نوع دفتر اليومية هذا، يجب عليك اختيار من يمكنه الوصول إلى إنشاء دفاتر يومية الإدخال بعناية.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="cd0d6-163">تسجيل القيم الفعلية استنادًا إلى أحداث المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-163">Record actuals based on project events</span></span>

<span data-ttu-id="cd0d6-164">يسجل Project Operations الحركات المالية التي تحدث أثناء المشروع.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="cd0d6-165">تم تسجيل هذه الحركات على أنها قيم فعليه.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="cd0d6-166">توضح الجداول التالية الأنواع المختلفة من القيم الفعلية التي يتم إنشاؤها، وذلك استنادا إلى ما إذا كان المشروع هو مشروع الوقت والمواد أو أحد المشاريع ثابتة السعر، أو في مرحلة المبيعات الأولية، أو أنه مشروع داخلي.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="cd0d6-167">ينتمي المورد إلى نفس الوحدة التنظيمية باعتباره وحدة التعاقد الخاصة بالمشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="cd0d6-168">حدث</span><span class="sxs-lookup"><span data-stu-id="cd0d6-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="cd0d6-169">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="cd0d6-170">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="cd0d6-171">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="cd0d6-172">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="cd0d6-173">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="cd0d6-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="cd0d6-174">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-174">Actuals</span></span></th>
<th><span data-ttu-id="cd0d6-175">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="cd0d6-175">Transaction currency</span></span></th>
<th><span data-ttu-id="cd0d6-176">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="cd0d6-176">Fixed price</span></span></th>
<th><span data-ttu-id="cd0d6-177">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="cd0d6-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="cd0d6-178">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="cd0d6-179">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-180">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="cd0d6-181">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="cd0d6-182">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="cd0d6-183">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-183">Cost actual</span></span></td>
<td><span data-ttu-id="cd0d6-184">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-185">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-186">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="cd0d6-187">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-188">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-189">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="cd0d6-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="cd0d6-190">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="cd0d6-191">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="cd0d6-192">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-192">Cost actual</span></span></td>
<td><span data-ttu-id="cd0d6-193">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-194">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-195">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-196">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-197">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-198">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="cd0d6-199">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-200">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="cd0d6-201">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="cd0d6-202">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="cd0d6-203">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="cd0d6-204">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-205">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-206">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-207">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-208">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-209">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-209">Billed sales</span></span></td>
<td><span data-ttu-id="cd0d6-210">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="cd0d6-211">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="cd0d6-212">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="cd0d6-213">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-214">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-215">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-216">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-217">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-218">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="cd0d6-219">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-220">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="cd0d6-221">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="cd0d6-222">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="cd0d6-223">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="cd0d6-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="cd0d6-224">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="cd0d6-225">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="cd0d6-226">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="cd0d6-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="cd0d6-227">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="cd0d6-228">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="cd0d6-229">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-230">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-230">Billed sales</span></span></td>
<td><span data-ttu-id="cd0d6-231">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="cd0d6-232">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="cd0d6-233">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="cd0d6-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="cd0d6-234">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-235">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="cd0d6-236">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-237">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="cd0d6-238">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="cd0d6-239">ينتمي المورد إلى وحدة تنظيمية تختلف عن وحدة التعاقد الخاصة بالمشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="cd0d6-240">حدث</span><span class="sxs-lookup"><span data-stu-id="cd0d6-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="cd0d6-241">مشروع قابل للفوترة أو مبيع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="cd0d6-242">مشروع في مرحلة المبيعات الأولية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="cd0d6-243">مشروع داخلي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="cd0d6-244">الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="cd0d6-245">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="cd0d6-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="cd0d6-246">القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-246">Actuals</span></span></th>
<th><span data-ttu-id="cd0d6-247">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="cd0d6-247">Transaction currency</span></span></th>
<th><span data-ttu-id="cd0d6-248">سعر ثابت</span><span class="sxs-lookup"><span data-stu-id="cd0d6-248">Fixed price</span></span></th>
<th><span data-ttu-id="cd0d6-249">عملة المعاملة‬</span><span class="sxs-lookup"><span data-stu-id="cd0d6-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="cd0d6-250">تم إنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="cd0d6-251">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-252">تم إرسال إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="cd0d6-253">لا يوجد نشاط في كيان القيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="cd0d6-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="cd0d6-254">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="cd0d6-255">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-255">Cost actual</span></span></td>
<td><span data-ttu-id="cd0d6-256">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="cd0d6-257">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="cd0d6-258">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="cd0d6-259">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="cd0d6-260">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-261">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</span><span class="sxs-lookup"><span data-stu-id="cd0d6-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="cd0d6-262">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-263">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="cd0d6-264">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-265">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="cd0d6-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="cd0d6-266">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="cd0d6-267">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="cd0d6-268">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-268">Cost actual</span></span></td>
<td><span data-ttu-id="cd0d6-269">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="cd0d6-270">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="cd0d6-271">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="cd0d6-272">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="cd0d6-273">القيمة الفعلية للتكلفة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-274">تكلفة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="cd0d6-275">عملة وحدة تعيين الموارد</span><span class="sxs-lookup"><span data-stu-id="cd0d6-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-276">مبيعات بين المؤسسات</span><span class="sxs-lookup"><span data-stu-id="cd0d6-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="cd0d6-277">عملة الوحدة المتعاقدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-278">القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="cd0d6-279">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-280">القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="cd0d6-281">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="cd0d6-282">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="cd0d6-283">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="cd0d6-284">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-285">المبيعات التي تمت فوترتها للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-286">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-287">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="cd0d6-288">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-289">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-289">Billed sales</span></span></td>
<td><span data-ttu-id="cd0d6-290">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="cd0d6-291">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="cd0d6-292">إلغاء مبيعات غير مفوترة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="cd0d6-293">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-294">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-295">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-296">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="cd0d6-297">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-298">المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="cd0d6-299">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-300">المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="cd0d6-301">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="cd0d6-302">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="cd0d6-303">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="cd0d6-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="cd0d6-304">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="cd0d6-305">مبيعات مفوترة للحدث الرئيسي</span><span class="sxs-lookup"><span data-stu-id="cd0d6-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="cd0d6-306">تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></span><span class="sxs-lookup"><span data-stu-id="cd0d6-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="cd0d6-307">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="cd0d6-308">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="cd0d6-309">غير قابل للتطبيق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-310">المبيعات المفوترة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-310">Billed sales</span></span></td>
<td><span data-ttu-id="cd0d6-311">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="cd0d6-312">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</span><span class="sxs-lookup"><span data-stu-id="cd0d6-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="cd0d6-313">مبيعات مفوترة - إلغاء</span><span class="sxs-lookup"><span data-stu-id="cd0d6-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="cd0d6-314">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-315">المبيعات المفوترة للكمية الجديدة</span><span class="sxs-lookup"><span data-stu-id="cd0d6-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="cd0d6-316">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="cd0d6-317">المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</span><span class="sxs-lookup"><span data-stu-id="cd0d6-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="cd0d6-318">عملة عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="cd0d6-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
