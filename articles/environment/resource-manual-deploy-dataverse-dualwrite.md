---
title: نشر تطبيق Project Operations Dataverse يدويًا مع دعم الكتابة المزدوجة
description: يوضح هذا الموضوع كيفية نشر تطبيق Project Operations Dataverse يدويًا بحيث يدعم الكتابة المزدوجة.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2ad147da542fc9e7a2705da7a834d1a6512907e5
ms.sourcegitcommit: 205a94ab4168de25b102f31d00a691c8205ba63e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/18/2021
ms.locfileid: "6273992"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a><span data-ttu-id="b7400-103">نشر تطبيق Project Operations Dataverse يدويًا مع دعم الكتابة المزدوجة</span><span class="sxs-lookup"><span data-stu-id="b7400-103">Manually deploy the Project Operations Dataverse app with dual-write support</span></span>

<span data-ttu-id="b7400-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="b7400-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b7400-105">يوضح هذا الموضوع كيفية نشر Microsoft Dynamics 365 Project Operations يدويًا في Microsoft Dataverse بحيث يدعم الكتابة المزدوجة.</span><span class="sxs-lookup"><span data-stu-id="b7400-105">This topic explains how to manually deploy Microsoft Dynamics 365 Project Operations in Microsoft Dataverse so that it supports dual-write.</span></span> <span data-ttu-id="b7400-106">تكتشف Project Operations تكوين البيئة وتضيف دعمًا إضافيًا للكتابة المزدوجة إذا تم استيفاء المتطلبات الأساسية.</span><span class="sxs-lookup"><span data-stu-id="b7400-106">Project Operations detects the environment's configuration and adds additional support for dual-write if the prerequisites are met.</span></span>

<span data-ttu-id="b7400-107">أثناء النشر من خلال Microsoft Dynamics Lifecycle Services (LCS)، إذا اتبعت الإرشادات الواردة في هذا الموضوع، فيمكنك تخطي نشر تكامل Microsoft Power Platform (المعروف سابقًا باسم بيئة Common Data Service).</span><span class="sxs-lookup"><span data-stu-id="b7400-107">During deployment through Microsoft Dynamics Lifecycle Services (LCS), if you've followed the instructions in this topic, you can skip the deployment of the Microsoft Power Platform integration (previously known as the Common Data Service environment).</span></span>

<span data-ttu-id="b7400-108">عملية نشر Project Operations في Dataverse بحيث تدعم الكتابة المزدوجة‬ ويكون لها أربع خطوات رئيسية:</span><span class="sxs-lookup"><span data-stu-id="b7400-108">The process of deploying Project Operations in Dataverse so that it supports dual-write has four main steps:</span></span>

