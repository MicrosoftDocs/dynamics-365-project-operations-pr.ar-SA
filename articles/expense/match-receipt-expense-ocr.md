---
title: التقاط إيصال باستخدام OCR
description: يوفر هذا الموضوع معلومات حول معالجة التعرف البصري على الأحرف (OCR) للإيصالات.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: fd0cb0fb094260fa3e82d7a2f200f328a39dd7a1
ms.sourcegitcommit: f78087174a8512199a1bcbd7e8610bbc80e64801
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "5499835"
---
# <a name="capture-a-receipt-using-ocr"></a><span data-ttu-id="1d91b-103">التقاط إيصال باستخدام OCR</span><span class="sxs-lookup"><span data-stu-id="1d91b-103">Capture a receipt using OCR</span></span>

<span data-ttu-id="1d91b-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="1d91b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1d91b-105">تم تحسين إدخال المصاريف من خلال إدخال معالجة التعرف الضوئي على الأحرف (OCR) للإيصالات.</span><span class="sxs-lookup"><span data-stu-id="1d91b-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="1d91b-106">تم تصميم هذه الوظيفة لتحسين تجربة المستخدم عند إنشاء تقارير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="1d91b-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="1d91b-107">الميزات الأساسية</span><span class="sxs-lookup"><span data-stu-id="1d91b-107">Key features</span></span>

- <span data-ttu-id="1d91b-108">يقوم النظام باستخراج اسم التاجر والتاريخ والمبلغ الإجمالي من الإيصالات.</span><span class="sxs-lookup"><span data-stu-id="1d91b-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="1d91b-109">سيحاول النظام مطابقة الإيصالات غير المرفقة بحركات المصروفات غير المرفقة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="1d91b-110">يمكنك إنشاء حركات مصروفات تم إدخالها يدويًا من الإيصالات.</span><span class="sxs-lookup"><span data-stu-id="1d91b-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="1d91b-111">إرفاق إيصالات بتقرير مصروفات</span><span class="sxs-lookup"><span data-stu-id="1d91b-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="1d91b-112">لإرفاق إيصالات بحركات بطاقة الائتمان تلقائيًا عند إنشاء تقرير مصروفات، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="1d91b-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="1d91b-113">افتح مساحة عمل **إدارة المصروفات** .</span><span class="sxs-lookup"><span data-stu-id="1d91b-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="1d91b-114">في علامة التبويب **الإيصالات** ، تحقق من وجود إيصالات غير مرفقة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="1d91b-115">يمكنك أيضًا تحميل الإيصالات من علامة التبويب **إيصالات** .</span><span class="sxs-lookup"><span data-stu-id="1d91b-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="1d91b-116">في علامة التبويب **المصروفات** ، تحقق من وجود مصروفات غير مرفقة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="1d91b-117">وعادة ما يقوم مسؤول المصروفات باستيراد هذه المصروفات من موفر بطاقة الائتمان.</span><span class="sxs-lookup"><span data-stu-id="1d91b-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="1d91b-118">حدد **تقرير مصروفات جديد**.</span><span class="sxs-lookup"><span data-stu-id="1d91b-118">Select **New expense report**.</span></span> <span data-ttu-id="1d91b-119">لاحظ أنه يمكنك تضمين المصاريف والإيصالات الآن أيضًا عند إنشاء تقرير المصاريف.</span><span class="sxs-lookup"><span data-stu-id="1d91b-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="1d91b-120">إذا أضفت كلاً من المصاريف والإيصالات، فسيتم تشغيل المطابقة التلقائية للإيصالات مقابل النفقات.</span><span class="sxs-lookup"><span data-stu-id="1d91b-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="1d91b-121">إنشاء أو مطابقة إيصالات بتقرير مصروفات</span><span class="sxs-lookup"><span data-stu-id="1d91b-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="1d91b-122">لإنشاء مصروفات أو مطابقة مصروفات من إيصال، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="1d91b-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="1d91b-123">في تقرير المصروفات، في علامة التبويب **الإيصالات** ، قم بإرفاق إيصال من خلال تحديد **إضافة إيصالات**.</span><span class="sxs-lookup"><span data-stu-id="1d91b-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="1d91b-124">ضمن الصورة التي تم تحميلها من الإيصال، لاحظ خيارات **الإنشاء** و **المطابقة** .</span><span class="sxs-lookup"><span data-stu-id="1d91b-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="1d91b-125">حدد **إنشاء** لإنشاء حركة مصروفات تم إدخالها يدويًا وملء القيم التي تم استخراجها من الإيصال.</span><span class="sxs-lookup"><span data-stu-id="1d91b-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="1d91b-126">إذا قمت بتحديد **مطابقة**، سيحاول النظام مطابقة المصروفات الحالية بالإيصال.</span><span class="sxs-lookup"><span data-stu-id="1d91b-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="1d91b-127">التثبيت</span><span class="sxs-lookup"><span data-stu-id="1d91b-127">Installation</span></span>

