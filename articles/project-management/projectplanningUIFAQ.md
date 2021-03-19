---
title: استكشاف الأخطاء العمل في شبكة المهام وإصلاحها
description: يوفر هذا الموضوع معلومات استكشاف الأخطاء وإصلاحها المطلوبة عند العمل في شبكة المهام.
author: ruhercul
manager: tfehr
ms.date: 01/19/2021
ms.topic: article
ms.product: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: dedd989cc7c959d9ea97a0abfb13f8f1b2150a56
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286547"
---
# <a name="troubleshoot-working-in-the-task-grid"></a><span data-ttu-id="6236b-103">استكشاف الأخطاء العمل في شبكة المهام وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="6236b-103">Troubleshoot working in the Task grid</span></span> 

<span data-ttu-id="6236b-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="6236b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6236b-105">يصف هذا الموضوع كيفية إصلاح المشكلات التي قد تواجهك أثناء العمل مع إدارة التكلفة.</span><span class="sxs-lookup"><span data-stu-id="6236b-105">This topic describes how to fix issues that you might encounter while working with cost management.</span></span>

## <a name="enable-cookies"></a><span data-ttu-id="6236b-106">تمكين ملفات تعريف الارتباط</span><span class="sxs-lookup"><span data-stu-id="6236b-106">Enable cookies</span></span>

<span data-ttu-id="6236b-107">يتطلب Project Operations تمكين ملفات تعريف الارتباط الخاصة بطرف ثالث من أجل عرض هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="6236b-107">Project Operations requires that third-party cookies be enabled in order to render the work breakdown structure.</span></span> <span data-ttu-id="6236b-108">عند عدم تمكين ملفات تعريف الارتباط الخاصة بطرف ثالث، فبدلا من مشاهدة المهام، سترى صفحة فارغة عند تحديد علامة التبويب **مهام** في صفحة **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6236b-108">When third-party cookies aren't enabled, instead of seeing tasks, you will see a blank page when you select the **Tasks** tab on the **Project** page.</span></span>

![علامة تبويب فارغة عند عدم تمكين ملفات تعريف الارتباط الخاصة بطرف ثالث](media/blankschedule.png)


### <a name="workaround"></a><span data-ttu-id="6236b-110">الطرق البديلة</span><span class="sxs-lookup"><span data-stu-id="6236b-110">Workaround</span></span>
<span data-ttu-id="6236b-111">بالنسبة لمستعرضات Microsoft Edge أو Google Chrome، تستعرض الإجراءات التالية كيفية تحديث إعداد المستعرض لتمكين ملفات تعريف الارتباط الخاصة بطرف ثالث.</span><span class="sxs-lookup"><span data-stu-id="6236b-111">For Microsoft Edge or Google Chrome browsers, the following procedures outline how to update your browser setting to enable third-party cookies.</span></span>

#### <a name="microsoft-edge"></a><span data-ttu-id="6236b-112">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6236b-112">Microsoft Edge</span></span>

1. <span data-ttu-id="6236b-113">افتح مستعرض Edge.</span><span class="sxs-lookup"><span data-stu-id="6236b-113">Open your Edge browser.</span></span>
2. <span data-ttu-id="6236b-114">في الزاوية العلوية اليسرى، حدد **علامة الحذف**(...) ثم حدد **الإعدادات**.</span><span class="sxs-lookup"><span data-stu-id="6236b-114">In the upper-right corner, select the **ellipsis** (...), and then select **Settings**.</span></span>
3. <span data-ttu-id="6236b-115">ضمن **ملفات تعريف الارتباط وأذونات الموقع**، قم بتحديد **ملفات تعريف الارتباط وبيانات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="6236b-115">Under **Cookies and site permissions**, select **Cookies and site data**.</span></span>
4. <span data-ttu-id="6236b-116">أوقف تشغيل **حظر ملفات تعريف الارتباط لطرف ثالث**.</span><span class="sxs-lookup"><span data-stu-id="6236b-116">Turn off **Block third-party cookies**.</span></span>

#### <a name="google-chrome"></a><span data-ttu-id="6236b-117">Google Chrome</span><span class="sxs-lookup"><span data-stu-id="6236b-117">Google Chrome</span></span>

