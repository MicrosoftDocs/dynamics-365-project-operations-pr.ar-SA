---
title: الصفحة الرئيسية للتقارير
description: يقدم هذا الموضوع معلومات حول التقارير في Dynamics 365 Project Service Automation.
author: ruhercul
manager: kfend
ms.service: dynamics-365-projectservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: ee9bdfc6-123d-4146-8706-eab76fa37b5f
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 42e24f42fd80b445718f81f4ff40e52c8cdaa7ba
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748707"
---
# <a name="reporting-home-page"></a><span data-ttu-id="0f597-103">الصفحة الرئيسية للتقارير</span><span class="sxs-lookup"><span data-stu-id="0f597-103">Reporting home page</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="0f597-104">يتيح Microsoft Dynamics 365 Project Service Automation للمؤسسات المستندة إلى الشاريع إدارة عمليات أعمالها بكفاءة.</span><span class="sxs-lookup"><span data-stu-id="0f597-104">Microsoft Dynamics 365 Project Service Automation lets project-based organizations efficiently manage the operations of their business.</span></span> <span data-ttu-id="0f597-105">في أي مشروع، يجب أن يقوم أعضاء الفريق بإدارة الفرصة وعرض الأسعار وتخطيط العمل وإدارة العمل وفقًا للخطة وفاتورة العمل، ثم القيام بالعمل لإكمال المشروع.</span><span class="sxs-lookup"><span data-stu-id="0f597-105">On any project, team members must manage the opportunity, quote and plan the work, resource the projects, manage the work according to the plan, bill for the work, and then do the work to complete the project.</span></span> <span data-ttu-id="0f597-106">تعد القدرة على الإبلاغ عن العمليات أساسية لتحديد صحة المؤسسة واتخاذ أي إجراء تصحيحي مطلوب.</span><span class="sxs-lookup"><span data-stu-id="0f597-106">The ability to report on operations is key to determining the health of the organization and taking any corrective action that's required.</span></span> <span data-ttu-id="0f597-107">يقوم PSA باستخدام أساليب وتقنيات إعداد التقارير في Microsoft Dynamics 365 فيما يتعلق بجميع التقارير الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="0f597-107">PSA uses Microsoft Dynamics 365 reporting methods and technologies for all its reporting.</span></span> <span data-ttu-id="0f597-108">لمزيد من المعلومات حول الخيارات الخاصة بإعداد التقارير، راجع [دليل كتابة التقارير Dynamics 365 Customer Engagement (on-premises)، الإصدار 9](../analytics/reporting-analytics-with-dynamics-365.md).</span><span class="sxs-lookup"><span data-stu-id="0f597-108">For more information about the options for reporting, see the [Report writing guide for Dynamics 365 Customer Engagement (on-premises), version 9](../analytics/reporting-analytics-with-dynamics-365.md).</span></span>

## <a name="report-wizard"></a><span data-ttu-id="0f597-109">معالج التقارير</span><span class="sxs-lookup"><span data-stu-id="0f597-109">Report Wizard</span></span>

<span data-ttu-id="0f597-110">يتيح معالج التقارير للمطورين إنشاء تقارير بسيطة.</span><span class="sxs-lookup"><span data-stu-id="0f597-110">The Report Wizard lets non-developers create simple reports.</span></span> <span data-ttu-id="0f597-111">ونظرًا لأن التطبيق تم تصميمه في نظام أساسي موجود، فإن التجربة هي نفسها التي تم توثيقها في [إنشاء تقرير أو تحريره باستخدام معالج التقارير](../basics/create-edit-copy-report-wizard.md).</span><span class="sxs-lookup"><span data-stu-id="0f597-111">Because the app is built on an existing platform, the experience is the same as the experience that is documented in [Create or edit a report using the Report Wizard](../basics/create-edit-copy-report-wizard.md).</span></span> <span data-ttu-id="0f597-112">ومع ذلك، ستقوم باستخدام الكيانات الخاصة بـ Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="0f597-112">However, you will use the Project Service Automation-specific entities.</span></span>

