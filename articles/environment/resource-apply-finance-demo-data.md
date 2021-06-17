---
title: تطبيق بيانات العرض التوضيحي على بيئة مستضافة في سحابة Finance
description: يوضح هذا الموضوع كيفية تطبيق البيانات التجريبية من Project Operations إلى بيئة Dynamics 365 Finance المستضافة على السحابة.
author: sigitac
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7d8a198b3bfd71ae08bc338d17896519b5ffd6b8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000121"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a><span data-ttu-id="e4180-103">تطبيق بيانات العرض التوضيحي على بيئة مستضافة في سحابة Finance</span><span class="sxs-lookup"><span data-stu-id="e4180-103">Apply demo data to a Finance Cloud-hosted environment</span></span>

<span data-ttu-id="e4180-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="e4180-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e4180-105">ينطبق هذا الموضوع فقط على Microsoft Dynamics 365 Finance الإصدار 10.0.13 ويمكن تنفيذه فقط على بيئة مستضافة على السحابة.</span><span class="sxs-lookup"><span data-stu-id="e4180-105">This topic is only applicable only Microsoft Dynamics 365 Finance version 10.0.13 and can be performed only on a Cloud-hosted environment.</span></span> <span data-ttu-id="e4180-106">أكمل الخطوات الواردة في هذا الموضوع **قبل** تطبيق تحديثات الجودة على البيئة.</span><span class="sxs-lookup"><span data-stu-id="e4180-106">Complete the steps in this topic **BEFORE** you apply quality updates to the environment.</span></span>

1. <span data-ttu-id="e4180-107">في مشروع LCS الخاص بك، افتح صفحة **تفاصيل البيئة**.</span><span class="sxs-lookup"><span data-stu-id="e4180-107">In your LCS project, open the **Environment details** page.</span></span> <span data-ttu-id="e4180-108">لاحظ أنه يتضمن التفاصيل اللازمة للاتصال بالبيئة باستخدام بروتوكول سطح المكتب البعيد (RDP).</span><span class="sxs-lookup"><span data-stu-id="e4180-108">Notice that it includes the details needed to connect to the environment by using Remote Desktop Protocol (RDP).</span></span>

![تفاصيل بيئة ](./media/1EnvironmentDetails.png)

<span data-ttu-id="e4180-110">المجموعة الأولى من بيانات الاعتماد المميزة هي بيانات اعتماد الحسابات المحلية وتحتوي على ارتباط تشعبي إلى الاتصال سطح المكتب البعيد.</span><span class="sxs-lookup"><span data-stu-id="e4180-110">The first set of highlighted credentials are the local account credentials and contain a hyperlink to the remote desktop connection.</span></span> <span data-ttu-id="e4180-111">تتضمن بيانات الاعتماد اسم المستخدم وكلمة المرور الخاصة بمسؤول البيئة.</span><span class="sxs-lookup"><span data-stu-id="e4180-111">The credentials include the environment admin username and password.</span></span> <span data-ttu-id="e4180-112">يتم استخدام المجموعة الثانية من بيانات الاعتماد لتسجيل الدخول إلى SQL Server في هذه البيئة.</span><span class="sxs-lookup"><span data-stu-id="e4180-112">The second set of credentials are used to log in to SQL Server in this environment.</span></span>

2. <span data-ttu-id="e4180-113">قم بالاتصال بالبيئة بواسطة الارتباط التشعبي في **الحسابات المحلية**، واستخدم **بيانات اعتماد الحساب المحلي** للمصادقة.</span><span class="sxs-lookup"><span data-stu-id="e4180-113">Remote to the environment by the hyperlink in **Local Accounts**, and use the **Local Account credentials** to authenticate.</span></span>
3. <span data-ttu-id="e4180-114">انتقل إلى **خدمات معلومات الإنترنت** > **مجموعات التطبيقات** > **AOSService** وأوقف الخدمة.</span><span class="sxs-lookup"><span data-stu-id="e4180-114">Go to **Internet Information Services** > **Application Pools** > **AOSService** and stop the service.</span></span> <span data-ttu-id="e4180-115">أنت توقف الخدمة عند هذه النقطة لكي يمكنك الاستمرار في استبدال قاعدة بيانات SQL.</span><span class="sxs-lookup"><span data-stu-id="e4180-115">You are stopping the service at this point so that you can continue to replace the SQL database.</span></span>

![إيقاف AOS](./media/2StopAOS.png)

4. <span data-ttu-id="e4180-117">انتقل إلى **الخدمات** وأوقف العنصرين التاليين:</span><span class="sxs-lookup"><span data-stu-id="e4180-117">Go to **Services** and stop the following two items:</span></span>

- <span data-ttu-id="e4180-118">Microsoft Dynamics 365 Unified Operations: خدمة إدارة الدفعات</span><span class="sxs-lookup"><span data-stu-id="e4180-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span></span>
- <span data-ttu-id="e4180-119">Microsoft Dynamics 365 Unified Operations: إطار عمل تصدير واستيراد البيانات</span><span class="sxs-lookup"><span data-stu-id="e4180-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span></span>

![إيقاف الخدمات](./media/3StopServices.png)

5. <span data-ttu-id="e4180-121">افتح Microsoft SQL Server Management Studio.</span><span class="sxs-lookup"><span data-stu-id="e4180-121">Open Microsoft SQL Server Management Studio.</span></span> <span data-ttu-id="e4180-122">سجل الدخول باستخدام بيانات اعتماد SQL server واستخدم مستخدم وكلمة مرور axdbadmin من صفحة **تفاصيل البيئة** لـ LCS.</span><span class="sxs-lookup"><span data-stu-id="e4180-122">Log in with SQL server credentials and use the axdbadmin user and password from the LCS **Environments details** page.</span></span>

