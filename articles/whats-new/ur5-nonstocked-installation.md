---
title: تحديث Project Operations في بيئة Finance
description: يقدم هذا الموضوع معلومات حول كيفية تحديث Project Operations في بيئة Dynamics 365 Finance الخاصة بك.
author: ruhercul
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d85a180aa094a048b4422605b25151d10785f67d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6011040"
---
# <a name="update-project-operations-in-your-finance-environment"></a><span data-ttu-id="ebff5-103">تحديث Project Operations في بيئة Finance</span><span class="sxs-lookup"><span data-stu-id="ebff5-103">Update Project Operations in your Finance environment</span></span>

<span data-ttu-id="ebff5-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="ebff5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="ebff5-105">يقدم هذا الموضوع معلومات حول كيفية تحديث Dynamics 365 Project Operations في بيئة Dynamics 365 Finance الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="ebff5-105">This topic provides information about how to update Dynamics 365 Project Operations in your Dynamics 365 Finance environment.</span></span> <span data-ttu-id="ebff5-106">هناك ثلاثة إجراءات مطلوبة لتحديث Project Operations إلى التحديث 5 (UR5):</span><span class="sxs-lookup"><span data-stu-id="ebff5-106">There are three procedures that are required to update Project Operations to Update 5 (UR5):</span></span>