## <a name="custom-sql-server-reporting-services-reports"></a><span data-ttu-id="0f597-113">تقارير خدمات التقارير المخصصة لخادم SQL</span><span class="sxs-lookup"><span data-stu-id="0f597-113">Custom SQL Server Reporting Services reports</span></span>

<span data-ttu-id="0f597-114">إذا كانت الأعمال تتطلب تقريرًا معينًا لا يمكن إنشاؤه باستخدام "معالج التقارير"، فيمكنك إنشاء تقرير مخصص.</span><span class="sxs-lookup"><span data-stu-id="0f597-114">If your business requires a specific report that can't be created by using the Report Wizard, you can create a custom report.</span></span> <span data-ttu-id="0f597-115">يجب أن يكون Microsoft Visual Studio مثبتًا لديك مع Microsoft SQL Server Data Tools وReport Authoring Extensions المناسبة.</span><span class="sxs-lookup"><span data-stu-id="0f597-115">You must have Microsoft Visual Studio installed, together with the appropriate Microsoft SQL Server Data Tools and Report Authoring Extensions.</span></span> <span data-ttu-id="0f597-116">لمزيد من المعلومات حول الأدوات والإصدارات، راجع [إعداد بيئة كتابة التقارير باستخدام SQL Server Data Tools](../analytics/report-writing-environment-using-sql-server-data-tools.md)</span><span class="sxs-lookup"><span data-stu-id="0f597-116">For more information about tools and versions, see [Report writing environment using SQL Server Data Tools](../analytics/report-writing-environment-using-sql-server-data-tools.md).</span></span> <span data-ttu-id="0f597-117">لمزيد من المعلومات حول كيفية إنشاء تقرير مخصص، راجع [إنشاء تقرير جديد باستخدام SQL Server Data Tools](../analytics/create-a-new-report-using-sql-server-data-tools.md).</span><span class="sxs-lookup"><span data-stu-id="0f597-117">For information about how to create a custom report, see [Create a new report using SQL Server Data Tools](../analytics/create-a-new-report-using-sql-server-data-tools.md).</span></span>

## <a name="power-bi-insights-apps"></a><span data-ttu-id="0f597-118">تطبيقات Power BI insights </span><span class="sxs-lookup"><span data-stu-id="0f597-118">Power BI insights apps</span></span>

<span data-ttu-id="0f597-119">يمنحك Microsoft Power BI وDynamics 365 معًا طريقة فعالية للعمل مع بياناتك، في شكل تطبيقات المعارف الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="0f597-119">Together, Microsoft Power BI and Dynamics 365 give you a powerful way to work with your data, in the form of insights apps.</span></span> <span data-ttu-id="0f597-120">للحصول على معلومات حول توفر تطبيقات المعارف الدقيقة، راجع [صفحة تطبيقات Power BI insights](https://powerbi.microsoft.com/power-bi-insights-apps/).</span><span class="sxs-lookup"><span data-stu-id="0f597-120">For information about the availability of insights apps, see the [Power BI insights apps page](https://powerbi.microsoft.com/power-bi-insights-apps/).</span></span>


## <a name="additional-resources"></a><span data-ttu-id="0f597-121">الموارد الإضافية</span><span class="sxs-lookup"><span data-stu-id="0f597-121">Additional resources</span></span>
<span data-ttu-id="0f597-122">لمزيد من المعلومات حول إعداد التقارير في PSA، راجع المواضيع التالية:</span><span class="sxs-lookup"><span data-stu-id="0f597-122">For more information about reporting in PSA, see the following topics:</span></span>

- [<span data-ttu-id="0f597-123">العمل مع نموذج بيانات Project Service</span><span class="sxs-lookup"><span data-stu-id="0f597-123">Working with the Project Service data model</span></span>](reports-working-project-service-data-model.md)
- [<span data-ttu-id="0f597-124">لوحات المعلومات</span><span class="sxs-lookup"><span data-stu-id="0f597-124">Dashboards</span></span>](reports-dashboards.md)

