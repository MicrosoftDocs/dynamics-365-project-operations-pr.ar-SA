---
title: تزويد بيئة جديدة
description: يوفر هذا الموضوع معلومات حول كيفية تزويد بيئة Project Operations جديدة.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 044a942a068b33318b98041cc94944d90c1d63c3
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121157"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="20a8c-103">تزويد بيئة جديدة</span><span class="sxs-lookup"><span data-stu-id="20a8c-103">Provision a new environment</span></span>

<span data-ttu-id="20a8c-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="20a8c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="20a8c-105">يوفر هذا الموضوع معلومات حول كيفية تزويد بيئة Dynamics 365 Project Operations جديدة للسيناريوهات المستندة إلى المورد/المنتجات غير المخزنة.</span><span class="sxs-lookup"><span data-stu-id="20a8c-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="20a8c-106">تمكين التزويد التلقائي Project Operations في مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="20a8c-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="20a8c-107">استخدم الخطوات التالية لتمكين سير عمل التزويد التلقائي لـ Project Operations لمشروع LCS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="20a8c-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="20a8c-108">انتقل إلى [LCS](https://lcs.dynamics.com/v2) وحدد تجانب **إدارة ميزة المعاينة**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="20a8c-109">في قائمة **ميزة المعاينة**، حدد **ميزة Project Operations** ثم حدد **تمكين ميزة المعاينة** لتمكين Project Operations.</span><span class="sxs-lookup"><span data-stu-id="20a8c-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="20a8c-110">يتم تنفيذ هذه الخطوة مرة واحدة فقط لكل مشروع LCS.</span><span class="sxs-lookup"><span data-stu-id="20a8c-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="20a8c-111">تزويد بيئة Project Operations</span><span class="sxs-lookup"><span data-stu-id="20a8c-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="20a8c-112">افتح Dynamics 365 Finance جديد [في بيئة عرض توضيحي](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) أو نشر [بيئة الحماية / الإنتاج](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="20a8c-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="20a8c-113">اتبع خطوات معالج **تزويد البيئة**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="20a8c-114">تأكد من أن إصدار التطبيق المحدد 10.0.13 أو أحدث.</span><span class="sxs-lookup"><span data-stu-id="20a8c-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="20a8c-115">لتزويد Project Operations، ضمن **إعدادات متقدمة**، حدد **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="20a8c-116">قم بتمكين **إعداد Common Data Service** من خلال اختيار **نعم** ثم أدخل المعلومات في الحقول المطلوبة:</span><span class="sxs-lookup"><span data-stu-id="20a8c-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="20a8c-117">اسم</span><span class="sxs-lookup"><span data-stu-id="20a8c-117">Name</span></span>
  - <span data-ttu-id="20a8c-118">المنطقة</span><span class="sxs-lookup"><span data-stu-id="20a8c-118">Region</span></span>
  - <span data-ttu-id="20a8c-119">اللغة‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-119">Language</span></span>
  - <span data-ttu-id="20a8c-120">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="20a8c-120">Currency</span></span>
 
5. <span data-ttu-id="20a8c-121">في حقل **قالب Common Data Service**، حدد **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="20a8c-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="20a8c-122">حدد نوع البيئة لعملية التوزيع الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="20a8c-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="20a8c-123">سيتيح لك الإصدار التجريبي الذي يستند إلى الاشتراك نشر بيئة CDS لمدة 30 يومًا.</span><span class="sxs-lookup"><span data-stu-id="20a8c-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![إعدادات النشر](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="20a8c-125">حدد **موافقة** للإقرار بشروط الخدمة ثم حدد **تم** للرجوع إلى إعدادات التوزيع.</span><span class="sxs-lookup"><span data-stu-id="20a8c-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![الموافقة على التوزيع](./media/2DeploymentConsent.png)

7. <span data-ttu-id="20a8c-127">أكمل الحقول المطلوبة المتبقية في المعالج وقم بتأكيد التوزيع.</span><span class="sxs-lookup"><span data-stu-id="20a8c-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="20a8c-128">يختلف وقت تزويد البيئة على حسب نوع البيئة.</span><span class="sxs-lookup"><span data-stu-id="20a8c-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="20a8c-129">قد تستغرق عملية التزويد ست ساعات.</span><span class="sxs-lookup"><span data-stu-id="20a8c-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="20a8c-130">بعد اكتمال التوزيع بنجاح، سيتم عرض البيئة بالحالة **تم نشرها**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="20a8c-131">للتأكد من أنه تم نشر البيئة بنجاح، حدد **تسجيل الدخول** وقم بتسجيل الدخول إلى البيئة للتأكيد.</span><span class="sxs-lookup"><span data-stu-id="20a8c-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![تفاصيل بيئة ](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="20a8c-133">تطبيق بيانات العرض التوضيحي لـ Finance في Project Operations (خطوة اختيارية)</span><span class="sxs-lookup"><span data-stu-id="20a8c-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="20a8c-134">طبق بيانات العرض التوضيحي لـ Finance في Project Operations على الإصدار 10.0.13 من البيئة المستضافة على السحابة كما هو موضح في [هذه المقالة](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="20a8c-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="20a8c-135">تطبيق التحديثات على بيئة Finance</span><span class="sxs-lookup"><span data-stu-id="20a8c-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="20a8c-136">تتطلب Project Operations بيئة Finance بإصدار تطبيق رقم **10.0.13 (10.0.569.20009)** أو الأعلى.</span><span class="sxs-lookup"><span data-stu-id="20a8c-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="20a8c-137">قد تحتاج إلى تطبيق تحديثات الجودة على بيئة Finance لديك لاستلام هذا الإصدار.</span><span class="sxs-lookup"><span data-stu-id="20a8c-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="20a8c-138">في LCS، في صفحة **تفاصيل البيئة**، في قسم **التحديثات المتوفرة**، حدد **عرض التحديث**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![عرض التحديثات](./media/5ViewUpdates.png)

2. <span data-ttu-id="20a8c-140">في صفحة **التحديثات الثنائية**، حدد **حفظ الحزمة.**</span><span class="sxs-lookup"><span data-stu-id="20a8c-140">On the **Binary updates** page, select **Save package.**</span></span>

![حفظ الحزمة](./media/6SavePackage.png)

3. <span data-ttu-id="20a8c-142">انقر فوق **تحديد الكل** ثم حدد **حفظ الحزمة**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-142">Click **Select all** and then select **Save package**.</span></span>

![مراجعة التحديثات وحفظها](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="20a8c-144">أدخل اسمًا ووصفًا للحزمة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="20a8c-145">تبعًا لاتصال الإنترنت، قد تستغرق هذه العملية بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="20a8c-145">Depending on the internet connection, this process might take some time.</span></span>

![تحميل الحزمة إلى مكتبة الأصول](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="20a8c-147">بعد حفظ الحزمة، حدد **تم** وقم بحفظ هذه الحزمة في مكتبة الأصول في مشروع LCS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="20a8c-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="20a8c-148">قد يستغرق حفظ الحزمة والتحقق من صحتها ~ 15 دقيقة.</span><span class="sxs-lookup"><span data-stu-id="20a8c-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="20a8c-149">لتطبيق التحديث، انتقل إلى صفحة **تفاصيل البيئة** في LCS وحدد **الصيانة** > **تطبيق التحديثات**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![صيانة البيئات](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="20a8c-151">في قائمة التحديثات، قم بتحديد الحزمة التي قمت بإنشائها، وقم بتحديد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-151">In the updates list select the package you created, and select **Apply**.</span></span>

![تطبيق التحديثات](./media/10ApplyUpdates.png)

<span data-ttu-id="20a8c-153">ستستغرق عملية "صيانة البيئة" بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="20a8c-153">Environment servicing will take some time.</span></span> <span data-ttu-id="20a8c-154">بعد انتهائها، ستعود البيئة إلى حالة تم نشرها.</span><span class="sxs-lookup"><span data-stu-id="20a8c-154">After it is complete, the environment will return to a deployed state.</span></span>

![البيئة المنشورة](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="20a8c-156">إنشاء اتصال كتابة مزدوج</span><span class="sxs-lookup"><span data-stu-id="20a8c-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="20a8c-157">في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="20a8c-158">تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="20a8c-159">بعد اكتمال الارتباط، حدد **ربط بـ CDS للتطبيقات‏‎** مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="20a8c-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="20a8c-160">ستتم إعادة توجيهك إلى الكتابة المزدوجة في Finance.</span><span class="sxs-lookup"><span data-stu-id="20a8c-160">You will be redirected to Dual Write in Finance.</span></span>

![ربط بـ CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="20a8c-162">حدد **تطبيق الحل** للوصول إلى الكيانات التي سيتم تعيينها في التكامل.</span><span class="sxs-lookup"><span data-stu-id="20a8c-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![تطبيق الحلول](./media/13ApplySolutions.png)

5. <span data-ttu-id="20a8c-164">حدد كلا الحلين، **Dynamics 365 Finance and Operations خريطة كيان الكتابة المزدوجة** و **خرائط كيان الكتابة المزدوجة في Dynamics 365 Project Operations**، ثم حدد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![تأكيد الحلول](./media/14ConfirmSolutions.png)

<span data-ttu-id="20a8c-166">بعد تطبيق الحلول، يتم تطبيق كيانات الكتابة المزدوجة على البيئة.</span><span class="sxs-lookup"><span data-stu-id="20a8c-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![تطبيق الحلول](./media/15ApplyingSolutions.png)

<span data-ttu-id="20a8c-168">بعد تطبيق الكيانات، يتم سرد كافة التعيينات المتوفرة في البيئة.</span><span class="sxs-lookup"><span data-stu-id="20a8c-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![خرائط الكتابة المزدوجة](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="20a8c-170">تحديث كيانات البيانات بعد التحديث</span><span class="sxs-lookup"><span data-stu-id="20a8c-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="20a8c-171">في Finance، انتقل إلى مساحة عمل **إدارة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-171">In Finance, go to the **Data management** workspace.</span></span>

![مساحة عمل إدارة البيانات](./media/16DataManagement.png)

2. <span data-ttu-id="20a8c-173">حدد تجانب **معلمات إطار العمل**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-173">Select the **Framework parameters** tile.</span></span>

![معلمات إطار العمل](./media/17FrameworkParameters.png)

3. <span data-ttu-id="20a8c-175">في صفحة **إعدادات الكيان**، حدد **تحديث قائمة الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![تحديث قائمة الكيانات](./media/18RefreshEntityList.png)

<span data-ttu-id="20a8c-177">سيستغرق التحديث مدة 20 دقيقة تقريبًا.</span><span class="sxs-lookup"><span data-stu-id="20a8c-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="20a8c-178">وستتلقى تحذيرًا عند اكتماله.</span><span class="sxs-lookup"><span data-stu-id="20a8c-178">You will receive an alert when it is complete.</span></span>

![تأكيد التحديث](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="20a8c-180">تشغيل خرائط ‏‫الكتابة المزدوجة في Project Operations</span><span class="sxs-lookup"><span data-stu-id="20a8c-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="20a8c-181">في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="20a8c-182">تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات.**</span><span class="sxs-lookup"><span data-stu-id="20a8c-182">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="20a8c-183">بعد تحديد الارتباط، ستتم إعادة توجيهك إلى قائمة الكيانات الموجودة في التعيينات.</span><span class="sxs-lookup"><span data-stu-id="20a8c-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="20a8c-184">ابدأ الخرائط كما هو موضح في الجدول التالي.</span><span class="sxs-lookup"><span data-stu-id="20a8c-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="20a8c-185">تأكد من اتباع التسلسل كما هو موضح.</span><span class="sxs-lookup"><span data-stu-id="20a8c-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="20a8c-186">**تعيين الكيان**</span><span class="sxs-lookup"><span data-stu-id="20a8c-186">**Entity Map**</span></span> | <span data-ttu-id="20a8c-187">**تحديث الكيان**</span><span class="sxs-lookup"><span data-stu-id="20a8c-187">**Refresh entity**</span></span> | <span data-ttu-id="20a8c-188">**المزامنة الأولية**</span><span class="sxs-lookup"><span data-stu-id="20a8c-188">**Initial sync**</span></span> | <span data-ttu-id="20a8c-189">**أصل المزامنة الأولية**</span><span class="sxs-lookup"><span data-stu-id="20a8c-189">**Master for initial sync**</span></span> | <span data-ttu-id="20a8c-190">**تشغيل المتطلبات الأساسية**</span><span class="sxs-lookup"><span data-stu-id="20a8c-190">**Run prerequisites**</span></span> | <span data-ttu-id="20a8c-191">**المزامنة الأولية للمتطلبات الأساسية**</span><span class="sxs-lookup"><span data-stu-id="20a8c-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="20a8c-192">**أدوار موارد المشروع لجميع الشركات (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="20a8c-193">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-193">No</span></span> | <span data-ttu-id="20a8c-194">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="20a8c-194">Yes</span></span> | <span data-ttu-id="20a8c-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="20a8c-195">Common Data Service</span></span> | <span data-ttu-id="20a8c-196">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-196">No</span></span> | <span data-ttu-id="20a8c-197">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-197">N\A</span></span> |
| <span data-ttu-id="20a8c-198">**الكيانات القانونية (cdm\_الشركات)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="20a8c-199">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-199">No</span></span> | <span data-ttu-id="20a8c-200">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="20a8c-200">Yes</span></span> | <span data-ttu-id="20a8c-201">تطبيقات Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="20a8c-201">Finance and Operations apps</span></span> | <span data-ttu-id="20a8c-202">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-202">No</span></span> | <span data-ttu-id="20a8c-203">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-203">N\A</span></span> |
| <span data-ttu-id="20a8c-204">**القيم الفعلية لتكامل Project Operations(msdyn\_القيم الفعلية)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="20a8c-205">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-205">No</span></span> | <span data-ttu-id="20a8c-206">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-206">No</span></span> | <span data-ttu-id="20a8c-207">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-207">N\A</span></span> | <span data-ttu-id="20a8c-208">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="20a8c-208">Yes</span></span> | <span data-ttu-id="20a8c-209">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-209">No</span></span> |
| <span data-ttu-id="20a8c-210">**بنود عقد المشروع (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="20a8c-211">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-211">No</span></span> | <span data-ttu-id="20a8c-212">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-212">No</span></span> | <span data-ttu-id="20a8c-213">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-213">N\A</span></span> | <span data-ttu-id="20a8c-214">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-214">No</span></span> | <span data-ttu-id="20a8c-215">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-215">No</span></span> |
| <span data-ttu-id="20a8c-216">**كيان التكامل لعلاقات معاملات المشروع (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="20a8c-217">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-217">No</span></span> | <span data-ttu-id="20a8c-218">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-218">No</span></span> | <span data-ttu-id="20a8c-219">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-219">N\A</span></span> | <span data-ttu-id="20a8c-220">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-220">No</span></span> | <span data-ttu-id="20a8c-221">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-221">N\A</span></span> |
| <span data-ttu-id="20a8c-222">**المراحل الرئيسية لبنود تعاقد التكامل مع Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="20a8c-223">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-223">No</span></span> | <span data-ttu-id="20a8c-224">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-224">No</span></span> | <span data-ttu-id="20a8c-225">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-225">N\A</span></span> | <span data-ttu-id="20a8c-226">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-226">No</span></span> | <span data-ttu-id="20a8c-227">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-227">N\A</span></span> |
| <span data-ttu-id="20a8c-228">**كيان تكامل Project Operations لتقديرات المصروفات (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="20a8c-229">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-229">No</span></span> | <span data-ttu-id="20a8c-230">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-230">No</span></span> | <span data-ttu-id="20a8c-231">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-231">N\A</span></span> | <span data-ttu-id="20a8c-232">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-232">No</span></span> | <span data-ttu-id="20a8c-233">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-233">N\A</span></span> |
| <span data-ttu-id="20a8c-234">**كيان تصدير فئات مصروفات مشروع لتكامل Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-234">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="20a8c-235">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-235">No</span></span> | <span data-ttu-id="20a8c-236">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-236">No</span></span> | <span data-ttu-id="20a8c-237">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-237">N\A</span></span> | <span data-ttu-id="20a8c-238">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-238">No</span></span> | <span data-ttu-id="20a8c-239">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-239">N\A</span></span> |
| <span data-ttu-id="20a8c-240">**كيان تصدير مصروفات مشروع لتكامل Project Operations (msdyn\_مصروفات)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="20a8c-241">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="20a8c-241">Yes</span></span> | <span data-ttu-id="20a8c-242">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-242">No</span></span> | <span data-ttu-id="20a8c-243">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-243">N\A</span></span> | <span data-ttu-id="20a8c-244">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-244">No</span></span> | <span data-ttu-id="20a8c-245">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-245">N\A</span></span> |
| <span data-ttu-id="20a8c-246">**كيان تكامل Project Operations لتقديرات الساعات (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="20a8c-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="20a8c-247">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="20a8c-247">Yes</span></span> | <span data-ttu-id="20a8c-248">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-248">No</span></span> | <span data-ttu-id="20a8c-249">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-249">N\A</span></span> | <span data-ttu-id="20a8c-250">Yes</span><span class="sxs-lookup"><span data-stu-id="20a8c-250">No</span></span> | <span data-ttu-id="20a8c-251">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="20a8c-251">N\A</span></span> |


4. <span data-ttu-id="20a8c-252">لتحديث الكيان، حدد اسم الخريطة، ثم حدد **تحديث الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![تحديث الخريطة‬](./media/20RefreshMapping.png)

5. <span data-ttu-id="20a8c-254">شغّل الخريطة بعد اكتمال التحديث.</span><span class="sxs-lookup"><span data-stu-id="20a8c-254">After the refresh is complete, run the map.</span></span> <span data-ttu-id="20a8c-255">قبل تمكين الخريطة التالية، تحقق من أن الخريطة الموجودة في الجدول بالحالة **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="20a8c-256">قد يستغرق تشغيل الخرائط بعدد كبير من المتطلبات المسبقة بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="20a8c-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="20a8c-257">لتشغيل خريطة بالمتطلبات المسبقة، قم بتمكين تبديل **إظهار خرائط الكيانات المرتبطة**.</span><span class="sxs-lookup"><span data-stu-id="20a8c-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="20a8c-258">إذا كان الجدول يشير إلى أن **المزامنة الأولية للمتطلبات الأساسية** بالقيمة **لا**، فتحقق من أن علامة **المزامنة الأولية** قيد **الإيقاف** في كافة خرائط المتطلبات الأساسية قبل تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="20a8c-258">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![تشغيل الخريطة](./media/21RunMap.png)

6. <span data-ttu-id="20a8c-260">تحقق من صحة كافة الخرائط ذات الصلة بالمشروع وأنها بالحالة تشغيل.</span><span class="sxs-lookup"><span data-stu-id="20a8c-260">Validate all project related maps are in the running state.</span></span>

![كل الخرائط قيد التشغيل](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="20a8c-262">تطبيق بيانات التكوين في CDS لـ Project Operations (اختياري)</span><span class="sxs-lookup"><span data-stu-id="20a8c-262">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="20a8c-263">إذا كنت قد قمت بتطبيق بيانات العرض التوضيحي على بيئة Finance، فراجع [إعداد بيانات التكوين وتطبيقها في Common Data Service لـ Project Operations](resource-apply-pro-setup-config-data.md) لتطبيق بيانات العرض التوضيحي على بيئة CDS.</span><span class="sxs-lookup"><span data-stu-id="20a8c-263">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="20a8c-264">تم الآن تزويد بيئة Project Operations وتكوينها.</span><span class="sxs-lookup"><span data-stu-id="20a8c-264">Your Project Operations environment is now provisioned and configured.</span></span> 
