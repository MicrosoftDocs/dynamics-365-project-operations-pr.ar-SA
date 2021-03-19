---
title: نشر Project Operations - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية تثبيت نشر Project Operations Lite – التعامل مع الفواتير الأولية‬.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0af8067fc0673890a317ac6f4e62d74b7f4eebca
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290073"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="68d54-103">نشر Project Operations - خفيف</span><span class="sxs-lookup"><span data-stu-id="68d54-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="68d54-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="68d54-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="68d54-105">يدعم Project Operations نماذج نشر متعددة.</span><span class="sxs-lookup"><span data-stu-id="68d54-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="68d54-106">لتحديد نموذج النشر الأفضل، راجع [أنواع النشر](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="68d54-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="68d54-107">ينتج عن هذا النشر، النشر الخفيف – التعامل مع الفواتير الأولية، **Common Data Service-نشر Project Operations فقط**.</span><span class="sxs-lookup"><span data-stu-id="68d54-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="68d54-108">تثبيت Project Operations في بيئة CDS جديدة</span><span class="sxs-lookup"><span data-stu-id="68d54-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="68d54-109">تثبيت في بيئة CDS موجودة</span><span class="sxs-lookup"><span data-stu-id="68d54-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="68d54-110">تثبيت Project Operations في بيئة CDS جديدة</span><span class="sxs-lookup"><span data-stu-id="68d54-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="68d54-111">بصفتك [المسؤول العمومي أو مسؤول Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص، أنشئ بيئة CDS جديدة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="68d54-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="68d54-112">تأكد من تمكين **قاعدة بيانات CDS** و **تطبيقات Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="68d54-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="68d54-113">للحصول على مزيد من المعلومات، راجع [إنشاء البيئات وإدارتها في مركز إدارة Power Platform](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="68d54-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="68d54-114">حدد **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="68d54-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="68d54-115">تثبيت Project Operations في بيئة CDS موجودة</span><span class="sxs-lookup"><span data-stu-id="68d54-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="68d54-116">بصفتك [المسؤول العمومي أو مسؤول Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص Project Operations، حدد موقع البيئة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com) حيث تريد تثبيت Project Operations.</span><span class="sxs-lookup"><span data-stu-id="68d54-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="68d54-117">قم بتثبيت **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="68d54-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="68d54-118">لمزيد من المعلومات، راجع [إدارة تطبيقات Dynamics 365](https://docs.microsoft.com/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="68d54-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]