---
title: الصفحة الرئيسية للترقية
description: يوضح هذا الموضوع مكان البحث عن معلومات هامة حول الميزات الجديدة والمتغيرة في Dynamics 365 Project Service Automation، وعملية الترقية إلى الإصدار الأحدث.
ms.prod: ''
ms.custom:
- dyn365-projectservice
ms.date: 05/30/2019
ms.topic: article
author: rumant
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: a2e17fbdfb71eb62053236bf6c8a3d1aedf332df
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012345"
---
# <a name="upgrade-home-page"></a><span data-ttu-id="76659-103">الصفحة الرئيسية للترقية</span><span class="sxs-lookup"><span data-stu-id="76659-103">Upgrade home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a><span data-ttu-id="76659-104">الترقية من الإصدار 2.x أو 1.x من PSA إلى الإصدار 3.x</span><span class="sxs-lookup"><span data-stu-id="76659-104">Upgrade from PSA version 2.x or 1.x to version 3.x</span></span>

### <a name="new-instances"></a><span data-ttu-id="76659-105">المثيلات الجديدة</span><span class="sxs-lookup"><span data-stu-id="76659-105">New instances</span></span>

<span data-ttu-id="76659-106">اعتبارًا من 17 مايو 2019، عند تحديد Project Service Automation أثناء توفير مثيل جديد، يتم تثبيت الإصدار رقم 3.x بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="76659-106">As of May 17, 2019, when Project Service Automation is selected during the provisioning of a new instance, version 3.x is installed by default.</span></span>

### <a name="existing-instances"></a><span data-ttu-id="76659-107">المثيلات الموجودة</span><span class="sxs-lookup"><span data-stu-id="76659-107">Existing instances</span></span>

<span data-ttu-id="76659-108">في السابق، كان يجب على العملاء الذين لديهم مثيل لـ PSA الإصدار 2.x والذين يحتاجون إلى الترقية إلى الإصدار 3.x، وهو إصدار واجهة العميل الموحدة (UCI) من PSA، الاتصال بدعم Microsoft وتقديم التفاصيل مثيلهم لكي يتمكن الدعم من تمكين المثيل للترقية إلى الإصدار 3.x.</span><span class="sxs-lookup"><span data-stu-id="76659-108">Previously, customers who have an instance of PSA version 2.x and needed to upgrade to version 3.x, which is the Unified client interface-based (UCI) version of PSA, had to contact Microsoft Support and provide the details of their instance so that support could enable the instance for upgrade to version 3.x.</span></span> <span data-ttu-id="76659-109">اعتبارًا من 1 مارس 2020، سيتمكن العملاء الذين لديهم مثيل من إصدار PSA 2.x ويحتاجون إلى الترقية إلى الإصدار 3.x، من ترقية مثيلاتهم مباشرة من مدخل المسؤول دون الحاجة إلى الاتصال بدعم Microsoft.</span><span class="sxs-lookup"><span data-stu-id="76659-109">As of March 1, 2020, customers who have an instance of PSA version 2.x and need to upgrade to version 3.x, will able to upgrade their instances directly from the Admin portal without having to contact Microsoft Support.</span></span>  

> [!NOTE]
> <span data-ttu-id="76659-110">يشتمل الإصدار 3.x من PSA على تغييرات مهمة.</span><span class="sxs-lookup"><span data-stu-id="76659-110">PSA version 3.x includes significant changes.</span></span> <span data-ttu-id="76659-111">لقد تم إنشاؤها في إظار الواجهة الموحدة للمساعدة في توفير تجربة محسنه للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="76659-111">It has been built on the Unified Interface framework to help provide an improved user experience.</span></span> <span data-ttu-id="76659-112">يقدم التطبيق المعاد تصميمه واجهة مستخدم منتظمة ومتناسقة (UI)، كما أنه يتبع مبادئ التصميم التفاعلية للعرض الأمثل على أي حجم شاشة أو جهاز.</span><span class="sxs-lookup"><span data-stu-id="76659-112">The redesigned app delivers a consistent, uniform user interface (UI), and it follows responsive design principles for optimal viewing on any screen size or device.</span></span> <span data-ttu-id="76659-113">قد تم إجراء تغييرات أخرى خلال التطبيق.</span><span class="sxs-lookup"><span data-stu-id="76659-113">There have been other changes throughout the application.</span></span> <span data-ttu-id="76659-114">تتضمن بعض المناطق التي تم تغييرها الأسعار وحجز الموارد وتعيينها والوقت والمصروفات والموافقات.</span><span class="sxs-lookup"><span data-stu-id="76659-114">Some of the areas that have been changed include pricing, booking and assigning resources, time, expenses, and approvals.</span></span>

<span data-ttu-id="76659-115">قبل أن تبدأ عملية الترقية، نوصي بإكمال المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="76659-115">Before you begin the upgrade process, we recommend that you complete the following tasks:</span></span>

