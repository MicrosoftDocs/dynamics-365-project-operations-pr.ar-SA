---
title: إعداد وتطبيق بيانات التكوين في Common Data Service لـ Project Operations
description: يقدم هذا الموضوع معلومات حول إعداد وتطبيق بيانات التكوين في Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5e72b88a4dae1eb89859fdfd55f6d5e6ee5befcd
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070517"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a><span data-ttu-id="841e5-103">إعداد وتطبيق بيانات التكوين في Common Data Service لـ Project Operations</span><span class="sxs-lookup"><span data-stu-id="841e5-103">Set up and apply configuration data in the Common Data Service for Project Operations</span></span>

<span data-ttu-id="841e5-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="841e5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="841e5-105">تثبيت بيانات الإعداد والتكوين</span><span class="sxs-lookup"><span data-stu-id="841e5-105">Install setup and configuration data</span></span>

1. <span data-ttu-id="841e5-106">قم بتنزيل وإلغاء حظر وفك ضغط [حزمة بيانات الإعداد والتكوين](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="841e5-106">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="841e5-107">انتقل إلى المجلد غير المضغوط وقم بتشغيل الملف القابل للتنفيذ، *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="841e5-107">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="841e5-108">في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.</span><span class="sxs-lookup"><span data-stu-id="841e5-108">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="841e5-110">في الصفحة 2 من معالج CMT، حدد **Microsoft 365** على أنه **نوع النشر**.</span><span class="sxs-lookup"><span data-stu-id="841e5-110">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="841e5-111">حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و **إظهار الخيارات المتقدمة** ‬.</span><span class="sxs-lookup"><span data-stu-id="841e5-111">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="841e5-112">حدد منطقة المستأجر، وأدخل بيانات اعتمادك، وحدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="841e5-112">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="841e5-114">في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي إليها، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="841e5-114">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="841e5-115">في الصفحة 4، حدد الملف المضغوط *SampleSetupAndConfigData* من المجلد غير المضغوط.</span><span class="sxs-lookup"><span data-stu-id="841e5-115">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![اختيار الملف المضغوط](./media/3ZipFile.png)

![تحديد ملف](./media/4SelectAFile.png)

9. <span data-ttu-id="841e5-118">بعد تحديد ملف zip، حدد **استيراد البيانات**.</span><span class="sxs-lookup"><span data-stu-id="841e5-118">After the zip file is selected, select **Import Data**.</span></span>

![استيراد البيانات](./media/5ImportData.png)

10. <span data-ttu-id="841e5-120">ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة.</span><span class="sxs-lookup"><span data-stu-id="841e5-120">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="841e5-121">بعد اكتمال الاستيراد، قم بإنهاء معالج CMT.</span><span class="sxs-lookup"><span data-stu-id="841e5-121">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="841e5-122">راجع مؤسستك للحصول على البيانات في 19 كيان التالي:</span><span class="sxs-lookup"><span data-stu-id="841e5-122">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="841e5-123">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="841e5-123">Currency</span></span>
  - <span data-ttu-id="841e5-124">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="841e5-124">Organizational Unit</span></span>
  - <span data-ttu-id="841e5-125">جهة اتصال</span><span class="sxs-lookup"><span data-stu-id="841e5-125">Contact</span></span>
  - <span data-ttu-id="841e5-126">مجموعة الضرائب</span><span class="sxs-lookup"><span data-stu-id="841e5-126">Tax Group</span></span>
  - <span data-ttu-id="841e5-127">مجموعة العملاء</span><span class="sxs-lookup"><span data-stu-id="841e5-127">Customer Group</span></span>
  - <span data-ttu-id="841e5-128">الوحدة</span><span class="sxs-lookup"><span data-stu-id="841e5-128">Unit</span></span>
  - <span data-ttu-id="841e5-129">مجموعة وحدات</span><span class="sxs-lookup"><span data-stu-id="841e5-129">Unit Group</span></span>
  - <span data-ttu-id="841e5-130">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="841e5-130">Price List</span></span>
  - <span data-ttu-id="841e5-131">قائمة أسعار معلمات المشروع</span><span class="sxs-lookup"><span data-stu-id="841e5-131">Project Parameter Price List</span></span>
  - <span data-ttu-id="841e5-132">معدل تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="841e5-132">Invoice Frequency</span></span>
  - <span data-ttu-id="841e5-133">فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="841e5-133">Bookable Resource Category</span></span>
  - <span data-ttu-id="841e5-134">فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="841e5-134">Transaction Category</span></span>
  - <span data-ttu-id="841e5-135">فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="841e5-135">Expense Category</span></span>
  - <span data-ttu-id="841e5-136">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="841e5-136">Role Price</span></span>
  - <span data-ttu-id="841e5-137">سعر فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="841e5-137">Transaction Category Price</span></span>
  - <span data-ttu-id="841e5-138">‏‫الخاصية‬</span><span class="sxs-lookup"><span data-stu-id="841e5-138">Characteristic</span></span>
  - <span data-ttu-id="841e5-139">المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="841e5-139">Bookable Resource</span></span>
  - <span data-ttu-id="841e5-140">تعيين فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="841e5-140">Bookable resource category Assn</span></span>
  - <span data-ttu-id="841e5-141">خاصية المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="841e5-141">Bookable Resource Characteristic</span></span>

![اكتمال الاستيراد](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="841e5-143">تحديث تكوينات Project Operations</span><span class="sxs-lookup"><span data-stu-id="841e5-143">Update Project Operations configurations</span></span>

1. <span data-ttu-id="841e5-144">انتقل إلى بيئة CE.</span><span class="sxs-lookup"><span data-stu-id="841e5-144">Navigate to the CE environment.</span></span> <span data-ttu-id="841e5-145">يمكنك البحث عنها عن طريق فتح [مركز إدارة Power Platform](https://admin.powerplatform.microsoft.com/environments) وتحديد البيئة ثم تحديد **فتح البيئة**.</span><span class="sxs-lookup"><span data-stu-id="841e5-145">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![فتح البيئة](./media/7OpenEnvironment.png)

2. <span data-ttu-id="841e5-147">انتقل إلى **المشروعات** > **الموارد** ثم حدد **جديد** لإنشاء مورد قابل للحجز للمستخدم الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="841e5-147">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![الموارد القابلة للحجز](./media/8BookableResources.png)

3. <span data-ttu-id="841e5-149">في علامة التبويب **عام** ، حدد المستخدم المسؤول الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="841e5-149">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="841e5-150">تحقق من أن المنطقة الزمنية تتطابق مع تلك التي تعيش فيها.</span><span class="sxs-lookup"><span data-stu-id="841e5-150">Verify that the time zone matches the one you are in.</span></span> 

![مورد جديد قابل للحجز](./media/9NewBookableResource.png)

4. <span data-ttu-id="841e5-152">في علامة تبويب **الجدولة** ، في حقل **الشركة** ، قم اختيار شركة **USPM** ، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="841e5-152">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![علامة تبويب الجدولة](./media/10SchedulingTab.png)

5. <span data-ttu-id="841e5-154">حدد علامة التبويب **ساعات العمل**.</span><span class="sxs-lookup"><span data-stu-id="841e5-154">Select the **Work hours** tab.</span></span>  

![ساعات العمل](./media/11WorkHours.png)

6. <span data-ttu-id="841e5-156">انقر نقرًا مزدوجًا فوق أي قيمة في التقويم وحدد **تحرير** > **كافة الأحداث في السلسلة**.</span><span class="sxs-lookup"><span data-stu-id="841e5-156">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![تقويم العمل](./media/12WorkCalendar.png)

7. <span data-ttu-id="841e5-158">قم بتغيير ساعات العمل إلى يوم عمل من ثمانية (8) ساعات وقم بتعليم عطلات نهاية الأسبوع على أنها أيام بدون عمل، وتأكد من تطابق المنطقة الزمنية مع المنطقة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="841e5-158">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="841e5-159">حدد **حفظ وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="841e5-159">Select **Save and close**.</span></span>

![تحديث التقويم](./media/13UpdateCalendar.png)

9. <span data-ttu-id="841e5-161">انتقل إلى **الإعدادات** > **قوالب التقويم** وحدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="841e5-161">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![قوالب التقويم](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="841e5-163">أدخل اسمًا، وحدد مورد القالب الذي قمت بإنشائه، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="841e5-163">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![حفظ قالب التقويم](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="841e5-165">انتقل إلى **المعلمات** وانقر نقرًا مزدوجًا فوق السجل.</span><span class="sxs-lookup"><span data-stu-id="841e5-165">Go to **Parameters** and double-click the record.</span></span> 
 
 ![معلمات المشروع](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="841e5-167">قم بتحديث الحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="841e5-167">Update the following fields:</span></span>

 - <span data-ttu-id="841e5-168">**الشركة الافتراضية** : USPM</span><span class="sxs-lookup"><span data-stu-id="841e5-168">**Default company** : USPM</span></span>
 - <span data-ttu-id="841e5-169">**الوحدة التنظيمية الافتراضية** : Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="841e5-169">**Default Organizational Unit** : Contoso Robotics Global</span></span>
 - <span data-ttu-id="841e5-170">**تكرار الفاتورة** : اليوم السابع واليوم الأخير</span><span class="sxs-lookup"><span data-stu-id="841e5-170">**Invoice Frequency** : Seventh and Last day</span></span>
 - <span data-ttu-id="841e5-171">**قالب ساعة العمل** : قم بالتغيير إلى القالب الذي قمت بإنشائه.</span><span class="sxs-lookup"><span data-stu-id="841e5-171">**Work hour template** : Change to the template you created.</span></span>

13. <span data-ttu-id="841e5-172">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="841e5-172">Select **Save**.</span></span> 

![معلمات المشروع المحدثة](./media/17UpdatedProjectParameters.png)
