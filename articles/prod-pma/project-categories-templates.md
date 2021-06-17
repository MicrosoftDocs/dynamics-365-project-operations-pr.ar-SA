---
title: مزامنة فئات مصروفات المشاريع بين Finance and Operations وProject Service Automation
description: يصف هذا الموضوع القوالب والمهام الأساسية المستخدمة لمزامنة فئات مصروفات المشروع بين Microsoft Dynamics 365 Finance وDynamics 365 Project Service Automation.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 2816d363dbfe6ef2d98a584b214f72d9b30c49bb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999835"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="9a4ad-103">مزامنة فئات مصروفات المشاريع بين Finance and Operations وProject Service Automation</span><span class="sxs-lookup"><span data-stu-id="9a4ad-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="9a4ad-104">يصف هذا الموضوع القوالب والمهام الأساسية المستخدمة لمزامنة فئات مصروفات المشروع بين Dynamics 365 Finance وDynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="9a4ad-105">يتوفر تكامل مهام المشروع ، وفئات حركات المصروفات ، وتقديرات الساعة ، وتقديرات المصروفات ، وتأمين الوظائف في الإصدار 8.0.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="9a4ad-106">القيم الفعلية المتكاملة متوفرة في الإصدار 8.0.1 أو أحدث.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="9a4ad-107">إذا كنت تستخدم إصدار Enterprise 7.3.0، بعد تثبيت قاعدة المعارف 4132657 وقاعدة المعارف 4132660، ستتمكن من استخدام القوالب لدمج مهام المشروع وفئات حركات المصروفات وتقديرات الساعات وتقديرات المصروفات والقيم الفعلية ولتكوين الوظائف قفل.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="9a4ad-108">إذا كان يجب عليك إعادة تعيين التوزيعات المحاسبية ، فننصحك أيضًا بتثبيت قاعدة المعارف 4131710.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="9a4ad-109">تدفق البيانات لـ Project Service Automation وFinance</span><span class="sxs-lookup"><span data-stu-id="9a4ad-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="9a4ad-110">يستخدم حل تكامل Project Service وFinance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Project Service Automation وFinance.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="9a4ad-111">تعمل قوالب التكامل المتوفرة مع ميزة تكامل البيانات على تمكين تدفق البيانات حول فئات حركات مصروفات المشروع بين Finance وProject Service Automation.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="9a4ad-112">إذا تم إتقان فئات مصروفات المشروع في Finance ، فسيكون تدفق التكامل أولاً من Finance إلى Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="9a4ad-113">يتم بعد ذلك تحديث معرّفات التكامل لفئات مصروفات المشروع من خلال المزامنة من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="9a4ad-114">إذا تم إتقان فئات مصروفات المشروع في Project Service Automation ، فسيكون تدفق التكامل أولاً من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="9a4ad-115">يجب تكوين فئات المشروع بالفعل في Finance قبل المزامنة من Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="9a4ad-116">ثم قم بالمزامنة من Finance مرة أخرى إلى Project Service Automation ، ثم من Project Service Automation إلى Finance مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="9a4ad-117">بهذه الطريقة ، فإنك تضمن أن الفئات مرتبطة ، وأنه لا يتم إنشاء أي تكرارات.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="9a4ad-118">عادةً ما يتم إتقان فئات مصروفات المشروع في Finance.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="9a4ad-119">ومع ذلك ، إذا لم تكن كذلك ، أو إذا تم بالفعل إنشاء فئات المصروفات في Project Service Automation ، فيجب عليك أولاً إجراء المزامنة باستخدام قالب فئات حركة مصروفات المشروع (PSA إلى Fin and Ops).</span><span class="sxs-lookup"><span data-stu-id="9a4ad-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="9a4ad-120">ثم قم بالمزامنة باستخدام قالب فئات معاملات مصروفات المشروع (Fin and Ops إلى PSA).</span><span class="sxs-lookup"><span data-stu-id="9a4ad-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="9a4ad-121">يجب عليك بعد ذلك تشغيل المزامنة من Project Service Automation إلى Finance مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="9a4ad-122">إذا أجريت المزامنة أولاً من Project Service Automation ، فيجب استيفاء المتطلبات التالية في Finance قبل تشغيل المزامنة:</span><span class="sxs-lookup"><span data-stu-id="9a4ad-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="9a4ad-123">يجب أن تكون الفئة المشتركة التي تطابق فئة المشروع التي تم إعدادها في Project Service Automation موجودة ، ويجب تمكينها لكل من **المشروع** و **المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="9a4ad-124">لكل كيان مالي قانوني يجب أن يتكامل معه ، يجب أن توجد فئات المشروع التالية:</span><span class="sxs-lookup"><span data-stu-id="9a4ad-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="9a4ad-125">**فئة المشروع** موجودة.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="9a4ad-126">تم تمكين **الاستخدام في المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="9a4ad-127">تم تمكين **نشط في دفتر اليومية**.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="9a4ad-128">تم تعيين **نوع الحركة** إلى **المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="9a4ad-129">يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات بين Project Service Automation وFinance.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="9a4ad-130">[![تدفق البيانات لتكامل Project Service Automation مع Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="9a4ad-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="9a4ad-131">مزامنة فئة مصروفات المشروع من Finance إلى Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="9a4ad-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="9a4ad-132">القالب والمهمة</span><span class="sxs-lookup"><span data-stu-id="9a4ad-132">Template and task</span></span>

