---
title: نظرة عامة على Project Service Automation
description: يقدم هذا الموضوع معلومات عن حل دمج Dynamics 365 Project Service Automation في Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 897e1a1c-d31c-42b8-bb59-6b67202d8d61
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 080a545d8713e52d9778367aec1969b815d683e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748677"
---
# <a name="project-service-automation-overview"></a><span data-ttu-id="f6371-103">نظرة عامة على Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f6371-103">Project Service Automation overview</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="f6371-104">يستخدم حل تكامل Project Service Automation إلى Finance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Dynamics 365 Finance وDynamics 365 Project Service Automation من خلال Common Data Service.</span><span class="sxs-lookup"><span data-stu-id="f6371-104">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Dynamics 365 Finance and Dynamics 365 Project Service Automation via Common Data Service.</span></span> <span data-ttu-id="f6371-105">تعمل قوالب التكامل المتوفرة مع ميزة تكامل البيانات على تمكين تدفق المشاريع وعقود المشروع وبنود عقود المشروع ومراحل بنود عقد المشروع ومهام المشروع وفئات حركات المصروفات وتقديرات الساعات وتقديرات المصروفات من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-105">The integration templates that are available with the Data integration feature enable the flow of projects, project contracts, project contract lines, project contract line milestones, project tasks, expense transaction categories, hour estimates, and expense estimates from Project Service Automation to Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="f6371-106">إذا كنت تستخدم الإصدار 7.3.0 ، فيجب عليك تثبيت قاعدة المعارف 4074835.</span><span class="sxs-lookup"><span data-stu-id="f6371-106">If you're using version 7.3.0, you must install KB 4074835.</span></span> <span data-ttu-id="f6371-107">ستتمكن بعد ذلك من دمج مشاريع السعر الثابت.</span><span class="sxs-lookup"><span data-stu-id="f6371-107">You will then be able to integrate fixed price projects.</span></span>
> - <span data-ttu-id="f6371-108">إذا كنت تستخدم الإصدار 7.3.0 ، وقمت بإحضار معاملات الرسوم من Project Service Automation ، فيجب عليك تثبيت قاعدة معارف 4345320 لتضمين هذه الرسوم في فاتورة المشروع.</span><span class="sxs-lookup"><span data-stu-id="f6371-108">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="f6371-109">إذا كنت تستخدم الإصدار 8.0 ، فستتمكن من استخدام تكامل مهام المشروع وفئات حركات المصروفات وتقديرات الساعة وتقديرات المصروفات وتأمين الوظائف.</span><span class="sxs-lookup"><span data-stu-id="f6371-109">If you're using version 8.0, you will be able to use project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking.</span></span>
> - <span data-ttu-id="f6371-110">إذا كنت تستخدم الإصدار 8.0.1 أو أحدث ، فستتمكن من مزامنة القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="f6371-110">If you're using version 8.0.1 or later, you will be able to synchronize actuals.</span></span>

<span data-ttu-id="f6371-111">قبل أن تتمكن من دمج Project Service Automation Finance ، يجب عليك تكوين معلمات تكامل Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f6371-111">Before you can integrate Project Service Automation Finance, you must configure the Project Service Automation integration parameters.</span></span> <span data-ttu-id="f6371-112">لمزيد من المعلومات، راجع [معلمات تكامل Project Service Automation](PSA-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="f6371-112">For more information, see [Project Service Automation integration parameters](PSA-parameters.md).</span></span>

<span data-ttu-id="f6371-113">يتيح حل التكامل هذا المزامنة المباشرة في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="f6371-113">This integration solution enables direct synchronization in the following scenarios:</span></span>

- <span data-ttu-id="f6371-114">احتفظ بعقود المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-114">Maintain project contracts in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="f6371-115">قم بإنشاء مشاريع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-115">Create projects in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="f6371-116">حافظ على بنود عقد المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-116">Maintain project contract lines in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="f6371-117">حافظ على معالم بنود عقد المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-117">Maintain project contract line milestones in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="f6371-118">حافظ على مهام المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-118">Maintain project tasks in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="f6371-119">احتفظ بفئات حركات المصروفات في Finance ، وقم بمزامنتها مباشرة من Finance إلى Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f6371-119">Maintain expense transaction categories in Finance, and synchronize them directly from Finance to Project Service Automation.</span></span>
- <span data-ttu-id="f6371-120">قم بإنشاء تقديرات ساعات المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-120">Create project hour estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="f6371-121">قم بإنشاء تقديرات مصروفات المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-121">Create project expense estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="f6371-122">قم بإنشاء وقت المشروع والمصروفات والرسوم الفعلية في Project Service Automation ، وأنشئ حركات المشروع في دفتر يومية تكامل Project Service Automation بحيث يمكن ترحيلها في Finance.</span><span class="sxs-lookup"><span data-stu-id="f6371-122">Create project time, expense, and fee actuals in Project Service Automation, and create project transactions in the Project Service Automation integration journal so that they can be posted in Finance.</span></span>