1. <span data-ttu-id="6236b-118">افتح مستعرض Chrome.</span><span class="sxs-lookup"><span data-stu-id="6236b-118">Open your Chrome browser.</span></span>
2. <span data-ttu-id="6236b-119">في الزاوية العلوية اليسرى، حدد النقاط الرأسية الثلاثة، ثم حدد **الإعدادات**.</span><span class="sxs-lookup"><span data-stu-id="6236b-119">In the upper-right corner, select the three vertical dots, and then select **Settings**.</span></span>
3. <span data-ttu-id="6236b-120">ضمن **الخصوصية والأمان**، قم بتحديد **ملفات تعريف الارتباط وبيانات الموقع الأخرى**.</span><span class="sxs-lookup"><span data-stu-id="6236b-120">Under **Privacy and security**, select **Cookies and other site data**.</span></span>
4. <span data-ttu-id="6236b-121">حدد **السماح بجميع ملفات تعريف الارتباط**.</span><span class="sxs-lookup"><span data-stu-id="6236b-121">Select **Allow all cookies**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6236b-122">إذا قمت بحظر ملفات تعريف الارتباط الخاصة بطرف ثالث، سيتم حظر كافة ملفات تعريف الارتباط وبيانات الموقع من المواقع الأخرى، حتى إذا كان الموقع مسموحًا به في قائمة الاستثناءات.</span><span class="sxs-lookup"><span data-stu-id="6236b-122">If you block third-party cookies, all cookies and site data from other sites will be blocked, even if the site is allowed on your exceptions list.</span></span>

## <a name="pex-endpoint"></a><span data-ttu-id="6236b-123">نقطة نهاية PEX</span><span class="sxs-lookup"><span data-stu-id="6236b-123">PEX Endpoint</span></span>

<span data-ttu-id="6236b-124">تتطلب Project Operations أن تشير معلمة المشروع إلى نقطة نهاية PEX.</span><span class="sxs-lookup"><span data-stu-id="6236b-124">Project Operations requires that a project parameter reference the PEX Endpoint.</span></span> <span data-ttu-id="6236b-125">تكون نقطة النهاية هذه مطلوبة للاتصال بالخدمة المستخدمة في عرض هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="6236b-125">This endpoint is required to communicate with the service used to render the work breakdown structure.</span></span> <span data-ttu-id="6236b-126">إذا لم يتم تمكين المعلمة، ستتلقى الخطأ، "معلمة المشروع غير صالحة".</span><span class="sxs-lookup"><span data-stu-id="6236b-126">If the parameter isn't enabled, you will receive the error, "The project parameter is not valid".</span></span> 

### <a name="workaround"></a><span data-ttu-id="6236b-127">الطرق البديلة</span><span class="sxs-lookup"><span data-stu-id="6236b-127">Workaround</span></span>
 ![حقل نقطة نهاية PEX في معلمة المشروع](media/projectparameter.png)

1. <span data-ttu-id="6236b-129">أضف حقل **نقطة نهاية PEX** إلى صفحة **معلمات المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6236b-129">Add the **PEX Endpoint** field to the **Project Parameters** page.</span></span>
2. <span data-ttu-id="6236b-130">قم بتحديث الحقل بالقيمة التالية: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=\<id>&type=2`</span><span class="sxs-lookup"><span data-stu-id="6236b-130">Update the field with the following value: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=\<id>&type=2`</span></span>
3. <span data-ttu-id="6236b-131">قم بإزالة الحقل من صفحة **معلمات المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6236b-131">Remove the field from the **Project Parameters** page.</span></span>

## <a name="privileges-for-project-for-the-web"></a><span data-ttu-id="6236b-132">امتيازات المشروع بالنسبة إلى الويب</span><span class="sxs-lookup"><span data-stu-id="6236b-132">Privileges for Project for the Web</span></span>

