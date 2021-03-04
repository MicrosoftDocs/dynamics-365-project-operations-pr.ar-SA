---
title: معالجة إيصالات المصروفات
description: يوفر هذا الموضوع معلومات حول معالجة التعرف البصري على الأحرف (OCR) للإيصالات. تم تصميم هذه الميزة لتحسين تجربة المستخدم عند إنشاء تقارير المصروفات في Microsoft Dynamics 365 Finance.
author: stsporen
manager: AnnBe
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: 64901610144f9dfe274bd4c2294ab32659743a1a
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960276"
---
# <a name="expense-receipt-processing"></a><span data-ttu-id="2ac50-104">معالجة إيصالات المصروفات</span><span class="sxs-lookup"><span data-stu-id="2ac50-104">Expense receipt processing</span></span>

<span data-ttu-id="2ac50-105">تم تحسين إدخال المصاريف من خلال إدخال معالجة التعرف الضوئي على الأحرف (OCR) للإيصالات.</span><span class="sxs-lookup"><span data-stu-id="2ac50-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="2ac50-106">تم تصميم هذه الميزة لتحسين تجربة المستخدم عند إنشاء تقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="2ac50-106">This feature is designed to improve the user experience when expense reports are created.</span></span>

## <a name="key-features"></a><span data-ttu-id="2ac50-107">الميزات الأساسية</span><span class="sxs-lookup"><span data-stu-id="2ac50-107">Key features</span></span>

- <span data-ttu-id="2ac50-108">يتم استخراج اسم التاجر والتاريخ والمبلغ الإجمالي من الإيصالات.</span><span class="sxs-lookup"><span data-stu-id="2ac50-108">The merchant name, date, and total amount are extracted from receipts.</span></span>
- <span data-ttu-id="2ac50-109">تحاول الميزة مطابقة الإيصالات غير المرفقة بحركات المصروفات غير المرفقة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-109">The feature tries to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="2ac50-110">بإمكان المستخدمين إنشاء حركات مصروفات تم إدخالها يدويًا من الإيصالات.</span><span class="sxs-lookup"><span data-stu-id="2ac50-110">Users can create manually entered expense transactions from receipts.</span></span>

## <a name="usage-examples"></a><span data-ttu-id="2ac50-111">أمثلة عن الاستخدام</span><span class="sxs-lookup"><span data-stu-id="2ac50-111">Usage examples</span></span>

<span data-ttu-id="2ac50-112">لإرفاق إيصالات بحركات بطاقة الائتمان تلقائيًا عند إنشاء تقرير مصروفات، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="2ac50-112">To automatically attach receipts that include credit card transactions when an expense report is created, do the following:</span></span>

  1. <span data-ttu-id="2ac50-113">افتح مساحة عمل **إدارة المصروفات** .</span><span class="sxs-lookup"><span data-stu-id="2ac50-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="2ac50-114">في علامة التبويب **الإيصالات** ، تحقق من وجود إيصالات غير مرفقة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="2ac50-115">يمكنك أيضًا تحميل الإيصالات من علامة التبويب **إيصالات** .</span><span class="sxs-lookup"><span data-stu-id="2ac50-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="2ac50-116">في علامة التبويب **المصروفات** ، تحقق من وجود مصروفات غير مرفقة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="2ac50-117">وعادة ما يقوم مسؤول المصروفات باستيراد هذه المصروفات من موفر بطاقة الائتمان.</span><span class="sxs-lookup"><span data-stu-id="2ac50-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="2ac50-118">حدد **تقرير مصروفات جديد**.</span><span class="sxs-lookup"><span data-stu-id="2ac50-118">Select **New expense report**.</span></span> <span data-ttu-id="2ac50-119">لاحظ أنه يمكنك تضمين المصاريف والإيصالات الآن أيضًا عند إنشاء تقرير المصاريف.</span><span class="sxs-lookup"><span data-stu-id="2ac50-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="2ac50-120">إذا أضفت كلاً من المصاريف والإيصالات، فسيتم تشغيل المطابقة التلقائية للإيصالات مقابل النفقات.</span><span class="sxs-lookup"><span data-stu-id="2ac50-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

