---
title: إضافة اشتراك Azure إلى مشروع LCS
description: يوفر هذا الموضوع معلومات حول كيفية توصيل اشتراك Azure الخاص بك بمشروع LCS.
author: sigitac
manager: Annbe
ms.date: 04/12/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a80c926ba67a1620e39d8c7677a05678454e6340
ms.sourcegitcommit: 7468d668c48c1d87934aab9a034decd51e56dec6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/13/2021
ms.locfileid: "5880522"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="9c6f5-103">إضافة اشتراك Azure إلى مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="9c6f5-103">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="9c6f5-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="9c6f5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="9c6f5-105">يجب نشر البيئات المستضافة على السحابة باستخدام اشتراك Azure موجود.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="9c6f5-106">يشرح هذا الموضوع كيفية توصيل اشتراك Azure الخاص بك بمشروع LCS.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="9c6f5-107">منح موافقة المسؤول</span><span class="sxs-lookup"><span data-stu-id="9c6f5-107">Grant admin consent</span></span>

1. <span data-ttu-id="9c6f5-108">في مشروع LCS الخاص بك، في قسم **البيئات**، حدد **إعدادات Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![إعدادات تطبيق Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="9c6f5-110">في صفحة **إعدادات المشروع**، في علامة التبويب **موصلات Azure**، حدد **تخويل**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="9c6f5-111">هذا يسمح بنشر البيئات في هذا المشروع.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-111">This allows environments to be deployed to this project.</span></span>

![موصلات Azure](./media/2AzureConnectors.png)

3. <span data-ttu-id="9c6f5-113">حدد **تخويل** مرة أخرى لتوفير موافقة المسؤول.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-113">Select **Authorize** again to provide admin consent.</span></span>

![منح موافقة المسؤول](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="9c6f5-115">اقبل طلب الأذونات.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-115">Accept the permissions request.</span></span>

![قبول طلب الأذونات](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="9c6f5-117">اكتمل التخويل الآن.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-117">The authorization is now complete.</span></span> 

![نجح التخويل](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="9c6f5-119">يوفر Dynamics Deployment Services الوصول إلى اشتراك Azure</span><span class="sxs-lookup"><span data-stu-id="9c6f5-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="9c6f5-120">اذهب إلى [Microsoft Azure الفوترة](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) وحدد الاشتراك الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="9c6f5-121">تحتاج Dynamics Deployment Services إلى الوصول إلى هذا الاشتراك لكي تتمكن من نشر البيئات.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![تفاصيل اشتراك Azure](./media/6AzureSubscription.png)

2. <span data-ttu-id="9c6f5-123">حدد **الوصول للتحكم (IAM)** في جزء التنقل، ثم حدد **إضافة تعيين دور**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="9c6f5-124">في شريط التمرير الموجود على الجانب الأيسر، حدد **دور المساهم**، وفي القائمة المتوفرة، ابحث عن وحدد **Dynamics Deployment Services**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="9c6f5-125">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-125">Select **Save**.</span></span>

![الوصول إلى الاشتراك](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="9c6f5-127">إضافة اشتراك موصل إلى مشروع LCS</span><span class="sxs-lookup"><span data-stu-id="9c6f5-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="9c6f5-128">في مشروع LCS الخاص بك، في صفحة **إعدادات Microsoft Azure**، حدد **إضافة** لإضافة موصل جديد.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="9c6f5-129">أدخل معرف اشتراك Azure الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="9c6f5-130">يمكنك العثور على معرف اشتراك Azure في [مدخل Azure](https://ms.portal.azure.com/)، أسفل **الإعدادات** في الجزء السفلي الأيمن من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="9c6f5-131">في حقل **التكوين لاستخدام Azure Resource Manager**، حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="9c6f5-132">تأكد من أن مجال مستأحر AAD الخاص باشتراك Azure يطابق المجال الذي يمتلك اشتراك Azure الذي تستخدمه، وحدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="9c6f5-133">في شاشة **إعداد Microsoft Azure**، حدد **التالي** للتأكيد.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="9c6f5-134">إذا تلقيت خطأ في هذه الشاشة، فقم بالرجوع إلى القسم [توفير وصول Dynamics Deployment Services إلى اشتراك Azure](#provide) في هذه الموضوع وتأكد من إتمام كافة الخطوات.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="9c6f5-135">قم بتنزيل شهادة إدارة Azure إلى مجلد محلي على الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-135">Download the Azure Management Certificate to a local folder on your computer.</span></span> <span data-ttu-id="9c6f5-136">اطلب من مسؤول اشتراك Azure تحميل الشهادة إلى مدخل إدارة Azure بتحديد الاشتراك ثم الذهاب إلى **الإعدادات** > **إدارة الشهادات**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-136">Ask your Azure subscription administrator to upload the certificate to Azure Management Portal by selecting the subscription and going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="9c6f5-137">تمكن هذه الشهادة LCS من الاتصال بـ Azure نيابة عنك.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-137">This certificate enables LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="9c6f5-138">يمكنك تخطي هذه الخطوة إذا كان المستخدم لديه حق الوصول إلى الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-138">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="9c6f5-139">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-139">Select  **Next**.</span></span>
8. <span data-ttu-id="9c6f5-140">حدد منطقه Azure التي سيتم النشر فيها وحدد مركز بيانات قريب من المكان الذي تخطط لاستخدام هذا النظام فيه.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-140">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="9c6f5-141">حدد **اتصال**.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-141">Select  **Connect**.</span></span>

<span data-ttu-id="9c6f5-142">لقد قمت بالاتصال بنجاح باشتراك Azure.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-142">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="9c6f5-143">يمكنك الآن نشر بيئات Dynamics 365 Finance المستضافة على السحابة.</span><span class="sxs-lookup"><span data-stu-id="9c6f5-143">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