<span data-ttu-id="6236b-133">يعتمد Project Operations على خدمة جدولة خارجية.</span><span class="sxs-lookup"><span data-stu-id="6236b-133">Project Operations relies on an external scheduling service.</span></span> <span data-ttu-id="6236b-134">تتطلب الخدمة أن يكون لدى المستخدم عدة أدوار معينة للقراءة والكتابة إلى الكيانات المرتبطة بهيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="6236b-134">The service requires that a user have several roles assigned to read and write to entities related to the work breakdown structure.</span></span> <span data-ttu-id="6236b-135">وتتضمن هذه الكيانات مهام المشروع وتخصيصات الموارد وتبعيات المهام.</span><span class="sxs-lookup"><span data-stu-id="6236b-135">These entities include project tasks, resource assignments, and task dependencies.</span></span> <span data-ttu-id="6236b-136">إذا لم بإمكان المستخدم عرض هيكل تنظيم العمل عند الانتقال إلى علامة التبويب **مهام**، فمن المحتمل أن يكون ذلك بسبب عدم تمكين Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6236b-136">If a user can't render the work breakdown structure when they go to the **Tasks** tab, it's probably because Project for Project Operations hasn't been enabled.</span></span> <span data-ttu-id="6236b-137">قد يتلقى المستخدم إما خطأ دور الأمان أو خطأ مرتبط برفض الوصول.</span><span class="sxs-lookup"><span data-stu-id="6236b-137">A user might receive either a security role error, or an error related to a denial of access.</span></span>


## <a name="workaround"></a><span data-ttu-id="6236b-138">الطرق البديلة</span><span class="sxs-lookup"><span data-stu-id="6236b-138">Workaround</span></span>

1. <span data-ttu-id="6236b-139">انتقل إلى **الإعدادات > الأمان > المستخدمون > مستخدمو التطبيق**.</span><span class="sxs-lookup"><span data-stu-id="6236b-139">Go to **Setting > Security > Users > Application Users**.</span></span>  

   ![قارئ التطبيق](media/applicationuser.jpg)
   
2. <span data-ttu-id="6236b-141">انقر نقرًا مزدوجًا فوق سجل مستخدم التطبيق للتحقق مما يلي:</span><span class="sxs-lookup"><span data-stu-id="6236b-141">Double-click the application user record to verify the following:</span></span>

 - <span data-ttu-id="6236b-142">المستخدم لديه حق الوصول إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="6236b-142">The user has access to the project.</span></span> <span data-ttu-id="6236b-143">يتم إجراء هذا التحقق عادة من خلال التأكد من أن المستخدم لديه دور أمان **مدير المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6236b-143">This verification is typically done by ensuring that the user has **Project Manager** security role.</span></span>
 - <span data-ttu-id="6236b-144">مستخدم تطبيق Microsoft Project موجود وتم تكوينه بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="6236b-144">The Microsoft Project application user exists and is configured correctly.</span></span>
 
3. <span data-ttu-id="6236b-145">إذا كان هذا المستخدم غير موجود، فيمكنك إنشاء سجل مستخدم جديد.</span><span class="sxs-lookup"><span data-stu-id="6236b-145">If this user doesn't exist, you can create a new user record.</span></span> <span data-ttu-id="6236b-146">حدد **مستخدمين جدد**.</span><span class="sxs-lookup"><span data-stu-id="6236b-146">Select **New Users**.</span></span> <span data-ttu-id="6236b-147">قم بتغيير نموذج الإدخال إلى **مستخدم التطبيق**، ثم أضف **معرف التطبيق**.</span><span class="sxs-lookup"><span data-stu-id="6236b-147">Change the entry form to **Application User**, and then add the **Application ID**.</span></span>

   ![تفاصيل مستخدم التطبيق](media/applicationuserdetails.jpg)