1. <span data-ttu-id="b7400-109">[إنشاء بيئة جديدة في Dataverse تدعم الكتابة المزدوجة](#create).</span><span class="sxs-lookup"><span data-stu-id="b7400-109">[Create a new environment in Dataverse that supports dual-write](#create).</span></span>
2. <span data-ttu-id="b7400-110">[إضافة المتطلبات المسبقة للكتابة المزدوجة إلى البيئة](#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="b7400-110">[Add dual-write prerequisites to the environment](#prerequisites).</span></span>
3. <span data-ttu-id="b7400-111">[أضف تطبيق Project Operations Dataverse ](#dataverse).</span><span class="sxs-lookup"><span data-stu-id="b7400-111">[Add the Project Operations Dataverse app](#dataverse).</span></span>
4. <span data-ttu-id="b7400-112">[ربط بيئتك](#link).</span><span class="sxs-lookup"><span data-stu-id="b7400-112">[Link your environments](#link).</span></span>

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a><span data-ttu-id="b7400-113">إنشاء بيئة جديدة في Dataverse تدعم الكتابة المزدوجة</span><span class="sxs-lookup"><span data-stu-id="b7400-113">Create a new environment in Dataverse that supports dual-write</span></span>

<span data-ttu-id="b7400-114">لإكمال هذا الإجراء، يتعين عليك تسجيل الدخول كمسؤول.</span><span class="sxs-lookup"><span data-stu-id="b7400-114">To complete this procedure, you must sign in as an administrator.</span></span>

1. <span data-ttu-id="b7400-115">افتح مركز الإدارة [Power Platform ](https://admin.powerplatform.com)، ثم قم بتسجيل الدخول كمسؤول.</span><span class="sxs-lookup"><span data-stu-id="b7400-115">Open the [Power Platform admin center](https://admin.powerplatform.com), and sign in as an administrator.</span></span>
2. <span data-ttu-id="b7400-116">إنشاء بيئة جديدة، وتسميتها.</span><span class="sxs-lookup"><span data-stu-id="b7400-116">Create a new environment, and name it.</span></span>
3. <span data-ttu-id="b7400-117">حدد نوع البيئة.</span><span class="sxs-lookup"><span data-stu-id="b7400-117">Select the environment type.</span></span> <span data-ttu-id="b7400-118">إذا قمت بالاشتراك في العرض التجريبي، فحدد **"تجريبي" (مستند إلى الاشتراك)**.</span><span class="sxs-lookup"><span data-stu-id="b7400-118">If you signed up for the trial offer, select **Trial (subscription-based)**.</span></span>
4. <span data-ttu-id="b7400-119">تأكيد منطقة النشر.</span><span class="sxs-lookup"><span data-stu-id="b7400-119">Confirm the deployment region.</span></span>
5. <span data-ttu-id="b7400-120">تمكين خيار **إنشاء قاعدة بيانات لهذه البيئة**.</span><span class="sxs-lookup"><span data-stu-id="b7400-120">Enable the **Create a database for this environment** option.</span></span> 
6. <span data-ttu-id="b7400-121">تأكد من اللغة، ثم تأكد من تطابق العملة مع العملة الخاصة بتطبيقات Finance and Operations الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="b7400-121">Confirm the language, and then confirm that the currency matches the currency for your Finance and Operations apps.</span></span>
7. <span data-ttu-id="b7400-122">تمكين الخيار **تطبيقات Dynamics 365** وتأكد من تعيين الحقل **النشر التلقائي لهذه التطبيقات** على **بلا**.</span><span class="sxs-lookup"><span data-stu-id="b7400-122">Enable the **Dynamics 365 apps** option, and confirm that the **Automatically deploy these apps** field is set to **None**.</span></span>
8. <span data-ttu-id="b7400-123">قم بإضافة مجموعة أمان، إذا كانت مجموعة الأمان مطلوبة.</span><span class="sxs-lookup"><span data-stu-id="b7400-123">Add a security group, if a security group is required.</span></span>
9. <span data-ttu-id="b7400-124">حدد **حفظ** لإنشاء البيئة.</span><span class="sxs-lookup"><span data-stu-id="b7400-124">Select **Save** to create the environment.</span></span>
10. <span data-ttu-id="b7400-125">انتظر حتى تكتمل عملية النشر حتى تصل البيئة إلى حالة **الجاهزية**.</span><span class="sxs-lookup"><span data-stu-id="b7400-125">Wait until the deployment is completed and the environment reaches the **Ready** state.</span></span>

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a><span data-ttu-id="b7400-126">إضافة المتطلبات المسبقة للكتابة المزدوجة إلى البيئة</span><span class="sxs-lookup"><span data-stu-id="b7400-126">Add dual-write prerequisites to the environment</span></span>

<span data-ttu-id="b7400-127">يتضمن دعم الكتابة المزدوجة الحقول الإضافية التي تمت إضافتها إلى الكيانات الرئيسية، مثل كيان **الشركة**.</span><span class="sxs-lookup"><span data-stu-id="b7400-127">Dual-write support includes additional fields that are added to key entities, such as the **Company** entity.</span></span> <span data-ttu-id="b7400-128">إذا كنت تقوم بإضافة دعم الكتابة المزدوجة إلى بيئة موجودة، فقد تضطر إلى تحديث البيانات لتمكين الدعم.</span><span class="sxs-lookup"><span data-stu-id="b7400-128">If you're adding dual-write support to an existing environment, you might have to update the data to enable the support.</span></span> <span data-ttu-id="b7400-129">لمزيد من المعلومات حول كيفية تمهيد البيانات، راجع [تمهيد بيانات شركة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data)</span><span class="sxs-lookup"><span data-stu-id="b7400-129">For information about how to bootstrap the data, see [Bootstrap company data](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span></span> <span data-ttu-id="b7400-130">لمزيد من المعلومات حول الكتابة المزدوجة، راجع [متطلبات نظام الكتابة المزدوجة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req)</span><span class="sxs-lookup"><span data-stu-id="b7400-130">For more information about dual-write, see [Dual-write system requirements](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span></span>

<span data-ttu-id="b7400-131">أكمل هذا الإجراء لإضافة متطلبات الكتابة المزدوجة إلى بيئتك.</span><span class="sxs-lookup"><span data-stu-id="b7400-131">Complete this procedure to add the dual-write prerequisites to your environment.</span></span>

1. <span data-ttu-id="b7400-132">افتح البيئة التي أنشأتها للتو، ثم انتقل إلى **مورد** \> **تطبيقات Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="b7400-132">Open the environment that you just created, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="b7400-133">حدد **الحل الأساسي للكتابة المزدوجة** في قائمة التطبيق، ثم قم بتثبيته.</span><span class="sxs-lookup"><span data-stu-id="b7400-133">Select **Dual-write core solution** in the app list, and install it.</span></span>
3. <span data-ttu-id="b7400-134">انتظر حتى تكتمل عملية التثبيت.</span><span class="sxs-lookup"><span data-stu-id="b7400-134">Wait until the installation is completed.</span></span> <span data-ttu-id="b7400-135">ثم حدد **حل تزامن تطبيق الكتابة المزدوجة** في قائمة التطبيقات، وقم بتثبيته.</span><span class="sxs-lookup"><span data-stu-id="b7400-135">Then select **Dual-write application orchestration solution** in the app list, and install it.</span></span>

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a><span data-ttu-id="b7400-136">إضافة تطبيق Project Operations Dataverse.</span><span class="sxs-lookup"><span data-stu-id="b7400-136">Add the Project Operations Dataverse app</span></span>

<span data-ttu-id="b7400-137">لا يمكنك إكمال هذا الإجراء إلا إذا أكملت الإجراءات السابقة قبل تثبيت Project Operations.</span><span class="sxs-lookup"><span data-stu-id="b7400-137">You can complete this procedure only if you completed the previous procedures before you installed Project Operations.</span></span> <span data-ttu-id="b7400-138">أثناء التثبيت، يقوم النظام بتحليل تكوين البيئة وإضافة دعم للكتابة المزدوجة في حالة الحاجة إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="b7400-138">During installation, the system analyzes the environment configuration and adds support for dual-write if it's required.</span></span>

1. <span data-ttu-id="b7400-139">افتح البيئة التي أنشأتها سابقًا، ثم انتقل إلى **مورد** \> **تطبيقات Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="b7400-139">Open the environment that you created earlier, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="b7400-140">حدد **Microsoft Dynamics 365 Project Operations** في قائمة التطبيق، ثم قم بتثبيتها.</span><span class="sxs-lookup"><span data-stu-id="b7400-140">Select **Microsoft Dynamics 365 Project Operations** in the app list, and install it.</span></span>

## <a name="link-your-environments"></a><a name="link"></a><span data-ttu-id="b7400-141">ربط بيئاتك</span><span class="sxs-lookup"><span data-stu-id="b7400-141">Link your environments</span></span>

<span data-ttu-id="b7400-142">بعد نشر بيئة Dataverse، يمكنك إعداد الارتباط في تطبيقات Finance and Operations الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="b7400-142">After the Dataverse environment is deployed, you can set up the link in your Finance and Operations apps.</span></span> <span data-ttu-id="b7400-143">اتبع الخطوات المتبعة في [استخدام معالج الكتابة المزدوجة لربط بيئاتك](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span><span class="sxs-lookup"><span data-stu-id="b7400-143">Follow the steps in [Use the dual-write wizard to link your environments](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span></span>
