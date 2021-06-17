---
title: إعداد بيانات التكوين وتطبيقها في Common Data Service
description: يقدم هذا الموضوع معلومات حول إعداد وتطبيق بيانات التكوين في Project Operations.
author: sigitac
ms.date: 05/10/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2ea00df6112fb69b61f1889463424fdfee79aec9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001275"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="b61a4-103">إعداد بيانات التكوين وتطبيقها في Common Data Service</span><span class="sxs-lookup"><span data-stu-id="b61a4-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="b61a4-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="b61a4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="b61a4-105">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="b61a4-105">Prerequisites</span></span>

<span data-ttu-id="b61a4-106">قبل أن تبدأ في تهيئة البيانات في Common Data Service (CDS)، فإنه يجب استيفاء المتطلبات الأساسية التالية:</span><span class="sxs-lookup"><span data-stu-id="b61a4-106">Before you begin to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="b61a4-107">تزويد بيئة CDS وبيئة Dynamics 365 Finance لـ Project Operations.</span><span class="sxs-lookup"><span data-stu-id="b61a4-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="b61a4-108">مشاركة معلومات الكيان القانوني من Dynamics 365 Finance مع بيئة CDS.</span><span class="sxs-lookup"><span data-stu-id="b61a4-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="b61a4-109">وهذا يعني أن كيان **الشركة** في CDS يتضمن سجلات الشركة التالية:</span><span class="sxs-lookup"><span data-stu-id="b61a4-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="b61a4-110">THPM</span><span class="sxs-lookup"><span data-stu-id="b61a4-110">THPM</span></span>
  - <span data-ttu-id="b61a4-111">USPM</span><span class="sxs-lookup"><span data-stu-id="b61a4-111">USPM</span></span>
  - <span data-ttu-id="b61a4-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="b61a4-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="b61a4-113">تثبيت بيانات الإعداد والتكوين</span><span class="sxs-lookup"><span data-stu-id="b61a4-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="b61a4-114">قم بتنزيل وإلغاء حظر وفك ضغط [حزمة بيانات الإعداد والتكوين](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span><span class="sxs-lookup"><span data-stu-id="b61a4-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span></span>
2. <span data-ttu-id="b61a4-115">انتقل إلى المجلد غير المضغوط وقم بتشغيل الملف القابل للتنفيذ، *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="b61a4-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="b61a4-116">في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="b61a4-118">في الصفحة 2 من معالج CMT، حدد **Microsoft 365** على أنه **نوع النشر**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="b61a4-119">حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و **إظهار الخيارات المتقدمة**‬.</span><span class="sxs-lookup"><span data-stu-id="b61a4-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="b61a4-120">حدد منطقة المستأجر، وأدخل بيانات اعتمادك، وحدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="b61a4-122">في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي إليها، ثم حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="b61a4-123">في الصفحة 4، حدد الملف المضغوط *SampleSetupAndConfigData* من المجلد غير المضغوط.</span><span class="sxs-lookup"><span data-stu-id="b61a4-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![اختيار الملف المضغوط](./media/3ZipFile.png)

![تحديد ملف](./media/4SelectAFile.png)

9. <span data-ttu-id="b61a4-126">بعد تحديد ملف zip، حدد **استيراد البيانات**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-126">After the zip file is selected, select **Import Data**.</span></span>

![استيراد البيانات](./media/5ImportData.png)