4. <span data-ttu-id="6236b-149">تحقق من تعيين الترخيص الصحيح للمستخدم ومن أن الخدمة قد تم تمكينها في تفاصيل خطط الخدمة الخاصة بالترخيص.</span><span class="sxs-lookup"><span data-stu-id="6236b-149">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
5. <span data-ttu-id="6236b-150">تحقق من أن المستخدم يمكنه فتح project.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="6236b-150">Verify that the user can open project.microsoft.com.</span></span>
6. <span data-ttu-id="6236b-151">تحقق من خلال معلمات المشروع من أن النظام يشير إلى معلمات نقطة النهاية الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="6236b-151">Verify through the project parameters that the system is pointing to the correct project endpoint.</span></span>
7. <span data-ttu-id="6236b-152">تحقق من أنه تم إنشاء مستخدم تطبيق المشروع.</span><span class="sxs-lookup"><span data-stu-id="6236b-152">Verify that the project application user is created.</span></span>
8. <span data-ttu-id="6236b-153">قم بتطبيق أدوار الأمان التالية على المستخدم:</span><span class="sxs-lookup"><span data-stu-id="6236b-153">Apply the following security roles to the user:</span></span>

  - <span data-ttu-id="6236b-154">مستخدم Dataverse</span><span class="sxs-lookup"><span data-stu-id="6236b-154">Dataverse User</span></span>
  - <span data-ttu-id="6236b-155">نظام Project Operations</span><span class="sxs-lookup"><span data-stu-id="6236b-155">Project Operations System</span></span>
  - <span data-ttu-id="6236b-156">نظام المشروع</span><span class="sxs-lookup"><span data-stu-id="6236b-156">Project System</span></span>

## <a name="error-when-updating-the-work-breakdown-structure"></a><span data-ttu-id="6236b-157">خطأ عند تحديث هيكل تنظيم العمل</span><span class="sxs-lookup"><span data-stu-id="6236b-157">Error when updating the work breakdown structure</span></span>

<span data-ttu-id="6236b-158">عند إجراء تحديث واحد أو أكثر على هيكل تنظيم العمل، تفشل التغييرات في النهاية ولا يتم حفظها.</span><span class="sxs-lookup"><span data-stu-id="6236b-158">When one or more updates are made to the work breakdown structure, the changes eventually fail and aren't saved.</span></span> <span data-ttu-id="6236b-159">يحدث خطأ في شبكة الجدولة مع ملاحظة أنه "يتعذر حفظ التغيير الأخير الذي قمت به."</span><span class="sxs-lookup"><span data-stu-id="6236b-159">An error occurs in the schedule grid noting that “Recent change you’ve made couldn’t be saved.”</span></span>

### <a name="workaround"></a><span data-ttu-id="6236b-160">الطرق البديلة</span><span class="sxs-lookup"><span data-stu-id="6236b-160">Workaround</span></span>

1. <span data-ttu-id="6236b-161">تحقق من تعيين الترخيص الصحيح للمستخدم ومن أن الخدمة قد تم تمكينها في تفاصيل خطط الخدمة الخاصة بالترخيص.</span><span class="sxs-lookup"><span data-stu-id="6236b-161">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
2. <span data-ttu-id="6236b-162">تحقق من أن المستخدم يمكنه فتح project.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="6236b-162">Verify that the user can open project.microsoft.com.</span></span>
3. <span data-ttu-id="6236b-163">تحقق من أن النظام يشير إلى معلمات نقطة النهاية الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="6236b-163">Verify that the system is pointing to the correct project endpoint,.</span></span>
4. <span data-ttu-id="6236b-164">تحقق من أنه تم إنشاء مستخدم تطبيق المشروع.</span><span class="sxs-lookup"><span data-stu-id="6236b-164">Verify that the Project Application user has been created.</span></span>
5. <span data-ttu-id="6236b-165">قم بتطبيق أدوار الأمان التالية على المستخدم:</span><span class="sxs-lookup"><span data-stu-id="6236b-165">Apply the following security roles to the user:</span></span>
  
  - <span data-ttu-id="6236b-166">مستخدم Dataverse أو مستخدم أساسي</span><span class="sxs-lookup"><span data-stu-id="6236b-166">Dataverse user or Base user</span></span>
  - <span data-ttu-id="6236b-167">نظام Project Operations</span><span class="sxs-lookup"><span data-stu-id="6236b-167">Project Operations System</span></span>
  - <span data-ttu-id="6236b-168">نظام المشروع</span><span class="sxs-lookup"><span data-stu-id="6236b-168">Project System</span></span>
  - <span data-ttu-id="6236b-169">نظام الكتابة المزدوج في Project Operations (يكون هذا الدور مطلوبا إذا كنت تقوم بنشر السيناريو المستند إلى الموارد/المنتجات غير المخزنة لـ Project Operations).</span><span class="sxs-lookup"><span data-stu-id="6236b-169">Project Operations Dual Write System (This role is required if you are deploying the resource/non-stocked based scenario of Project Operations.)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]