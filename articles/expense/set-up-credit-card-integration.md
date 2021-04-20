---
title: إعداد تكامل بطاقة الائتمان
description: يشرح هذا الموضوع كيفية العمل مع حركات بطاقات الائتمان ذات الصلة بالمصروفات.
author: suvaidya
manager: AnnBe
ms.date: 04/02/2021
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
ms.openlocfilehash: 72ff98f5985af4362cde3c9914e0d20247f1f09a
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/07/2021
ms.locfileid: "5866667"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="0d506-103">إعداد تكامل بطاقة الائتمان</span><span class="sxs-lookup"><span data-stu-id="0d506-103">Set up credit card integration</span></span>

<span data-ttu-id="0d506-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="0d506-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0d506-105">يمكن إعداد حركات بطاقات الائتمان المرتبطة بالمصروفات بحيث يتم استيرادها تلقائيا وفقا لجدول زمني متكرر.</span><span class="sxs-lookup"><span data-stu-id="0d506-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="0d506-106">وبدلاً من ذلك، يمكن استيراد الحركات يدويا عند الحاجة اليها.</span><span class="sxs-lookup"><span data-stu-id="0d506-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="0d506-107">يتم استيراد حركات بطاقات الائتمان من خلال كيان بيانات حركات بطاقات الائتمان.</span><span class="sxs-lookup"><span data-stu-id="0d506-107">The credit card transactions are imported through the credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="0d506-108">استيراد حركات بطاقات الائتمان</span><span class="sxs-lookup"><span data-stu-id="0d506-108">Import credit card transactions</span></span>

<span data-ttu-id="0d506-109">لاستيراد حركات بطاقات الائتمان، اتبع هذه الخطوات:</span><span class="sxs-lookup"><span data-stu-id="0d506-109">To import credit card transactions, follow these steps:</span></span>

1. <span data-ttu-id="0d506-110">في صفحة **حركات بطاقة الائتمان** حدد **استيراد الحركات**.</span><span class="sxs-lookup"><span data-stu-id="0d506-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="0d506-111">إذا كنت تقوم بفتح إدارة البيانات للمرة الاولى، فيجب على النظام تحديث قائمه كيانات البيانات قبل التمكن من المتابعة.</span><span class="sxs-lookup"><span data-stu-id="0d506-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="0d506-112">في حقل **الاسم**، أدخل وصفًا فريدًا لوظيفة الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="0d506-112">In the **Name** field, enter a unique description for the import job.</span></span>
3. <span data-ttu-id="0d506-113">في حقل **تنسيق بيانات المصدر** حدد تنسيق الملف الذي يحتوي على حركات بطاقة الائتمان المراد استيرادها.</span><span class="sxs-lookup"><span data-stu-id="0d506-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="0d506-114">حدد **تحميل** ثم ابحث عن الملف وحدده ليتم استيراده.</span><span class="sxs-lookup"><span data-stu-id="0d506-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="0d506-115">بعد ان يتم تحميل الملف، تحقق من صحة تعيين ملف حركات بطاقات الائتمان وأعمدة كيان بيانات حركات بطاقات الائتمان وذلك بتحديد الارتباط **عرض الخريطة** على اللوحة.</span><span class="sxs-lookup"><span data-stu-id="0d506-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="0d506-116">إذا كانت هناك أخطاء في التعيين، أو إذا كان يجب عليك تغيير التعيين، فقم بإجراء تغييرات التعيين إما من علامة التبويب **تعيين الرسوم المرئية** أو من علامة التبويب **تفاصيل التعيين**.</span><span class="sxs-lookup"><span data-stu-id="0d506-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="0d506-117">لأتمتة حركات بطاقة الائتمان، قم بتحديد **إنشاء مهمة بيانات متكررة**.</span><span class="sxs-lookup"><span data-stu-id="0d506-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="0d506-118">يمكنك بعد ذلك تعيين التكرار الذي يحدد عدد مرات تكرار استيراد حركات بطاقة الائتمان.</span><span class="sxs-lookup"><span data-stu-id="0d506-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="0d506-119">عند الانتهاء، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0d506-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="0d506-120">لاستيراد الملف المحدد الآن، حدد **استيراد**.</span><span class="sxs-lookup"><span data-stu-id="0d506-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="0d506-121">في حالة حدوث أخطاء أثناء عملية الاستيراد، يمكنك عرض سجل التنفيذ أو البيانات المرحلية لرؤية الأخطاء التي يجب إصلاحها للمساعدة في ضمان نجاح الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="0d506-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help ensure a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="0d506-122">إذا كنت تريد استيراد أكثر من تنسيق ملف واحد، فيجب إنشاء وظائف استيراد منفصلة لكل نوع تنسيق.</span><span class="sxs-lookup"><span data-stu-id="0d506-122">If you need to import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="0d506-123">إعادة تعيين حركات بطاقات الائتمان للموظفين الذين تم إنهاؤهم</span><span class="sxs-lookup"><span data-stu-id="0d506-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="0d506-124">بعد إنهاء سجل موظف، يتم تعطيل حساب ‏‫خدمات مجال Active Directory (AD DS)‬ للموظف.</span><span class="sxs-lookup"><span data-stu-id="0d506-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="0d506-125">ومع ذلك، قد تكون هناك حركات بطاقة ائتمان نشطة يجب أن تظل مصروفة ومُسددة.</span><span class="sxs-lookup"><span data-stu-id="0d506-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="0d506-126">في صفحة **حركات بطاقات الائتمان**، يمكنك إعادة تعيين الموظف لأي من حركات بطاقات الائتمان حيث تم إنهاء عمل الموظف المرتبط.</span><span class="sxs-lookup"><span data-stu-id="0d506-126">On the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="0d506-127">حدد حركه بطاقة ائتمان واحده أو أكثر، ثم حدد **إعادة تعيين الحركات**.</span><span class="sxs-lookup"><span data-stu-id="0d506-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="0d506-128">يمكنك بعد ذلك تحديد موظف آخر لتعيين حركات بطاقة الائتمان اليه.</span><span class="sxs-lookup"><span data-stu-id="0d506-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="0d506-129">بعد إعاده تعيين حركات بطاقة الائتمان، يمكن تحديدها لتقرير المصروفات ودفعها من خلال العملية المعتادة لتعويض تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="0d506-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>

