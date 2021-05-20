---
title: تكامل ‏‫الكتابة المزدوجة في Project Operations
description: يوفر هذا موضوع نظرة عامة على تكامل الكتابة المزدوجة في Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d9d6a7c367872219b4aca32aecb15d6837ebe296
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955642"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="936f7-103">نظرة عامة حول تكامل ‏‫الكتابة المزدوجة في Project Operations</span><span class="sxs-lookup"><span data-stu-id="936f7-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="936f7-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="936f7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="936f7-105">يستخدم Project Operations [إمكانات الكتابة المزدوجة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) لمزامنة البيانات عبر Microsoft Dataverse وDynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="936f7-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="936f7-106">يوضح الشكل التوضيحي التالي كيفية مزامنة البيانات كجزء من هذا التكامل بين Dataverse وFinance.</span><span class="sxs-lookup"><span data-stu-id="936f7-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![نظرة عامة حول تدفقات بيانات Project Operations](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="936f7-108">توفر Project Operations في Dataverse واجهة مستخدم حديثة وقابلة للتوسع بسهولة بدون تعليمات برمجية/بتعمليات برمجية طفيفة باستخدام إمكانات Power Platform.</span><span class="sxs-lookup"><span data-stu-id="936f7-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="936f7-109">ويمكن لمديري المشروع ومديري الموارد وأعضاء فريق المشروع وموظفي المكتب الأمامي الآخرين، تنفيذ أنشطتهم في Project Operations على Dataverse.</span><span class="sxs-lookup"><span data-stu-id="936f7-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="936f7-110">يوفر Project Operations في Finance دعم محاسبة المشروع وتقدير الإيرادات.</span><span class="sxs-lookup"><span data-stu-id="936f7-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="936f7-111">يتم ربط Project Operations بإطار العمل المالي في Finance لحساب ضريبة المبيعات وأسعار صرف العملات ورفع تقارير بالأبعاد المالية وغير ذلك.</span><span class="sxs-lookup"><span data-stu-id="936f7-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="936f7-112">تعتمد تجارب محاسب المشروع في الغالب على Finance.</span><span class="sxs-lookup"><span data-stu-id="936f7-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="936f7-113">يتكون تكامل Project Operations من تكامل المكون التالي:</span><span class="sxs-lookup"><span data-stu-id="936f7-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="936f7-114">تكامل بيانات التكوين والإعداد في Project Operations</span><span class="sxs-lookup"><span data-stu-id="936f7-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="936f7-115">تقديرات المشروع والقيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="936f7-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="936f7-116">فواتير المشروع</span><span class="sxs-lookup"><span data-stu-id="936f7-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="936f7-117">إدارة المصروفات</span><span class="sxs-lookup"><span data-stu-id="936f7-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="936f7-118">فاتورة المورّد</span><span class="sxs-lookup"><span data-stu-id="936f7-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