<span data-ttu-id="9a4ad-133">للوصول إلى القالب، في مركز إدارة Microsoft Power Apps، حدد **المشاريع**، ثم في الركن الأيمن العلوي، حدد **مشروع جديد** لتحديد القوالب العامة.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-133">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="9a4ad-134">يتم استخدام القالب والمهمة الأساسية التالية لمزامنة فئات مصروفات المشروع من Finance إلى Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="9a4ad-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="9a4ad-135">**اسم القالب في تكامل البيانات:** فئات معاملات مصروفات المشروع (Fin and Ops إلى PSA)</span><span class="sxs-lookup"><span data-stu-id="9a4ad-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="9a4ad-136">**اسم المهمة في المشروع:** مزامنة الفئات إلى PSA</span><span class="sxs-lookup"><span data-stu-id="9a4ad-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="9a4ad-137">مجموعة الكيانات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-137">Entity set</span></span>

| <span data-ttu-id="9a4ad-138">التمويل</span><span class="sxs-lookup"><span data-stu-id="9a4ad-138">Finance</span></span>                           | <span data-ttu-id="9a4ad-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="9a4ad-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="9a4ad-140">كيان التكامل للفئات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-140">Integration entity for categories</span></span> | <span data-ttu-id="9a4ad-141">فئات المعاملات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="9a4ad-142">تدفق الكيانات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-142">Entity flow</span></span>

<span data-ttu-id="9a4ad-143">تتم إدارة فئات مصروفات المشروع في Finance ، وتتم مزامنتها مع Project Service Automation كفئات حركات.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="9a4ad-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="9a4ad-144">Power Query</span></span>

<span data-ttu-id="9a4ad-145">عندما تقوم بالمزامنة مع Project Service Automation ، يجب عليك استخدام Microsoft Power Query لـ Excel لتعيين نوع الفوترة في فئة الحركة.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="9a4ad-146">يوفر قالب فئات حركات مصروفات المشروع (Fin and Ops إلى PSA) عمودًا افتراضيًا وتعيينًا.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="9a4ad-147">إذا قمت بإنشاء القالب الخاص بك ، فيجب إضافة عمود شرطي في Power Query.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="9a4ad-148">اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-148">Follow these steps.</span></span>

1. <span data-ttu-id="9a4ad-149">انقر فوق السهم لفتح تعيين مهمة فئات مصروفات المشروع في قالب فئات حركات مصروفات المشروع (Fin and Ops إلى PSA).</span><span class="sxs-lookup"><span data-stu-id="9a4ad-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="9a4ad-150">انقر فوق ارتباط **الاستعلام المتقدم والتصفية** لفتح Power Query.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="9a4ad-151">حدد **إضافة العمود الشرطي**.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="9a4ad-152">أدخل اسمًا للعمود الجديد، مثل **نوع الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="9a4ad-153">أدخل الشرط التالي: **إذا كانت CATEGORYID لا تساوي قيمة خالية ، فسيكون 19235001 ، وإلا فسيكون فارغًا**.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="9a4ad-154">انقر فوق **موافق** في العمود.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="9a4ad-155">تاكد من تعيين هذا العمود الجديد في صفحه التعيين.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="9a4ad-156">يُظهر الرسم التوضيحي التالي مثالاً لتعيينات مهام القالب في تكامل البيانات.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="9a4ad-157">يُظهر التعيين معلومات الحقل التي ستتم مزامنتها من Finance إلى Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="9a4ad-158">[![تعيين فئة مصروفات المشروع إلى قالب Project Service Automation](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="9a4ad-158">[![Project expense category to Project Service Automation template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="9a4ad-159">مزامنة فئة مصروفات المشروع من Project Service Automation إلى Finance</span><span class="sxs-lookup"><span data-stu-id="9a4ad-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="9a4ad-160">القالب والمهمة</span><span class="sxs-lookup"><span data-stu-id="9a4ad-160">Template and task</span></span>

<span data-ttu-id="9a4ad-161">يتم استخدام القالب والمهمة الأساسية التالية لمزامنة فئات مصروفات المشروع من Project Service Automation إلى Finance:</span><span class="sxs-lookup"><span data-stu-id="9a4ad-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="9a4ad-162">**اسم القالب في تكامل البيانات:** فئات معاملات مصروفات المشروع (PSA إلى Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="9a4ad-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="9a4ad-163">**اسم المهمة في المشروع:** مزامنة الفئات إلى Fin Ops</span><span class="sxs-lookup"><span data-stu-id="9a4ad-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="9a4ad-164">مجموعة الكيانات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-164">Entity set</span></span>

| <span data-ttu-id="9a4ad-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="9a4ad-165">Project Service Automation</span></span> | <span data-ttu-id="9a4ad-166">التمويل</span><span class="sxs-lookup"><span data-stu-id="9a4ad-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="9a4ad-167">فئات المعاملات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-167">Transaction categories</span></span>     | <span data-ttu-id="9a4ad-168">كيان التكامل للفئات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="9a4ad-169">تدفق الكيانات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-169">Entity flow</span></span>

<span data-ttu-id="9a4ad-170">تتم إدارة فئات مصروفات المشروع في Finance ، وتتم مزامنتها مع Project Service Automation كفئات حركات.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="9a4ad-171">تعمل المزامنة مرة أخرى إلى Finance على تحديث فئة المشروع في Finance بمعرف التكامل من Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="9a4ad-172">تعيين القالب في تكامل البيانات</span><span class="sxs-lookup"><span data-stu-id="9a4ad-172">Template mapping in Data integration</span></span>

<span data-ttu-id="9a4ad-173">يُظهر الرسم التوضيحي التالي مثالاً لتعيينات مهام القالب في تكامل البيانات.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="9a4ad-174">يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.</span><span class="sxs-lookup"><span data-stu-id="9a4ad-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="9a4ad-175">[![تعيين Project Service Automation إلى قالب Finance](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="9a4ad-175">[![Project Service Automation to Finance template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]