<span data-ttu-id="2ac50-121">لإنشاء مصروفات أو مطابقة مصروفات من إيصال، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="2ac50-121">To create an expense, or match an expense from a receipt, do the following:</span></span>

  1. <span data-ttu-id="2ac50-122">في تقرير المصروفات، في علامة التبويب **الإيصالات** ، قم بإرفاق إيصال من خلال تحديد **إضافة إيصالات**.</span><span class="sxs-lookup"><span data-stu-id="2ac50-122">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="2ac50-123">ضمن الصورة التي تم تحميلها من الإيصال، لاحظ خيارات **الإنشاء** و **المطابقة** .</span><span class="sxs-lookup"><span data-stu-id="2ac50-123">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="2ac50-124">حدد **إنشاء** لإنشاء حركة مصروفات تم إدخالها يدويًا وملء القيم التي تم استخراجها من الإيصال.</span><span class="sxs-lookup"><span data-stu-id="2ac50-124">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="2ac50-125">إذا قمت بتحديد **مطابقة**، سيحاول النظام مطابقة المصروفات الحالية بالإيصال.</span><span class="sxs-lookup"><span data-stu-id="2ac50-125">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="2ac50-126">التثبيت</span><span class="sxs-lookup"><span data-stu-id="2ac50-126">Installation</span></span>

<span data-ttu-id="2ac50-127">تعمل هذه الميزة بالتزامن مع ميزة **إعادة صياغة تقارير المصروفات** للمساعدة في تبسيط تجربة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="2ac50-127">This feature works in combination with the **Expense reports re-imagined** feature to help simplify the expense experience.</span></span> <span data-ttu-id="2ac50-128">تتوفر هذه الميزة لبيئات المستوى 2 + فقط، وهي بيئة الاختبار المعزولة وبيئة الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="2ac50-128">This feature is only available for Tier 2+ environments, which are Sandbox and Production.</span></span>

<span data-ttu-id="2ac50-129">لاستخدام إمكانيات المصروفات المتقدمة هذه، قم بتثبيت الوظيفة الإضافية لخدمة إدارة المصروفات لـ Microsoft Dynamics 365 Finance، وقم بتشغيل الميزات الموجودة في المثيل الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="2ac50-129">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="2ac50-130">يمكنك الوصول إلى الوظيفة الإضافية من مشروعك الخاص في Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="2ac50-130">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="2ac50-131">قم بتسجيل الدخول إلى LCS، وافتح البيئة المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-131">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="2ac50-132">انتقل إلى **التفاصيل الكاملة**.</span><span class="sxs-lookup"><span data-stu-id="2ac50-132">Go to **Full details**.</span></span>
3. <span data-ttu-id="2ac50-133">حدد **صيانة** أو قم بالتمرير لأسفل إلى علامة التبويب السريع **الوظائف الإضافية الخاصة بالبيئة** .</span><span class="sxs-lookup"><span data-stu-id="2ac50-133">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="2ac50-134">حدد **تثبيت وظيفة إضافية جديدة**.</span><span class="sxs-lookup"><span data-stu-id="2ac50-134">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="2ac50-135">حدد **خدمة إدارة المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="2ac50-135">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="2ac50-136">اتبع دليل التثبيت، ووافق على البنود والشروط.</span><span class="sxs-lookup"><span data-stu-id="2ac50-136">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="2ac50-137">حدد **تثبيت**.</span><span class="sxs-lookup"><span data-stu-id="2ac50-137">Select **Install**.</span></span>

