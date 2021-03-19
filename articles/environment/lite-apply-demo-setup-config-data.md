---
title: تطبيق إعداد العرض التوضيحي وبيانات التكوين - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين في Project Operations.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 694dbc74591de74895095a9da6e590069711fc83
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290118"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="8bd8a-103">تطبيق إعداد العرض التوضيحي وبيانات التكوين لـ Project Operations - خفيف</span><span class="sxs-lookup"><span data-stu-id="8bd8a-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="8bd8a-104">_\*\*النشر الخفيف - التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="8bd8a-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="8bd8a-105">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="8bd8a-105">Prerequisites</span></span>

<span data-ttu-id="8bd8a-106">قبل بدء التكوين، يجب أن تتوفر لديك بيئة Common Data Service (CDS) تم تزويدها لـ Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="8bd8a-107">إرشادات</span><span class="sxs-lookup"><span data-stu-id="8bd8a-107">Instructions</span></span>

1. <span data-ttu-id="8bd8a-108">قم بتنزيل [حزمة البيانات الرئيسية](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="8bd8a-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="8bd8a-109">انتقل إلى المجلد *ProjOpsDemoDataSetupAndMaster - Integrated CMT*، وقم بتشغيل الملف القابل للتنفيذ *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="8bd8a-110">في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="8bd8a-112">في الصفحة 2 من معالج CMT، حدد **Microsoft 365** على أنه **نوع النشر**.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="8bd8a-113">حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و **إظهار الخيارات المتقدمة**‬.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="8bd8a-114">حدد منطقة المستأجر، وأدخل بيانات اعتمادك، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="8bd8a-116">في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي اليها، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="8bd8a-117">في الصفحة 4، حدد ملف zip، *MasterAndSetupData*، من المجلد الذي تم فك ضغطه، *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

   ![ملف مضغوط](./media/3ZipFile.png)

   ![تحديد ملف](./media/4SelectAFile.png)

9. <span data-ttu-id="8bd8a-120">بعد تحديد ملف zip، حدد **استيراد البيانات**.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-120">After the zip file is selected, select **Import Data**.</span></span>

   ![استيراد البيانات](./media/5ImportData.png)

10. <span data-ttu-id="8bd8a-122">ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="8bd8a-123">بعد اكتمالها، يمكنك إنهاء معالج CMT.</span><span class="sxs-lookup"><span data-stu-id="8bd8a-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="8bd8a-124">راجع مؤسستك للحصول على البيانات في الكيانات العشرين التالية:</span><span class="sxs-lookup"><span data-stu-id="8bd8a-124">Check your organization for data in the following 20 entities:</span></span>

    -   <span data-ttu-id="8bd8a-125">عملة</span><span class="sxs-lookup"><span data-stu-id="8bd8a-125">Currency</span></span>
    -   <span data-ttu-id="8bd8a-126">الحساب</span><span class="sxs-lookup"><span data-stu-id="8bd8a-126">Account</span></span>
    -   <span data-ttu-id="8bd8a-127">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="8bd8a-127">Organizational Unit</span></span>
    -   <span data-ttu-id="8bd8a-128">‏‫جهة الاتصال‬</span><span class="sxs-lookup"><span data-stu-id="8bd8a-128">Contact</span></span>
    -   <span data-ttu-id="8bd8a-129">الوحدة</span><span class="sxs-lookup"><span data-stu-id="8bd8a-129">Unit</span></span>
    -   <span data-ttu-id="8bd8a-130">مجموعة وحدات</span><span class="sxs-lookup"><span data-stu-id="8bd8a-130">Unit Group</span></span>
    -   <span data-ttu-id="8bd8a-131">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="8bd8a-131">Price List</span></span>
    -   <span data-ttu-id="8bd8a-132">قائمة أسعار معلمات المشروع</span><span class="sxs-lookup"><span data-stu-id="8bd8a-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="8bd8a-133">معدل تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="8bd8a-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="8bd8a-134">فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="8bd8a-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="8bd8a-135">فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="8bd8a-135">Transaction Category</span></span>
    -   <span data-ttu-id="8bd8a-136">فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="8bd8a-136">Expense Category</span></span>
    -   <span data-ttu-id="8bd8a-137">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="8bd8a-137">Role Price</span></span>
    -   <span data-ttu-id="8bd8a-138">سعر فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="8bd8a-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="8bd8a-139">‏‫الخاصية‬</span><span class="sxs-lookup"><span data-stu-id="8bd8a-139">Characteristic</span></span>
    -   <span data-ttu-id="8bd8a-140">المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="8bd8a-140">Bookable Resource</span></span>
    -   <span data-ttu-id="8bd8a-141">تعيين فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="8bd8a-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="8bd8a-142">خاصية المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="8bd8a-142">Bookable Resource Characteristic</span></span>

    ![اكتمال الاستيراد](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]