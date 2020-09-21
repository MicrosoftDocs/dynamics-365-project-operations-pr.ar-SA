---
title: مزامنة تقديرات المشاريع مباشرة من Project Service Automation إلى Finance and Operations
description: يصف هذا الموضوع القوالب والمهام الأساسية المستخدمة لمزامنة تقديرات ساعات المشروع وتقديرات نفقات المشروع مباشرةً من Microsoft Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: d688ce9a-41e3-4ebe-952e-700f8351fbe9
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: a24a967d82c2e005e61234d34da8a583b61ff7b1
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748643"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="b0c7e-103">مزامنة تقديرات المشاريع مباشرة من Project Service Automation إلى Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="b0c7e-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="b0c7e-104">يصف هذا الموضوع القوالب والمهام الأساسية المستخدمة لمزامنة تقديرات ساعات المشروع وتقديرات نفقات المشروع مباشرةً من Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="b0c7e-105">يتوفر تكامل مهام المشروع ، وفئات حركات المصروفات ، وتقديرات الساعة ، وتقديرات المصروفات ، وتأمين الوظائف في الإصدار 8.0.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="b0c7e-106">القيم الفعلية المتكاملة متوفرة في الإصدار 8.0.1 أو أحدث.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="b0c7e-107">تدفق البيانات لـ Project Service Automation إلى Finance</span><span class="sxs-lookup"><span data-stu-id="b0c7e-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="b0c7e-108">يستخدم حل تكامل Project Service إلى Finance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Project Service Automation وFinance.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="b0c7e-109">تعمل قوالب التكامل المتوفرة مع ميزة تكامل البيانات على تمكين تدفق البيانات حول تقديرات ساعات المشروع وتقديرات نفقات المشروع من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="b0c7e-110">يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات بين Project Service Automation وFinance.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="b0c7e-111">[![تدفق البيانات لتكامل Project Service Automation مع Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="b0c7e-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="b0c7e-112">تقديرات ساعات المشاريع</span><span class="sxs-lookup"><span data-stu-id="b0c7e-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="b0c7e-113">القوالب والمهام</span><span class="sxs-lookup"><span data-stu-id="b0c7e-113">Template and tasks</span></span>

<span data-ttu-id="b0c7e-114">للوصول إلى القوالب المتوفرة، في مركز إدارة Microsoft Power Apps، حدد **المشاريع**، ثم في الركن الأيمن العلوي، حدد **مشروع جديد** لتحديد القوالب العامة.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="b0c7e-115">يتم استخدام القالب والمهام الأساسية التالية لمزامنة تقديرات ساعات المشروع من Project Service Automation إلى Finance:</span><span class="sxs-lookup"><span data-stu-id="b0c7e-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="b0c7e-116">**اسم القالب في تكامل البيانات:** تقديرات ساعات المشاريع (PSA إلى Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="b0c7e-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="b0c7e-117">**اسم المهام في المشروع:**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="b0c7e-118">علاقات الحركة</span><span class="sxs-lookup"><span data-stu-id="b0c7e-118">Transaction relationships</span></span>
    - <span data-ttu-id="b0c7e-119">تقديرات المصروفات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="b0c7e-120">مجموعة الكيانات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-120">Entity set</span></span>

| <span data-ttu-id="b0c7e-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="b0c7e-121">Project Service Automation</span></span> | <span data-ttu-id="b0c7e-122">التمويل</span><span class="sxs-lookup"><span data-stu-id="b0c7e-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="b0c7e-123">مهام المشروع</span><span class="sxs-lookup"><span data-stu-id="b0c7e-123">Project tasks</span></span>              | <span data-ttu-id="b0c7e-124">كيان التكامل لتقديرات ساعة المشروع</span><span class="sxs-lookup"><span data-stu-id="b0c7e-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="b0c7e-125">تدفق الكيانات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-125">Entity flow</span></span>

<span data-ttu-id="b0c7e-126">تتم إدارة تقديرات ساعات المشروع في Project Service Automation ، وتتم مزامنتها مع Finance كتوقعات ساعة المشروع.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="b0c7e-127">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="b0c7e-127">Prerequisites</span></span>

<span data-ttu-id="b0c7e-128">قبل ان تتم مزامنة تقديرات ساعات المشروع ، يتعين عليك مزامنة المشروعات ومهام المشروع وفئات حركات مصروفات المشروع.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="b0c7e-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="b0c7e-129">Power Query</span></span>

