---
title: تزويد بيئة جديدة
description: يوفر هذا الموضوع معلومات حول كيفية تزويد بيئة Project Operations جديدة.
author: sigitac
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 45700371c50e3b5a840df45fc24fa8a5b4584b61
ms.sourcegitcommit: 87b7a8d793c19c50f3765b8d788cde24a6a0ca24
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949346"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="ac9fc-103">تزويد بيئة جديدة</span><span class="sxs-lookup"><span data-stu-id="ac9fc-103">Provision a new environment</span></span>

<span data-ttu-id="ac9fc-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="ac9fc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ac9fc-105">يوفر هذا الموضوع معلومات حول كيفية تزويد بيئة Dynamics 365 Project Operations جديدة للسيناريوهات المستندة إلى المورد/المنتجات غير المخزنة.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="ac9fc-106">تمكين التزويد التلقائي Project Operations في مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="ac9fc-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="ac9fc-107">استخدم الخطوات التالية لتمكين سير عمل التزويد التلقائي لـ Project Operations لمشروع LCS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="ac9fc-108">انتقل إلى [LCS](https://lcs.dynamics.com/v2) وحدد تجانب **إدارة ميزة المعاينة**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="ac9fc-109">في قائمة **ميزة المعاينة**، قم بتحديد **Project Operations** وحدد **تمكين ميزة المعاينة** لتمكين Project Operations.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-109">In the **Preview feature** list, select **Project Operations** and the select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="ac9fc-110">يتم تنفيذ هذه الخطوة مرة واحدة فقط لكل مشروع LCS.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="ac9fc-111">تزويد بيئة Project Operations</span><span class="sxs-lookup"><span data-stu-id="ac9fc-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="ac9fc-112">افتح Dynamics 365 Finance جديد [في بيئة عرض توضيحي](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) أو نشر [بيئة الحماية / الإنتاج](https://docs.microsoft.com/edynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="ac9fc-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/edynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="ac9fc-113">اتبع خطوات معالج **تزويد البيئة**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="ac9fc-114">تأكد من أن إصدار التطبيق المحدد 10.0.13 أو أحدث.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="ac9fc-115">لتزويد Project Operations، ضمن **إعدادات متقدمة**، حدد **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="ac9fc-116">قم بتمكين **إعداد Common Data Service** من خلال اختيار **نعم** ثم أدخل المعلومات في الحقول المطلوبة:</span><span class="sxs-lookup"><span data-stu-id="ac9fc-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="ac9fc-117">اسم</span><span class="sxs-lookup"><span data-stu-id="ac9fc-117">Name</span></span>
  - <span data-ttu-id="ac9fc-118">المنطقة</span><span class="sxs-lookup"><span data-stu-id="ac9fc-118">Region</span></span>
  - <span data-ttu-id="ac9fc-119">اللغة‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-119">Language</span></span>
  - <span data-ttu-id="ac9fc-120">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="ac9fc-120">Currency</span></span>
 
5. <span data-ttu-id="ac9fc-121">في حقل **قالب Common Data Service**، حدد **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="ac9fc-122">حدد نوع البيئة لعملية التوزيع الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="ac9fc-123">سيتيح لك الإصدار التجريبي الذي يستند إلى الاشتراك نشر بيئة CDS لمدة 30 يومًا.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![إعدادات النشر](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="ac9fc-125">حدد **موافقة** للإقرار بشروط الخدمة ثم حدد **تم** للرجوع إلى إعدادات التوزيع.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![الموافقة على التوزيع](./media/2DeploymentConsent.png)

7. <span data-ttu-id="ac9fc-127">أكمل الحقول المطلوبة المتبقية في المعالج وقم بتأكيد التوزيع.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="ac9fc-128">يختلف وقت تزويد البيئة على حسب نوع البيئة.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="ac9fc-129">قد تستغرق عملية التزويد ست ساعات.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="ac9fc-130">بعد اكتمال التوزيع بنجاح، سيتم عرض البيئة بالحالة **تم نشرها**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="ac9fc-131">للتأكد من أنه تم نشر البيئة بنجاح، حدد **تسجيل الدخول** وقم بتسجيل الدخول إلى البيئة للتأكيد.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![تفاصيل بيئة ](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="ac9fc-133">تطبيق بيانات العرض التوضيحي لـ Finance في Project Operations (خطوة اختيارية)</span><span class="sxs-lookup"><span data-stu-id="ac9fc-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="ac9fc-134">طبق بيانات العرض التوضيحي لـ Finance في Project Operations على الإصدار 10.0.13 من البيئة المستضافة على السحابة كما هو موضح في [هذه المقالة](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="ac9fc-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="ac9fc-135">تطبيق التحديثات على بيئة Finance</span><span class="sxs-lookup"><span data-stu-id="ac9fc-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="ac9fc-136">تتطلب Project Operations بيئة Finance بإصدار تطبيق رقم**10.0.13 (10.0.569.20009)** أو الأعلى.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="ac9fc-137">قد تحتاج إلى تطبيق تحديثات الجودة على بيئة Finance لديك لاستلام هذا الإصدار.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="ac9fc-138">في LCS، في صفحة **تفاصيل البيئة**، في قسم **التحديثات المتوفرة**، حدد **عرض التحديث**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![عرض التحديثات](./media/5ViewUpdates.png)

2. <span data-ttu-id="ac9fc-140">في صفحة **التحديثات الثنائية**، حدد **حفظ الحزمة.**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-140">On the **Binary updates** page, select **Save package.**</span></span>

![حفظ الحزمة](./media/6SavePackage.png)

3. <span data-ttu-id="ac9fc-142">انقر فوق **تحديد الكل** ثم حدد **حفظ الحزمة**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-142">Click **Select all** and then select **Save package**.</span></span>

![مراجعة التحديثات وحفظها](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="ac9fc-144">أدخل اسمًا ووصفًا للحزمة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="ac9fc-145">تبعًا لاتصال الإنترنت، قد تستغرق هذه العملية بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-145">Depending on the internet connection, this process might take some time.</span></span>

![تحميل الحزمة إلى مكتبة الأصول](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="ac9fc-147">بعد حفظ الحزمة، حدد **تم** وقم بحفظ هذه الحزمة في مكتبة الأصول في مشروع LCS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="ac9fc-148">قد يستغرق حفظ الحزمة والتحقق من صحتها ~ 15 دقيقة.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="ac9fc-149">لتطبيق التحديث، انتقل إلى صفحة **تفاصيل البيئة** في LCS وحدد **الصيانة** > **تطبيق التحديثات**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![صيانة البيئات](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="ac9fc-151">في قائمة التحديثات، قم بتحديد الحزمة التي قمت بإنشائها، وقم بتحديد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-151">In the updates list select the package you created, and select **Apply**.</span></span>

![تطبيق التحديثات](./media/10ApplyUpdates.png)

<span data-ttu-id="ac9fc-153">ستستغرق عملية "صيانة البيئة" بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-153">Environment servicing will take some time.</span></span> <span data-ttu-id="ac9fc-154">بعد انتهائها، ستعود البيئة إلى حالة تم نشرها.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-154">After it is complete, the environment will return to a deployed state.</span></span>

![البيئة المنشورة](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="ac9fc-156">إنشاء اتصال كتابة مزدوج</span><span class="sxs-lookup"><span data-stu-id="ac9fc-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="ac9fc-157">في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="ac9fc-158">تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="ac9fc-159">بعد اكتمال الارتباط، حدد **ربط بـ CDS للتطبيقات‏‎** مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="ac9fc-160">ستتم إعادة توجيهك إلى الكتابة المزدوجة في Finance.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-160">You will be redirected to Dual Write in Finance.</span></span>

![ربط بـ CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="ac9fc-162">حدد **تطبيق الحل** للوصول إلى الكيانات التي سيتم تعيينها في التكامل.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![تطبيق الحلول](./media/13ApplySolutions.png)

5. <span data-ttu-id="ac9fc-164">حدد كلا الحلين، **Dynamics 365 Finance and Operations خريطة كيان الكتابة المزدوجة** و**خرائط كيان الكتابة المزدوجة في Dynamics 365 Project Operations**، ثم حدد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![تأكيد الحلول](./media/14ConfirmSolutions.png)

<span data-ttu-id="ac9fc-166">بعد تطبيق الحلول، يتم تطبيق كيانات الكتابة المزدوجة على البيئة.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![تطبيق الحلول](./media/15ApplyingSolutions.png)

<span data-ttu-id="ac9fc-168">بعد تطبيق الكيانات، يتم سرد كافة التعيينات المتوفرة في البيئة.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![خرائط الكتابة المزدوجة](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="ac9fc-170">تحديث كيانات البيانات بعد التحديث</span><span class="sxs-lookup"><span data-stu-id="ac9fc-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="ac9fc-171">في Finance، انتقل إلى مساحة عمل **إدارة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-171">In Finance, go to the **Data management** workspace.</span></span>

![مساحة عمل إدارة البيانات](./media/16DataManagement.png)

2. <span data-ttu-id="ac9fc-173">حدد تجانب **معلمات إطار العمل**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-173">Select the **Framework parameters** tile.</span></span>

![معلمات إطار العمل](./media/17FrameworkParameters.png)

3. <span data-ttu-id="ac9fc-175">في صفحة **إعدادات الكيان**، حدد **تحديث قائمة الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![تحديث قائمة الكيانات](./media/18RefreshEntityList.png)

<span data-ttu-id="ac9fc-177">سيستغرق التحديث مدة 20 دقيقة تقريبًا.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="ac9fc-178">وستتلقى تحذيرًا عند اكتماله.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-178">You will receive an alert when it is complete.</span></span>

![تأكيد التحديث](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="ac9fc-180">تشغيل خرائط ‏‫الكتابة المزدوجة في Project Operations</span><span class="sxs-lookup"><span data-stu-id="ac9fc-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="ac9fc-181">في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="ac9fc-182">تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات.**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-182">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="ac9fc-183">بعد تحديد الارتباط، ستتم إعادة توجيهك إلى قائمة الكيانات الموجودة في التعيينات.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="ac9fc-184">ابدأ الخرائط كما هو موضح في الجدول التالي.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="ac9fc-185">تأكد من اتباع التسلسل كما هو موضح.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="ac9fc-186">**تعيين الكيان**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-186">**Entity Map**</span></span> | <span data-ttu-id="ac9fc-187">**تحديث الكيان**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-187">**Refresh entity**</span></span> | <span data-ttu-id="ac9fc-188">**المزامنة الأولية**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-188">**Initial sync**</span></span> | <span data-ttu-id="ac9fc-189">**أصل المزامنة الأولية**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-189">**Master for initial sync**</span></span> | <span data-ttu-id="ac9fc-190">**تشغيل المتطلبات الأساسية**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-190">**Run prerequisites**</span></span> | <span data-ttu-id="ac9fc-191">**المزامنة الأولية للمتطلبات الأساسية**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="ac9fc-192">**أدوار موارد المشروع لجميع الشركات (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="ac9fc-193">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-193">No</span></span> | <span data-ttu-id="ac9fc-194">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="ac9fc-194">Yes</span></span> | <span data-ttu-id="ac9fc-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="ac9fc-195">Common Data Service</span></span> | <span data-ttu-id="ac9fc-196">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-196">No</span></span> | <span data-ttu-id="ac9fc-197">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-197">N\A</span></span> |
| <span data-ttu-id="ac9fc-198">**الكيانات القانونية (cdm\_الشركات)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="ac9fc-199">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-199">No</span></span> | <span data-ttu-id="ac9fc-200">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="ac9fc-200">Yes</span></span> | <span data-ttu-id="ac9fc-201">تطبيقات Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="ac9fc-201">Finance and Operations apps</span></span> | <span data-ttu-id="ac9fc-202">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-202">No</span></span> | <span data-ttu-id="ac9fc-203">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-203">N\A</span></span> |
| <span data-ttu-id="ac9fc-204">**القيم الفعلية لتكامل Project Operations(msdyn\_القيم الفعلية)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="ac9fc-205">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-205">No</span></span> | <span data-ttu-id="ac9fc-206">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-206">No</span></span> | <span data-ttu-id="ac9fc-207">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-207">N\A</span></span> | <span data-ttu-id="ac9fc-208">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="ac9fc-208">Yes</span></span> | <span data-ttu-id="ac9fc-209">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-209">No</span></span> |
| <span data-ttu-id="ac9fc-210">**بنود عقد المشروع (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="ac9fc-211">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-211">No</span></span> | <span data-ttu-id="ac9fc-212">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-212">No</span></span> | <span data-ttu-id="ac9fc-213">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-213">N\A</span></span> | <span data-ttu-id="ac9fc-214">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-214">No</span></span> | <span data-ttu-id="ac9fc-215">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-215">No</span></span> |
| <span data-ttu-id="ac9fc-216">**كيان التكامل لعلاقات معاملات المشروع (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="ac9fc-217">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-217">No</span></span> | <span data-ttu-id="ac9fc-218">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-218">No</span></span> | <span data-ttu-id="ac9fc-219">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-219">N\A</span></span> | <span data-ttu-id="ac9fc-220">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-220">No</span></span> | <span data-ttu-id="ac9fc-221">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-221">N\A</span></span> |
| <span data-ttu-id="ac9fc-222">**المراحل الرئيسية لبنود تعاقد التكامل مع Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="ac9fc-223">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-223">No</span></span> | <span data-ttu-id="ac9fc-224">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-224">No</span></span> | <span data-ttu-id="ac9fc-225">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-225">N\A</span></span> | <span data-ttu-id="ac9fc-226">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-226">No</span></span> | <span data-ttu-id="ac9fc-227">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-227">N\A</span></span> |
| <span data-ttu-id="ac9fc-228">**كيان تكامل Project Operations لتقديرات المصروفات (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="ac9fc-229">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-229">No</span></span> | <span data-ttu-id="ac9fc-230">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-230">No</span></span> | <span data-ttu-id="ac9fc-231">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-231">N\A</span></span> | <span data-ttu-id="ac9fc-232">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-232">No</span></span> | <span data-ttu-id="ac9fc-233">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-233">N\A</span></span> |
| <span data-ttu-id="ac9fc-234">**كيان تكامل Project Operations لتقديرات الساعات (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-234">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="ac9fc-235">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-235">No</span></span> | <span data-ttu-id="ac9fc-236">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-236">No</span></span> | <span data-ttu-id="ac9fc-237">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-237">N\A</span></span> | <span data-ttu-id="ac9fc-238">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-238">No</span></span> | <span data-ttu-id="ac9fc-239">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-239">N\A</span></span> |
| <span data-ttu-id="ac9fc-240">**كيان تصدير مصروفات مشروع لتكامل Project Operations (msdyn\_مصروفات)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="ac9fc-241">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="ac9fc-241">Yes</span></span> | <span data-ttu-id="ac9fc-242">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-242">No</span></span> | <span data-ttu-id="ac9fc-243">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-243">N\A</span></span> | <span data-ttu-id="ac9fc-244">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-244">No</span></span> | <span data-ttu-id="ac9fc-245">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-245">N\A</span></span> |
| <span data-ttu-id="ac9fc-246">**كيان تكامل Project Operations لتقديرات الساعات (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="ac9fc-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="ac9fc-247">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="ac9fc-247">Yes</span></span> | <span data-ttu-id="ac9fc-248">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-248">No</span></span> | <span data-ttu-id="ac9fc-249">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-249">N\A</span></span> | <span data-ttu-id="ac9fc-250">Yes</span><span class="sxs-lookup"><span data-stu-id="ac9fc-250">No</span></span> | <span data-ttu-id="ac9fc-251">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="ac9fc-251">N\A</span></span> |

4. <span data-ttu-id="ac9fc-252">لتحديث الكيان، حدد اسم الخريطة، ثم حدد **تحديث الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 
5. <span data-ttu-id="ac9fc-253">تابع تشغيل الخريطة بعد اكتمال التحديث.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-253">Proceed with running the map after the refresh is complete.</span></span>

![تحديث الخريطة‬](./media/20RefreshMapping.png)

<span data-ttu-id="ac9fc-255">قبل تمكين الخريطة التالية، تحقق من أن الخريطة الموجودة في الجدول بالحالة **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="ac9fc-256">قد يستغرق تشغيل الخرائط بعدد كبير من المتطلبات المسبقة بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="ac9fc-257">لتشغيل خريطة بالمتطلبات المسبقة، قم بتمكين تبديل **إظهار خرائط الكيانات المرتبطة**.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="ac9fc-258">إذا كان الجدول يشير إلى أن **المزامنة الأولية للمتطلبات الأساسية** بالقيمة **لا**، فتحقق من أن علامة **المزامنة الأولية** قيد **الإيقاف** في كافة خرائط المتطلبات الأساسية قبل تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-258">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![تشغيل الخريطة](./media/21RunMap.png)

6. <span data-ttu-id="ac9fc-260">تحقق من صحة كافة الخرائط ذات الصلة بالمشروع وأنها بالحالة تشغيل.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-260">Validate all project related maps are in the running state.</span></span>

![كل الخرائط قيد التشغيل](./media/22AllMapsRunning.png)

<span data-ttu-id="ac9fc-262">تم الآن تزويد بيئة Project Operations وتكوينها.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-262">Your Project Operations environment is now provisioned and configured.</span></span>
