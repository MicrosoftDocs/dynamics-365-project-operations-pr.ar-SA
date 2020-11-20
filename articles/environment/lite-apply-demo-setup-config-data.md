---
title: تطبيق إعداد العرض التوضيحي وبيانات التكوين - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين في Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5cfc270c07a568d692f6cd180b9c367ae185044c
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401247"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="e2dcc-103">تطبيق إعداد العرض التوضيحي وبيانات التكوين لـ Project Operations - خفيف</span><span class="sxs-lookup"><span data-stu-id="e2dcc-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="e2dcc-104">_\*\*النشر الخفيف - التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="e2dcc-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2dcc-105">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="e2dcc-105">Prerequisites</span></span>

<span data-ttu-id="e2dcc-106">قبل بدء التكوين، يجب أن تتوفر لديك بيئة Common Data Service (CDS) تم تزويدها لـ Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="e2dcc-107">إرشادات</span><span class="sxs-lookup"><span data-stu-id="e2dcc-107">Instructions</span></span>

1. <span data-ttu-id="e2dcc-108">قم بتنزيل [حزمة البيانات الرئيسية](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="e2dcc-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="e2dcc-109">انتقل إلى المجلد *ProjOpsDemoDataSetupAndMaster - Integrated CMT*، وقم بتشغيل الملف القابل للتنفيذ *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="e2dcc-110">في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="e2dcc-112">في الصفحة 2 من معالج CMT، حدد **Microsoft 365** على أنه **نوع النشر**.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="e2dcc-113">حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و **إظهار الخيارات المتقدمة**‬.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="e2dcc-114">حدد منطقة المستأجر، وأدخل بيانات اعتمادك، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="e2dcc-116">في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي اليها، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="e2dcc-117">في الصفحة 4، حدد ملف zip، *MasterAndSetupData*، من المجلد الذي تم فك ضغطه، *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![ملف مضغوط](./media/3ZipFile.png)

![تحديد ملف](./media/4SelectAFile.png)

9. <span data-ttu-id="e2dcc-120">بعد تحديد ملف zip، حدد **استيراد البيانات**.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-120">After the zip file is selected, select **Import Data**.</span></span>

![استيراد البيانات](./media/5ImportData.png)

10. <span data-ttu-id="e2dcc-122">ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="e2dcc-123">بعد اكتمالها، يمكنك إنهاء معالج CMT.</span><span class="sxs-lookup"><span data-stu-id="e2dcc-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="e2dcc-124">راجع مؤسستك للحصول على البيانات في الكيانات العشرين التالية:</span><span class="sxs-lookup"><span data-stu-id="e2dcc-124">Check your organization for data in the following 20 entities:</span></span>

-   <span data-ttu-id="e2dcc-125">عملة</span><span class="sxs-lookup"><span data-stu-id="e2dcc-125">Currency</span></span>
-   <span data-ttu-id="e2dcc-126">عميل</span><span class="sxs-lookup"><span data-stu-id="e2dcc-126">Account</span></span>
-   <span data-ttu-id="e2dcc-127">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="e2dcc-127">Organizational Unit</span></span>
-   <span data-ttu-id="e2dcc-128">جهة اتصال</span><span class="sxs-lookup"><span data-stu-id="e2dcc-128">Contact</span></span>
-   <span data-ttu-id="e2dcc-129">مجموعة الضرائب</span><span class="sxs-lookup"><span data-stu-id="e2dcc-129">Tax Group</span></span>
-   <span data-ttu-id="e2dcc-130">مجموعة العملاء</span><span class="sxs-lookup"><span data-stu-id="e2dcc-130">Customer Group</span></span>
-   <span data-ttu-id="e2dcc-131">الوحدة</span><span class="sxs-lookup"><span data-stu-id="e2dcc-131">Unit</span></span>
-   <span data-ttu-id="e2dcc-132">مجموعة وحدات</span><span class="sxs-lookup"><span data-stu-id="e2dcc-132">Unit Group</span></span>
-   <span data-ttu-id="e2dcc-133">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="e2dcc-133">Price List</span></span>
-   <span data-ttu-id="e2dcc-134">قائمة أسعار معلمات المشروع</span><span class="sxs-lookup"><span data-stu-id="e2dcc-134">Project Parameter Price List</span></span> 
-   <span data-ttu-id="e2dcc-135">معدل تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="e2dcc-135">Invoice Frequency</span></span>
-   <span data-ttu-id="e2dcc-136">فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="e2dcc-136">Bookable Resource Category</span></span>
-   <span data-ttu-id="e2dcc-137">فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="e2dcc-137">Transaction Category</span></span>
-   <span data-ttu-id="e2dcc-138">فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="e2dcc-138">Expense Category</span></span>
-   <span data-ttu-id="e2dcc-139">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="e2dcc-139">Role Price</span></span>
-   <span data-ttu-id="e2dcc-140">سعر فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="e2dcc-140">Transaction Category Price</span></span>
-   <span data-ttu-id="e2dcc-141">‏‫الخاصية‬</span><span class="sxs-lookup"><span data-stu-id="e2dcc-141">Characteristic</span></span>
-   <span data-ttu-id="e2dcc-142">المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="e2dcc-142">Bookable Resource</span></span>
-   <span data-ttu-id="e2dcc-143">تعيين فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="e2dcc-143">Bookable resource category Assn</span></span>
-   <span data-ttu-id="e2dcc-144">خاصية المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="e2dcc-144">Bookable Resource Characteristic</span></span>

![اكتمال الاستيراد](./media/6CompleteImport.png)