<span data-ttu-id="b0c7e-130">في قالب تقديرات الساعات للمشروع ، يجب استخدام Microsoft Power Query ل Excel لإكمال هذه المهام:</span><span class="sxs-lookup"><span data-stu-id="b0c7e-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="b0c7e-131">قم بتعيين معرف نموذج التنبؤ الافتراضي الذي سيتم استخدامه عندما يقوم التكامل بإنشاء تنبؤات جديده بالساعات.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="b0c7e-132">يقوم بتصفية إيه سجلات خاصه بالموارد في المهمة التي ستؤدي إلى التكامل في التنبؤ بالساعات.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="b0c7e-133">تصفيه إيه صفوف فئات حركات فارغه.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="b0c7e-134">قد ينتج عن الفشل في إكمال هذه المهمة تنبؤات بالساعة غير صحيحه.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="b0c7e-135">تعيين معرف نموذج التنبؤ الافتراضي</span><span class="sxs-lookup"><span data-stu-id="b0c7e-135">Set the default forecast model ID</span></span>

<span data-ttu-id="b0c7e-136">لتحديث معرف نموذج التنبؤ الافتراضي في القالب ، انقر فوق سهم **التعيين** لفتح التعيين.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="b0c7e-137">ثم حدد ارتباط **الاستعلام المتقدم والتصفية**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="b0c7e-138">إذا كنت تستخدم قالب تقديرات ساعات المشروع الافتراضية (PSA إلى Fin and Ops)، فحدد **الشرط المدرج** في قائمة **الخطوات المطبقة**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="b0c7e-139">في إدخال **الوظيفة**، استبدل **O\_التنبؤ** باسم معرف نموذج التنبؤ الذي يجب استخدامه مع التكامل.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="b0c7e-140">يحتوي القالب الافتراضي علي معرف نموذج تنبؤ من بيانات العرض التوضيحي.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="b0c7e-141">إذا كنت تقوم بإنشاء قالب جديد ، فيجب عليك أضافه هذا العمود.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="b0c7e-142">في Power Query، حدد **إضافه عمود شرطي**، وادخل اسما للعمود الجديد، مثل **معرف النموذج**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-142">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="b0c7e-143">أدخل الشرط للعمود ، حيث ، إذا لم تكن مهمة المشروع فارغه، \<فأدخل معرف نموذج التنبؤ\>؛ قيمه فارغة أخرى.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="b0c7e-144">تصفيه السجلات الخاصة بالمورد</span><span class="sxs-lookup"><span data-stu-id="b0c7e-144">Filter out resource-specific records</span></span>

<span data-ttu-id="b0c7e-145">يحتوي نموذج تقديرات ساعات المشروع (PSA إلى Fin and Ops) على عامل تصفية افتراضي يزيل أي سجلات خاصة بالموارد.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="b0c7e-146">إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة عامل التصفية هذا.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="b0c7e-147">حدد ارتباط **الاستعلام المتقدم والتصفية** للتصفية في عمود **msdyn\_islinetask** بحيث يتم تضمين السجلات **الزائفة** فقط.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="b0c7e-148">تصفيه صفوف فئات حركات فارغه</span><span class="sxs-lookup"><span data-stu-id="b0c7e-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="b0c7e-149">يجب أضافه عامل تصفيه لأزاله إيه صفوف تشتمل علي فئات حركات فارغه.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="b0c7e-150">هذه المهمة مطلوبه ، بغض النظر عما إذا كنت تستخدم القالب الافتراضي أو إنشاء قالب خاص بك.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="b0c7e-151">يقوم عامل التصفية هذا بازاله أي صفوف ملخص من Project Service Automation والذي قد يتسبب في عدم صحة تنبؤات الساعات في Finance.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="b0c7e-152">حدد ارتباط **الاستعلام المتقدم والتصفية** لتصفية السجلات الفارغة في عمود **msdyn\_transactioncategory\_القيمة**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="b0c7e-153">تعيين القالب في تكامل البيانات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-153">Template mapping in Data integration</span></span>

