---
title: تزويد بيئة جديدة
description: يوفر هذا الموضوع معلومات حول كيفية تزويد بيئة Project Operations جديدة.
author: sigitac
manager: Annbe
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 09af2a7693c45d1d0b9c75420d018cc50d2cc0fa
ms.sourcegitcommit: 04c446746aad97fc3f4c3d441983c586b918a3a6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/11/2020
ms.locfileid: "4727774"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="91469-103">تزويد بيئة جديدة</span><span class="sxs-lookup"><span data-stu-id="91469-103">Provision a new environment</span></span>

<span data-ttu-id="91469-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="91469-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="91469-105">يوفر هذا الموضوع معلومات حول كيفية توفير بيئة Dynamics 365 Project Operations جديدة للسيناريوهات القائمة على الموارد/غير المخزنة.</span><span class="sxs-lookup"><span data-stu-id="91469-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="91469-106">تمكين التزويد التلقائي Project Operations في مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="91469-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="91469-107">استخدم الخطوات التالية لتمكين سير عمل التزويد التلقائي لـ Project Operations لمشروع LCS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="91469-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="91469-108">انتقل إلى [LCS](https://lcs.dynamics.com/v2) وحدد تجانب **إدارة ميزة المعاينة**.</span><span class="sxs-lookup"><span data-stu-id="91469-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="91469-109">في قائمة **ميزة المعاينة**، حدد **ميزة Project Operations** ثم حدد **تمكين ميزة المعاينة** لتمكين Project Operations.</span><span class="sxs-lookup"><span data-stu-id="91469-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="91469-110">يتم تنفيذ هذه الخطوة مرة واحدة فقط لكل مشروع LCS.</span><span class="sxs-lookup"><span data-stu-id="91469-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="91469-111">تزويد بيئة Project Operations</span><span class="sxs-lookup"><span data-stu-id="91469-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="91469-112">افتح Dynamics 365 Finance جديد [في بيئة عرض توضيحي](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) أو نشر [بيئة الحماية / الإنتاج](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="91469-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="91469-113">اتبع خطوات معالج **تزويد البيئة**.</span><span class="sxs-lookup"><span data-stu-id="91469-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="91469-114">تأكد من أن إصدار التطبيق المحدد 10.0.13 أو أحدث.</span><span class="sxs-lookup"><span data-stu-id="91469-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="91469-115">لتزويد Project Operations، ضمن **إعدادات متقدمة**، حدد **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="91469-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="91469-116">قم بتمكين **إعداد Common Data Service** من خلال اختيار **نعم** ثم أدخل المعلومات في الحقول المطلوبة:</span><span class="sxs-lookup"><span data-stu-id="91469-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="91469-117">اسم</span><span class="sxs-lookup"><span data-stu-id="91469-117">Name</span></span>
  - <span data-ttu-id="91469-118">المنطقة</span><span class="sxs-lookup"><span data-stu-id="91469-118">Region</span></span>
  - <span data-ttu-id="91469-119">اللغة‬</span><span class="sxs-lookup"><span data-stu-id="91469-119">Language</span></span>
  - <span data-ttu-id="91469-120">‏‏العملة</span><span class="sxs-lookup"><span data-stu-id="91469-120">Currency</span></span>
 
5. <span data-ttu-id="91469-121">في حقل **قالب Common Data Service**، حدد **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="91469-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="91469-122">حدد نوع البيئة لعملية التوزيع الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="91469-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="91469-123">سيتيح لك الإصدار التجريبي الذي يستند إلى الاشتراك نشر بيئة CDS لمدة 30 يومًا.</span><span class="sxs-lookup"><span data-stu-id="91469-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![إعدادات النشر](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="91469-125">حدد **موافقة** للإقرار بشروط الخدمة ثم حدد **تم** للرجوع إلى إعدادات التوزيع.</span><span class="sxs-lookup"><span data-stu-id="91469-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![الموافقة على التوزيع](./media/2DeploymentConsent.png)