![SQL Server Management Studio](./media/4SSMS.png)

6. <span data-ttu-id="e4180-124">في مستكشف الكائنات، **قواعد البيانات** وحدد مكان **AXDB**.</span><span class="sxs-lookup"><span data-stu-id="e4180-124">In Object Explorer, **Databases** and locate **AXDB**.</span></span> <span data-ttu-id="e4180-125">ستقوم باستبدال قاعدة البيانات بقاعدة البيانات الجديدة الموجودة في [مركز التنزيل](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span><span class="sxs-lookup"><span data-stu-id="e4180-125">You will replace database with a new database that is located in the [Download Center](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span></span> 
7. <span data-ttu-id="e4180-126">انسخ الملف المضغوط إلى VM الذي تتصل به عن بعد وقم باستخراج المحتويات المضغوطة.</span><span class="sxs-lookup"><span data-stu-id="e4180-126">Copy the zip file to the VM you are remoted into and extract zip contents.</span></span>
8. <span data-ttu-id="e4180-127">في SQL Server Management Studio، انقر بزر الماوس الأيمن فوق **AxDB**، ثم حدد **المهام** > **استعادة** > **قاعدة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="e4180-127">In SQL Server Management Studio, right-click **AxDB**, and then select **Tasks** > **Restore** > **Database**.</span></span>

![استعادة قاعدة البيانات](./media/5RestoreDatabase.png)

9. <span data-ttu-id="e4180-129">حدد **الجهاز المصدر** وانتقل إلى الملف الذي تم استخراجه من الملف المضغوط الذي قمت بنسخه.</span><span class="sxs-lookup"><span data-stu-id="e4180-129">Select **Source Device** and navigate to the file extracted from zip you copied.</span></span>

![الأجهزة المصدر](./media/6SourceDevice.png)

10. <span data-ttu-id="e4180-131">حدد **الخيارات**، ثم حدد **الكتابة فوق قاعدة البيانات الموجودة** و **إغلاق الاتصالات الموجودة بقاعدة البيانات الوجهة**.</span><span class="sxs-lookup"><span data-stu-id="e4180-131">Select **Options**, and then select **Overwrite the existing database** and **Close existing connections to destination database**.</span></span> 
11. <span data-ttu-id="e4180-132">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e4180-132">Select **OK**.</span></span>

![استعادة الإعدادات](./media/7RestoreSetting.png)

<span data-ttu-id="e4180-134">ستتلقى تأكيدًا بأن عملية استعادة AXDB كانت ناجحة.</span><span class="sxs-lookup"><span data-stu-id="e4180-134">You will receive confirmation that the AXDB restore was successful.</span></span> <span data-ttu-id="e4180-135">بعد تلقي هذا التأكيد، يمكنك إغلاق SQL Services Management Studio.</span><span class="sxs-lookup"><span data-stu-id="e4180-135">After you receive this confirmation, you can close SQL Services Management Studio.</span></span>

12. <span data-ttu-id="e4180-136">ارجع إلى **خدمات معلومات الإنترنت** > **مجموعات التطبيقات** > **AOSService** وابدأ AOSService.</span><span class="sxs-lookup"><span data-stu-id="e4180-136">Go back to **Internet Information Services** > **Application Pools** > **AOSService** and start the AOSService.</span></span>
13. <span data-ttu-id="e4180-137">انتقل إلى **الخدمات** وأبدا الخدمتين اللتين قمت بإيقافهما في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="e4180-137">Go to **Services** and start the two services you stopped earlier.</span></span>

14. <span data-ttu-id="e4180-138">حدد موقع أداة AdminUserProvisioning في VM هذا.</span><span class="sxs-lookup"><span data-stu-id="e4180-138">Locate the AdminUserProvisioning tool on this VM.</span></span> <span data-ttu-id="e4180-139">ابحث أسفل، K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span><span class="sxs-lookup"><span data-stu-id="e4180-139">Look under, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span></span>
15. <span data-ttu-id="e4180-140">قم بتشغيل ملف .ext باستخدام عنوان المستخدم الخاص بك في حقل **عنوان البريد الإلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="e4180-140">Run the .ext file using your user address in the **Email Address** field.</span></span> 
16. <span data-ttu-id="e4180-141">حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="e4180-141">Select **Submit**.</span></span>

![تزويد المستخدم المسؤول](./media/8AdminUserProvisioning.png)

<span data-ttu-id="e4180-143">يستغرق إكمال هذا الإجراء عدة دقائق.</span><span class="sxs-lookup"><span data-stu-id="e4180-143">This takes a couple of minutes to complete.</span></span> <span data-ttu-id="e4180-144">ينبغي أن تتلقي رسالة تأكيد بأن المستخدم المسؤول قد تم تحديثه بنجاح.</span><span class="sxs-lookup"><span data-stu-id="e4180-144">You should receive a confirmation message that the Admin user was successfully updated.</span></span>

17. <span data-ttu-id="e4180-145">في النهاية، قم بتشغيل موجه الأوامر كمسؤول وتنفيذ iisreset</span><span class="sxs-lookup"><span data-stu-id="e4180-145">Lastly, run Command Prompt as Administrator and perform iisreset</span></span>

![إعادة تعيين IIS](./media/9IISReset.png)

18. <span data-ttu-id="e4180-147">قم بإغلاق جلسة عمل سطح المكتب البعيد واستخدم صفحة **تفاصيل بيئة** LCS لتسجيل الدخول إلى البيئة للتأكد من أنها تعمل كما هو متوقع.</span><span class="sxs-lookup"><span data-stu-id="e4180-147">Close the remote desktop session and use the LCS **Environment details** page to log in to the environment to confirm it is working as expected.</span></span>

![Finance and Operations](./media/10FinanceAndOperations.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]