## <a name="data-synchronization"></a><span data-ttu-id="f6371-123">مزامنة البيانات</span><span class="sxs-lookup"><span data-stu-id="f6371-123">Data synchronization</span></span>

<span data-ttu-id="f6371-124">يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات كجزء من التكامل بين Project Service Automation وFinance.</span><span class="sxs-lookup"><span data-stu-id="f6371-124">The following illustration shows how data is synchronized as part of the integration between Project Service Automation and Finance.</span></span>

> [!NOTE]
> <span data-ttu-id="f6371-125">ليست كل القوالب متوفرة حاليا.</span><span class="sxs-lookup"><span data-stu-id="f6371-125">Not all templates are currently available.</span></span> <span data-ttu-id="f6371-126">سيتم إصدار القوالب بمجرد اكتمالها.</span><span class="sxs-lookup"><span data-stu-id="f6371-126">Templates will be released as they are completed.</span></span>

<span data-ttu-id="f6371-127">[![تكامل Project Service Automation مع Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span><span class="sxs-lookup"><span data-stu-id="f6371-127">[![Project Service Automation integration with Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span></span>

## <a name="system-requirements-for-finance"></a><span data-ttu-id="f6371-128">متطلبات النظام لـ Finance</span><span class="sxs-lookup"><span data-stu-id="f6371-128">System requirements for Finance</span></span>

<span data-ttu-id="f6371-129">لاستخدام حل تمامل Project Service Automation مع Finance ، يجب عليك تثبيت إصدار Enterprise 7.3 مع تحديث النظام الأساسي 12 أو إصدار لاحق.</span><span class="sxs-lookup"><span data-stu-id="f6371-129">To use the Project Service Automation to Finance integration solution, you must install Enterprise edition 7.3 with Platform update 12 or later.</span></span>

## <a name="system-requirements-for-project-service-automation"></a><span data-ttu-id="f6371-130">متطلبات النظام لـ Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f6371-130">System requirements for Project Service Automation</span></span>

<span data-ttu-id="f6371-131">لاستخدام حل تكامل Project Service Automation مع Finance ، يجب عليك تثبيت المكونات التالية:</span><span class="sxs-lookup"><span data-stu-id="f6371-131">To use the Project Service Automation to Finance integration solution, you must install the following components:</span></span>

- <span data-ttu-id="f6371-132">Dynamics 365 Project Service Automation الإصدار 9.0.0.0 أو إصدار أحدث</span><span class="sxs-lookup"><span data-stu-id="f6371-132">Dynamics 365 Project Service Automation version 9.0.0.0 or later</span></span>
- <span data-ttu-id="f6371-133">العميل المتوقع إلى الحل النقدي لـ Dynamics 365 Sales، الإصدار 1.14.0.0 (v14) أو إصدار لاحق</span><span class="sxs-lookup"><span data-stu-id="f6371-133">Prospect to cash solution for Dynamics 365 Sales, version 1.14.0.0 (v14) or later</span></span>
- <span data-ttu-id="f6371-134">حل تكامل Project Service Automation مع Finance لـ Dynamics 365 Project Service Automation لإصدار 1.0.0.0 أو إصدار لاحق.</span><span class="sxs-lookup"><span data-stu-id="f6371-134">Project Service Automation to Finance solution for Dynamics 365 Project Service Automation version 1.0.0.0 or later</span></span>

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a><span data-ttu-id="f6371-135">قم بتثبيت حل تكامل Project Service Automation مع Finance في مثيل Project Service Automation الخاص بك</span><span class="sxs-lookup"><span data-stu-id="f6371-135">Install the Project Service Automation to Finance integration solution in your Project Service Automation instance</span></span>

<span data-ttu-id="f6371-136">قم بتنزيل حل تمامل Project Service Automation مع Finance من [مركز تنزيل Microsoft‬](https://www.microsoft.com/download/details.aspx?id=57016)، واتبع التعليمات المضمنة مع الحل.</span><span class="sxs-lookup"><span data-stu-id="f6371-136">Download the Project Service Automation to Finance integration solution from [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016), and follow the instructions that are included with the solution.</span></span>
