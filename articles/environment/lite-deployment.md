---
title: نشر Project Operations - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية تثبيت نشر Project Operations Lite – التعامل مع الفواتير الأولية‬.
author: stsporen
ms.date: 10/02/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb1f1ad86e19d84d68a40b32b2fdb08dc4777a78
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995515"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="1d5ba-103">نشر Project Operations - خفيف</span><span class="sxs-lookup"><span data-stu-id="1d5ba-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="1d5ba-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="1d5ba-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="1d5ba-105">يدعم Project Operations نماذج نشر متعددة.</span><span class="sxs-lookup"><span data-stu-id="1d5ba-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="1d5ba-106">لتحديد نموذج النشر الأفضل، راجع [أنواع النشر](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="1d5ba-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="1d5ba-107">ينتج عن هذا النشر، النشر الخفيف – التعامل مع الفواتير الأولية، **Common Data Service-نشر Project Operations فقط**.</span><span class="sxs-lookup"><span data-stu-id="1d5ba-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="1d5ba-108">تثبيت Project Operations في بيئة CDS جديدة</span><span class="sxs-lookup"><span data-stu-id="1d5ba-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="1d5ba-109">تثبيت في بيئة CDS موجودة</span><span class="sxs-lookup"><span data-stu-id="1d5ba-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="1d5ba-110">تثبيت Project Operations في بيئة CDS جديدة</span><span class="sxs-lookup"><span data-stu-id="1d5ba-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="1d5ba-111">بصفتك [المسؤول العمومي أو مسؤول Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص، أنشئ بيئة CDS جديدة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="1d5ba-111">As the [Global or Power Platform Administrator](/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="1d5ba-112">تأكد من تمكين **قاعدة بيانات CDS** و **تطبيقات Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="1d5ba-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="1d5ba-113">للحصول على مزيد من المعلومات، راجع [إنشاء البيئات وإدارتها في مركز إدارة Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="1d5ba-113">For more information, see [Create and manage environments in the Power Platform admin center](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="1d5ba-114">حدد **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="1d5ba-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="1d5ba-115">تثبيت Project Operations في بيئة CDS موجودة</span><span class="sxs-lookup"><span data-stu-id="1d5ba-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="1d5ba-116">بصفتك [المسؤول العمومي أو مسؤول Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص Project Operations، حدد موقع البيئة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com) حيث تريد تثبيت Project Operations.</span><span class="sxs-lookup"><span data-stu-id="1d5ba-116">As the [Global or Power Platform Administrator](/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="1d5ba-117">قم بتثبيت **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="1d5ba-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="1d5ba-118">لمزيد من المعلومات، راجع [إدارة تطبيقات Dynamics 365](/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="1d5ba-118">For more information, see [Manage Dynamics 365 apps](/power-platform/admin/manage-apps).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]