<span data-ttu-id="2ac50-138">في مساحة عمل **إدارة الميزات** ، قم بتشغيل الميزات التالية:</span><span class="sxs-lookup"><span data-stu-id="2ac50-138">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="2ac50-139">إعادة صياغة تقارير المصروفات</span><span class="sxs-lookup"><span data-stu-id="2ac50-139">Expense reports re-imagined</span></span>
- <span data-ttu-id="2ac50-140">المطابقة التلقائية للمصروفات وإنشاءها من الإيصال</span><span class="sxs-lookup"><span data-stu-id="2ac50-140">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="2ac50-141">عند تشغيل هذه الميزات، تحدث الإجراءات التالية:</span><span class="sxs-lookup"><span data-stu-id="2ac50-141">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="2ac50-142">يتم استبدال مساحة عمل **إدارة المصروفات** الموجودة بمساحة العمل الجديدة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-142">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="2ac50-143">تتم إضافة عنصر قائمة جديد لرؤية حقل المصروفات.</span><span class="sxs-lookup"><span data-stu-id="2ac50-143">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="2ac50-144">لا يزال بإمكانك فتح صفحة **تقارير المصروفات** السابقة من خلال الانتقال إلى **إدارة المصروفات > مصروفاتي > تقارير المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="2ac50-144">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="2ac50-145">وتستمر عمليات سير العمل وأي موافقات في الانتقال إلى صفحه تقارير المصروفات الموجودة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-145">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="2ac50-146">ستتم معالجة الايصالات من خلال Microsoft Azure Cognitive Services، وسيتم استخراج بيانات التعريف وإضافتها.</span><span class="sxs-lookup"><span data-stu-id="2ac50-146">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="2ac50-147">تمت إضافة خيار يتيح لك إنشاء تقرير مصروفات يتضمن الإيصالات غير المرفقة المتطابقة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-147">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="2ac50-148">يتيح لك الخيار الذي تمت إضافته إلى تقارير المصاريف إنشاء بند مصروفات من إيصال، أو يحاول مطابقة إيصال موجود ببند مصاريف موجود.</span><span class="sxs-lookup"><span data-stu-id="2ac50-148">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

<span data-ttu-id="2ac50-149">لمزيد من المعلومات حول ميزة إعادة صياغة تقارير المصروفات، راجع [إعادة صياغة تقارير المصروفات](ExpenseWorkspaceNew.md).</span><span class="sxs-lookup"><span data-stu-id="2ac50-149">For more information about the Expense reports re-imagined feature, see [Expense reports reimagined](ExpenseWorkspaceNew.md).</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="2ac50-150">الأسئلة الشائعة</span><span class="sxs-lookup"><span data-stu-id="2ac50-150">Frequently asked questions</span></span>

<span data-ttu-id="2ac50-151">**هل تستخدم Microsoft البيانات الخاصة بي لنماذجها؟**</span><span class="sxs-lookup"><span data-stu-id="2ac50-151">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="2ac50-152">لا، لقد أنشأت Microsoft نموذجًا عامًا للتعلم الآلي لخدمة معالجة الإيصالات.</span><span class="sxs-lookup"><span data-stu-id="2ac50-152">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="2ac50-153">لا يستند هذا النموذج إلى الايصالات التي قمت بتحميلها.</span><span class="sxs-lookup"><span data-stu-id="2ac50-153">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="2ac50-154">**أين تتوفر هذه الميزة وأين تتم معالجتها؟**</span><span class="sxs-lookup"><span data-stu-id="2ac50-154">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="2ac50-155">يتم دعمه حاليًا في الولايات المتحدة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-155">Currently, the United States is supported.</span></span>

<span data-ttu-id="2ac50-156">**إلى أين تذهب إيصالاتي؟**</span><span class="sxs-lookup"><span data-stu-id="2ac50-156">**Where do my receipts go?**</span></span>

<span data-ttu-id="2ac50-157">ستتصل الشركة المالية بالخدمات الإدراكية لاستخراج بيانات الحقل.</span><span class="sxs-lookup"><span data-stu-id="2ac50-157">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="2ac50-158">سوف تحتفظ الخدمات الإدراكية بنسخة من إيصالك لفترة تصل إلى 24 ساعة أثناء حدوث المعالجة.</span><span class="sxs-lookup"><span data-stu-id="2ac50-158">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="2ac50-159">بعد اكتمال المعالجة، ستقوم خدمات الإدراك بإزالة الإيصال.</span><span class="sxs-lookup"><span data-stu-id="2ac50-159">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="2ac50-160">لا تزال الإيصالات مُخزنة في التمويل.</span><span class="sxs-lookup"><span data-stu-id="2ac50-160">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="2ac50-161">لمزيد من المعلومات، راجع [تمكين فهم الإيصالات باستخدام الإمكانية الجديدة لأداة التعرف على النماذج](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="2ac50-161">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>