7. <span data-ttu-id="91469-127">اختياري - تطبيق بيانات تجريبية على البيئة.</span><span class="sxs-lookup"><span data-stu-id="91469-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="91469-128">انتقل إلى **إعدادات متقدمة**، وحدد **تخصيص تكوين قاعدة بيانات SQL**، ثم قم بتعيين **تحديد مجموعة البيانات لقاعدة بيانات التطبيق** إلى **عرض توضيحي**.</span><span class="sxs-lookup"><span data-stu-id="91469-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="91469-129">أكمل الحقول المطلوبة المتبقية في المعالج وقم بتأكيد التوزيع.</span><span class="sxs-lookup"><span data-stu-id="91469-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="91469-130">يختلف وقت توفير البيئة وفقا لنوع البيئة.</span><span class="sxs-lookup"><span data-stu-id="91469-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="91469-131">قد تستغرق عملية التزويد ست ساعات.</span><span class="sxs-lookup"><span data-stu-id="91469-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="91469-132">بعد اكتمال التوزيع بنجاح، سيتم عرض البيئة بالحالة **تم نشرها**.</span><span class="sxs-lookup"><span data-stu-id="91469-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="91469-133">لتأكيد نشر البيئة بنجاح، قم بتحديد **تسجيل الدخول** سجل الدخول إلى البيئة للتأكيد.</span><span class="sxs-lookup"><span data-stu-id="91469-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![تفاصيل بيئة ](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="91469-135">تطبيق التحديثات على بيئة Finance</span><span class="sxs-lookup"><span data-stu-id="91469-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="91469-136">تتطلب Project Operations بيئة Finance بإصدار تطبيق رقم **10.0.13 (10.0.569.20009)** أو الأعلى.</span><span class="sxs-lookup"><span data-stu-id="91469-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="91469-137">قد تحتاج إلى تطبيق تحديثات الجودة على بيئة Finance لديك لاستلام هذا الإصدار.</span><span class="sxs-lookup"><span data-stu-id="91469-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="91469-138">في LCS، في صفحة **تفاصيل البيئة**، في قسم **التحديثات المتوفرة**، حدد **عرض التحديث**.</span><span class="sxs-lookup"><span data-stu-id="91469-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![عرض التحديثات](./media/5ViewUpdates.png)

2. <span data-ttu-id="91469-140">في صفحة **التحديثات الثنائية**، حدد **حفظ الحزمة.**</span><span class="sxs-lookup"><span data-stu-id="91469-140">On the **Binary updates** page, select **Save package.**</span></span>

![حفظ الحزمة](./media/6SavePackage.png)

3. <span data-ttu-id="91469-142">انقر فوق **تحديد الكل** ثم حدد **حفظ الحزمة**.</span><span class="sxs-lookup"><span data-stu-id="91469-142">Click **Select all** and then select **Save package**.</span></span>

