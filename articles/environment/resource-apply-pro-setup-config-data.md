---
title: إعداد بيانات التكوين وتطبيقها في Common Data Service
description: يقدم هذا الموضوع معلومات حول إعداد وتطبيق بيانات التكوين في Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7742e81316b217066f9f3b8d5c23aa64f1a7efc4
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642212"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="54bcd-103">إعداد بيانات التكوين وتطبيقها في Common Data Service</span><span class="sxs-lookup"><span data-stu-id="54bcd-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="54bcd-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="54bcd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="54bcd-105">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="54bcd-105">Prerequisites</span></span>

<span data-ttu-id="54bcd-106">قبل أن تبدأ تكوين البيانات في Common Data Service (CDS)، يجب استيفاء المتطلبات الأساسية التالية:</span><span class="sxs-lookup"><span data-stu-id="54bcd-106">Before you beging to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="54bcd-107">تزويد بيئة CDS وبيئة Dynamics 365 Finance لـ Project Operations.</span><span class="sxs-lookup"><span data-stu-id="54bcd-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="54bcd-108">مشاركة معلومات الكيان القانوني من Dynamics 365 Finance مع بيئة CDS.</span><span class="sxs-lookup"><span data-stu-id="54bcd-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="54bcd-109">وهذا يعني أن كيان **الشركة** في CDS يتضمن سجلات الشركة التالية:</span><span class="sxs-lookup"><span data-stu-id="54bcd-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="54bcd-110">THPM</span><span class="sxs-lookup"><span data-stu-id="54bcd-110">THPM</span></span>
  - <span data-ttu-id="54bcd-111">USPM</span><span class="sxs-lookup"><span data-stu-id="54bcd-111">USPM</span></span>
  - <span data-ttu-id="54bcd-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="54bcd-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="54bcd-113">تثبيت بيانات الإعداد والتكوين</span><span class="sxs-lookup"><span data-stu-id="54bcd-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="54bcd-114">قم بتنزيل وإلغاء حظر وفك ضغط [حزمة بيانات الإعداد والتكوين](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="54bcd-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="54bcd-115">انتقل إلى المجلد غير المضغوط وقم بتشغيل الملف القابل للتنفيذ، *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="54bcd-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="54bcd-116">في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="54bcd-118">في الصفحة 2 من معالج CMT، حدد **Microsoft 365** على أنه **نوع النشر**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="54bcd-119">حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و **إظهار الخيارات المتقدمة**‬.</span><span class="sxs-lookup"><span data-stu-id="54bcd-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="54bcd-120">حدد منطقة المستأجر، وأدخل بيانات اعتمادك، وحدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="54bcd-122">في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي إليها، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="54bcd-123">في الصفحة 4، حدد الملف المضغوط *SampleSetupAndConfigData* من المجلد غير المضغوط.</span><span class="sxs-lookup"><span data-stu-id="54bcd-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![اختيار الملف المضغوط](./media/3ZipFile.png)

![تحديد ملف](./media/4SelectAFile.png)

9. <span data-ttu-id="54bcd-126">بعد تحديد ملف zip، حدد **استيراد البيانات**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-126">After the zip file is selected, select **Import Data**.</span></span>

![استيراد البيانات](./media/5ImportData.png)

10. <span data-ttu-id="54bcd-128">ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة.</span><span class="sxs-lookup"><span data-stu-id="54bcd-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="54bcd-129">بعد اكتمال الاستيراد، قم بإنهاء معالج CMT.</span><span class="sxs-lookup"><span data-stu-id="54bcd-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="54bcd-130">راجع مؤسستك للحصول على البيانات في 19 كيان التالي:</span><span class="sxs-lookup"><span data-stu-id="54bcd-130">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="54bcd-131">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="54bcd-131">Currency</span></span>
  - <span data-ttu-id="54bcd-132">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="54bcd-132">Organizational Unit</span></span>
  - <span data-ttu-id="54bcd-133">جهة اتصال</span><span class="sxs-lookup"><span data-stu-id="54bcd-133">Contact</span></span>
  - <span data-ttu-id="54bcd-134">مجموعة الضرائب</span><span class="sxs-lookup"><span data-stu-id="54bcd-134">Tax Group</span></span>
  - <span data-ttu-id="54bcd-135">مجموعة العملاء</span><span class="sxs-lookup"><span data-stu-id="54bcd-135">Customer Group</span></span>
  - <span data-ttu-id="54bcd-136">الوحدة</span><span class="sxs-lookup"><span data-stu-id="54bcd-136">Unit</span></span>
  - <span data-ttu-id="54bcd-137">مجموعة وحدات</span><span class="sxs-lookup"><span data-stu-id="54bcd-137">Unit Group</span></span>
  - <span data-ttu-id="54bcd-138">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="54bcd-138">Price List</span></span>
  - <span data-ttu-id="54bcd-139">قائمة أسعار معلمات المشروع</span><span class="sxs-lookup"><span data-stu-id="54bcd-139">Project Parameter Price List</span></span>
  - <span data-ttu-id="54bcd-140">معدل تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="54bcd-140">Invoice Frequency</span></span>
  - <span data-ttu-id="54bcd-141">فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="54bcd-141">Bookable Resource Category</span></span>
  - <span data-ttu-id="54bcd-142">فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="54bcd-142">Transaction Category</span></span>
  - <span data-ttu-id="54bcd-143">فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="54bcd-143">Expense Category</span></span>
  - <span data-ttu-id="54bcd-144">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="54bcd-144">Role Price</span></span>
  - <span data-ttu-id="54bcd-145">سعر فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="54bcd-145">Transaction Category Price</span></span>
  - <span data-ttu-id="54bcd-146">‏‫الخاصية‬</span><span class="sxs-lookup"><span data-stu-id="54bcd-146">Characteristic</span></span>
  - <span data-ttu-id="54bcd-147">المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="54bcd-147">Bookable Resource</span></span>
  - <span data-ttu-id="54bcd-148">تعيين فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="54bcd-148">Bookable resource category Assn</span></span>
  - <span data-ttu-id="54bcd-149">خاصية المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="54bcd-149">Bookable Resource Characteristic</span></span>

