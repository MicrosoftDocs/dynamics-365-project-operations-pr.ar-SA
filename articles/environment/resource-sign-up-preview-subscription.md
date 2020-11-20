---
title: إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة
description: يوفر هذا الموضوع معلومات حول كيفية الاشتراك في Project Operations ونشرها للسيناريوهات المستندة إلى المورد/المنتجات غير المخزنة.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: dc3b353f19b915f645aed91dc2a8127117027034
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121112"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="b1026-103">إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة</span><span class="sxs-lookup"><span data-stu-id="b1026-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="b1026-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="b1026-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b1026-105">يشرح هذا الموضوع كيفية الاشتراك في المعاينة/عرض الشريك ونشر بيئة Project Operations للسيناريوهات المستندة إلى مورد/منتجات غير مخزنة.</span><span class="sxs-lookup"><span data-stu-id="b1026-105">This topic explains how to subscribe to the preview/partner offer and deploy Project Operations environment for resource/ non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1026-106">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="b1026-106">Prerequisites</span></span>

- <span data-ttu-id="b1026-107">ستتلقى رسالة بريد إلكتروني لدعوتك للمشاركة في المعاينة.</span><span class="sxs-lookup"><span data-stu-id="b1026-107">You will receive an email inviting you to participate in the preview.</span></span> <span data-ttu-id="b1026-108">يمكنك طلب معاينة من [موقع الويب الخاص بـ Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span><span class="sxs-lookup"><span data-stu-id="b1026-108">You can request a preview on the [Project Operations website](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span></span>
- <span data-ttu-id="b1026-109">يجب أن يكون لدي المستخدم الذي ينشر المعاينة حقوق المسؤول العمومي لمستأجر Azure.</span><span class="sxs-lookup"><span data-stu-id="b1026-109">The user who deploys the preview must have Azure tenant global administrator rights.</span></span>
- <span data-ttu-id="b1026-110">يتطلب نشر بيئة Finance وجود اشتراك Azure صالح والذي ستتم فوترته لكل بيئة.</span><span class="sxs-lookup"><span data-stu-id="b1026-110">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="b1026-111">يمكنك استخدام الاشتراك الموجود في المؤسسات أو استخدام [الإصدار التجريبي من Azure](https://azure.microsoft.com/en-us/free/) لبدء العمل.</span><span class="sxs-lookup"><span data-stu-id="b1026-111">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="b1026-112">سيتم توفير بيئة CDS مجانًا لفترة زمنية محددة بمدة 30 يومًا.</span><span class="sxs-lookup"><span data-stu-id="b1026-112">The CDS environment will be provided free for a limited 30 day period.</span></span>

## <a name="subscribe"></a><span data-ttu-id="b1026-113">الاشتراك</span><span class="sxs-lookup"><span data-stu-id="b1026-113">Subscribe</span></span>

<span data-ttu-id="b1026-114">عند الموافقة على [طلب المعاينة](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u)، ستتلقى عرضين من Microsoft بواسطة البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="b1026-114">When your [preview request](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) is approved, you will receive three offers from Microsoft by email.</span></span> <span data-ttu-id="b1026-115">تسمح لك هذه العروض بنشر معاينة Project Operations:</span><span class="sxs-lookup"><span data-stu-id="b1026-115">These offers allow you to deploy the Project Operations Preview:</span></span>

- <span data-ttu-id="b1026-116">Dynamics 365 Project Operations (CRM) - إصدار تجريبي للمعاينة</span><span class="sxs-lookup"><span data-stu-id="b1026-116">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span>
- <span data-ttu-id="b1026-117">Office 365 Project Operations - إصدار تجريبي للمعاينة</span><span class="sxs-lookup"><span data-stu-id="b1026-117">Office 365 Project Operations - Preview Trial</span></span>
- <span data-ttu-id="b1026-118">Dynamics 365 Finance - الإصدار التجريبي للمعاينة</span><span class="sxs-lookup"><span data-stu-id="b1026-118">Dynamics 365 Finance - Preview Trial</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b1026-119">شخص واحد فقط، مسؤول المستأجر، في مؤسسة تحتاج إلى تنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="b1026-119">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="b1026-120">إذا لم تكن أنت المشترك في هذا الإصدار، فانتظر حتى يتم تسجيل مؤسستك وتستلم بيانات اعتماد المستخدم الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="b1026-120">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>

### <a name="dynamics-365-project-operations-crm---preview-trial"></a><span data-ttu-id="b1026-121">Dynamics 365 Project Operations (CRM) - إصدار تجريبي للمعاينة</span><span class="sxs-lookup"><span data-stu-id="b1026-121">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span> 

<span data-ttu-id="b1026-122">قبل البدء، تأكد من تسجيل الدخول إلى مستعرض باستخدام حساب عمل المستخدم في المستأجر حيث تريد معاينة Project Operations.</span><span class="sxs-lookup"><span data-stu-id="b1026-122">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="b1026-123">استرجع كود العرض الأول، **Dynamics 365 Project Operations (CRM) - الإصدار التجريبي للمعاينة** عن طريق لصقه في عنوان URL للمستعرض.</span><span class="sxs-lookup"><span data-stu-id="b1026-123">Redeem the first offer code, **Dynamics 365 Project Operations (CRM) - Preview Trial** by pasting it into the browser URL.</span></span>

![استرداد العرض](./media/16RedeemFirstOfferNew.png)

2. <span data-ttu-id="b1026-125">أكد طلبك.</span><span class="sxs-lookup"><span data-stu-id="b1026-125">Confirm your order.</span></span>

![تأكيد الأمر](./media/17ConfirmOrderNew.png)

<span data-ttu-id="b1026-127">سترى أنه تم استرجاع عرض التأكيد بنجاح.</span><span class="sxs-lookup"><span data-stu-id="b1026-127">You will see confirmation offer was successfully redeemed.</span></span>

![تأكيد](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a><span data-ttu-id="b1026-129">Office 365 Project Operations - إصدار تجريبي للمعاينة</span><span class="sxs-lookup"><span data-stu-id="b1026-129">Office 365 Project Operations - Preview Trial</span></span>

<span data-ttu-id="b1026-130">كرر الخطوات نفسها التي تم تنفيذها لكود العرض الأول.</span><span class="sxs-lookup"><span data-stu-id="b1026-130">Repeat the same steps as with the first offer code.</span></span> <span data-ttu-id="b1026-131">تأكد من إضافة كود العرض الثاني باستخدام حساب المستخدم نفسه الذي تم استخدامه مع كود العرض الأول.</span><span class="sxs-lookup"><span data-stu-id="b1026-131">Make sure to add the second offer code using the same user account that was used with the first offer code.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="b1026-132">إصدار تجريبي لمعاينة Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="b1026-132">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="b1026-133">كرر نفس الخطوات مع العرض الأخير من البريد الإلكتروني الترحيبي.</span><span class="sxs-lookup"><span data-stu-id="b1026-133">Repeat the same steps with the last offer from the Welcome email.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="b1026-134">تعيين التراخيص</span><span class="sxs-lookup"><span data-stu-id="b1026-134">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b1026-135">ستحتاج إلى حق وصول إداري إلى مدخل Microsoft 365 الخاص بمؤسستك لإكمال الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="b1026-135">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="b1026-136">انتقل إلى [مركز إدارة](https://portal.office.com/) لتعيين التراخيص إلى المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="b1026-136">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

![الصفحة الرئيسية لمركز الإدارة](./media/14AdminPortal.png)

2. <span data-ttu-id="b1026-138">في صفحة **المستخدمين النشطين**، حدد المستخدمين الذين ترغب في تعيين ترخيص لهم.</span><span class="sxs-lookup"><span data-stu-id="b1026-138">On the **Active users** page, select the users that you want to assign a license to.</span></span>

![تعيين التراخيص](./media/15AssignLicenses.png)

3. <span data-ttu-id="b1026-140">تأكد من تحديد تراخيص **معاينة Dynamics 365 Project Operations (CRM) Preview** و **Office 365 Project Operations - معاينة** وحدد **حفظ التغييرات**.</span><span class="sxs-lookup"><span data-stu-id="b1026-140">Verify that the **Dynamics 365 Project Operations (CRM) Preview** and **Office 365 Project Operations - Preview** license have been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="b1026-141">لا يلزم تعيين مستخدم إلى عرض الإصدار التجريبي من Finance.</span><span class="sxs-lookup"><span data-stu-id="b1026-141">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="b1026-142">بدء مشروع جديد في LCS</span><span class="sxs-lookup"><span data-stu-id="b1026-142">Start a new project in LCS</span></span>

<span data-ttu-id="b1026-143">قم بإنشاء مشروع LCS جديد كما هو موضح في موضوع، [بدء مشروع جديد في LCS](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="b1026-143">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="b1026-144">إضافة اشتراك Azure إلى مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="b1026-144">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="b1026-145">لإكمال هذه المهمة، اتبع الخطوات الواردة في الموضوع، [إضافة اشتراك Azure إلى مشروع LCS](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="b1026-145">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="b1026-146">نشر بيئة عرض توضيحي من Finance مع Project Operations لسيناريوهات المورد/المنتجات غير المخزنة</span><span class="sxs-lookup"><span data-stu-id="b1026-146">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="b1026-147">اتبع الإرشادات الموضحة في موضوع، [توفير بيئة جديدة](resource-provision-new-environment.md) لإكمال النشر.</span><span class="sxs-lookup"><span data-stu-id="b1026-147">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="b1026-148">استخدم نوع نشر [بيئة العرض التوضيحي](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) للمعاينة.</span><span class="sxs-lookup"><span data-stu-id="b1026-148">Use the [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="b1026-149">تثبيت إعداد CDS وبيانات التكوين</span><span class="sxs-lookup"><span data-stu-id="b1026-149">Install CDS setup and configuration data</span></span>

<span data-ttu-id="b1026-150">قم بتثبيت إعداد CDS وبيانات التكوين كما هو موضح في الموضوع، [إعداد بيانات التكوين وتطبيقها في Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="b1026-150">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="b1026-151">أكمل هذه الخطوة فقط بعد نشر بيئة العرض التوضيحي لتطبيق Finance وبعد أن تصبح بيانات العرض التوضيحي في FO جاهزة.</span><span class="sxs-lookup"><span data-stu-id="b1026-151">Complete this step only after Finance demo environment is deployed and demo data in FO is ready.</span></span>