10. <span data-ttu-id="b61a4-128">ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة.</span><span class="sxs-lookup"><span data-stu-id="b61a4-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="b61a4-129">بعد اكتمال الاستيراد، قم بإنهاء معالج CMT.</span><span class="sxs-lookup"><span data-stu-id="b61a4-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="b61a4-130">راجع مؤسستك للحصول على البيانات في 26 كيان التالي:</span><span class="sxs-lookup"><span data-stu-id="b61a4-130">Check your organization for data in the following 26 entities:</span></span>

  - <span data-ttu-id="b61a4-131">عملة</span><span class="sxs-lookup"><span data-stu-id="b61a4-131">Currency</span></span>
  - <span data-ttu-id="b61a4-132">مخطط الحسابات</span><span class="sxs-lookup"><span data-stu-id="b61a4-132">Chart of Accounts</span></span>
  - <span data-ttu-id="b61a4-133">التقويم المالي</span><span class="sxs-lookup"><span data-stu-id="b61a4-133">Fiscal Calendar</span></span>
  - <span data-ttu-id="b61a4-134">أنواع أسعار صرف العملة</span><span class="sxs-lookup"><span data-stu-id="b61a4-134">Currency Exchange Rate Types</span></span>
  - <span data-ttu-id="b61a4-135">يوم السداد</span><span class="sxs-lookup"><span data-stu-id="b61a4-135">Payment Day</span></span>
  - <span data-ttu-id="b61a4-136">جدولة الدفع</span><span class="sxs-lookup"><span data-stu-id="b61a4-136">Payment Schedule</span></span>
  - <span data-ttu-id="b61a4-137">شروط السداد</span><span class="sxs-lookup"><span data-stu-id="b61a4-137">Payment Term</span></span>
  - <span data-ttu-id="b61a4-138">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="b61a4-138">Organizational Unit</span></span>
  - <span data-ttu-id="b61a4-139">‏‫جهة الاتصال‬</span><span class="sxs-lookup"><span data-stu-id="b61a4-139">Contact</span></span>
  - <span data-ttu-id="b61a4-140">مجموعة الضرائب</span><span class="sxs-lookup"><span data-stu-id="b61a4-140">Tax Group</span></span>
  - <span data-ttu-id="b61a4-141">مجموعة العملاء</span><span class="sxs-lookup"><span data-stu-id="b61a4-141">Customer Group</span></span>
  - <span data-ttu-id="b61a4-142">مجموعة الموردين</span><span class="sxs-lookup"><span data-stu-id="b61a4-142">Vendor Group</span></span>
  - <span data-ttu-id="b61a4-143">الوحدة</span><span class="sxs-lookup"><span data-stu-id="b61a4-143">Unit</span></span>
  - <span data-ttu-id="b61a4-144">مجموعة وحدات</span><span class="sxs-lookup"><span data-stu-id="b61a4-144">Unit Group</span></span>
  - <span data-ttu-id="b61a4-145">قائمة الأسعار</span><span class="sxs-lookup"><span data-stu-id="b61a4-145">Price List</span></span>
  - <span data-ttu-id="b61a4-146">قائمة أسعار معلمات المشروع</span><span class="sxs-lookup"><span data-stu-id="b61a4-146">Project Parameter Price List</span></span>
  - <span data-ttu-id="b61a4-147">معدل تكرار الفاتورة</span><span class="sxs-lookup"><span data-stu-id="b61a4-147">Invoice Frequency</span></span>
  - <span data-ttu-id="b61a4-148">فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="b61a4-148">Bookable Resource Category</span></span>
  - <span data-ttu-id="b61a4-149">فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="b61a4-149">Transaction Category</span></span>
  - <span data-ttu-id="b61a4-150">فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="b61a4-150">Expense Category</span></span>
  - <span data-ttu-id="b61a4-151">سعر الدور</span><span class="sxs-lookup"><span data-stu-id="b61a4-151">Role Price</span></span>
  - <span data-ttu-id="b61a4-152">سعر فئة المعاملة</span><span class="sxs-lookup"><span data-stu-id="b61a4-152">Transaction Category Price</span></span>
  - <span data-ttu-id="b61a4-153">‏‫الخاصية‬</span><span class="sxs-lookup"><span data-stu-id="b61a4-153">Characteristic</span></span>
  - <span data-ttu-id="b61a4-154">المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="b61a4-154">Bookable Resource</span></span>
  - <span data-ttu-id="b61a4-155">تعيين فئة المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="b61a4-155">Bookable resource category Assn</span></span>
  - <span data-ttu-id="b61a4-156">خاصية المورد القابل للحجز</span><span class="sxs-lookup"><span data-stu-id="b61a4-156">Bookable Resource Characteristic</span></span>

