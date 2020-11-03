---
title: إضافة اشتراك Azure إلى مشروع LCS
description: يوفر هذا الموضوع معلومات حول كيفية توصيل اشتراك Azure الخاص بك بمشروع LCS.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0b5703542ac58adcc710890d9676dd0090a82f25
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070515"
---
# <a name="add-an-azure-subscription-to-lcs-project"></a><span data-ttu-id="8aa15-103">إضافة اشتراك Azure إلى مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="8aa15-103">Add an Azure subscription to LCS project</span></span>

<span data-ttu-id="8aa15-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="8aa15-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8aa15-105">يجب نشر البيئات المستضافة على السحابة باستخدام اشتراك Azure موجود.</span><span class="sxs-lookup"><span data-stu-id="8aa15-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="8aa15-106">يشرح هذا الموضوع كيفية توصيل اشتراك Azure الخاص بك بمشروع LCS.</span><span class="sxs-lookup"><span data-stu-id="8aa15-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="8aa15-107">منح موافقة المسؤول</span><span class="sxs-lookup"><span data-stu-id="8aa15-107">Grant admin consent</span></span>

1. <span data-ttu-id="8aa15-108">في مشروع LCS الخاص بك، في قسم **البيئات** ، حدد **إعدادات Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![إعدادات تطبيق Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="8aa15-110">في صفحة **إعدادات المشروع** ، في علامة التبويب **موصلات Azure** ، حدد **تخويل**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="8aa15-111">هذا يسمح بنشر البيئات في هذا المشروع.</span><span class="sxs-lookup"><span data-stu-id="8aa15-111">This allows environments to be deployed to this project.</span></span>

![موصلات Azure](./media/2AzureConnectors.png)

3. <span data-ttu-id="8aa15-113">حدد **تخويل** مرة أخرى لتوفير موافقة المسؤول.</span><span class="sxs-lookup"><span data-stu-id="8aa15-113">Select **Authorize** again to provide admin consent.</span></span>

![منح موافقة المسؤول](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="8aa15-115">اقبل طلب الأذونات.</span><span class="sxs-lookup"><span data-stu-id="8aa15-115">Accept the permissions request.</span></span>

![قبول طلب الأذونات](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="8aa15-117">اكتمل التخويل الآن.</span><span class="sxs-lookup"><span data-stu-id="8aa15-117">The authorization is now complete.</span></span> 

![نجح التخويل](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="8aa15-119">يوفر Dynamics Deployment Services الوصول إلى اشتراك Azure</span><span class="sxs-lookup"><span data-stu-id="8aa15-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="8aa15-120">اذهب إلى [Microsoft Azure الفوترة](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) وحدد الاشتراك الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="8aa15-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="8aa15-121">تحتاج Dynamics Deployment Services إلى الوصول إلى هذا الاشتراك لكي تتمكن من نشر البيئات.</span><span class="sxs-lookup"><span data-stu-id="8aa15-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![تفاصيل اشتراك Azure](./media/6AzureSubscription.png)

2. <span data-ttu-id="8aa15-123">حدد **الوصول للتحكم (IAM)** في جزء التنقل، ثم حدد **إضافة تعيين دور**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="8aa15-124">في شريط التمرير الموجود على الجانب الأيسر، حدد **دور المساهم** ، وفي القائمة المتوفرة، ابحث عن وحدد **Dynamics Deployment Services**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-124">In the slider on the right side, select **Contributor role** , and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="8aa15-125">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-125">Select **Save**.</span></span>

![الوصول إلى الاشتراك](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="8aa15-127">إضافة اشتراك موصل إلى مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="8aa15-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="8aa15-128">في مشروع LCS الخاص بك، في صفحة **إعدادات Microsoft Azure** ، حدد **إضافة** لإضافة موصل جديد.</span><span class="sxs-lookup"><span data-stu-id="8aa15-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="8aa15-129">أدخل معرف اشتراك Azure الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="8aa15-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="8aa15-130">يمكنك العثور على معرف اشتراك Azure في [مدخل Azure](https://ms.portal.azure.com/)، أسفل **الإعدادات** في الجزء السفلي الأيمن من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="8aa15-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="8aa15-131">في حقل **التكوين لاستخدام Azure Resource Manager** ، حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="8aa15-132">تأكد من أن مجال مستأحر AAD الخاص باشتراك Azure يطابق المجال الذي يمتلك اشتراك Azure الذي تستخدمه، وحدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="8aa15-133">في شاشة **إعداد Microsoft Azure** ، حدد **التالي** للتأكيد.</span><span class="sxs-lookup"><span data-stu-id="8aa15-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="8aa15-134">إذا تلقيت خطأ في هذه الشاشة، فقم بالرجوع إلى القسم [توفير وصول Dynamics Deployment Services إلى اشتراك Azure](#provide) في هذه الموضوع وتأكد من إتمام كافة الخطوات.</span><span class="sxs-lookup"><span data-stu-id="8aa15-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="8aa15-135">قم بتنزيل شهادة إدارة Azure إلى مجلد محلي على جهاز الكمبيوتر الخاص بك ثم قم بتحميلها إلى مدخل إدارة Azure بالانتقال إلى **الإعدادات** > **إدارة الشهادات**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-135">Download the Azure Management Certificate to a local folder on your computer, and then upload it to Azure Management Portal by going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="8aa15-136">ستعمل هذه الشهادة على تمكين LCS من الاتصال مع Azure نيابة عنك.</span><span class="sxs-lookup"><span data-stu-id="8aa15-136">This certificate will enable LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="8aa15-137">يمكنك تخطي هذه الخطوة إذا كان المستخدم لديه حق الوصول إلى الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="8aa15-137">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="8aa15-138">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-138">Select  **Next**.</span></span>
8. <span data-ttu-id="8aa15-139">حدد منطقه Azure التي سيتم النشر فيها وحدد مركز بيانات قريب من المكان الذي تخطط لاستخدام هذا النظام فيه.</span><span class="sxs-lookup"><span data-stu-id="8aa15-139">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="8aa15-140">حدد **اتصال**.</span><span class="sxs-lookup"><span data-stu-id="8aa15-140">Select  **Connect**.</span></span>

<span data-ttu-id="8aa15-141">لقد قمت بالاتصال بنجاح باشتراك Azure.</span><span class="sxs-lookup"><span data-stu-id="8aa15-141">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="8aa15-142">يمكنك الآن نشر بيئات Dynamics 365 Finance المستضافة على السحابة.</span><span class="sxs-lookup"><span data-stu-id="8aa15-142">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>


