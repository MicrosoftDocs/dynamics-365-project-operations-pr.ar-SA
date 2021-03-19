---
title: الصفحة الرئيسية للتقارير
description: يقدم هذا الموضوع معلومات حول التقارير في Dynamics 365 Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 78c62f69c6529669789a461f1ded8e3ea5f8219e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283262"
---
# <a name="reporting-home-page"></a><span data-ttu-id="17943-103">الصفحة الرئيسية لإعداد التقارير</span><span class="sxs-lookup"><span data-stu-id="17943-103">Reporting home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="17943-104">يسمح Microsoft Dynamics 365 Project Service Automation للمؤسسات المستندة إلى المشاريع بإدارة عمليات أعمالها بكفاءة.</span><span class="sxs-lookup"><span data-stu-id="17943-104">Microsoft Dynamics 365 Project Service Automation lets project-based organizations efficiently manage the operations of their business.</span></span> <span data-ttu-id="17943-105">في أي مشروع، يجب أن يقوم أعضاء الفريق بإدارة الفرصة وعرض الأسعار وتخطيط العمل وإدارة العمل وفقًا للخطة وفاتورة العمل، ثم القيام بالعمل لإكمال المشروع.</span><span class="sxs-lookup"><span data-stu-id="17943-105">On any project, team members must manage the opportunity, quote and plan the work, resource the projects, manage the work according to the plan, bill for the work, and then do the work to complete the project.</span></span> <span data-ttu-id="17943-106">تعد القدرة على الإبلاغ عن العمليات أساسية لتحديد صحة المؤسسة واتخاذ أي إجراء تصحيحي مطلوب.</span><span class="sxs-lookup"><span data-stu-id="17943-106">The ability to report on operations is key to determining the health of the organization and taking any corrective action that's required.</span></span> <span data-ttu-id="17943-107">يقوم PSA باستخدام أساليب وتقنيات إعداد التقارير في Microsoft Dynamics 365 فيما يتعلق بجميع التقارير الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="17943-107">PSA uses Microsoft Dynamics 365 reporting methods and technologies for all its reporting.</span></span> <span data-ttu-id="17943-108">لمزيد من المعلومات حول الخيارات الخاصة بإعداد التقارير، راجع [دليل كتابة التقارير Dynamics 365 Customer Engagement (on-premises)، الإصدار 9](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span><span class="sxs-lookup"><span data-stu-id="17943-108">For more information about the options for reporting, see the [Report writing guide for Dynamics 365 Customer Engagement (on-premises), version 9](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span></span>

## <a name="report-wizard"></a><span data-ttu-id="17943-109">معالج التقارير</span><span class="sxs-lookup"><span data-stu-id="17943-109">Report Wizard</span></span>

<span data-ttu-id="17943-110">يتيح معالج التقارير للمطورين إنشاء تقارير بسيطة.</span><span class="sxs-lookup"><span data-stu-id="17943-110">The Report Wizard lets non-developers create simple reports.</span></span> <span data-ttu-id="17943-111">ونظرًا لأن التطبيق تم تصميمه في نظام أساسي موجود، فإن التجربة هي نفسها التي تم توثيقها في [إنشاء تقرير أو تحريره باستخدام معالج التقارير](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span><span class="sxs-lookup"><span data-stu-id="17943-111">Because the app is built on an existing platform, the experience is the same as the experience that is documented in [Create or edit a report using the Report Wizard](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span></span> <span data-ttu-id="17943-112">ومع ذلك، ستقوم باستخدام الكيانات الخاصة بـ Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="17943-112">However, you will use the Project Service Automation-specific entities.</span></span>

## <a name="custom-sql-server-reporting-services-reports"></a><span data-ttu-id="17943-113">تقارير خدمات التقارير المخصصة لخادم SQL</span><span class="sxs-lookup"><span data-stu-id="17943-113">Custom SQL Server Reporting Services reports</span></span>

<span data-ttu-id="17943-114">إذا كانت الأعمال تتطلب تقريرًا معينًا لا يمكن إنشاؤه باستخدام "معالج التقارير"، فيمكنك إنشاء تقرير مخصص.</span><span class="sxs-lookup"><span data-stu-id="17943-114">If your business requires a specific report that can't be created by using the Report Wizard, you can create a custom report.</span></span> <span data-ttu-id="17943-115">يجب أن يكون Microsoft Visual Studio مثبتًا لديك مع Microsoft SQL Server Data Tools وReport Authoring Extensions المناسبة.</span><span class="sxs-lookup"><span data-stu-id="17943-115">You must have Microsoft Visual Studio installed, together with the appropriate Microsoft SQL Server Data Tools and Report Authoring Extensions.</span></span> <span data-ttu-id="17943-116">لمزيد من المعلومات حول الأدوات والإصدارات، راجع [إعداد بيئة كتابة التقارير باستخدام SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools)</span><span class="sxs-lookup"><span data-stu-id="17943-116">For more information about tools and versions, see [Report writing environment using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span></span> <span data-ttu-id="17943-117">لمزيد من المعلومات حول كيفية إنشاء تقرير مخصص، راجع [إنشاء تقرير جديد باستخدام SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="17943-117">For information about how to create a custom report, see [Create a new report using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span></span>

## <a name="power-bi-insights-apps"></a><span data-ttu-id="17943-118">تطبيقات Power BI insights </span><span class="sxs-lookup"><span data-stu-id="17943-118">Power BI insights apps</span></span>

<span data-ttu-id="17943-119">يمنحك كل من Microsoft Power BI وDynamics 365 طريقة فعالة للعمل مع بياناتك، على شكل تطبيقات المعارف الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="17943-119">Together, Microsoft Power BI and Dynamics 365 give you a powerful way to work with your data, in the form of insights apps.</span></span> <span data-ttu-id="17943-120">للحصول على معلومات حول توفر تطبيقات المعارف الدقيقة، راجع [صفحة تطبيقات Power BI insights](https://powerbi.microsoft.com/power-bi-insights-apps/).</span><span class="sxs-lookup"><span data-stu-id="17943-120">For information about the availability of insights apps, see the [Power BI insights apps page](https://powerbi.microsoft.com/power-bi-insights-apps/).</span></span>


## <a name="additional-resources"></a><span data-ttu-id="17943-121">الموارد الإضافية</span><span class="sxs-lookup"><span data-stu-id="17943-121">Additional resources</span></span>
<span data-ttu-id="17943-122">لمزيد من المعلومات حول إعداد التقارير في PSA، راجع المواضيع التالية:</span><span class="sxs-lookup"><span data-stu-id="17943-122">For more information about reporting in PSA, see the following topics:</span></span>

- [<span data-ttu-id="17943-123">العمل مع نموذج بيانات Project Service</span><span class="sxs-lookup"><span data-stu-id="17943-123">Working with the Project Service data model</span></span>](reports-working-project-service-data-model.md)
- [<span data-ttu-id="17943-124">لوحات المعلومات</span><span class="sxs-lookup"><span data-stu-id="17943-124">Dashboards</span></span>](reports-dashboards.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]