## <a name="delete-credit-card-transactions"></a><span data-ttu-id="0d506-130">حذف حركات بطاقات الائتمان</span><span class="sxs-lookup"><span data-stu-id="0d506-130">Delete credit card transactions</span></span> 

<span data-ttu-id="0d506-131">في بعض الأحيان، بعد استيراد حركات بطاقات الائتمان، قد يلزم حذف حركات معينة.</span><span class="sxs-lookup"><span data-stu-id="0d506-131">Sometimes, after credit card transactions are imported, certain transactions may need to be deleted.</span></span> <span data-ttu-id="0d506-132">وقد يعود سبب ذلك إلى كون الحركات مكررة أو لأن البيانات قد تكون غير دقيقة.</span><span class="sxs-lookup"><span data-stu-id="0d506-132">This could be because the transactions are duplicates or because the data might isn't accurate.</span></span> <span data-ttu-id="0d506-133">يمكن للمسؤولين استخدام ميزة **"حذف حركات بطاقات الائتمان"** لتحديد وحذف حركات بطاقات الائتمان **غير المرفقة** بتقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="0d506-133">Admins can use the **"Delete credit card transactions"** feature to select and delete credit card transactions that are **not attached** to an expense report.</span></span> 

1. <span data-ttu-id="0d506-134">انتقل إلى **المهام الدورية** > **حذف معاملات بطاقات الائتمان**.</span><span class="sxs-lookup"><span data-stu-id="0d506-134">Go to **Periodic tasks** > **Delete credit card transactions**.</span></span>
2. <span data-ttu-id="0d506-135">حدد **تصفية** وقدم معلومات لتحديد السجلات التي يجب تضمينها.</span><span class="sxs-lookup"><span data-stu-id="0d506-135">Select **Filter** and provide information to identify the records to include.</span></span>
3. <span data-ttu-id="0d506-136">حدد **موافق** لحذف السجلات.</span><span class="sxs-lookup"><span data-stu-id="0d506-136">Select **OK** to delete the records.</span></span> 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