![اكتمال الاستيراد](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="54bcd-151">تحديث تكوينات Project Operations</span><span class="sxs-lookup"><span data-stu-id="54bcd-151">Update Project Operations configurations</span></span>

1. <span data-ttu-id="54bcd-152">انتقل إلى بيئة CE.</span><span class="sxs-lookup"><span data-stu-id="54bcd-152">Navigate to the CE environment.</span></span> <span data-ttu-id="54bcd-153">يمكنك البحث عنها عن طريق فتح [مركز إدارة Power Platform](https://admin.powerplatform.microsoft.com/environments) وتحديد البيئة ثم تحديد **فتح البيئة**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-153">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![فتح البيئة](./media/7OpenEnvironment.png)

2. <span data-ttu-id="54bcd-155">انتقل إلى **المشروعات** > **الموارد** ثم حدد **جديد** لإنشاء مورد قابل للحجز للمستخدم الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="54bcd-155">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![الموارد القابلة للحجز](./media/8BookableResources.png)

3. <span data-ttu-id="54bcd-157">في علامة التبويب **عام**، حدد المستخدم المسؤول الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="54bcd-157">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="54bcd-158">تحقق من أن المنطقة الزمنية تتطابق مع تلك التي تعيش فيها.</span><span class="sxs-lookup"><span data-stu-id="54bcd-158">Verify that the time zone matches the one you are in.</span></span> 

![مورد جديد قابل للحجز](./media/9NewBookableResource.png)

4. <span data-ttu-id="54bcd-160">في علامة تبويب **الجدولة**، في حقل **الشركة**، قم اختيار شركة **USPM**، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-160">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![علامة تبويب الجدولة](./media/10SchedulingTab.png)

5. <span data-ttu-id="54bcd-162">حدد علامة التبويب **ساعات العمل**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-162">Select the **Work hours** tab.</span></span>  

![ساعات العمل](./media/11WorkHours.png)

6. <span data-ttu-id="54bcd-164">انقر نقرًا مزدوجًا فوق أي قيمة في التقويم وحدد **تحرير** > **كافة الأحداث في السلسلة**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-164">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![تقويم العمل](./media/12WorkCalendar.png)

7. <span data-ttu-id="54bcd-166">قم بتغيير ساعات العمل إلى يوم عمل من ثمانية (8) ساعات وقم بتعليم عطلات نهاية الأسبوع على أنها أيام بدون عمل، وتأكد من تطابق المنطقة الزمنية مع المنطقة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="54bcd-166">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="54bcd-167">حدد **حفظ وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-167">Select **Save and close**.</span></span>

![تحديث التقويم](./media/13UpdateCalendar.png)

9. <span data-ttu-id="54bcd-169">انتقل إلى **الإعدادات** > **قوالب التقويم** وحدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-169">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![قوالب التقويم](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="54bcd-171">أدخل اسمًا، وحدد مورد القالب الذي قمت بإنشائه، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-171">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![حفظ قالب التقويم](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="54bcd-173">انتقل إلى **المعلمات** وانقر نقرًا مزدوجًا فوق السجل.</span><span class="sxs-lookup"><span data-stu-id="54bcd-173">Go to **Parameters** and double-click the record.</span></span> 
 
 ![معلمات المشروع](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="54bcd-175">قم بتحديث الحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="54bcd-175">Update the following fields:</span></span>

 - <span data-ttu-id="54bcd-176">**الشركة الافتراضية**: USPM</span><span class="sxs-lookup"><span data-stu-id="54bcd-176">**Default company**: USPM</span></span>
 - <span data-ttu-id="54bcd-177">**الوحدة التنظيمية الافتراضية**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="54bcd-177">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="54bcd-178">**تكرار الفاتورة**: اليوم السابع واليوم الأخير</span><span class="sxs-lookup"><span data-stu-id="54bcd-178">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="54bcd-179">**قالب ساعة العمل**: قم بالتغيير إلى القالب الذي قمت بإنشائه.</span><span class="sxs-lookup"><span data-stu-id="54bcd-179">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="54bcd-180">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="54bcd-180">Select **Save**.</span></span> 

![معلمات المشروع المحدثة](./media/17UpdatedProjectParameters.png)