![مراجعة التحديثات وحفظها](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="91469-144">أدخل اسمًا ووصفًا للحزمة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="91469-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="91469-145">تبعًا لاتصال الإنترنت، قد تستغرق هذه العملية بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="91469-145">Depending on the internet connection, this process might take some time.</span></span>

![تحميل الحزمة إلى مكتبة الأصول](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="91469-147">بعد حفظ الحزمة، حدد **تم** وقم بحفظ هذه الحزمة في مكتبة الأصول في مشروع LCS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="91469-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="91469-148">قد يستغرق حفظ الحزمة والتحقق من صحتها ~ 15 دقيقة.</span><span class="sxs-lookup"><span data-stu-id="91469-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="91469-149">لتطبيق التحديث، انتقل إلى صفحة **تفاصيل البيئة** في LCS وحدد **الصيانة** > **تطبيق التحديثات**.</span><span class="sxs-lookup"><span data-stu-id="91469-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![صيانة البيئات](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="91469-151">في قائمة التحديثات، قم بتحديد الحزمة التي قمت بإنشائها، وقم بتحديد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="91469-151">In the updates list select the package you created, and select **Apply**.</span></span>

![تطبيق التحديثات](./media/10ApplyUpdates.png)

<span data-ttu-id="91469-153">ستستغرق عملية "صيانة البيئة" بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="91469-153">Environment servicing will take some time.</span></span> <span data-ttu-id="91469-154">بعد انتهائها، ستعود البيئة إلى حالة تم نشرها.</span><span class="sxs-lookup"><span data-stu-id="91469-154">After it is complete, the environment will return to a deployed state.</span></span>

![البيئة المنشورة](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="91469-156">إنشاء اتصال كتابة مزدوج</span><span class="sxs-lookup"><span data-stu-id="91469-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="91469-157">في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.</span><span class="sxs-lookup"><span data-stu-id="91469-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="91469-158">تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات**.</span><span class="sxs-lookup"><span data-stu-id="91469-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="91469-159">بعد اكتمال الارتباط، حدد **ربط بـ CDS للتطبيقات‏‎** مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="91469-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="91469-160">ستتم إعادة توجيهك إلى الكتابة المزدوجة في Finance.</span><span class="sxs-lookup"><span data-stu-id="91469-160">You will be redirected to Dual Write in Finance.</span></span>

![ربط بـ CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="91469-162">حدد **تطبيق الحل** للوصول إلى الكيانات التي سيتم تعيينها في التكامل.</span><span class="sxs-lookup"><span data-stu-id="91469-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![تطبيق الحلول](./media/13ApplySolutions.png)

5. <span data-ttu-id="91469-164">حدد الحلين، **Dynamics 365 Finance and Operations خريطة كيان‬ الكتابة المزدوجة‬** و **Dynamics 365 Project Operations خرائط كيان‬ الكتابة المزدوجة‬**، ثم حدد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="91469-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![تأكيد الحلول](./media/14ConfirmSolutions.png)

<span data-ttu-id="91469-166">بعد تطبيق الحلول، يتم تطبيق كيانات الكتابة المزدوجة على البيئة.</span><span class="sxs-lookup"><span data-stu-id="91469-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![تطبيق الحلول](./media/15ApplyingSolutions.png)

<span data-ttu-id="91469-168">بعد تطبيق الكيانات، يتم سرد كافة التعيينات المتوفرة في البيئة.</span><span class="sxs-lookup"><span data-stu-id="91469-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![خرائط الكتابة المزدوجة](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="91469-170">تحديث كيانات البيانات بعد التحديث</span><span class="sxs-lookup"><span data-stu-id="91469-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="91469-171">في Finance، انتقل إلى مساحة عمل **إدارة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="91469-171">In Finance, go to the **Data management** workspace.</span></span>

![مساحة عمل إدارة البيانات](./media/16DataManagement.png)

2. <span data-ttu-id="91469-173">حدد تجانب **معلمات إطار العمل**.</span><span class="sxs-lookup"><span data-stu-id="91469-173">Select the **Framework parameters** tile.</span></span>

![معلمات إطار العمل](./media/17FrameworkParameters.png)

3. <span data-ttu-id="91469-175">في صفحة **إعدادات الكيان**، حدد **تحديث قائمة الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="91469-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![تحديث قائمة الكيانات](./media/18RefreshEntityList.png)

<span data-ttu-id="91469-177">سيستغرق التحديث مدة 20 دقيقة تقريبًا.</span><span class="sxs-lookup"><span data-stu-id="91469-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="91469-178">وستتلقى تحذيرًا عند اكتماله.</span><span class="sxs-lookup"><span data-stu-id="91469-178">You will receive an alert when it is complete.</span></span>

![تأكيد التحديث](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="91469-180">تحديث إعدادات الأمان على Project Operations في Dataverse</span><span class="sxs-lookup"><span data-stu-id="91469-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="91469-181">انتقل إلى Project Operations في بيئة Dataverse الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="91469-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="91469-182">انتقل إلى **الإعدادات** > **الأمان** > **أدوار الأمان**.</span><span class="sxs-lookup"><span data-stu-id="91469-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="91469-183">في صفحة **أدوار الأمان**، في قائمة الأدوار، حدد **مستخدم تطبيق الكتابة المزدوجة** وحدد علامة التبويب **الكيانات المخصصة**.</span><span class="sxs-lookup"><span data-stu-id="91469-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="91469-184">تحقق من أن الدور يحتوي على أذونات **قراءة** و **إلحاق بـ** لـ:</span><span class="sxs-lookup"><span data-stu-id="91469-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="91469-185">**نوع سعر الصرف للعملة**</span><span class="sxs-lookup"><span data-stu-id="91469-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="91469-186">**مخطط الحسابات**</span><span class="sxs-lookup"><span data-stu-id="91469-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="91469-187">**التقويم المالي**</span><span class="sxs-lookup"><span data-stu-id="91469-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="91469-188">**دفتر الأستاذ**</span><span class="sxs-lookup"><span data-stu-id="91469-188">**Ledger**</span></span>

5. <span data-ttu-id="91469-189">بعد تحديث دور الأمان، انتقل إلى **الإعدادات** > **الأمان** > **الفرق**، وحدد الفريق الافتراضي في طريق عرض الفريق **مالك العمل المحلي**.</span><span class="sxs-lookup"><span data-stu-id="91469-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="91469-190">حدد **إدارة الأدوار** وتحقق من أن امتياز أمان **مستخدم تطبيق الكتابة المزدوجة** يتم تطبيقه على هذا الفريق.</span><span class="sxs-lookup"><span data-stu-id="91469-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="91469-191">تشغيل خرائط ‏‫الكتابة المزدوجة في Project Operations</span><span class="sxs-lookup"><span data-stu-id="91469-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="91469-192">في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.</span><span class="sxs-lookup"><span data-stu-id="91469-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="91469-193">تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات.**</span><span class="sxs-lookup"><span data-stu-id="91469-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="91469-194">بعد تحديد الارتباط، ستتم إعادة توجيهك إلى قائمة الكيانات الموجودة في التعيينات.</span><span class="sxs-lookup"><span data-stu-id="91469-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="91469-195">ابدأ الخرائط كما هو موضح في الجدول التالي.</span><span class="sxs-lookup"><span data-stu-id="91469-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="91469-196">تأكد من اتباع التسلسل كما هو موضح.</span><span class="sxs-lookup"><span data-stu-id="91469-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="91469-197">**تعيين الكيان**</span><span class="sxs-lookup"><span data-stu-id="91469-197">**Entity Map**</span></span> | <span data-ttu-id="91469-198">**تحديث الكيان**</span><span class="sxs-lookup"><span data-stu-id="91469-198">**Refresh entity**</span></span> | <span data-ttu-id="91469-199">**المزامنة الأولية**</span><span class="sxs-lookup"><span data-stu-id="91469-199">**Initial sync**</span></span> | <span data-ttu-id="91469-200">**أصل المزامنة الأولية**</span><span class="sxs-lookup"><span data-stu-id="91469-200">**Master for initial sync**</span></span> | <span data-ttu-id="91469-201">**تشغيل المتطلبات الأساسية**</span><span class="sxs-lookup"><span data-stu-id="91469-201">**Run prerequisites**</span></span> | <span data-ttu-id="91469-202">**المزامنة الأولية للمتطلبات الأساسية**</span><span class="sxs-lookup"><span data-stu-id="91469-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="91469-203">**أدوار موارد المشروع لجميع الشركات (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="91469-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="91469-204">لا </span><span class="sxs-lookup"><span data-stu-id="91469-204">No</span></span> | <span data-ttu-id="91469-205">نعم </span><span class="sxs-lookup"><span data-stu-id="91469-205">Yes</span></span> | <span data-ttu-id="91469-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="91469-206">Common Data Service</span></span> | <span data-ttu-id="91469-207">لا </span><span class="sxs-lookup"><span data-stu-id="91469-207">No</span></span> | <span data-ttu-id="91469-208">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-208">N\A</span></span> |
| <span data-ttu-id="91469-209">**الكيانات القانونية (cdm\_الشركات)**</span><span class="sxs-lookup"><span data-stu-id="91469-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="91469-210">لا </span><span class="sxs-lookup"><span data-stu-id="91469-210">No</span></span> | <span data-ttu-id="91469-211">نعم </span><span class="sxs-lookup"><span data-stu-id="91469-211">Yes</span></span> | <span data-ttu-id="91469-212">تطبيقات Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="91469-212">Finance and Operations apps</span></span> | <span data-ttu-id="91469-213">لا </span><span class="sxs-lookup"><span data-stu-id="91469-213">No</span></span> | <span data-ttu-id="91469-214">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-214">N\A</span></span> |
| <span data-ttu-id="91469-215">**دفتر الأستاذ (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="91469-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="91469-216">لا </span><span class="sxs-lookup"><span data-stu-id="91469-216">No</span></span> | <span data-ttu-id="91469-217">نعم </span><span class="sxs-lookup"><span data-stu-id="91469-217">Yes</span></span> | <span data-ttu-id="91469-218">تطبيقات Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="91469-218">Finance and Operations apps</span></span> | <span data-ttu-id="91469-219">نعم </span><span class="sxs-lookup"><span data-stu-id="91469-219">Yes</span></span> | <span data-ttu-id="91469-220">نعم، تطبيقات Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="91469-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="91469-221">**القيم الفعلية لتكامل Project Operations(msdyn\_القيم الفعلية)**</span><span class="sxs-lookup"><span data-stu-id="91469-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="91469-222">لا </span><span class="sxs-lookup"><span data-stu-id="91469-222">No</span></span> | <span data-ttu-id="91469-223">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-223">No</span></span> | <span data-ttu-id="91469-224">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-224">N\A</span></span> | <span data-ttu-id="91469-225">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="91469-225">Yes</span></span> | <span data-ttu-id="91469-226">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-226">No</span></span> |
| <span data-ttu-id="91469-227">**بنود عقد المشروع (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="91469-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="91469-228">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-228">No</span></span> | <span data-ttu-id="91469-229">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-229">No</span></span> | <span data-ttu-id="91469-230">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-230">N\A</span></span> | <span data-ttu-id="91469-231">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-231">No</span></span> | <span data-ttu-id="91469-232">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-232">No</span></span> |
| <span data-ttu-id="91469-233">**كيان التكامل لعلاقات معاملات المشروع (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="91469-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="91469-234">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-234">No</span></span> | <span data-ttu-id="91469-235">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-235">No</span></span> | <span data-ttu-id="91469-236">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-236">N\A</span></span> | <span data-ttu-id="91469-237">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-237">No</span></span> | <span data-ttu-id="91469-238">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-238">N\A</span></span> |
| <span data-ttu-id="91469-239">**المراحل الرئيسية لبنود تعاقد التكامل مع Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="91469-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="91469-240">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-240">No</span></span> | <span data-ttu-id="91469-241">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-241">No</span></span> | <span data-ttu-id="91469-242">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-242">N\A</span></span> | <span data-ttu-id="91469-243">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-243">No</span></span> | <span data-ttu-id="91469-244">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-244">N\A</span></span> |
| <span data-ttu-id="91469-245">**كيان تكامل Project Operations لتقديرات المصروفات (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="91469-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="91469-246">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-246">No</span></span> | <span data-ttu-id="91469-247">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-247">No</span></span> | <span data-ttu-id="91469-248">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-248">N\A</span></span> | <span data-ttu-id="91469-249">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-249">No</span></span> | <span data-ttu-id="91469-250">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-250">N\A</span></span> |
| <span data-ttu-id="91469-251">**كيان تصدير فئات مصروفات مشروع لتكامل Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="91469-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="91469-252">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-252">No</span></span> | <span data-ttu-id="91469-253">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-253">No</span></span> | <span data-ttu-id="91469-254">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-254">N\A</span></span> | <span data-ttu-id="91469-255">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-255">No</span></span> | <span data-ttu-id="91469-256">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-256">N\A</span></span> |
| <span data-ttu-id="91469-257">**كيان تصدير مصروفات مشروع لتكامل Project Operations (msdyn\_مصروفات)**</span><span class="sxs-lookup"><span data-stu-id="91469-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="91469-258">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="91469-258">Yes</span></span> | <span data-ttu-id="91469-259">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-259">No</span></span> | <span data-ttu-id="91469-260">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-260">N\A</span></span> | <span data-ttu-id="91469-261">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-261">No</span></span> | <span data-ttu-id="91469-262">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-262">N\A</span></span> |
| <span data-ttu-id="91469-263">**كيان تكامل Project Operations لتقديرات الساعات (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="91469-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="91469-264">‏‏نعم</span><span class="sxs-lookup"><span data-stu-id="91469-264">Yes</span></span> | <span data-ttu-id="91469-265">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-265">No</span></span> | <span data-ttu-id="91469-266">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-266">N\A</span></span> | <span data-ttu-id="91469-267">Yes</span><span class="sxs-lookup"><span data-stu-id="91469-267">No</span></span> | <span data-ttu-id="91469-268">‏‫غير متوفر‬</span><span class="sxs-lookup"><span data-stu-id="91469-268">N\A</span></span> |


4. <span data-ttu-id="91469-269">لتحديث الكيان، حدد اسم الخريطة، ثم حدد **تحديث الكيانات**.</span><span class="sxs-lookup"><span data-stu-id="91469-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![تحديث الخريطة‬](./media/20RefreshMapping.png)

5. <span data-ttu-id="91469-271">شغّل الخريطة بعد اكتمال التحديث.</span><span class="sxs-lookup"><span data-stu-id="91469-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="91469-272">قبل تمكين الخريطة التالية، تحقق من أن الخريطة الموجودة في الجدول بالحالة **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="91469-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="91469-273">قد يستغرق تشغيل الخرائط بعدد كبير من المتطلبات المسبقة بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="91469-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="91469-274">لتشغيل خريطة بالمتطلبات المسبقة، قم بتمكين تبديل **إظهار خرائط الكيانات المرتبطة**.</span><span class="sxs-lookup"><span data-stu-id="91469-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="91469-275">إذا كان الجدول يشير إلى أن **المزامنة الأولية للمتطلبات الأساسية** بالقيمة **لا**، فتحقق من أن علامة **المزامنة الأولية** قيد **الإيقاف** في كافة خرائط المتطلبات الأساسية قبل تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="91469-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![تشغيل الخريطة](./media/21RunMap.png)

6. <span data-ttu-id="91469-277">تحقق من صحة كافة الخرائط ذات الصلة بالمشروع وأنها بالحالة تشغيل.</span><span class="sxs-lookup"><span data-stu-id="91469-277">Validate all project related maps are in the running state.</span></span>

![كل الخرائط قيد التشغيل](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="91469-279">تطبيق بيانات التكوين في CDS لـ Project Operations (اختياري)</span><span class="sxs-lookup"><span data-stu-id="91469-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="91469-280">إذا كنت قد قمت بتطبيق بيانات العرض التوضيحي على بيئة Finance، فراجع [إعداد بيانات التكوين وتطبيقها في Common Data Service لـ Project Operations](resource-apply-pro-setup-config-data.md) لتطبيق بيانات العرض التوضيحي على بيئة CDS.</span><span class="sxs-lookup"><span data-stu-id="91469-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="91469-281">تم الآن تزويد بيئة Project Operations وتكوينها.</span><span class="sxs-lookup"><span data-stu-id="91469-281">Your Project Operations environment is now provisioned and configured.</span></span> 
