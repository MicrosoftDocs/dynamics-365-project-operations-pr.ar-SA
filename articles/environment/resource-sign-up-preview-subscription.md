---
title: إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة
description: يوفر هذا الموضوع معلومات حول كيفية الاشتراك في Project Operations ونشرها للسيناريوهات المستندة إلى المورد/المنتجات غير المخزنة.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4d35a8bf9e8a841b45808b26ae2587c5b7d99d72
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948722"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="bd3b2-103">إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة</span><span class="sxs-lookup"><span data-stu-id="bd3b2-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="bd3b2-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="bd3b2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="bd3b2-105">يشرح هذا الموضوع كيفية الاشتراك في المعاينة/عرض الشريك ونشر بيئة Project Operations للسيناريوهات المستندة إلى مورد/منتجات غير مخزنة.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-105">This topic explains how to subscribe to the preview/partner offer and deploy Project Operations environment for resource/ non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd3b2-106">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="bd3b2-106">Prerequisites</span></span>

- <span data-ttu-id="bd3b2-107">ستتلقى رسالة بريد إلكتروني لدعوتك للمشاركة في المعاينة.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-107">You will receive an email inviting you to participate in the preview.</span></span> <span data-ttu-id="bd3b2-108">يمكنك طلب معاينة من [موقع الويب الخاص بـ Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span><span class="sxs-lookup"><span data-stu-id="bd3b2-108">You can request a preview on the [Project Operations website](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span></span>
- <span data-ttu-id="bd3b2-109">يجب أن يكون لدي المستخدم الذي ينشر المعاينة حقوق المسؤول العمومي لمستأجر Azure.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-109">The user who deploys the preview must have Azure tenant global administrator rights.</span></span>
- <span data-ttu-id="bd3b2-110">يتطلب نشر بيئة Finance وجود اشتراك Azure صالح والذي ستتم فوترته لكل بيئة.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-110">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="bd3b2-111">يمكنك استخدام الاشتراك الموجود في المؤسسات أو استخدام [الإصدار التجريبي من Azure](https://azure.microsoft.com/en-us/free/) لبدء العمل.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-111">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="bd3b2-112">سيتم توفير بيئة CDS مجانًا لفترة زمنية محددة بمدة 30 يومًا.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-112">The CDS environment will be provided free for a limited 30 day period.</span></span>

## <a name="subscribe"></a><span data-ttu-id="bd3b2-113">الاشتراك</span><span class="sxs-lookup"><span data-stu-id="bd3b2-113">Subscribe</span></span>

<span data-ttu-id="bd3b2-114">عند اعتماد [طلب المعاينة](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) الخاص بك، ستتلقى عرضين من Microsoft بواسطة البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-114">When your [preview request](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) is approved, you will receive two offers from Microsoft by email.</span></span> <span data-ttu-id="bd3b2-115">تسمح لك هذه العروض بنشر معاينة Project Operations:</span><span class="sxs-lookup"><span data-stu-id="bd3b2-115">These offers allow you to deploy the Project Operations Preview:</span></span>

- <span data-ttu-id="bd3b2-116">Dynamics 365 Project Operations – إصدار تجريبي للمعاينة</span><span class="sxs-lookup"><span data-stu-id="bd3b2-116">Dynamics 365 Project Operations – Preview Trial</span></span>
- <span data-ttu-id="bd3b2-117">إصدار تجريبي لمعاينة Dynamics 365 for Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-117">Dynamics 365 for Finance and Operations Preview Trial.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bd3b2-118">شخص واحد فقط، مسؤول المستأجر، في مؤسسة تحتاج إلى تنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-118">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="bd3b2-119">إذا لم تكن أنت المشترك في هذا الإصدار، فانتظر حتى يتم تسجيل مؤسستك وتستلم بيانات اعتماد المستخدم الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-119">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>

### <a name="dynamics-365-project-operations--preview-trial"></a><span data-ttu-id="bd3b2-120">Dynamics 365 Project Operations – إصدار تجريبي للمعاينة</span><span class="sxs-lookup"><span data-stu-id="bd3b2-120">Dynamics 365 Project Operations – Preview trial</span></span>

1. <span data-ttu-id="bd3b2-121">استرد العرض الأول، **الإصدار التجريبي من Dynamics 365 Project Operations** باستخدام عنوان URL المضمن في البريد الإلكتروني الترحيبي.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-121">Redeem the first offer, **Dynamics 365 Project Operations Trial**, with the URL provided in your welcome email.</span></span>

