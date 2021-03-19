---
title: إعداد تكامل بطاقة الائتمان
description: يوضح هذا الموضوع كيفية استيراد حركات بطاقات الائتمان مرتبطة بالمصروفات وصيانتها.
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
ms.openlocfilehash: cd60d338e2b2a2d74d4d7f55bb5a1723f10c29ab
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276152"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="c21f6-103">إعداد تكامل بطاقة الائتمان</span><span class="sxs-lookup"><span data-stu-id="c21f6-103">Set up credit card integration</span></span>

<span data-ttu-id="c21f6-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="c21f6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c21f6-105">يمكن إعداد حركات بطاقات الائتمان المرتبطة بالمصروفات بحيث يتم استيرادها تلقائيا وفقا لجدول زمني متكرر.</span><span class="sxs-lookup"><span data-stu-id="c21f6-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="c21f6-106">وبدلاً من ذلك، يمكن استيراد الحركات يدويا عند الحاجة اليها.</span><span class="sxs-lookup"><span data-stu-id="c21f6-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="c21f6-107">يتم استيراد حركات بطاقات الائتمان من خلال كيان بيانات بطاقات الائتمان.</span><span class="sxs-lookup"><span data-stu-id="c21f6-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="c21f6-108">استيراد حركات بطاقات الائتمان</span><span class="sxs-lookup"><span data-stu-id="c21f6-108">Import credit card transactions</span></span>

1. <span data-ttu-id="c21f6-109">في صفحة **حركات بطاقة الائتمان** حدد **استيراد الحركات**.</span><span class="sxs-lookup"><span data-stu-id="c21f6-109">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="c21f6-110">إذا كنت تقوم بفتح إدارة البيانات للمرة الاولى، فيجب على النظام تحديث قائمه كيانات البيانات قبل التمكن من المتابعة.</span><span class="sxs-lookup"><span data-stu-id="c21f6-110">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="c21f6-111">في حقل **الاسم** أدخل وصفا فريدًا لمهمة الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="c21f6-111">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="c21f6-112">في حقل **تنسيق بيانات المصدر** حدد تنسيق الملف الذي يحتوي على حركات بطاقة الائتمان المراد استيرادها.</span><span class="sxs-lookup"><span data-stu-id="c21f6-112">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="c21f6-113">حدد **تحميل** ثم ابحث عن الملف وحدده ليتم استيراده.</span><span class="sxs-lookup"><span data-stu-id="c21f6-113">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="c21f6-114">بعد ان يتم تحميل الملف، قم بالتحقق من تعيين ملف حركة بطاقة الائتمان وأعمدة كيان بيانات حركات بطاقات الائتمان وذلك بتحديد الارتباط **عرض الخريطة** على اللوحة.</span><span class="sxs-lookup"><span data-stu-id="c21f6-114">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="c21f6-115">إذا كانت هناك أخطاء في التعيين، أو إذا كان يجب عليك تغيير التعيين، فقم بإجراء تغييرات التعيين إما من علامة التبويب **تعيين الرسوم المرئية** أو من علامة التبويب **تفاصيل التعيين**.</span><span class="sxs-lookup"><span data-stu-id="c21f6-115">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="c21f6-116">لأتمتة حركات بطاقة الائتمان، قم بتحديد **إنشاء مهمة بيانات متكررة**.</span><span class="sxs-lookup"><span data-stu-id="c21f6-116">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="c21f6-117">يمكنك بعد ذلك تعيين التكرار الذي يحدد عدد مرات تكرار استيراد حركات بطاقة الائتمان.</span><span class="sxs-lookup"><span data-stu-id="c21f6-117">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="c21f6-118">عند الانتهاء، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c21f6-118">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="c21f6-119">لاستيراد الملف المحدد الآن، حدد **استيراد**.</span><span class="sxs-lookup"><span data-stu-id="c21f6-119">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="c21f6-120">في حالة حدوث أخطاء أثناء عملية الاستيراد، يمكنك عرض سجل التنفيذ أو البيانات المرحلية لمعرفة الأخطاء التي يجب عليك إصلاحها لضمان نجاح عمليه الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="c21f6-120">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="c21f6-121">إذا كان يجب عليك استيراد أكثر من تنسيق ملف واحد، فيجب إنشاء مهام استيراد منفصلة لكل نوع من أنواع التنسيقات.</span><span class="sxs-lookup"><span data-stu-id="c21f6-121">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="c21f6-122">إعادة تعيين حركات بطاقات الائتمان للموظفين الذين تم إنهاؤهم</span><span class="sxs-lookup"><span data-stu-id="c21f6-122">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="c21f6-123">بعد إنهاء سجل موظف، يتم تعطيل حساب ‏‫خدمات مجال Active Directory (AD DS)‬ للموظف.</span><span class="sxs-lookup"><span data-stu-id="c21f6-123">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="c21f6-124">ومع ذلك، قد تكون هناك حركات بطاقة ائتمان نشطة يجب أن تظل مصروفة ومُسددة.</span><span class="sxs-lookup"><span data-stu-id="c21f6-124">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="c21f6-125">من صفحة **حركات بطاقة الائتمان** ، يمكنك إعاده تعيين الموظف لآيه حركة بطاقة ائتمان في المكان الذي تم فيه إنهاء الموظف المرتبط.</span><span class="sxs-lookup"><span data-stu-id="c21f6-125">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="c21f6-126">حدد حركه بطاقة ائتمان واحده أو أكثر، ثم حدد **إعادة تعيين الحركات**.</span><span class="sxs-lookup"><span data-stu-id="c21f6-126">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="c21f6-127">يمكنك بعد ذلك تحديد موظف آخر لتعيين حركات بطاقة الائتمان اليه.</span><span class="sxs-lookup"><span data-stu-id="c21f6-127">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="c21f6-128">بعد إعاده تعيين حركات بطاقة الائتمان، يمكن تحديدها لتقرير المصروفات ودفعها من خلال العملية المعتادة لتعويض تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="c21f6-128">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]