<span data-ttu-id="1d91b-128">لاستخدام إمكانيات المصروفات المتقدمة هذه، قم بتثبيت الوظيفة الإضافية لخدمة إدارة المصروفات لـ Microsoft Dynamics 365 Finance، وقم بتشغيل الميزات الموجودة في المثيل الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="1d91b-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="1d91b-129">يمكنك الوصول إلى الوظيفة الإضافية من مشروعك الخاص في Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="1d91b-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="1d91b-130">قم بتسجيل الدخول إلى LCS، وافتح البيئة المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="1d91b-131">انتقل إلى **التفاصيل الكاملة**.</span><span class="sxs-lookup"><span data-stu-id="1d91b-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="1d91b-132">حدد **صيانة** أو قم بالتمرير لأسفل إلى علامة التبويب السريع **الوظائف الإضافية الخاصة بالبيئة** .</span><span class="sxs-lookup"><span data-stu-id="1d91b-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="1d91b-133">حدد **تثبيت وظيفة إضافية جديدة**.</span><span class="sxs-lookup"><span data-stu-id="1d91b-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="1d91b-134">حدد **خدمة إدارة المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="1d91b-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="1d91b-135">اتبع دليل التثبيت، ووافق على البنود والشروط.</span><span class="sxs-lookup"><span data-stu-id="1d91b-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="1d91b-136">حدد **تثبيت**.</span><span class="sxs-lookup"><span data-stu-id="1d91b-136">Select **Install**.</span></span>

<span data-ttu-id="1d91b-137">في مساحة عمل **إدارة الميزات** ، قم بتشغيل الميزات التالية:</span><span class="sxs-lookup"><span data-stu-id="1d91b-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="1d91b-138">إعادة صياغة تقارير المصروفات</span><span class="sxs-lookup"><span data-stu-id="1d91b-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="1d91b-139">المطابقة التلقائية للمصروفات وإنشاءها من الإيصال</span><span class="sxs-lookup"><span data-stu-id="1d91b-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="1d91b-140">عند تشغيل هذه الميزات، تحدث الإجراءات التالية:</span><span class="sxs-lookup"><span data-stu-id="1d91b-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="1d91b-141">يتم استبدال مساحة عمل **إدارة المصروفات** الموجودة بمساحة العمل الجديدة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="1d91b-142">تتم إضافة عنصر قائمة جديد لرؤية حقل المصروفات.</span><span class="sxs-lookup"><span data-stu-id="1d91b-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="1d91b-143">لا يزال بإمكانك فتح صفحة **تقارير المصروفات** السابقة من خلال الانتقال إلى **إدارة المصروفات > مصروفاتي > تقارير المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="1d91b-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="1d91b-144">وتستمر عمليات سير العمل وأي موافقات في الانتقال إلى صفحه تقارير المصروفات الموجودة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="1d91b-145">ستتم معالجة الايصالات من خلال Microsoft Azure Cognitive Services، وسيتم استخراج بيانات التعريف وإضافتها.</span><span class="sxs-lookup"><span data-stu-id="1d91b-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="1d91b-146">تمت إضافة خيار يتيح لك إنشاء تقرير مصروفات يتضمن الإيصالات غير المرفقة المتطابقة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="1d91b-147">يتيح لك الخيار الذي تمت إضافته إلى تقارير المصاريف إنشاء بند مصروفات من إيصال، أو يحاول مطابقة إيصال موجود ببند مصاريف موجود.</span><span class="sxs-lookup"><span data-stu-id="1d91b-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="1d91b-148">الأسئلة الشائعة</span><span class="sxs-lookup"><span data-stu-id="1d91b-148">Frequently asked questions</span></span>

<span data-ttu-id="1d91b-149">**هل تستخدم Microsoft البيانات الخاصة بي لنماذجها؟**</span><span class="sxs-lookup"><span data-stu-id="1d91b-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="1d91b-150">لا، لقد أنشأت Microsoft نموذجًا عامًا للتعلم الآلي لخدمة معالجة الإيصالات.</span><span class="sxs-lookup"><span data-stu-id="1d91b-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="1d91b-151">لا يستند هذا النموذج إلى الايصالات التي قمت بتحميلها.</span><span class="sxs-lookup"><span data-stu-id="1d91b-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="1d91b-152">**أين تتوفر هذه الميزة وأين تتم معالجتها؟**</span><span class="sxs-lookup"><span data-stu-id="1d91b-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="1d91b-153">يتم دعمه حاليًا في الولايات المتحدة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="1d91b-154">**إلى أين تذهب إيصالاتي؟**</span><span class="sxs-lookup"><span data-stu-id="1d91b-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="1d91b-155">ستتصل الشركة المالية بالخدمات الإدراكية لاستخراج بيانات الحقل.</span><span class="sxs-lookup"><span data-stu-id="1d91b-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="1d91b-156">سوف تحتفظ الخدمات الإدراكية بنسخة من إيصالك لفترة تصل إلى 24 ساعة أثناء حدوث المعالجة.</span><span class="sxs-lookup"><span data-stu-id="1d91b-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="1d91b-157">بعد اكتمال المعالجة، ستقوم خدمات الإدراك بإزالة الإيصال.</span><span class="sxs-lookup"><span data-stu-id="1d91b-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="1d91b-158">لا تزال الإيصالات مُخزنة في التمويل.</span><span class="sxs-lookup"><span data-stu-id="1d91b-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="1d91b-159">لمزيد من المعلومات، راجع [تمكين فهم الإيصالات باستخدام الإمكانية الجديدة لأداة التعرف على النماذج](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="1d91b-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
