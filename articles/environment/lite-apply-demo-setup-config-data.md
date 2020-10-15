---
title: تطبيق اعداد بيانات العرض التوضيحي وبيانات التكوين
description: يقدم هذا الموضوع معلومات حول كيفية تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين في Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42e02f393e89d20b2a462645f519a3792bee8f2f
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948717"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="60c8c-103">تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين لعملية نشر Project Operations Lite – التعامل مع الفواتير الأولية‬.‬</span><span class="sxs-lookup"><span data-stu-id="60c8c-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="60c8c-104">_\*\*النشر الخفيف - التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="60c8c-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="60c8c-105">قم بتنزيل [حزمة البيانات الرئيسية](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="60c8c-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="60c8c-106">انتقل إلى المجلد *ProjOpsDemoDataSetupAndMaster - Integrated CMT*، وقم بتشغيل الملف القابل للتنفيذ *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="60c8c-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="60c8c-107">في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.</span><span class="sxs-lookup"><span data-stu-id="60c8c-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="60c8c-109">في الصفحة 2 من معالج CMT، حدد **Office 365** على أنه **نوع النشر**.</span><span class="sxs-lookup"><span data-stu-id="60c8c-109">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="60c8c-110">حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و**إظهار الخيارات المتقدمة**‬.</span><span class="sxs-lookup"><span data-stu-id="60c8c-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="60c8c-111">حدد منطقة المستأجر، وأدخل بيانات اعتمادك، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="60c8c-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="60c8c-113">في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي اليها، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="60c8c-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="60c8c-114">في الصفحة 4، حدد ملف zip، *MasterAndSetupData*، من المجلد الذي تم فك ضغطه، *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="60c8c-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![ملف مضغوط](./media/3ZipFile.png)

![تحديد ملف](./media/4SelectAFile.png)

9. <span data-ttu-id="60c8c-117">بعد تحديد ملف zip، حدد **استيراد البيانات**.</span><span class="sxs-lookup"><span data-stu-id="60c8c-117">After the zip file is selected, select **Import Data**.</span></span>

![استيراد البيانات](./media/5ImportData.png)

10. <span data-ttu-id="60c8c-119">ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة.</span><span class="sxs-lookup"><span data-stu-id="60c8c-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="60c8c-120">بعد اكتمالها، يمكنك إنهاء معالج CMT.</span><span class="sxs-lookup"><span data-stu-id="60c8c-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="60c8c-121">راجع مؤسستك للحصول على البيانات في الكيانات العشرين التالية:</span><span class="sxs-lookup"><span data-stu-id="60c8c-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="60c8c-122">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="60c8c-122">Currency</span></span>
- <span data-ttu-id="60c8c-123">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="60c8c-123">Organizational Unit</span></span>
- <span data-ttu-id="60c8c-124">جهة اتصال</span><span class="sxs-lookup"><span data-stu-id="60c8c-124">Contact</span></span>
- <span data-ttu-id="60c8c-125">مجموعة الضرائب</span><span class="sxs-lookup"><span data-stu-id="60c8c-125">Tax Group</span></span>
- <span data-ttu-id="60c8c-126">مجموعة العملاء</span><span class="sxs-lookup"><span data-stu-id="60c8c-126">Customer Group</span></span>
- <span data-ttu-id="60c8c-127">الوحدة</span><span class="sxs-lookup"><span data-stu-id="60c8c-127">Unit</span></span>
- <span data-ttu-id="60c8c-128">مجموعة وحدات</span><span class="sxs-lookup"><span data-stu-id="60c8c-128">Unit Group</span></span>
- <span data-ttu-id="60c8c-129">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="60c8c-129">Price List</span></span>
- <span data-ttu-id="60c8c-130">قائمة أسعار معلمات المشروع</span><span class="sxs-lookup"><span data-stu-id="60c8c-130">Project Parameter Price List</span></span>
- <span data-ttu-id="60c8c-131">معدل تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="60c8c-131">Invoice Frequency</span></span>
- <span data-ttu-id="60c8c-132">تفاصيل تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="60c8c-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="60c8c-133">فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="60c8c-133">Bookable Resource Category</span></span>
- <span data-ttu-id="60c8c-134">فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="60c8c-134">Transaction Category</span></span>
- <span data-ttu-id="60c8c-135">فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="60c8c-135">Expense Category</span></span>
- <span data-ttu-id="60c8c-136">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="60c8c-136">Role Price</span></span>
- <span data-ttu-id="60c8c-137">سعر فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="60c8c-137">Transaction Category Price</span></span>
- <span data-ttu-id="60c8c-138">‏‫الخاصية‬</span><span class="sxs-lookup"><span data-stu-id="60c8c-138">Characteristic</span></span>
- <span data-ttu-id="60c8c-139">المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="60c8c-139">Bookable Resource</span></span>
- <span data-ttu-id="60c8c-140">تعيين فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="60c8c-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="60c8c-141">خاصية المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="60c8c-141">Bookable Resource Characteristic</span></span>

![اكتمال الاستيراد](./media/6CompleteImport.png)