<span data-ttu-id="b0c7e-154">يُظهر الرسم التوضيحي التالي مثالاً لتعيينات مهام القالب في تكامل البيانات.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="b0c7e-155">يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="b0c7e-156">[![تعيين القالب](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="b0c7e-156">[![Template mapping](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="b0c7e-157">تقديرات مصروفات المشاريع</span><span class="sxs-lookup"><span data-stu-id="b0c7e-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="b0c7e-158">القوالب والمهام</span><span class="sxs-lookup"><span data-stu-id="b0c7e-158">Template and tasks</span></span>

<span data-ttu-id="b0c7e-159">يتم استخدام القالب والمهام الأساسية التالية لمزامنة تقديرات مصروفات المشروع من Project Service Automation إلى Finance:</span><span class="sxs-lookup"><span data-stu-id="b0c7e-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="b0c7e-160">**اسم القالب في تكامل البيانات:** تقديرات مصروفات المشاريع (PSA إلى Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="b0c7e-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="b0c7e-161">**اسم المهام في المشروع:**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="b0c7e-162">علاقات الحركة</span><span class="sxs-lookup"><span data-stu-id="b0c7e-162">Transaction relationships</span></span> 
    - <span data-ttu-id="b0c7e-163">تقديرات المصروفات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="b0c7e-164">مجموعة الكيانات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-164">Entity set</span></span>

| <span data-ttu-id="b0c7e-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="b0c7e-165">Project Service Automation</span></span> | <span data-ttu-id="b0c7e-166">التمويل</span><span class="sxs-lookup"><span data-stu-id="b0c7e-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="b0c7e-167">اتصالات المعاملات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-167">Transaction Connections</span></span>    | <span data-ttu-id="b0c7e-168">كيان التكامل لعلاقات معاملات المشروع</span><span class="sxs-lookup"><span data-stu-id="b0c7e-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="b0c7e-169">بنود التقدير</span><span class="sxs-lookup"><span data-stu-id="b0c7e-169">Estimate Lines</span></span>             | <span data-ttu-id="b0c7e-170">كيان التكامل لتقديرات مصروفات المشاريع</span><span class="sxs-lookup"><span data-stu-id="b0c7e-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="b0c7e-171">تدفق الكيانات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-171">Entity flow</span></span>

<span data-ttu-id="b0c7e-172">تتم إدارة تقديرات مصروفات المشاريع في Project Service Automation ، وتتم مزامنتها مع Finance كتوقعات مصروفات المشاريع.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="b0c7e-173">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="b0c7e-173">Prerequisites</span></span>

<span data-ttu-id="b0c7e-174">قبل ان تتم مزامنة تقديرات مصروفات المشروع ، يتعين عليك مزامنة المشروعات ومهام المشروع وفئات حركات مصروفات المشروع.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="b0c7e-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="b0c7e-175">Power Query</span></span>

<span data-ttu-id="b0c7e-176">في قالب تقديرات مصروفات المشروع ، يجب عليك استخدام Power Query لإكمال المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="b0c7e-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="b0c7e-177">تصفيه لتضمين سجلات سطور التقدير للمصروفات فقط.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="b0c7e-178">قم بتعيين معرف نموذج التنبؤ الافتراضي الذي سيتم استخدامه عندما يقوم التكامل بإنشاء تنبؤات جديده بالساعات.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="b0c7e-179">تحويل أنواع الفواتير.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-179">Transform the billing types.</span></span>
- <span data-ttu-id="b0c7e-180">تحويل أنواع الحركات.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="b0c7e-181">تصفيه لتضمين سطور التقدير للمصروفات فقط.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="b0c7e-182">يحتوي قالب تقديرات مصروفات المشروع (PSA إلى Fin and Ops) على عامل تصفية افتراضي يتضمن فقط بنود المصروفات في التكامل.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="b0c7e-183">إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة عامل التصفية هذا.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="b0c7e-184">حدد مهمة **علاقات الحركات**، ثم انقر فوق سهم **التعيين** لفتح التعيين.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="b0c7e-185">حدد ارتباط **الاستعلام المتقدم والتصفية**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="b0c7e-186">قم بتصفية عمود **msdyn\_transactiontype1** بحيث يتضمن **msdyn\_estimateline** فقط.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="b0c7e-187">تعيين معرف نموذج التنبؤ الافتراضي</span><span class="sxs-lookup"><span data-stu-id="b0c7e-187">Set the default forecast model ID</span></span>

<span data-ttu-id="b0c7e-188">لتحديث معرف نموذج التنبؤ الافتراضي في القالب، فحدد **تقديرات المصروفات**، ثم انقر فوق سهم **التعيين** لفتح التعيين.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="b0c7e-189">حدد ارتباط **الاستعلام المتقدم والتصفية**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="b0c7e-190">إذا كنت تستخدم القالب الافتراضي لتقديرات مصروفات المشروع (PSA إلى Fin and Ops) ، في Power Query ، حدد **الشرط المدرج** الأول من قسم **الخطوات المطبقة**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="b0c7e-191">في إدخال **الوظيفة**، استبدل **O\_التنبؤ** باسم معرف نموذج التنبؤ الذي يجب استخدامه مع التكامل.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="b0c7e-192">يحتوي القالب الافتراضي علي معرف نموذج تنبؤ من بيانات العرض التوضيحي.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="b0c7e-193">إذا كنت تقوم بإنشاء قالب جديد ، فيجب عليك أضافه هذا العمود.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="b0c7e-194">في Power Query، حدد **إضافه عمود شرطي**، وادخل اسما للعمود الجديد، مثل **معرف النموذج**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-194">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="b0c7e-195">أدخل الشرط للعمود ، حيث ، إذا لم يكن معرف سطر التقدير فارغًا، \<فأدخل معرف نموذج التنبؤ\>؛ قيمه فارغة أخرى.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="b0c7e-196">تحويل أنواع الفواتير</span><span class="sxs-lookup"><span data-stu-id="b0c7e-196">Transform the billing types</span></span>

<span data-ttu-id="b0c7e-197">يتضمن قالب تقديرات مصروفات المشروع (PSA إلى Fin and Ops) عمودًا شرطيًا يتم استخدامه لتحويل أنواع الفواتير التي يتم استلامها من Project Service Automation أثناء التكامل.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="b0c7e-198">إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة هذا العمود الشرطي.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="b0c7e-199">حدد ارتباط **الاستعلام المتقدم والتصفية** ثم حدد **إضافة عمود شرطي**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="b0c7e-200">أدخل اسمًا للعمود الجديد، مثل **نوع الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="b0c7e-201">ثم أدخل الشرط التالي:</span><span class="sxs-lookup"><span data-stu-id="b0c7e-201">Then enter the following condition:</span></span>

<span data-ttu-id="b0c7e-202">في حالة **msdyn\_billingtype** = 192350000، إذن **NonChargeable**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="b0c7e-203">وإلا إذا **msdyn\_billingtype** = 192350001، إذن **Chargeable**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="b0c7e-204">وإلا إذا **msdyn\_billingtype** = 192350002، إذن **Chargeable**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="b0c7e-205">وإلا **NotAvailable**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="b0c7e-206">تحويل أنواع الحركات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-206">Transform the transaction types</span></span>

<span data-ttu-id="b0c7e-207">يتضمن قالب تقديرات مصروفات المشروع (PSA إلى Fin and Ops) عمودًا شرطيًا يتم استخدامه لتحويل أنواع الحركات التي يتم استلامها من Project Service Automation أثناء التكامل.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="b0c7e-208">إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة هذا العمود الشرطي.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="b0c7e-209">حدد ارتباط **الاستعلام المتقدم والتصفية** ثم حدد **إضافة عمود شرطي**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="b0c7e-210">أدخل اسمًا للعمود الجديد، مثل **نوع الحركة**.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="b0c7e-211">ثم أدخل الشرط التالي:</span><span class="sxs-lookup"><span data-stu-id="b0c7e-211">Then enter the following condition:</span></span>

<span data-ttu-id="b0c7e-212">في حالة **msdyn\_transactiontypecode** = 192350000، إذن **التكلفة**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="b0c7e-213">وإلا إذا **msdyn\_transactiontypecode** = 192350005، إذن **المبيعات**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="b0c7e-214">وإلا **فارغ**</span><span class="sxs-lookup"><span data-stu-id="b0c7e-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="b0c7e-215">تعيين القالب في تكامل البيانات</span><span class="sxs-lookup"><span data-stu-id="b0c7e-215">Template mapping in Data integration</span></span>

<span data-ttu-id="b0c7e-216">توضح الرسوم التوضيحية التالية أمثلة لتعيينات مهام القالب في تكامل البيانات.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="b0c7e-217">يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="b0c7e-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="b0c7e-218">[![تعيين القالب](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="b0c7e-218">[![Template mapping](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="b0c7e-219">[![تعيين القالب](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="b0c7e-219">[![Template mapping](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>