- [<span data-ttu-id="ebff5-107">استيراد الحزمة إلى مشروع المعاينة الخاص بك</span><span class="sxs-lookup"><span data-stu-id="ebff5-107">Import the package into your preview project</span></span>](#import)
- [<span data-ttu-id="ebff5-108">تطبيق التحديث</span><span class="sxs-lookup"><span data-stu-id="ebff5-108">Apply the update</span></span>](#apply)
- [<span data-ttu-id="ebff5-109">تحديث بيئة Dataverse الخاصة بك</span><span class="sxs-lookup"><span data-stu-id="ebff5-109">Update your Dataverse environment</span></span>](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a><span data-ttu-id="ebff5-110">استيراد الحزمة إلى مشروع LCS الخاص بك</span><span class="sxs-lookup"><span data-stu-id="ebff5-110">Import the package into your LCS project</span></span>

1. <span data-ttu-id="ebff5-111">قم بتسجيل الدخول إلى [Lifecycle Services (LCS)](https://lcs.dynamics.com/) كمالك مشروع أو مدير بيئة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-111">Sign in to [Lifecycle Services (LCS)](https://lcs.dynamics.com/) as a Project Owner or Environment manager.</span></span>
2. <span data-ttu-id="ebff5-112">من قائمة المشروعات، حدد مشروع LCS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="ebff5-112">From the list of projects, select your LCS project.</span></span>
3. <span data-ttu-id="ebff5-113">في صفحة **المشروع**، في مجموعة **البيئات**، افتح البيئة التي ترغب في تحديثها.</span><span class="sxs-lookup"><span data-stu-id="ebff5-113">On the **Project** page, in the **Environments** group, open the environment that you want to update.</span></span>
4. <span data-ttu-id="ebff5-114">تحقق من تشغيل البيئة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-114">Verify that the environment is running.</span></span> <span data-ttu-id="ebff5-115">إذا لم يتم بدء تشغيل البيئة فابدأ تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="ebff5-115">If it isn't started, start the environment.</span></span>
5. <span data-ttu-id="ebff5-116">في قسم **الإصدار الجديد** أسفل **التحديثات المتوفرة**، قم بتحديد **عرض التحديث** لـ 10.0.15.</span><span class="sxs-lookup"><span data-stu-id="ebff5-116">In the **New release** section under **Available updates**, select **View update** for 10.0.15.</span></span>

![زر عرض التحديث](media/view-update.png)

6. <span data-ttu-id="ebff5-118">في صفحة **التحديثات الثنائية**، حدد **حفظ الحزمة**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-118">On the **Binary updates** page, select **Save package**.</span></span>
7. <span data-ttu-id="ebff5-119">في صفحة **المراجعة وحفظ التغييرات**، حدد **حفظ الحزمة**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-119">On the **Review and save updates** page, select **Save package**.</span></span>
8. <span data-ttu-id="ebff5-120">في جزء **حفظ الحزمة إلى مكتبة الأصول** الذي يتم فتحه، أدخل اسم الحزمة ثم حدد **حفظ الحزمة**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-120">On the **Save package to asset library** pane that opens, enter the package name and then select **Save package**.</span></span>
9. <span data-ttu-id="ebff5-121">وعند انتهاء LCS من حفظ الحزمة، يتم تمكين الزر **تم**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-121">When LCS has finished saving the package, the **Done** button is enabled.</span></span> <span data-ttu-id="ebff5-122">حدد **تم**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-122">Select **Done**.</span></span> <span data-ttu-id="ebff5-123">سيتحقق LCS من الحزمة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-123">LCS will verify the package.</span></span> <span data-ttu-id="ebff5-124">قد يستغرق التحقق دقائق قليلة أو حتى ساعة واحدة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-124">Verification can take a few minutes or up to one hour.</span></span>


## <a name="apply-the-package-update"></a><a name="apply"></a><span data-ttu-id="ebff5-125">تطبيق تحديث الحزمة</span><span class="sxs-lookup"><span data-stu-id="ebff5-125">Apply the package update</span></span>

1. <span data-ttu-id="ebff5-126">في LCS، من صفحة **تفاصيل البيئة**، قم بتحديد **الاحتفاظ** > **تطبيق التحديثات**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-126">In LCS, on the **Environment details** page, select **Maintain** > **Apply Updates**.</span></span>
2. <span data-ttu-id="ebff5-127">من القائمة، حدد الحزمة التي قمت بحفظها قبل ذلك، ثم حدد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-127">From the list, select the package that you saved earlier, and then select **Apply**.</span></span>
3. <span data-ttu-id="ebff5-128">حدد **نعم** لتأكيد أنك تريد نشر الحزمة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-128">Select **Yes** to confirm that you want to deploy the package.</span></span>

![مربع حوار تأكيد نشر الحزمة](media/confirm-package-deployment.png)

4. <span data-ttu-id="ebff5-130">حدد **نعم** لتأكيد أنك تريد تحديث التطبيق.</span><span class="sxs-lookup"><span data-stu-id="ebff5-130">Select **Yes** to confirm that you want to update the application.</span></span>

![مربع حوار تأكيد تحديث التطبيق](media/confirm-application-update.png)

<span data-ttu-id="ebff5-132">سيتم بدء النشر وتحديث التطبيق.</span><span class="sxs-lookup"><span data-stu-id="ebff5-132">The deployment and application update will start.</span></span> 

<span data-ttu-id="ebff5-133">في صفحة **تفاصيل البيئة**، في الزاوية العلوية اليسرى، سيتم تحديث حالة البيئة إلى **خدمة**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-133">On the **Environment details** page, in the top-right corner, the environment status will update to **Servicing**.</span></span> <span data-ttu-id="ebff5-134">خلال ساعتين تقريبًا، سيكتمل التحديث.</span><span class="sxs-lookup"><span data-stu-id="ebff5-134">In approximately two hours, the update will be complete.</span></span> <span data-ttu-id="ebff5-135">سيتم تحديث معلومات إصدار التطبيق إلى **Microsoft Dynamics 365 for Finance and Operations10.0.15)** وسيتم تحدث حالة البيئة إلى **تم نشره**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-135">The application release information will update to **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** and the environment status will update to **Deployed**.</span></span>


## <a name="update-your-dataverse-environment"></a><a name="update"></a><span data-ttu-id="ebff5-136">تحديث بيئة Dataverse الخاصة بك</span><span class="sxs-lookup"><span data-stu-id="ebff5-136">Update your Dataverse environment</span></span>

1. <span data-ttu-id="ebff5-137">سجل دخولك إلى [مركز إدارة Power Platform](https://admin.powerplatform.com/).</span><span class="sxs-lookup"><span data-stu-id="ebff5-137">Sign in to the [Power Platform admin center](https://admin.powerplatform.com/).</span></span>
2. <span data-ttu-id="ebff5-138">في القائمة، ابحث عن البيئة التي استخدمتها لتثبيت Project Operations وافتحها.</span><span class="sxs-lookup"><span data-stu-id="ebff5-138">In the list, find and open the environment that you used to install Project Operations.</span></span>
3. <span data-ttu-id="ebff5-139">في صفحة **البيئات**، قم بتحديد **الموارد** > **تطبيقات Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-139">On the **Environments** page, select **Resource** > **Dynamics 365 apps**.</span></span>
4. <span data-ttu-id="ebff5-140">في القائمة، حدد موقع **Microsoft Dynamics 365 Project Operations**، وفي عمود **الحالة**، قم بتحديد **التحديث المتاح**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-140">In the list, locate **Microsoft Dynamics 365 Project Operations**, and in the **Status** column, select **Update Available**.</span></span>
5. <span data-ttu-id="ebff5-141">حدد خانة الاختيار **أوافق على شروط الخدمة**، ثم حدد **تحديث**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-141">Select the **I agree to the terms of service** check box, and then select **Update**.</span></span> <span data-ttu-id="ebff5-142">سيتم تثبيت أحدث إصدار من الحل.</span><span class="sxs-lookup"><span data-stu-id="ebff5-142">The latest version of the solution will be installed.</span></span>

<span data-ttu-id="ebff5-143">بعد اكتمال التثبيت، سيكون لديك الإصدار 4.5.0.134 مثبتًا.</span><span class="sxs-lookup"><span data-stu-id="ebff5-143">After the installation is complete, you'll have version 4.5.0.134 installed.</span></span>

## <a name="configure-new-features"></a><span data-ttu-id="ebff5-144">تكوين الميزات الجديدة</span><span class="sxs-lookup"><span data-stu-id="ebff5-144">Configure new features</span></span>

### <a name="enable-dual-write-mapping"></a><span data-ttu-id="ebff5-145">تمكين تعيين الكتابة المزدوجة</span><span class="sxs-lookup"><span data-stu-id="ebff5-145">Enable dual-write mapping</span></span>

<span data-ttu-id="ebff5-146">بعد الانتهاء من التحديث الخاص ببيئات Finance وDataverse يمكنك تمكين تعيينات الكتابة المزدوجة المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-146">After you complete the update on the Finance and Dataverse environments, you can enable the required dual-write mappings.</span></span> <span data-ttu-id="ebff5-147">استكمل الإجراءات التالية لتمكين تعيينات الكتابة المزدوجة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-147">Complete the following procedures to enable dual-write mappings.</span></span>

- [<span data-ttu-id="ebff5-148">تحديث إعدادات الأمان في بيئة Customer Engagement</span><span class="sxs-lookup"><span data-stu-id="ebff5-148">Update security settings on Customer Engagement environment</span></span>](#security)
- [<span data-ttu-id="ebff5-149">تحديث كيانات البيانات</span><span class="sxs-lookup"><span data-stu-id="ebff5-149">Refresh data entities</span></span>](#refresh)
- [<span data-ttu-id="ebff5-150">تحديث وتشغيل تعيينات الكتابة المزدوجة</span><span class="sxs-lookup"><span data-stu-id="ebff5-150">Update and run the dual-write mappings</span></span>](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a><span data-ttu-id="ebff5-151">تحديث إعدادات الأمان في بيئة Dataverse</span><span class="sxs-lookup"><span data-stu-id="ebff5-151">Update security settings on the Dataverse environment</span></span>

<span data-ttu-id="ebff5-152">التحديثات التالية لامتيازات الأمان الخاصة بالكيانات مطلوبة كجزء من التحديث إلى UR5.</span><span class="sxs-lookup"><span data-stu-id="ebff5-152">The following updates to the security privileges for entities are required as part of the update to UR5.</span></span>

1. <span data-ttu-id="ebff5-153">في بيئة Dataverse الخاصة بك، انتقل إلى **الإعدادات**، وفي مجموعة **النظام**، حدد **الأمان**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-153">In your Dataverse environment, go to **Settings**, and in the **System** group, select **Security**.</span></span>

![إعدادات بيئة Dataverse](media/Picture21.png)

2. <span data-ttu-id="ebff5-155">حدد **أدوار الأمان**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-155">Select **Security Roles**.</span></span>
3. <span data-ttu-id="ebff5-156">من قائمة الأدوار، حدد **مستخدم تطبيق الكتابة المزدوجة** وحدد علامة التبويب **الكيانات المخصصة**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-156">From the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span> 
4. <span data-ttu-id="ebff5-157">تحقق من أن الدور يحتوي على أذونات **قراءة** و **إلحاق بـ** لـ:</span><span class="sxs-lookup"><span data-stu-id="ebff5-157">Verify that the role has **Read** and **Append To** permissions for:</span></span>

      - <span data-ttu-id="ebff5-158">**نوع سعر الصرف للعملة**</span><span class="sxs-lookup"><span data-stu-id="ebff5-158">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="ebff5-159">**مخطط الحسابات**</span><span class="sxs-lookup"><span data-stu-id="ebff5-159">**Chart Of Accounts**</span></span> 
      - <span data-ttu-id="ebff5-160">**التقويم المالي**</span><span class="sxs-lookup"><span data-stu-id="ebff5-160">**Fiscal Calendar**</span></span> 
      - <span data-ttu-id="ebff5-161">**دفتر الأستاذ**</span><span class="sxs-lookup"><span data-stu-id="ebff5-161">**Ledger**</span></span>

5. <span data-ttu-id="ebff5-162">بعد تحديث دور الأمان، انتقل إلى **الإعدادات** > **الأمان** > **الفرق**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-162">After the security role is updated, go to **Settings** > **Security** > **Teams**.</span></span> <span data-ttu-id="ebff5-163">تحقق من أنه قد تم تطبيق دور **مستخدم تطبيق الكتابة المزدوجة** على الفريق.</span><span class="sxs-lookup"><span data-stu-id="ebff5-163">Verify that the **dual-write app user** role has been applied to the team.</span></span> 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a><span data-ttu-id="ebff5-164">تحديث كيانات البيانات من التحديث</span><span class="sxs-lookup"><span data-stu-id="ebff5-164">Refresh data entities from the update</span></span>

1. <span data-ttu-id="ebff5-165">في بيئة Finance، افتح مساحة عمل **إدارة البيانات**، ثم افتح صفحة **معلمات إطار العمل**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-165">In your Finance environment, open the **Data management** workspace, and then open the **Framework parameters** page.</span></span>
2. <span data-ttu-id="ebff5-166">في علامة تبويب **إعدادات الكيان**، قم بتحديد **تحديث قائمة الكيان**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-166">On the **Entity settings** tab, select **Refresh entity list**.</span></span>
3. <span data-ttu-id="ebff5-167">حدد **إغلاق** لتأكيد تحديث الكيان.</span><span class="sxs-lookup"><span data-stu-id="ebff5-167">Select **Close** to confirm the entity refresh.</span></span>

 > [!NOTE]
 > <span data-ttu-id="ebff5-168">يستغرق اكتمال هذه العملية حوالي 20 دقيقة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-168">This process will take approximately 20 minutes to complete.</span></span> <span data-ttu-id="ebff5-169">سيتم إعلامك عند اكتمال التحديث.</span><span class="sxs-lookup"><span data-stu-id="ebff5-169">You will be notified when the refresh is complete.</span></span>

### <a name="update-dual-write-mappings"></a><a name="run"></a><span data-ttu-id="ebff5-170">تحديث تعيينات الكتابة المزدوجة</span><span class="sxs-lookup"><span data-stu-id="ebff5-170">Update dual-write mappings</span></span>

1. <span data-ttu-id="ebff5-171">في مساحة عمل **إدارة البيانات**، قم بتحديد **الكتابة المزدوجة**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-171">In the **Data management** workspace, select **Dual-write**.</span></span>
2. <span data-ttu-id="ebff5-172">حدد **تطبيق الحلول**، وحدد كلا الحلين في القائمة، ثم حدد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-172">Select **Apply solutions**, select both solutions in the list, and then select **Apply**.</span></span>
3. <span data-ttu-id="ebff5-173">في صفحة **الكتابة المزدوجة**، قم بتحديد خرائط الجدول التالية، ثم قم بتحديد **إيقاف**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-173">On the **Dual-write** page, select the following table maps, and then select **Stop**.</span></span>

    - <span data-ttu-id="ebff5-174">**القيم الفعلية لتكامل Project Operations (msdyn_actuals)**</span><span class="sxs-lookup"><span data-stu-id="ebff5-174">**Project Operations integration actuals (msdyn_actuals)**</span></span>
    - <span data-ttu-id="ebff5-175">**فئات مصروفات مشروع تكامل Project Operations (msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="ebff5-175">**Project Operations integration project expense categories (msdyn_expensecategories)**</span></span>
    - <span data-ttu-id="ebff5-176">**كيان تصدير مصروفات مشروع القيم الفعلية لتكامل Project Operations (msdyn_expenses)**</span><span class="sxs-lookup"><span data-stu-id="ebff5-176">**Project Operations integration actuals project expenses export entity (msdyn_expenses)**</span></span>

4. <span data-ttu-id="ebff5-177">في صفحة **إصدار خريطة الجدول**، قم بتطبيق إصدار جديد من الخريطة على كل كيان من الكيانات الثلاثة.</span><span class="sxs-lookup"><span data-stu-id="ebff5-177">On the **Table map version** page, apply a new version of the map to each of the three entities.</span></span>
5. <span data-ttu-id="ebff5-178">في صفحة **الكتابة المزدوجة**، حدد تشغيل لإعادة تشغيل الخرائط.</span><span class="sxs-lookup"><span data-stu-id="ebff5-178">On the **Dual-write** page, select run to restart the maps.</span></span>
6. <span data-ttu-id="ebff5-179">من قائمة الخرائط، حدد خريطة **دفتر الأستاذ (msdyn_ledgers)** مع كافة المتطلبات وحدد خانة الاختيار **المزامنة الأولية**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-179">From the list of maps, select the **Ledger (msdyn_ledgers)** map with all prerequisites and select the **Initial sync** check box.</span></span> 
7. <span data-ttu-id="ebff5-180">في حقل **أصل المزامنة الأولية‬**، قم بتحديد **تطبيقات Finance and Operations** ثم قم بتحديد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="ebff5-180">In the **Master for initial sync** field, select **Finance and Operations apps** and then select **Run**.</span></span>
 
 ![مزامنة خريطة دفتر الأستاذ](media/DW6.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]