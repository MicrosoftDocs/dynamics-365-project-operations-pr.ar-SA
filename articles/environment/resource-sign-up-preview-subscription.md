---
title: إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة
description: يوفر هذا الموضوع معلومات حول كيفية الاشتراك في Project Operations ونشرها للسيناريوهات المستندة إلى المورد/المنتجات غير المخزنة.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: da93fcf23ee3f255812842e31cb22b5d39daa963
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334811"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="6f74c-103">إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة</span><span class="sxs-lookup"><span data-stu-id="6f74c-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="6f74c-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="6f74c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="6f74c-105">يوضح هذا الموضوع كيفية الاشتراك في العرض التجريبي ونشر بيئة Project Operations للسيناريوهات المستندة إلى الموارد/المنتجات غير المخزنة.</span><span class="sxs-lookup"><span data-stu-id="6f74c-105">This topic explains how to subscribe to the trial offer and deploy Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f74c-106">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="6f74c-106">Prerequisites</span></span>
- <span data-ttu-id="6f74c-107">يجب أن يكون لدي المستخدم الذي ينشر المعاينة حقوق المسؤول العمومي لمستأجر Azure.</span><span class="sxs-lookup"><span data-stu-id="6f74c-107">The user who deploys the preview must have Azure tenant global administrator rights.</span></span> <span data-ttu-id="6f74c-108">يمكنك إنشاء مستأجر أثناء عملية استرداد العرض الأول.</span><span class="sxs-lookup"><span data-stu-id="6f74c-108">You can create a tenant during the first offer redemption.</span></span> 
- <span data-ttu-id="6f74c-109">يتطلب نشر بيئة Finance وجود اشتراك Azure صالح والذي ستتم فوترته لكل بيئة.</span><span class="sxs-lookup"><span data-stu-id="6f74c-109">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="6f74c-110">يمكنك استخدام الاشتراك الموجود في المؤسسات أو استخدام [الإصدار التجريبي من Azure](https://azure.microsoft.com/en-us/free/) لبدء العمل.</span><span class="sxs-lookup"><span data-stu-id="6f74c-110">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="6f74c-111">سيتم توفير بيئة CDS مجانًا لفترة زمنية محددة بمدة 30 يومًا.</span><span class="sxs-lookup"><span data-stu-id="6f74c-111">The CDS environment will be provided free for a limited 30 day period.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6f74c-112">شخص واحد فقط، مسؤول المستأجر، في مؤسسة تحتاج إلى تنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="6f74c-112">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="6f74c-113">إذا لم تكن أنت المشترك في هذا الإصدار، فانتظر حتى يتم تسجيل مؤسستك وتستلم بيانات اعتماد المستخدم الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="6f74c-113">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>
> 
> <span data-ttu-id="6f74c-114">تستخدم الإصدارات التجريبية مرة واحدة في المستأجر.</span><span class="sxs-lookup"><span data-stu-id="6f74c-114">Trials are single use in the tenant.</span></span> <span data-ttu-id="6f74c-115">يمكنك تشغيل النسخة التجريبية مرة واحدة فقط.</span><span class="sxs-lookup"><span data-stu-id="6f74c-115">You can only run a trial one time.</span></span> <span data-ttu-id="6f74c-116">من المستحسن إنشاء مستأجر جديد لغرض الإصدار التجريبي.</span><span class="sxs-lookup"><span data-stu-id="6f74c-116">We recommend that you create a new tenant for the purpose of the trial.</span></span>


### <a name="dynamics-365-project-operations-ce---preview-trial"></a><span data-ttu-id="6f74c-117">Dynamics 365 Project Operations(CE) - معاينة الإصدار التجريبي</span><span class="sxs-lookup"><span data-stu-id="6f74c-117">Dynamics 365 Project Operations (CE) - Preview Trial</span></span> 

<span data-ttu-id="6f74c-118">قبل البدء، تأكد من تسجيل الدخول إلى مستعرض باستخدام حساب عمل المستخدم في المستأجر حيث تريد معاينة Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6f74c-118">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="6f74c-119">استرداد رمز العرض الأول، **Dynamics 365 Project Operations**، هنا [الإصدار التجريبي لـ Project Operations](https://aka.ms/try-po).</span><span class="sxs-lookup"><span data-stu-id="6f74c-119">Redeem the first offer code, **Dynamics 365 Project Operations** here [Project Operations Trial](https://aka.ms/try-po).</span></span>
2. <span data-ttu-id="6f74c-120">أكد طلبك.</span><span class="sxs-lookup"><span data-stu-id="6f74c-120">Confirm your order.</span></span>

  <span data-ttu-id="6f74c-121">سترى أنه تم استرجاع عرض التأكيد بنجاح.</span><span class="sxs-lookup"><span data-stu-id="6f74c-121">You will see confirmation offer was successfully redeemed.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="6f74c-122">إصدار تجريبي لمعاينة Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="6f74c-122">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="6f74c-123">انتقل إلى [الإصدار التجريبي من Dynamics 365 for Finance Preview](https://aka.ms/trypoche) وكرر الخطوات من القسم السابق مع العرض، قم بالتسجيل في البيئة المستضافة على السحابة.</span><span class="sxs-lookup"><span data-stu-id="6f74c-123">Go to [Dynamics 365 for Finance Preview Trial](https://aka.ms/trypoche) and repeat the steps from the previous section with the offer, Sign up for the Cloud Hosted Environment.</span></span>  

## <a name="assign-licenses"></a><span data-ttu-id="6f74c-124">تعيين التراخيص</span><span class="sxs-lookup"><span data-stu-id="6f74c-124">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6f74c-125">ستحتاج إلى حق وصول إداري إلى مدخل Microsoft 365 الخاص بمؤسستك لإكمال الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="6f74c-125">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="6f74c-126">انتقل إلى [مركز إدارة](https://portal.office.com/) لتعيين التراخيص إلى المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="6f74c-126">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

2. <span data-ttu-id="6f74c-127">في صفحة **المستخدمين النشطين**، حدد المستخدمين الذين ترغب في تعيين ترخيص لهم.</span><span class="sxs-lookup"><span data-stu-id="6f74c-127">On the **Active users** page, select the users that you want to assign a license to.</span></span>

3. <span data-ttu-id="6f74c-128">تحقق من أنه تم تحديد ترخيص **Dynamics 365 Project Operations** وحدد **حفظ التغييرات**.</span><span class="sxs-lookup"><span data-stu-id="6f74c-128">Verify that the **Dynamics 365 Project Operations** license has been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="6f74c-129">لا يلزم تعيين مستخدم إلى عرض الإصدار التجريبي من Finance.</span><span class="sxs-lookup"><span data-stu-id="6f74c-129">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="6f74c-130">بدء مشروع جديد في LCS</span><span class="sxs-lookup"><span data-stu-id="6f74c-130">Start a new project in LCS</span></span>

<span data-ttu-id="6f74c-131">قم بإنشاء مشروع LCS جديد كما هو موضح في موضوع، [بدء مشروع جديد في LCS](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="6f74c-131">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="6f74c-132">إضافة اشتراك Azure إلى مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="6f74c-132">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="6f74c-133">لإكمال هذه المهمة، اتبع الخطوات الواردة في الموضوع، [إضافة اشتراك Azure إلى مشروع LCS](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="6f74c-133">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="6f74c-134">نشر بيئة عرض توضيحي من Finance مع Project Operations لسيناريوهات المورد/المنتجات غير المخزنة</span><span class="sxs-lookup"><span data-stu-id="6f74c-134">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="6f74c-135">اتبع الإرشادات الموضحة في موضوع، [توفير بيئة جديدة](resource-provision-new-environment.md) لإكمال النشر.</span><span class="sxs-lookup"><span data-stu-id="6f74c-135">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="6f74c-136">استخدم نوع نشر [بيئة العرض التوضيحي](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) للمعاينة.</span><span class="sxs-lookup"><span data-stu-id="6f74c-136">Use the [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="6f74c-137">تثبيت إعداد CDS وبيانات التكوين</span><span class="sxs-lookup"><span data-stu-id="6f74c-137">Install CDS setup and configuration data</span></span>

<span data-ttu-id="6f74c-138">قم بتثبيت إعداد CDS وبيانات التكوين كما هو موضح في الموضوع، [إعداد بيانات التكوين وتطبيقها في Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="6f74c-138">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="6f74c-139">أكمل هذه الخطوة فقط بعد نشر بيئة العرض التوضيحي لـ Finance وسوف تكون بيانات العرض التوضيحي جاهزة.</span><span class="sxs-lookup"><span data-stu-id="6f74c-139">Complete this step only after Finance demo environment is deployed and demo data is ready.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