![العرض الأول](./media/1FirstOffer.png)

2. <span data-ttu-id="bd3b2-123">تحقق من أنك قمت بتسجيل الدخول باسم المستخدم الذي ينتمي إلى المؤسسة التي ستقوم بالاشتراك في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-123">Verify that you are logged in as the user who belongs to the organization who will be subscribing to the service.</span></span>
3. <span data-ttu-id="bd3b2-124">تابع عملية استرداد العرض.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-124">Proceed with redeeming the offer.</span></span> 
4. <span data-ttu-id="bd3b2-125">حدد **نعم، أضفه إلى حسابي**.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-125">Select **Yes, add it to my account**.</span></span>

![استرداد العرض](./media/2RedeemFirstOffer.png)

![تأكيد العرض](./media/3ConfirmFirstOffer.png)

![تم استرداد العرض](./media/4OfferSuccessfulyRedeemed.png)

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="bd3b2-129">إصدار تجريبي لمعاينة Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="bd3b2-129">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="bd3b2-130">كرر نفس الخطوات مع العرض الثاني من البريد الإلكتروني الترحيبي.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-130">Repeat the same steps with the second offer from the Welcome email.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="bd3b2-131">تعيين التراخيص</span><span class="sxs-lookup"><span data-stu-id="bd3b2-131">Assign Licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bd3b2-132">ستحتاج إلى حق وصول إداري إلى مدخل Office 365 الخاص بمؤسستك لإكمال الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-132">You will need administrative access to your organization's Office 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="bd3b2-133">انتقل إلى [مركز إدارة Microsoft 365](https://portal.office.com/) لتعيين التراخيص إلى المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-133">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign licenses to your users.</span></span>

![مدخل مسؤول Office](./media/5OfficeAdminPortal.png)

2. <span data-ttu-id="bd3b2-135">في صفحة **المستخدمين النشطين**، حدد المستخدمين الذين ترغب في تعيين ترخيص لهم.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-135">On the **Active users** page, select the users that you want to assign a license to.</span></span>

![تعيين التراخيص](./media/6AssignLicenses.png)

3. <span data-ttu-id="bd3b2-137">تحقق من تحديد ترخيص Project Operations وحدد **حفظ التغييرات**.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-137">Verify that the Project Operations license has been selected and select **Save changes**.</span></span> 

> [!NOTE]
> <span data-ttu-id="bd3b2-138">لا يلزم تعيين مستخدم إلى عرض الإصدار التجريبي من Finance.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-138">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="bd3b2-139">بدء مشروع جديد في LCS</span><span class="sxs-lookup"><span data-stu-id="bd3b2-139">Start a new project in LCS</span></span>

<span data-ttu-id="bd3b2-140">قم بإنشاء مشروع LCS جديد كما هو موضح في موضوع، [بدء مشروع جديد في LCS](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="bd3b2-140">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="bd3b2-141">إضافة اشتراك Azure إلى مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="bd3b2-141">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="bd3b2-142">لإكمال هذه المهمة، اتبع الخطوات الواردة في الموضوع، [إضافة اشتراك Azure إلى مشروع LCS](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="bd3b2-142">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="bd3b2-143">نشر بيئة عرض توضيحي من Finance مع Project Operations لسيناريوهات المورد/المنتجات غير المخزنة</span><span class="sxs-lookup"><span data-stu-id="bd3b2-143">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="bd3b2-144">اتبع الإرشادات الموضحة في موضوع، [توفير بيئة جديدة](resource-provision-new-environment.md) لإكمال النشر.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-144">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="bd3b2-145">استخدم نوع نشر [بيئة العرض التوضيحي](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) للمعاينة.</span><span class="sxs-lookup"><span data-stu-id="bd3b2-145">Use the [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span>

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="bd3b2-146">تثبيت إعداد CDS وبيانات التكوين</span><span class="sxs-lookup"><span data-stu-id="bd3b2-146">Install CDS setup and configuration data</span></span>

<span data-ttu-id="bd3b2-147">قم بتثبيت إعداد CDS وبيانات التكوين كما هو موضح في الموضوع، [إعداد بيانات التكوين وتطبيقها في Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="bd3b2-147">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>