![اكتمال الاستيراد](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="b61a4-158">تحديث تكوينات Project Operations</span><span class="sxs-lookup"><span data-stu-id="b61a4-158">Update Project Operations configurations</span></span>

1. <span data-ttu-id="b61a4-159">انتقل إلى بيئة CE.</span><span class="sxs-lookup"><span data-stu-id="b61a4-159">Navigate to the CE environment.</span></span> <span data-ttu-id="b61a4-160">يمكنك البحث عنها عن طريق فتح [مركز إدارة Power Platform](https://admin.powerplatform.microsoft.com/environments) وتحديد البيئة ثم تحديد **فتح البيئة**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-160">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![فتح البيئة](./media/7OpenEnvironment.png)

2. <span data-ttu-id="b61a4-162">انتقل إلى **المشروعات** > **الموارد** ثم حدد **جديد** لإنشاء مورد قابل للحجز للمستخدم الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="b61a4-162">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![الموارد القابلة للحجز](./media/8BookableResources.png)

3. <span data-ttu-id="b61a4-164">في علامة التبويب **عام**، حدد المستخدم المسؤول الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="b61a4-164">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="b61a4-165">تحقق من أن المنطقة الزمنية تتطابق مع تلك التي تعيش فيها.</span><span class="sxs-lookup"><span data-stu-id="b61a4-165">Verify that the time zone matches the one you are in.</span></span> 

![مورد جديد قابل للحجز](./media/9NewBookableResource.png)

4. <span data-ttu-id="b61a4-167">في علامة تبويب **الجدولة**، في حقل **الشركة**، قم اختيار شركة **USPM**، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-167">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![علامة تبويب الجدولة](./media/10SchedulingTab.png)

5. <span data-ttu-id="b61a4-169">حدد علامة التبويب **ساعات العمل**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-169">Select the **Work hours** tab.</span></span>  

![ساعات العمل](./media/11WorkHours.png)

6. <span data-ttu-id="b61a4-171">انقر نقرًا مزدوجًا فوق أي قيمة في التقويم وحدد **تحرير** > **كافة الأحداث في السلسلة**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-171">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![تقويم العمل](./media/12WorkCalendar.png)

7. <span data-ttu-id="b61a4-173">قم بتغيير ساعات العمل إلى يوم عمل من ثمانية (8) ساعات وقم بتعليم عطلات نهاية الأسبوع على أنها أيام بدون عمل، وتأكد من تطابق المنطقة الزمنية مع المنطقة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="b61a4-173">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="b61a4-174">حدد **حفظ وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-174">Select **Save and close**.</span></span>

![تحديث التقويم](./media/13UpdateCalendar.png)

9. <span data-ttu-id="b61a4-176">انتقل إلى **الإعدادات** > **قوالب التقويم** وحدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-176">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![قوالب التقويم](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="b61a4-178">أدخل اسمًا، وحدد مورد القالب الذي قمت بإنشائه، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-178">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![حفظ قالب التقويم](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="b61a4-180">انتقل إلى **المعلمات** وانقر نقرًا مزدوجًا فوق السجل.</span><span class="sxs-lookup"><span data-stu-id="b61a4-180">Go to **Parameters** and double-click the record.</span></span> 
 
 ![معلمات المشروع](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="b61a4-182">قم بتحديث الحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="b61a4-182">Update the following fields:</span></span>

 - <span data-ttu-id="b61a4-183">**الشركة الافتراضية**: USPM</span><span class="sxs-lookup"><span data-stu-id="b61a4-183">**Default company**: USPM</span></span>
 - <span data-ttu-id="b61a4-184">**الوحدة المؤسسية الافتراضية**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="b61a4-184">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="b61a4-185">**تكرار الفاتورة**: اليوم السابع واليوم الأخير</span><span class="sxs-lookup"><span data-stu-id="b61a4-185">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="b61a4-186">**قالب ساعة العمل**: قم بالتغيير إلى القالب الذي قمت بإنشائه.</span><span class="sxs-lookup"><span data-stu-id="b61a4-186">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="b61a4-187">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="b61a4-187">Select **Save**.</span></span> 

![معلمات المشروع المحدثة](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
