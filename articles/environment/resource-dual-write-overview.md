---
title: تكامل ‏‫الكتابة المزدوجة في Project Operations
description: يوفر هذا موضوع نظرة عامة على تكامل الكتابة المزدوجة في Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ce4f7bf8185e6f3f942df14d30d7b8d0a3e4444a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998665"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="22058-103">نظرة عامة حول تكامل ‏‫الكتابة المزدوجة في Project Operations</span><span class="sxs-lookup"><span data-stu-id="22058-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="22058-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="22058-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="22058-105">يستخدم Project Operations [إمكانات الكتابة المزدوجة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) لمزامنة البيانات عبر Microsoft Dataverse وDynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="22058-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="22058-106">يوضح الشكل التوضيحي التالي كيفية مزامنة البيانات كجزء من هذا التكامل بين Dataverse وFinance.</span><span class="sxs-lookup"><span data-stu-id="22058-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![نظرة عامة حول تدفقات بيانات Project Operations](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="22058-108">توفر Project Operations في Dataverse واجهة مستخدم حديثة وقابلة للتوسع بسهولة بدون تعليمات برمجية/بتعمليات برمجية طفيفة باستخدام إمكانات Power Platform.</span><span class="sxs-lookup"><span data-stu-id="22058-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="22058-109">ويمكن لمديري المشروع ومديري الموارد وأعضاء فريق المشروع وموظفي المكتب الأمامي الآخرين، تنفيذ أنشطتهم في Project Operations على Dataverse.</span><span class="sxs-lookup"><span data-stu-id="22058-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="22058-110">يوفر Project Operations في Finance دعم محاسبة المشروع وتقدير الإيرادات.</span><span class="sxs-lookup"><span data-stu-id="22058-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="22058-111">يتم ربط Project Operations بإطار العمل المالي في Finance لحساب ضريبة المبيعات وأسعار صرف العملات ورفع تقارير بالأبعاد المالية وغير ذلك.</span><span class="sxs-lookup"><span data-stu-id="22058-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="22058-112">تعتمد تجارب محاسب المشروع في الغالب على Finance.</span><span class="sxs-lookup"><span data-stu-id="22058-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="22058-113">يتكون تكامل Project Operations من تكامل المكون التالي:</span><span class="sxs-lookup"><span data-stu-id="22058-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="22058-114">تكامل بيانات التكوين والإعداد في Project Operations</span><span class="sxs-lookup"><span data-stu-id="22058-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="22058-115">تقديرات المشروع والقيم الفعلية</span><span class="sxs-lookup"><span data-stu-id="22058-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="22058-116">فواتير المشروع</span><span class="sxs-lookup"><span data-stu-id="22058-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="22058-117">إدارة المصروفات</span><span class="sxs-lookup"><span data-stu-id="22058-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="22058-118">فاتورة المورّد</span><span class="sxs-lookup"><span data-stu-id="22058-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