- <span data-ttu-id="76659-116">تحقق مما إذا كان تم تثبيت Dynamics 365 Field Service وProject Service Automation على المثيل المحدد.</span><span class="sxs-lookup"><span data-stu-id="76659-116">Verify whether both Dynamics 365 Field Service and Project Service Automation are installed on the identified instance.</span></span> <span data-ttu-id="76659-117">إذا تم تثبيت كلا الحلين ، يجب أن تخطط للترقية قبل أن تستأنف الاستخدام المنتظم للمثيل.</span><span class="sxs-lookup"><span data-stu-id="76659-117">If both solutions are installed, you should plan to upgrade both before you resume regular use of the instance.</span></span>
- <span data-ttu-id="76659-118">راجع الموضوعات التالية بعناية.</span><span class="sxs-lookup"><span data-stu-id="76659-118">Carefully review the following topics.</span></span> <span data-ttu-id="76659-119">سيساعدك الوعي وفهم التغييرات بين الإصدارات في عملية الترقية.</span><span class="sxs-lookup"><span data-stu-id="76659-119">Awareness and understanding of the changes between versions will help you with the upgrade process.</span></span> <span data-ttu-id="76659-120">توفر هذه المواضيع معلومات حول التغييرات الرئيسية في PSA، مع اعتبارات وتوصيات للتخطيط للترقية إلى الإصدار 3.x.</span><span class="sxs-lookup"><span data-stu-id="76659-120">These topics provide information about the major changes in PSA, together with considerations and recommendations for planning your upgrade to version 3.x.</span></span>

    - [<span data-ttu-id="76659-121">الجديد أو المتغير في الإصدار 3 من Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="76659-121">What's new or changed in Project Service Automation version 3</span></span>](whats-new-changed-v3.md)
    - [<span data-ttu-id="76659-122">اعتبارات الترقية - الإصدار 2.x أو 1.x من Project Service Automation إلى الإصدار 3.x</span><span class="sxs-lookup"><span data-stu-id="76659-122">Upgrade considerations - Project Service Automation version 2.x or 1.x to version 3</span></span>](upgrade-v3.md)

- <span data-ttu-id="76659-123">قم بترقية مثيل آلية تحديد الوصول لتقييم التغييرات في تنفيذك قبل أن تقوم بترقية مثيل الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="76659-123">Upgrade your sandbox instance to evaluate the changes in your implementation before you upgrade your production instance.</span></span>

<span data-ttu-id="76659-124">بعد الانتهاء من مراجعة المواضيع التي تمت الاشارة إليها مسبقا والاستعداد للترقية إلى الإصدار رقم 3 من PSA أو الإصدار المستند إلى UCI، قم بإرسال طلب إلى دعم Microsoft لتوفير الترقية من مركز الإدارة.</span><span class="sxs-lookup"><span data-stu-id="76659-124">After you've reviewed the topics that were mentioned earlier and are ready to upgrade to PSA version 3.x or the UCI-based version, submit a request to Microsoft support to make the upgrade available from Admin center.</span></span> <span data-ttu-id="76659-125">في طلبك، قم بتوفير تفاصيل المثيل الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="76659-125">In your request, provide the details of your instance.</span></span>

## <a name="older-versions-of-psa-psa-version-2x-in-a-newly-created-instance"></a><span data-ttu-id="76659-126">الإصدارات القديمة من PSA (الإصدار 2.x من PSA) في مثيل تم إنشاؤه حديثًا</span><span class="sxs-lookup"><span data-stu-id="76659-126">Older versions of PSA (PSA version 2.x) in a newly created instance</span></span>

<span data-ttu-id="76659-127">اعتبارًا من 17 مايو 2019، سيكون لكافة المثيلات الجديدة UCI بمثابة العميل الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="76659-127">As of May 17, 2019, all new instances will have UCI as the default client.</span></span> <span data-ttu-id="76659-128">للمواءمة مع هذا التغيير، سيتم توفير إصدار 3.x من PSA والإصدار 8.x من Field Service بشكل افتراضي، لأن هذه الإصدارات مصممة للعمل مع عميل UCI.</span><span class="sxs-lookup"><span data-stu-id="76659-128">For alignment with this change, PSA version 3.x and Field Service version 8.x will be provisioned by default, because these versions are designed to work with the UCI client.</span></span>

<span data-ttu-id="76659-129">بدءًا من 1 مارس 2020، لن يتمكن عملاء Dynamics PSA من إنشاء بيئة جديدة باستخدام الإصدارات القديمة من PSA، على سبيل المثال إصدار PSA 2.x أو أقل.</span><span class="sxs-lookup"><span data-stu-id="76659-129">Starting March 1, 2020, customers of Dynamics PSA will no longer be able to create a new environment with older versions of PSA, for example PSA version 2.x or lower.</span></span> <span data-ttu-id="76659-130">لإنشاء بيئة جديدة، يجب استخدام الإصدار 3.x من PSA.</span><span class="sxs-lookup"><span data-stu-id="76659-130">Any new environment will be to get only version 3.x of PSA.</span></span>

> [!NOTE]
> <span data-ttu-id="76659-131">للحصول على أفضل تجربه عند استخدام الإصدارات القديمة من تطبيقي Field Service وPSA، انتقل إلى صفحة **إعدادات النظام** وبالنسبة للحقل، حقل **استخدام الواجهة الموحدة الجديدة فقط (موصى به)**، حدد **لا** نظرًا لأن هذه الإصدارات لم يتم تصميمها ليتم تحميلها بشكل صحيح في UCI.</span><span class="sxs-lookup"><span data-stu-id="76659-131">For the best experience when you use older versions of the Field Service and PSA applications, go to the **System settings** page and for the field, **Use the new Unified Interface only (recommended)** field, select **No** as these versions aren't designed to be correctly loaded in UCI.</span></span> <span data-ttu-id="76659-132">بعد أن تقوم بإيقاف تشغيل UCI، يمكنك فتح وتشغيل هذه الإصدارات من Field Service وPSA باستخدام عميل الويب القديم.</span><span class="sxs-lookup"><span data-stu-id="76659-132">After you have turned off UCI, you can open and run these versions of Field Service and PSA by using the old web client.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]