---
title: استيراد حركات بطاقات الائتمان والمحافظة عليها
description: يوضح هذا الموضوع كيفية استيراد حركات بطاقات الائتمان مرتبطة بالمصروفات وصيانتها. يمكن إعداد هذه الحركات بحيث يتم استيرادها تلقائيًا وفقا لجدول زمني متكرر، أو يمكن استيرادها يدويًا عند الحاجة اليها.
author: KimANelson
manager: AnnBe
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPbsMainDataLines
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 274023
ms.assetid: 3605eda1-a7ed-4675-8031-5279c5a8f5e4
ms.search.region: Global
ms.author: suvaidya
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: c434356c08e8490931bd60ea5b10fe2706cb0f51
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5951058"
---
# <a name="import-and-maintain-credit-card-transactions"></a><span data-ttu-id="ebe3a-104">استيراد حركات بطاقات الائتمان والمحافظة عليها</span><span class="sxs-lookup"><span data-stu-id="ebe3a-104">Import and maintain credit card transactions</span></span>

<span data-ttu-id="ebe3a-105">يمكن إعداد حركات بطاقات الائتمان المرتبطة بالمصروفات بحيث يتم استيرادها تلقائيا وفقا لجدول زمني متكرر.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="ebe3a-106">وبدلاً من ذلك، يمكن استيراد الحركات يدويا عند الحاجة اليها.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="ebe3a-107">يتم استيراد حركات بطاقات الائتمان من خلال كيان بيانات بطاقات الائتمان.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

<span data-ttu-id="ebe3a-108">لمزيد من المعلومات حول كيانات البيانات، راجع [كيانات البيانات](/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span><span class="sxs-lookup"><span data-stu-id="ebe3a-108">For more information about data entities, see [Data entities](/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="ebe3a-109">استيراد حركات بطاقات الائتمان</span><span class="sxs-lookup"><span data-stu-id="ebe3a-109">Import credit card transactions</span></span>

1. <span data-ttu-id="ebe3a-110">في صفحة **حركات بطاقة الائتمان** حدد **استيراد الحركات**.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="ebe3a-111">إذا كنت تقوم بفتح إدارة البيانات للمرة الاولى، فيجب على النظام تحديث قائمه كيانات البيانات قبل التمكن من المتابعة.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="ebe3a-112">في حقل **الاسم** أدخل وصفا فريدًا لمهمة الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-112">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="ebe3a-113">في حقل **تنسيق بيانات المصدر** حدد تنسيق الملف الذي يحتوي على حركات بطاقة الائتمان المراد استيرادها.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="ebe3a-114">حدد **تحميل** ثم ابحث عن الملف وحدده ليتم استيراده.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="ebe3a-115">بعد ان يتم تحميل الملف، قم بالتحقق من تعيين ملف حركة بطاقة الائتمان وأعمدة كيان بيانات حركات بطاقات الائتمان وذلك بتحديد الارتباط **عرض الخريطة** على اللوحة.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="ebe3a-116">إذا كانت هناك أخطاء في التعيين، أو إذا كان يجب عليك تغيير التعيين، فقم بإجراء تغييرات التعيين إما من علامة التبويب **تعيين الرسوم المرئية** أو من علامة التبويب **تفاصيل التعيين**.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="ebe3a-117">لأتمتة حركات بطاقة الائتمان، قم بتحديد **إنشاء مهمة بيانات متكررة**.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="ebe3a-118">يمكنك بعد ذلك تعيين التكرار الذي يحدد عدد مرات تكرار استيراد حركات بطاقة الائتمان.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="ebe3a-119">عند الانتهاء، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="ebe3a-120">لاستيراد الملف المحدد الآن، حدد **استيراد**.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="ebe3a-121">في حالة حدوث أخطاء أثناء عملية الاستيراد، يمكنك عرض سجل التنفيذ أو البيانات المرحلية لمعرفة الأخطاء التي يجب عليك إصلاحها لضمان نجاح عمليه الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="ebe3a-122">إذا كان يجب عليك استيراد أكثر من تنسيق ملف واحد، فيجب إنشاء مهام استيراد منفصلة لكل نوع من أنواع التنسيقات.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-122">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="ebe3a-123">إعادة تعيين حركات بطاقات الائتمان للموظفين الذين تم إنهاؤهم</span><span class="sxs-lookup"><span data-stu-id="ebe3a-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="ebe3a-124">بعد إنهاء سجل موظف، يتم تعطيل حساب ‏‫خدمات مجال Active Directory (AD DS)‬ للموظف.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="ebe3a-125">ومع ذلك، قد تكون هناك حركات بطاقة ائتمان نشطة يجب أن تظل مصروفة ومُسددة.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="ebe3a-126">من صفحة **حركات بطاقة الائتمان** ، يمكنك إعاده تعيين الموظف لآيه حركة بطاقة ائتمان في المكان الذي تم فيه إنهاء الموظف المرتبط.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-126">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="ebe3a-127">حدد حركه بطاقة ائتمان واحده أو أكثر، ثم حدد **إعادة تعيين الحركات**.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="ebe3a-128">يمكنك بعد ذلك تحديد موظف آخر لتعيين حركات بطاقة الائتمان اليه.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="ebe3a-129">بعد إعاده تعيين حركات بطاقة الائتمان، يمكن تحديدها لتقرير المصروفات ودفعها من خلال العملية المعتادة لتعويض تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="ebe3a-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]