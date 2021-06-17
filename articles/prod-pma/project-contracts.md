---
title: عقود المشاريع
description: يقدم هذا الموضوع أمثله علي عقود المشروع التي يمكنك إنشاؤها لأنواع مختلفه من المشروعات ومصادر التمويل ، وكيف يمكنك أداره العقود وعملاء المشروع الفواتير.
author: Yowelle
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a794ec38ac07c1418f9e95b741941a83492bb3d5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999745"
---
# <a name="project-contracts"></a><span data-ttu-id="f8652-103">عقود المشاريع</span><span class="sxs-lookup"><span data-stu-id="f8652-103">Project contracts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="f8652-104">تقدم هذه المقالة أمثله علي عقود المشروع التي يمكنك إنشاؤها لأنواع مختلفه من المشروعات ومصادر التمويل ، وكيف يمكنك أداره العقود وعملاء المشروع الفواتير.</span><span class="sxs-lookup"><span data-stu-id="f8652-104">This article provides examples of the project contracts that you can create for various types of projects and funding sources, and how you can manage contracts and invoice project customers.</span></span>

<span data-ttu-id="f8652-105">نوع المشروع الذي تقوم بإنشاءه لعقد مشروع يحدد الطريقة التي يتم استخدامها لفوترة عملاء المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-105">The type of project that you create for a project contract determines the method that is used to invoice project customers.</span></span> <span data-ttu-id="f8652-106">يمكنك تغيير عقد مشروع والمشروع المرتبط به ، ولكن لا يمكنك تغيير نوع المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-106">You can change a project contract and the related project, but you can't change the project type.</span></span> 

<span data-ttu-id="f8652-107">باستخدام عقد مشروع ، يمكنك فوتره مشروع واحد أو أكثر في نفس الوقت.</span><span class="sxs-lookup"><span data-stu-id="f8652-107">By using a project contract, you can invoice one or more projects at the same time.</span></span> <span data-ttu-id="f8652-108">كما يساعد عقد المشروع علي ضمان اتساق إجراء فوتره لكل مشروع فرعي في بنيه مشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-108">The project contract also helps guarantee a consistent invoicing procedure for every subproject in a project structure.</span></span> 

<span data-ttu-id="f8652-109">يجب ان يكون كل مشروع ستتم فوترته مقترنا بعقد مشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-109">Every project that will be invoiced must be associated with a project contract.</span></span> <span data-ttu-id="f8652-110">تنطبق إعدادات عقد المشروع علي كافة المشروعات والمشاريع الفرعية المرتبطة بعقد المشروع هذا.</span><span class="sxs-lookup"><span data-stu-id="f8652-110">The settings for a project contract apply to all projects and subprojects that are associated with that project contract.</span></span> 

<span data-ttu-id="f8652-111">يستطيع عقد المشروع تحديد مصدر واحد أو أكثر من مصادر التمويل.</span><span class="sxs-lookup"><span data-stu-id="f8652-111">A project contract can specify one or more sources of funding.</span></span> <span data-ttu-id="f8652-112">التالي ، يمكنك تقسيم الفوترة بين العديد من الممولين المتعددة ، واعداد حدود التمويل بحيث لا تتم فوتره مصادر التمويل أكثر من مبلغ محدد ، وتكوين قواعد التمويل لشحن النفقات.</span><span class="sxs-lookup"><span data-stu-id="f8652-112">Therefore, you can split the billing among multiple funders, set up funding limits so that funding sources are not billed more than a specified amount, and configure funding rules for charging expenditures.</span></span>

## <a name="funding-for-project-contracts"></a><span data-ttu-id="f8652-113">تمويل عقود المشروع</span><span class="sxs-lookup"><span data-stu-id="f8652-113">Funding for project contracts</span></span>
<span data-ttu-id="f8652-114">وتحدد بعض عقود المشروعات التي تشترك فيها العديد من المسئولية في تمويل تكاليف المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-114">Some project contracts specify that multiple parties share the responsibility for funding the project costs.</span></span> <span data-ttu-id="f8652-115">وإليك بعض الأمثلة:</span><span class="sxs-lookup"><span data-stu-id="f8652-115">Here are some examples:</span></span>

-   <span data-ttu-id="f8652-116">العميل الكبير الذي يحتوي علي العديد من طلبات الأقسام يتم تقسيم أموال المشروع حسب القسم.</span><span class="sxs-lookup"><span data-stu-id="f8652-116">A large customer that has multiple divisions requests that funding of a project be split by division.</span></span>
-   <span data-ttu-id="f8652-117">تشترك شركتك في تكاليف مشروع كبير مع مؤسسه خارجيه.</span><span class="sxs-lookup"><span data-stu-id="f8652-117">Your company shares the costs of a large project with an external organization.</span></span>
-   <span data-ttu-id="f8652-118">يتم تمويل مشروع الطريق بشكل مشترك من قبل بلديتين.</span><span class="sxs-lookup"><span data-stu-id="f8652-118">A  road project is co-funded by two municipalities.</span></span>
-   <span data-ttu-id="f8652-119">مشروع الجسر ممول بمنحة حكومية ومؤسسة خاصة.</span><span class="sxs-lookup"><span data-stu-id="f8652-119">A bridge project is funded by a government grant and a private corporation.</span></span>

<span data-ttu-id="f8652-120">في Dynamics 365 Finance، يمكنك تقسيم الفواتير لعمليه واحده أو مشروع بالكامل بين العديد من العملاء أو المنح أو المؤسسات.</span><span class="sxs-lookup"><span data-stu-id="f8652-120">In Dynamics 365 Finance, you can split the billing for a single transaction or an entire project among multiple customers, grants, or organizations.</span></span> 

<span data-ttu-id="f8652-121">في المشاريع التي لديها ممولين متعددين ، تسمى جميع الأطراف التي تساهم في تمويل مشروع تمويل متقدم مصادر التمويل.</span><span class="sxs-lookup"><span data-stu-id="f8652-121">In projects that have multiple funders, all parties that contribute to the funding of an advanced funding project are called funding sources.</span></span> <span data-ttu-id="f8652-122">وبعد تحديد عميل أو مؤسسه أو منحه كمصدر تمويل ، يمكن تعيينها لقاعده تمويل واحده أو أكثر.</span><span class="sxs-lookup"><span data-stu-id="f8652-122">After a customer, organization, or grant is defined as a funding source, it can be assigned to one or more funding rules.</span></span> <span data-ttu-id="f8652-123">تحتوي قواعد التمويل علي المعايير التي تحدد كيفيه تخصيص المصاريف لمصادر التمويل المختلفة الخاصة بأحد المشاريع.</span><span class="sxs-lookup"><span data-stu-id="f8652-123">Funding rules contain the criteria that determines how charges are allocated to the various funding sources for a project.</span></span> 

<span data-ttu-id="f8652-124">ولأنه لا يمكن تقسيم الأصناف المخزنة ، مثل تلك التي تظهر علي طلبات الشراء وأوامر الشراء ، الا انه لا يمكن تقسيم مبلغ التكلفة بين مصادر تمويل متعددة في وقت التوزيع.</span><span class="sxs-lookup"><span data-stu-id="f8652-124">Because stocked items, such as those that appear on purchase requisitions and purchase orders, can't be split, the cost amount can't be split among multiple funding sources at the time of distribution.</span></span> <span data-ttu-id="f8652-125">لذا ، تبقي قيمه مصدر التمويل 0 (صفر) إلى ان يتم ترحيل إصدار المخزون.</span><span class="sxs-lookup"><span data-stu-id="f8652-125">Therefore, the funding source value remains 0 (zero) until the inventory issue is posted.</span></span> <span data-ttu-id="f8652-126">عند ترحيل إصدار المخزون ، يتم توزيع مبلغ التكلفة وفقا لقواعد توزيع الحساب الخاصة بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-126">When the inventory issue is posted, the cost amount is distributed according to the account distribution rules for the project.</span></span>

<span data-ttu-id="f8652-127">فيما يلي بعض الخطوات التي يمكنك اتخاذها لتسهيل تقسيم الفواتير بين مصادر تمويل متعددة:</span><span class="sxs-lookup"><span data-stu-id="f8652-127">Here are some steps that you can take to make it easier to split the billing among multiple funding sources:</span></span>

-   <span data-ttu-id="f8652-128">حدد ان تكون كافة الحركات التي تم إدخالها لمشروع تستخدم نفس عمله المبيعات التي يستخدمها عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-128">Specify that all transactions that are entered for a project use the same sales currency as the project contract.</span></span>
-   <span data-ttu-id="f8652-129">اعداد حدود التمويل ، بحيث لا تتم فوتره مصدر التمويل أكثر من مبلغ محدد نحو مشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-129">Set up funding limits, so that a funding source isn't invoiced more than a specified amount toward a project.</span></span>
-   <span data-ttu-id="f8652-130">تكوين قواعد التمويل وحدود التمويل لكل عامل ، وصنف ، وفئة ، ومجموعه فئة ، ونوع حركه (أو لكافة أنواع الحركات).</span><span class="sxs-lookup"><span data-stu-id="f8652-130">Configure funding rules and funding limits for each worker, item, category, category group, and transaction type (or for all transaction types).</span></span>
-   <span data-ttu-id="f8652-131">حدد تواريخ البدء والانتهاء الاختيارية لتحديد الفترة الزمنية التي تكون فيها كل قاعده تمويل صالحه.</span><span class="sxs-lookup"><span data-stu-id="f8652-131">Select optional start and end dates to define the period when each funding rule is valid.</span></span>
-   <span data-ttu-id="f8652-132">حدد النسبة المئوية التي يكون كل مصدر تمويل مسؤولا عنها.</span><span class="sxs-lookup"><span data-stu-id="f8652-132">Specify the percentage that each funding source is responsible for.</span></span>
-   <span data-ttu-id="f8652-133">حدد مصدر التمويل المسؤول عن الفروق التقريبية التي تنتج عن حسابات تخصيص التمويل.</span><span class="sxs-lookup"><span data-stu-id="f8652-133">Specify which funding source is responsible for rounding differences that are caused by funding allocation calculations.</span></span>
-   <span data-ttu-id="f8652-134">قم باعداد القواعد التي تحدد كيفيه فوتره تكاليف المشروع إلى العملاء الخارجيين ويتم تحميلها إلى المؤسسات الداخلية.</span><span class="sxs-lookup"><span data-stu-id="f8652-134">Set up rules that determine how project costs are invoiced to external customers and charged to internal organizations.</span></span>
-   <span data-ttu-id="f8652-135">قم بتسجيل الحركات في حساب تمويل في القائمة حتى يمكن الحصول علي أموال اضافيه ، أو حتى تقرر تحمل التكاليف داخليا.</span><span class="sxs-lookup"><span data-stu-id="f8652-135">Record transactions in an on-hold funding account until additional funding can be obtained, or until you decide to bear the costs internally.</span></span>

<span data-ttu-id="f8652-136">لتحديد مجموعه الضرائب التي سيتم اقرانها بأحدي الحركات ، يتم البحث في المشروع عن تعيين مجموعه ضريبة.</span><span class="sxs-lookup"><span data-stu-id="f8652-136">To determine which tax group to associate with a transaction, the project is searched for a tax group assignment.</span></span> <span data-ttu-id="f8652-137">إذا لم يتم تعيين اي مجموعه ضرائب علي مستوي المشروع ، سيتم البحث في عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-137">If no tax group assignment has been made at the project level, the project contract is searched.</span></span>

### <a name="example-multiple-funding-sources-simple"></a><span data-ttu-id="f8652-138">مثال: مصادر تمويل متعددة (بسيطه)</span><span class="sxs-lookup"><span data-stu-id="f8652-138">Example: Multiple funding sources (simple)</span></span>

<span data-ttu-id="f8652-139">يوفر الجدول التالي سيناريوهات أداره توزيع التمويل بين مصادر التمويل المتعددة.</span><span class="sxs-lookup"><span data-stu-id="f8652-139">The following table provides scenarios for managing funding allocation among multiple funding sources.</span></span> <span data-ttu-id="f8652-140">تعتمد هذه السيناريوهات علي الافتراضات التالية:</span><span class="sxs-lookup"><span data-stu-id="f8652-140">These scenarios are based on the following assumptions:</span></span>

-   <span data-ttu-id="f8652-141">تكون إعدادات الاولويه عوامل في تخصيص الارصده قبل تطبيق معايير قواعد التمويل الأخرى.</span><span class="sxs-lookup"><span data-stu-id="f8652-141">Priority settings are factored into the allocation of funds before other funding rule criteria are applied.</span></span>
-   <span data-ttu-id="f8652-142">لم يتم تحديد نطاق التواريخ لتحديد الفترة رقم d عندما تكون قاعده التمويل صالحه.</span><span class="sxs-lookup"><span data-stu-id="f8652-142">No date range has been specified to define the period d when the funding rule is valid.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f8652-143"><strong>السيناريو</strong></span><span class="sxs-lookup"><span data-stu-id="f8652-143"><strong>Scenario</strong></span></span></td>
<td><span data-ttu-id="f8652-144"><strong>مصدر التمويل</strong></span><span class="sxs-lookup"><span data-stu-id="f8652-144"><strong>Funding source</strong></span></span></td>
<td><span data-ttu-id="f8652-145"><strong>النسبة المئوية للتوزيع</strong></span><span class="sxs-lookup"><span data-stu-id="f8652-145"><strong>Allocation percentage</strong></span></span></td>
<td><span data-ttu-id="f8652-146"><strong>أولوية التوزيع</strong></span><span class="sxs-lookup"><span data-stu-id="f8652-146"><strong>Allocation priority</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f8652-147">إذا كنت ترغب في تخصيص التكاليف لأحد مصادر التمويل حتى يتم استنفاد أموالها ، فقم بتخصيص التكاليف علي مصدر التمويل الثاني حتى يتم استنفاد أموالها ، وأخيرا قم بتخصيص التكاليف المتبقية إلى مصدر تمويل ثالث.</span><span class="sxs-lookup"><span data-stu-id="f8652-147">You want to allocate costs to one funding source until its funds are exhausted, allocate costs to a second funding source until its funds are exhausted, and finally allocate the remaining costs to a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="f8652-148">مصدر　التمويل　1</span><span class="sxs-lookup"><span data-stu-id="f8652-148">Funding　source　1</span></span></li>
<li><span data-ttu-id="f8652-149">مصدر　التمويل　2</span><span class="sxs-lookup"><span data-stu-id="f8652-149">Funding　source　2</span></span></li>
<li><span data-ttu-id="f8652-150">مصدر　التمويل　3</span><span class="sxs-lookup"><span data-stu-id="f8652-150">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="f8652-151">100%</span><span class="sxs-lookup"><span data-stu-id="f8652-151">100%</span></span></li>
<li><span data-ttu-id="f8652-152">100%</span><span class="sxs-lookup"><span data-stu-id="f8652-152">100%</span></span></li>
<li><span data-ttu-id="f8652-153">100%</span><span class="sxs-lookup"><span data-stu-id="f8652-153">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="f8652-154">1</span><span class="sxs-lookup"><span data-stu-id="f8652-154">1</span></span></li>
<li><span data-ttu-id="f8652-155">2</span><span class="sxs-lookup"><span data-stu-id="f8652-155">2</span></span></li>
<li><span data-ttu-id="f8652-156">3</span><span class="sxs-lookup"><span data-stu-id="f8652-156">3</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f8652-157">إذا كنت ترغب في تخصيص 75% من التكاليف إلى مصدر تمويل واحد و 25 بالمائة إلى مصدر تمويل ثان.</span><span class="sxs-lookup"><span data-stu-id="f8652-157">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="f8652-158">وعندما يتم استنفاد أحد مصادر التمويل هذه ، فانك ترغب في دفع التكاليف المتبقية من مصدر تمويل ثالث.</span><span class="sxs-lookup"><span data-stu-id="f8652-158">When either of those funding sources is exhausted, you want to pay the remaining costs from a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="f8652-159">مصدر　التمويل　1</span><span class="sxs-lookup"><span data-stu-id="f8652-159">Funding　source　1</span></span></li>
<li><span data-ttu-id="f8652-160">مصدر　التمويل　2</span><span class="sxs-lookup"><span data-stu-id="f8652-160">Funding　source　2</span></span></li>
<li><span data-ttu-id="f8652-161">مصدر　التمويل　3</span><span class="sxs-lookup"><span data-stu-id="f8652-161">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="f8652-162">75‏%</span><span class="sxs-lookup"><span data-stu-id="f8652-162">75%</span></span></li>
<li><span data-ttu-id="f8652-163">25‏%</span><span class="sxs-lookup"><span data-stu-id="f8652-163">25%</span></span></li>
<li><span data-ttu-id="f8652-164">100%</span><span class="sxs-lookup"><span data-stu-id="f8652-164">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="f8652-165">1</span><span class="sxs-lookup"><span data-stu-id="f8652-165">1</span></span></li>
<li><span data-ttu-id="f8652-166">1</span><span class="sxs-lookup"><span data-stu-id="f8652-166">1</span></span></li>
<li><span data-ttu-id="f8652-167">2</span><span class="sxs-lookup"><span data-stu-id="f8652-167">2</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f8652-168">إذا كنت ترغب في تخصيص 75% من التكاليف إلى مصدر تمويل واحد و 25 بالمائة إلى مصدر تمويل ثان.</span><span class="sxs-lookup"><span data-stu-id="f8652-168">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="f8652-169">عندما يتم استنفاد أي من مصادر التمويل هذه ، فأنت تريد تقسيم التكاليف المتبقية بين مصدر تمويل ثالث ومصدر تمويل رابع.</span><span class="sxs-lookup"><span data-stu-id="f8652-169">When either of those funding sources is exhausted, you want to split the remaining costs between a third funding source and a fourth funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="f8652-170">مصدر　التمويل　1</span><span class="sxs-lookup"><span data-stu-id="f8652-170">Funding　source　1</span></span></li>
<li><span data-ttu-id="f8652-171">مصدر　التمويل　2</span><span class="sxs-lookup"><span data-stu-id="f8652-171">Funding　source　2</span></span></li>
<li><span data-ttu-id="f8652-172">مصدر　التمويل　3</span><span class="sxs-lookup"><span data-stu-id="f8652-172">Funding　source　3</span></span></li>
<li><span data-ttu-id="f8652-173">مصدر　التمويل　4</span><span class="sxs-lookup"><span data-stu-id="f8652-173">Funding　source　4</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="f8652-174">75‏%</span><span class="sxs-lookup"><span data-stu-id="f8652-174">75%</span></span></li>
<li><span data-ttu-id="f8652-175">25‏%</span><span class="sxs-lookup"><span data-stu-id="f8652-175">25%</span></span></li>
<li><span data-ttu-id="f8652-176">50‏%</span><span class="sxs-lookup"><span data-stu-id="f8652-176">50%</span></span></li>
<li><span data-ttu-id="f8652-177">50‏%</span><span class="sxs-lookup"><span data-stu-id="f8652-177">50%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="f8652-178">1</span><span class="sxs-lookup"><span data-stu-id="f8652-178">1</span></span></li>
<li><span data-ttu-id="f8652-179">1</span><span class="sxs-lookup"><span data-stu-id="f8652-179">1</span></span></li>
<li><span data-ttu-id="f8652-180">2</span><span class="sxs-lookup"><span data-stu-id="f8652-180">2</span></span></li>
<li><span data-ttu-id="f8652-181">2</span><span class="sxs-lookup"><span data-stu-id="f8652-181">2</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f8652-182">تريد تخصيص أول 25 بالمائة من التكاليف لمصدر تمويل واحد والباقي لمصدر تمويل ثان.</span><span class="sxs-lookup"><span data-stu-id="f8652-182">You want to allocate the first 25 percent of costs to one funding source and the rest to a second funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="f8652-183">مصدر　التمويل　1</span><span class="sxs-lookup"><span data-stu-id="f8652-183">Funding　source　1</span></span></li>
<li><span data-ttu-id="f8652-184">مصدر　التمويل　2</span><span class="sxs-lookup"><span data-stu-id="f8652-184">Funding　source　2</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="f8652-185">25‏%</span><span class="sxs-lookup"><span data-stu-id="f8652-185">25%</span></span></li>
<li><span data-ttu-id="f8652-186">100%</span><span class="sxs-lookup"><span data-stu-id="f8652-186">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="f8652-187">1</span><span class="sxs-lookup"><span data-stu-id="f8652-187">1</span></span></li>
<li><span data-ttu-id="f8652-188">2</span><span class="sxs-lookup"><span data-stu-id="f8652-188">2</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a><span data-ttu-id="f8652-189">مثال: مصادر تمويل متعددة (معقدة)</span><span class="sxs-lookup"><span data-stu-id="f8652-189">Example: Multiple funding sources (complex)</span></span>

<span data-ttu-id="f8652-190">لديك ثلاثه من مصادر التمويل التي ترغب في استخدامها بالترتيب التالي:</span><span class="sxs-lookup"><span data-stu-id="f8652-190">You have three funding sources that you want to use in the following order:</span></span>

1.  <span data-ttu-id="f8652-191">استخدم مصدر التمويل 2 ومصدر التمويل 3 بشكل متساو إلى ان يتم استنفاد مصدر التمويل 2.</span><span class="sxs-lookup"><span data-stu-id="f8652-191">Use funding source 2 and funding source 3 equally until funding source 2 is exhausted.</span></span>
2.  <span data-ttu-id="f8652-192">متابعه استخدام مصدر التمويل 3 حتى الاستنفاد.</span><span class="sxs-lookup"><span data-stu-id="f8652-192">Continue to use funding source 3 until it is exhausted.</span></span>
3.  <span data-ttu-id="f8652-193">استخدام مصدر التمويل 1 بعد استنفاد مصدر التمويل 3.</span><span class="sxs-lookup"><span data-stu-id="f8652-193">Use funding source 1 after funding source 3 is exhausted.</span></span>

<span data-ttu-id="f8652-194">لتحقيق هذا الهدف ، يجب عليك القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="f8652-194">To accomplish this goal, you must do the following:</span></span>

-   <span data-ttu-id="f8652-195">اعداد حدود التمويل لمصدر التمويل رقم 2 ومصدر التمويل 3 ، بالنسبة للمبالغ الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="f8652-195">Set up funding limits for funding source 2 and funding source 3, for their respective amounts.</span></span>
-   <span data-ttu-id="f8652-196">قم بإنشاء قواعد التمويل التالية:</span><span class="sxs-lookup"><span data-stu-id="f8652-196">Create the following funding rules:</span></span>
    -   <span data-ttu-id="f8652-197">القاعدة 1 (الاولويه 1): تخصيص 50 بالمائة من الحركات إلى مصدر التمويل 2 و 50 بالمائة إلى مصدر التمويل 3.</span><span class="sxs-lookup"><span data-stu-id="f8652-197">Rule 1 (Priority 1): Allocate 50 percent of transactions to funding source 2 and 50 percent to funding source 3.</span></span>
    -   <span data-ttu-id="f8652-198">القاعدة 2 (الاولويه 2): تخصيص 100 بالمائة من الحركات إلى مصدر التمويل 3.</span><span class="sxs-lookup"><span data-stu-id="f8652-198">Rule 2 (Priority 2): Allocate 100 percent of transactions to funding source 3.</span></span>
    -   <span data-ttu-id="f8652-199">القاعدة 3 (الاولويه 3): تخصيص 100 بالمائة من الحركات إلى مصدر التمويل 1.</span><span class="sxs-lookup"><span data-stu-id="f8652-199">Rule 3 (Priority 3): Allocate 100 percent of transactions to funding source 1.</span></span>

<span data-ttu-id="f8652-200">يعمل هذا الاعداد لأنه يتم التحقق من الحركات في مقابل القواعد والحدود لتحديد ما إذا كانت اي منها تنطبق علي الحركة ام لا.</span><span class="sxs-lookup"><span data-stu-id="f8652-200">This setup works because transactions are checked against rules and limits to determine whether any of them apply to the transaction.</span></span> <span data-ttu-id="f8652-201">وفي حاله عدم تطبيق إيه قواعد أو حدود معينه علي الحركة ، يتم تطبيق جميع قواعد المعاملات.</span><span class="sxs-lookup"><span data-stu-id="f8652-201">If no specific rules or limits apply to the transaction, the All transactions rule applies.</span></span> <span data-ttu-id="f8652-202">تتطابق قاعده كافة الحركات مع كل الحركات.</span><span class="sxs-lookup"><span data-stu-id="f8652-202">The All transactions rule matches all transactions.</span></span> 

<span data-ttu-id="f8652-203">إذا تم العثور علي قاعده تطابق أحدي الحركات ، يتم تطبيق النسبة المئوية التي تم تخصيصها في هذه القاعدة أولا ، ولكن فقط بعد فحص المطابقات في مقابل إيه حدود تم اعدادها.</span><span class="sxs-lookup"><span data-stu-id="f8652-203">If a rule is found that matches a transaction, the percentage that has been allocated in that rule is applied first, but only after the matches are checked against any limits that have been set up.</span></span> <span data-ttu-id="f8652-204">إذا تم استيفاء حد ، وتم استنفاد أموال مصدر التمويل ، سيتم تجاهل قاعده التمويل المقترنة بحد التمويل ، ويقوم البرنامج بالتحقق من القاعدة التالية التي تنطبق عليها.</span><span class="sxs-lookup"><span data-stu-id="f8652-204">If a limit has been met, and a funding source’s funds are exhausted, the funding rule that is associated with the funding limit is disregarded, and the program checks for the next rule that applies.</span></span> 

<span data-ttu-id="f8652-205">وفي بعض الحالات ، يمكن تخصيص جزء من المعاملة فقط ضمن قاعده.</span><span class="sxs-lookup"><span data-stu-id="f8652-205">In some cases, only part of a transaction can be allocated under a rule.</span></span> <span data-ttu-id="f8652-206">وقد يحدث هذا بسبب الوصول إلى حد عند تخصيص المعاملة.</span><span class="sxs-lookup"><span data-stu-id="f8652-206">This might happen because a limit is reached when the transaction is allocated.</span></span> <span data-ttu-id="f8652-207">في هذه الحالة ، يتم تخصيص مبلغ محدد فقط طبقا لهذه القاعدة ، مثل 50 بالمائة لكل مصدر تمويل.</span><span class="sxs-lookup"><span data-stu-id="f8652-207">In this case, only a certain amount is allocated according to that rule, such as 50 percent to each funding source.</span></span> <span data-ttu-id="f8652-208">هذه هي الحالة في القاعدة رقم 1 ، والتي تم وصفها سابقا في هذا القسم.</span><span class="sxs-lookup"><span data-stu-id="f8652-208">This is the case in rule 1, which is described earlier in this section.</span></span> <span data-ttu-id="f8652-209">يتم تخصيص الباقي وفقا للقاعدة التالية في التسلسل.</span><span class="sxs-lookup"><span data-stu-id="f8652-209">The remainder is allocated according to the next rule in the sequence.</span></span> 

<span data-ttu-id="f8652-210">يفحص الجدول التالي هذا السيناريو بمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="f8652-210">The following table examines this scenario in more detail.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f8652-211"><strong>التركيز</strong></span><span class="sxs-lookup"><span data-stu-id="f8652-211"><strong>Focus</strong></span></span></td>
<td><span data-ttu-id="f8652-212"><strong>التفاصيل</strong></span><span class="sxs-lookup"><span data-stu-id="f8652-212"><strong>Details</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f8652-213">قواعد التمويل</span><span class="sxs-lookup"><span data-stu-id="f8652-213">Funding rules</span></span></td>
<td><ul>
<li><span data-ttu-id="f8652-214">القاعدة 1 (الاولويه 1): كافة الحركات.</span><span class="sxs-lookup"><span data-stu-id="f8652-214">Rule 1 (Priority 1): All transactions.</span></span> <span data-ttu-id="f8652-215">تخصيص مصدر التمويل 2 عند 50% ومصدر التمويل 3 عند 50%.</span><span class="sxs-lookup"><span data-stu-id="f8652-215">Allocate funding source 2 at 50% and funding source 3 at 50%.</span></span></li>
<li><span data-ttu-id="f8652-216">القاعدة 2 (الاولويه 2): كافة الحركات.</span><span class="sxs-lookup"><span data-stu-id="f8652-216">Rule 2 (Priority 2): All transactions.</span></span> <span data-ttu-id="f8652-217">تخصيص مصدر التمويل 3 عند 100%.</span><span class="sxs-lookup"><span data-stu-id="f8652-217">Allocate funding source 3 at 100%.</span></span></li>
<li><span data-ttu-id="f8652-218">القاعدة 3 (الاولويه 2): كافة الحركات.</span><span class="sxs-lookup"><span data-stu-id="f8652-218">Rule 3 (Priority 2): All transactions.</span></span> <span data-ttu-id="f8652-219">تخصيص مصدر التمويل 1 عند 100%.</span><span class="sxs-lookup"><span data-stu-id="f8652-219">Allocate funding source 1 at 100%.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f8652-220">حدود التمويل</span><span class="sxs-lookup"><span data-stu-id="f8652-220">Funding limits</span></span></td>
<td><ul>
<li><span data-ttu-id="f8652-221">حد مصدر التمويل 1 = 10,000.00</span><span class="sxs-lookup"><span data-stu-id="f8652-221">Funding source 1 limit = 10,000.00</span></span></li>
<li><span data-ttu-id="f8652-222">حد مصدر التمويل 2 = 500.00</span><span class="sxs-lookup"><span data-stu-id="f8652-222">Funding source 2 limit = 500.00</span></span></li>
<li><span data-ttu-id="f8652-223">حد مصدر التمويل 3 = 750.00</span><span class="sxs-lookup"><span data-stu-id="f8652-223">Funding source 3 limit = 750.00</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f8652-224">المعاملة 1</span><span class="sxs-lookup"><span data-stu-id="f8652-224">Transaction 1</span></span></td>
<td><span data-ttu-id="f8652-225"><strong>مبلغ الحركة:</strong> 100.00<strong>التمويل:</strong> يتم دفع المعاملة وفقًا للقاعدة 1 فقط ، لأن المعاملة مدفوعة بالكامل بعد تطبيق القاعدة 1.</span><span class="sxs-lookup"><span data-stu-id="f8652-225"><strong>Transaction amount:</strong> 100.00<strong>Funding:</strong> The transaction is paid according to rule 1 only, because the transaction is fully paid after rule 1 is applied.</span></span> <span data-ttu-id="f8652-226">فونديد الحركة بشكل متساو بين مصدر التمويل 2 ومصدر التمويل 3.</span><span class="sxs-lookup"><span data-stu-id="f8652-226">The transaction is funded equally between funding source 2 and funding source 3.</span></span>
<ul>
<li><span data-ttu-id="f8652-227">مصدر التمويل 2: 50.00</span><span class="sxs-lookup"><span data-stu-id="f8652-227">Funding source 2: 50.00</span></span></li>
<li><span data-ttu-id="f8652-228">مصدر التمويل 3: 50.00</span><span class="sxs-lookup"><span data-stu-id="f8652-228">Funding source 3: 50.00</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f8652-229">المعاملة 2</span><span class="sxs-lookup"><span data-stu-id="f8652-229">Transaction 2</span></span></td>
<td><span data-ttu-id="f8652-230"><strong>مبلغ الحركة:</strong> 5,000.00<strong>التمويل:</strong> يتم دفع المعاملة وفقًا لكل القواعد الثلاثة.</span><span class="sxs-lookup"><span data-stu-id="f8652-230"><strong>Transaction amount:</strong> 5,000.00<strong>Funding:</strong> The transaction is paid according to all three rules.</span></span> <span data-ttu-id="f8652-231"><strong>القاعدة 1</strong>
</span><span class="sxs-lookup"><span data-stu-id="f8652-231"><strong>Rule 1</strong>
</span></span><ul>
<li><span data-ttu-id="f8652-232">مصدر التمويل 2: 450.00</span><span class="sxs-lookup"><span data-stu-id="f8652-232">Funding source 2: 450.00</span></span></li>
<li><span data-ttu-id="f8652-233">مصدر التمويل 3: 450.00</span><span class="sxs-lookup"><span data-stu-id="f8652-233">Funding source 3: 450.00</span></span></li>
</ul><span data-ttu-id="f8652-234">
<strong>القاعدة 2</strong>
</span><span class="sxs-lookup"><span data-stu-id="f8652-234">
<strong>Rule 2</strong>
</span></span><ul>
<li><span data-ttu-id="f8652-235">مصدر التمويل 3: 250.00 (= 750.00 – 50.00 – 450.00)</span><span class="sxs-lookup"><span data-stu-id="f8652-235">Funding source 3: 250.00 (= 750.00 – 50.00 – 450.00)</span></span></li>
</ul><span data-ttu-id="f8652-236">
<strong>القاعدة 3</strong>
</span><span class="sxs-lookup"><span data-stu-id="f8652-236">
<strong>Rule 3</strong>
</span></span><ul>
<li><span data-ttu-id="f8652-237">مصدر التمويل 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span><span class="sxs-lookup"><span data-stu-id="f8652-237">Funding source 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f8652-238">إجمالي الارصده التي يتم توزيعها لكل مصدر تمويل</span><span class="sxs-lookup"><span data-stu-id="f8652-238">Total funds that are distributed for each funding source</span></span></td>
<td><ul>
<li><span data-ttu-id="f8652-239">مصدر التمويل 1: 3,850.00</span><span class="sxs-lookup"><span data-stu-id="f8652-239">Funding source 1: 3,850.00</span></span></li>
<li><span data-ttu-id="f8652-240">مصدر التمويل 2: 500.00</span><span class="sxs-lookup"><span data-stu-id="f8652-240">Funding source 2: 500.00</span></span></li>
<li><span data-ttu-id="f8652-241">مصدر التمويل 3: 750.00</span><span class="sxs-lookup"><span data-stu-id="f8652-241">Funding source 3: 750.00</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a><span data-ttu-id="f8652-242">قواعد الفوترة</span><span class="sxs-lookup"><span data-stu-id="f8652-242">Billing rules</span></span>
<span data-ttu-id="f8652-243">عند التفاوض علي عقد مشروع مع عميل ، يمكنك تحديد كيفيه فوتره العميل للعمل في أحد المشروعات ومتى تتمكن من ذلك.</span><span class="sxs-lookup"><span data-stu-id="f8652-243">When you negotiate a project contract with a customer, you define how and when you can invoice the customer for work on a project.</span></span> <span data-ttu-id="f8652-244">بعد اعداد عقد المشروع والمشروع ، يمكنك اعداد قواعد الفوترة الخاصة بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-244">After you set up the project contract and the project, you can set up billing rules for the project.</span></span> <span data-ttu-id="f8652-245">تستند قواعد الفوترة إلى شروط المشروع المحددة في عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-245">Billing rules are based on the project terms that are specified in the project contract.</span></span> <span data-ttu-id="f8652-246">تعتمد قواعد الفوترة التي يمكنك إنشاؤها علي شروط تعاقد المشروع ونوع المشروع ، مثل الوقت والمواد أو السعر الثابت الذي يتم اقرانه بقاعده الفوترة.</span><span class="sxs-lookup"><span data-stu-id="f8652-246">The billing rules that you can create depend on the terms of the project contract and the project type, such as Time and material or Fixed-price, that you associate with the billing rule.</span></span> <span data-ttu-id="f8652-247">يمكنك إنشاء أكثر من قاعده فوتره واحده لعقد مشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-247">You can create more than one billing rule for a project contract.</span></span> <span data-ttu-id="f8652-248">يمكنك أيضا تعيين قاعده فوتره لمشاريع متعددة مقترنة بنفس عقد المشروع والحصول علي شروط فوتره مماثله.</span><span class="sxs-lookup"><span data-stu-id="f8652-248">You can also assign a billing rule to multiple projects that are associated with the same project contract and have similar billing terms.</span></span> 

<span data-ttu-id="f8652-249">يمكنك اعداد الأنواع التالية من قواعد الفوترة:</span><span class="sxs-lookup"><span data-stu-id="f8652-249">You can set up the following types of billing rules:</span></span>

-   <span data-ttu-id="f8652-250">**وحده التسليم** – فوتره عميل عند إكمال وحده تسليم.</span><span class="sxs-lookup"><span data-stu-id="f8652-250">**Unit of delivery** – Invoice a customer when you complete a unit of delivery.</span></span> <span data-ttu-id="f8652-251">يمكنك تحديد وحدات التسليم في العقد.</span><span class="sxs-lookup"><span data-stu-id="f8652-251">You define the units of delivery in the contract.</span></span>
-   <span data-ttu-id="f8652-252">**التقدم** – فوتره العميل عندما تكمل نسبه محدده من المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-252">**Progress** – Invoice a customer when you complete a specified percentage of the project.</span></span> <span data-ttu-id="f8652-253">يمكنك اعداد قاعده فوتره لحساب النسبة المئوية للعمل المنجز تلقائيا ، أو يمكنك يدويا حساب النسبة المئوية للعمل المنجز والمبلغ الذي سيقوم بفوترة العميل.</span><span class="sxs-lookup"><span data-stu-id="f8652-253">You can set up a billing rule to automatically calculate the percentage of work completed, or you can manually calculate the percentage of work completed and the amount to invoice the customer.</span></span>
-   <span data-ttu-id="f8652-254">**حدث رئيسي** - إصدار فاتورة للعميل بالمبلغ الكامل لحدث رئيسي للمشروع عند الوصول إلى الحدث الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="f8652-254">**Milestone** – Invoice a customer for the full amount of a project milestone when the milestone is reached.</span></span>
-   <span data-ttu-id="f8652-255">**الرسوم** – إصدار فاتورة للعميل مقابل خدماتك بالإضافة إلى رسوم إدارية ، والتي تكون عادةً نسبة مئوية من تكلفة الخدمات.</span><span class="sxs-lookup"><span data-stu-id="f8652-255">**Fee** – Invoice a customer for your services plus a management fee, which is typically a percentage of the cost of services.</span></span>
-   <span data-ttu-id="f8652-256">**الوقت والمواد** - إصدار فاتورة للعميل بقيمة الوقت والمواد المستخدمة في المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-256">**Time and material** – Invoice a customer for the value of time and materials that are used on a project.</span></span>

<span data-ttu-id="f8652-257">بالنسبة لكافة أنواع قواعد الفوترة ، يمكنك تحديد نسبه احتجاز تم خصمها من فواتير العملاء حتى يصل أحد المشاريع إلى مرحله متفق عليها.</span><span class="sxs-lookup"><span data-stu-id="f8652-257">For all types of billing rules, you can specify a retention percentage that is deducted from customer invoices until a project reaches an agreed-upon stage.</span></span> <span data-ttu-id="f8652-258">يتم تحديد النسبة المئوية لاحتجاز الدفع في عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-258">The payment retention percentage is specified in the project contract.</span></span> <span data-ttu-id="f8652-259">يتم حساب المبلغ استنادا إلى القيمة الاجماليه للسطور والمطروحة منه في فاتورة العميل.</span><span class="sxs-lookup"><span data-stu-id="f8652-259">The amount is calculated based on, and subtracted from, the total value of the lines in a customer invoice.</span></span> 

<span data-ttu-id="f8652-260">بالنسبة إل قواعد فوترة **الوقت والمواد** و **التقدم**، يمكنك تعيين فئات خاضعه للرسوم.</span><span class="sxs-lookup"><span data-stu-id="f8652-260">For **Time and material** and **Progress** billing rules, you can assign chargeable categories.</span></span> <span data-ttu-id="f8652-261">تشير الفئات الخاضعة للرسوم إلى الحركات التي ينبغي تضمينها في فواتير العملاء.</span><span class="sxs-lookup"><span data-stu-id="f8652-261">Chargeable categories indicate the transactions that should be included in customer invoices.</span></span> 

<span data-ttu-id="f8652-262">عندما تكون مستعدا لفوترة العميل ، يتم حساب المبلغ الذي سيتم تحرير الفواتير له علي أساس قواعد الفوترة ، ويتم إنشاء مقترح فاتورة مشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-262">When you are ready to invoice the customer, the amount to invoice for the project is calculated based on the billing rules, and a project invoice proposal is generated.</span></span> 

<span data-ttu-id="f8652-263">توفر الأقسام التالية أمثله توضح كيفيه اعداد قواعد الفوترة لأحد المشروعات وأدارتها.</span><span class="sxs-lookup"><span data-stu-id="f8652-263">The following sections provide examples that show how to set up and manage billing rules for a project.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a><span data-ttu-id="f8652-264">مثال: قم بإنشاء قاعده فوتره تستند إلى عدد الوحدات التي تم تسليمها</span><span class="sxs-lookup"><span data-stu-id="f8652-264">Example: Create a billing rule that is based on the number of units delivered</span></span>

<span data-ttu-id="f8652-265">تدخل مؤسستك في اتفاقيه لتوفير إجمالي خمس جلسات عمل تدريب لموظفي العميل بتكلفه مقدارها 10,000 في كل جلسة تدريب.</span><span class="sxs-lookup"><span data-stu-id="f8652-265">Your organization enters into an agreement to provide a total of five training sessions to a customer’s employees at a cost of 10,000 per training session.</span></span> <span data-ttu-id="f8652-266">يمكنك فوتره العميل بعد كل جلسة تدريب.</span><span class="sxs-lookup"><span data-stu-id="f8652-266">You invoice the customer after each training session.</span></span> 

<span data-ttu-id="f8652-267">عندما تقوم باعداد قواعد الفوترة الخاصة بالعقد ، استخدم القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="f8652-267">When you set up the billing rules for the contract, you use the following values:</span></span>

-   <span data-ttu-id="f8652-268">وحده التسليم هي جلسة تدريب واحده.</span><span class="sxs-lookup"><span data-stu-id="f8652-268">The unit of delivery is one training session.</span></span>
-   <span data-ttu-id="f8652-269">ويكون سعر الوحدة هو 10,000 لكل جلسة تدريب.</span><span class="sxs-lookup"><span data-stu-id="f8652-269">The unit price is 10,000 per training session.</span></span>
-   <span data-ttu-id="f8652-270">العدد الإجمالي للوحدات هو خمس جلسات تدريب.</span><span class="sxs-lookup"><span data-stu-id="f8652-270">The total number of units is five training sessions.</span></span>

<span data-ttu-id="f8652-271">عند الانتهاء من جلسة تدريب واحده ، يمكنك إنشاء فاتورة ل 10,000 ، وللوحدة الاولي التي تم تسليمها ، وإرسال الفاتورة إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="f8652-271">When you have completed one training session, you can create an invoice for 10,000, for the first unit that was delivered, and send the invoice to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a><span data-ttu-id="f8652-272">مثال: إنشاء قاعده فوتره تستند إلى نسبه مئوية محدده من اكتمال المشروع (الحساب اليدوي)</span><span class="sxs-lookup"><span data-stu-id="f8652-272">Example: Create a billing rule that is based on a specified percentage of project completion (manual calculation)</span></span>

<span data-ttu-id="f8652-273">تقوم مؤسستك ، وشركك الاستشارية ، بإدخالها في الاتفاقية مع العميل لتطوير جزء من المنتج الذي يقوم العميل بتطويره.</span><span class="sxs-lookup"><span data-stu-id="f8652-273">Your organization, a software consulting firm, enters into an agreement with a customer to develop part of a product that the customer is developing.</span></span> <span data-ttu-id="f8652-274">موافقه مؤسستك علي تقديم رمز البرنامج خلال فتره من سته أشهر.</span><span class="sxs-lookup"><span data-stu-id="f8652-274">Your organization agrees to deliver the software code over a period of six months.</span></span> <span data-ttu-id="f8652-275">يوافق العميل علي دفع المؤسسة إجمالي 100,000 للعمل.</span><span class="sxs-lookup"><span data-stu-id="f8652-275">The customer agrees to pay your organization a total of 100,000 for the work.</span></span> <span data-ttu-id="f8652-276">يمكنك إنشاء قاعده فوتره لفوترة العميل علي أساس النسبة المئوية للعمل الذي تم إكماله في المشروع ، كما هو محدد في العقد.</span><span class="sxs-lookup"><span data-stu-id="f8652-276">You create a billing rule to invoice the customer based on the percentage of work that is completed on the project, as specified in the contract.</span></span>

-   <span data-ttu-id="f8652-277">وفي نهاية الشهر الأول ، تتوافق مع العميل علي تحديد النسبة المئوية للعمل الذي تم إكماله.</span><span class="sxs-lookup"><span data-stu-id="f8652-277">At the end of the first month, you meet with the customer to determine the percentage of work completed.</span></span> <span data-ttu-id="f8652-278">بعد ان تقوم أنت والعميل بمراجعه المشروع ، فانك تقرر ان المشروع اكتمل بنسبه 15%.</span><span class="sxs-lookup"><span data-stu-id="f8652-278">After you and the customer review the project, you decide that the project is 15 percent completed.</span></span>
-   <span data-ttu-id="f8652-279">يمكنك إنشاء فاتورة ل15,000 (15 النسبة المئوية من 100,000) وإرسالها إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="f8652-279">You create an invoice for 15,000 (15 percent of 100,000) and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a><span data-ttu-id="f8652-280">مثال: إنشاء قاعده فوتره تستند إلى نسبه مئوية محدده من اكتمال المشروع (الحساب التلقائي)</span><span class="sxs-lookup"><span data-stu-id="f8652-280">Example: Create a billing rule that is based on a specified percentage of project completion (automatic calculation)</span></span>

<span data-ttu-id="f8652-281">لدي مؤسستك ، وهو شركه تطوير برامج ، موافقه لتطوير حزمه محاسبه رواتب لعميل ل 30,000.</span><span class="sxs-lookup"><span data-stu-id="f8652-281">Your organization, a software development firm, agrees to develop a payroll accounting package for a customer for 30,000.</span></span> <span data-ttu-id="f8652-282">يوافق العميل على الدفع لمؤسستك بناءً على النسبة المئوية للعمل المنجز.</span><span class="sxs-lookup"><span data-stu-id="f8652-282">The customer agrees to pay your organization based on the percentage of work completed.</span></span> <span data-ttu-id="f8652-283">يمكنك تقدير ان تكاليف المشروع هي 20,000.</span><span class="sxs-lookup"><span data-stu-id="f8652-283">You estimate that the project costs are 20,000.</span></span> <span data-ttu-id="f8652-284">يحدد عقد المشروع فئات العمل التي تستخدمها في عمليه الفوترة.</span><span class="sxs-lookup"><span data-stu-id="f8652-284">The project contract specifies the categories of work that you use in the billing process.</span></span> <span data-ttu-id="f8652-285">يمكنك اعداد قواعد الفوترة التي تقوم تلقائيا بحساب مبالغ الفاتورة للنسبة المئوية للعمل المكتمل لكل فئة.</span><span class="sxs-lookup"><span data-stu-id="f8652-285">You set up billing rules that automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="f8652-286">قم باعداد موازنة لكل فئة:</span><span class="sxs-lookup"><span data-stu-id="f8652-286">You set up a budget for each category:</span></span>

-   <span data-ttu-id="f8652-287">**التطوير** – تكلفه 15,000 وإيرادات 20,000</span><span class="sxs-lookup"><span data-stu-id="f8652-287">**Development** – Cost of 15,000 and revenue of 20,000</span></span>
-   <span data-ttu-id="f8652-288">**التثبيت** – تكلفه 5,000 وإيرادات 10,000</span><span class="sxs-lookup"><span data-stu-id="f8652-288">**Installation** – Cost of 5,000 and revenue of 10,000</span></span>

<span data-ttu-id="f8652-289">عندما تقوم بإنشاء فاتورة عميل للمرة الاولي ، يتم حساب مبلغ الفاتورة تلقائيا بناء علي المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="f8652-289">When you create a customer invoice for the first time, the invoice amount is automatically calculated based on the following information:</span></span>

-   <span data-ttu-id="f8652-290">وبعد شهر ، يقوم العامل الموجود في المشروع بتسليم جدول زمني للمشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-290">After a month, the worker on the project submits a timesheet for the project.</span></span> <span data-ttu-id="f8652-291">تكون تكلفه ساعات العامل 5,000 للتطوير و 1,000 للتثبيت.</span><span class="sxs-lookup"><span data-stu-id="f8652-291">The cost of the worker’s hours is 5,000 for development and 1,000 for installation.</span></span> <span data-ttu-id="f8652-292">اكتمال عمل التطوير 33 بالمائة (5,000 التكلفة الفعلية/تكلفه الموازنة 15000) ، واكتمال عمل التثبيت بنسبه 20% (1,000 التكلفة الفعلية/5000 تكلفه الموازنة).</span><span class="sxs-lookup"><span data-stu-id="f8652-292">The development work is 33 percent completed (5,000 actual cost/15,000 budget cost), and the installation work is 20 percent completed (1,000 actual cost/5,000 budget cost).</span></span>
-   <span data-ttu-id="f8652-293">يتم حساب مبلغ الفاتورة 8,667 تلقائيا (33 بالمائة من 20,000 + 20 بالمائة من 10,000).</span><span class="sxs-lookup"><span data-stu-id="f8652-293">The invoice amount of 8,667 is automatically calculated (33 percent of 20,000 + 20 percent of 10,000).</span></span>
-   <span data-ttu-id="f8652-294">تقوم بإنشاء فاتورة بمبلغ 8667 وإرسالها إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="f8652-294">You create an invoice for 8,667 and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a><span data-ttu-id="f8652-295">مثال: إنشاء قاعده فوتره تستند إلى احداث رئيسيه تمت الموافقة عليها</span><span class="sxs-lookup"><span data-stu-id="f8652-295">Example: Create a billing rule that is based on agreed-upon milestones</span></span>

<span data-ttu-id="f8652-296">المؤسسة الخاصة بك ، وهي شركه الاداره ، موافقه لإجراء بحث السوق لمنتج المستهلك الذي يخطط العميل لبيعه.</span><span class="sxs-lookup"><span data-stu-id="f8652-296">Your organization, a management consulting firm, agrees to conduct market research for a consumer product that the customer plans to sell.</span></span> <span data-ttu-id="f8652-297">يوافق العميل علي استخدام الخدمات الخاصة بك لفتره من ثلاثه أشهر ، بدءا من شهر مارس ، والموافقة علي دفع مؤسسه 50,000.</span><span class="sxs-lookup"><span data-stu-id="f8652-297">The customer agrees to use your services for a period of three months, starting in March, and agrees to pay your organization 50,000.</span></span> <span data-ttu-id="f8652-298">يحتوي المشروع علي ثلاثه احداث رئيسيه:</span><span class="sxs-lookup"><span data-stu-id="f8652-298">The project has three milestones:</span></span>

-   <span data-ttu-id="f8652-299">الحدث الرئيسي 1: تجميع بيانات المستهلك-31 مارس</span><span class="sxs-lookup"><span data-stu-id="f8652-299">Milestone 1: Collect consumer data – March 31</span></span>
-   <span data-ttu-id="f8652-300">الحدث الرئيسي 2: تحليل بيانات المستهلك-30 ابريل</span><span class="sxs-lookup"><span data-stu-id="f8652-300">Milestone 2: Analyze consumer data – April 30</span></span>
-   <span data-ttu-id="f8652-301">الحدث الرئيسي 3: تقديم اقتراح جدوى المنتج - 31 مايو</span><span class="sxs-lookup"><span data-stu-id="f8652-301">Milestone 3: Present a product viability proposal – May 31</span></span>

<span data-ttu-id="f8652-302">يوافق العميل علي دفع مؤسستك 10,000 للحدث الرئيسي الأول ، 20,000 للحدث الرئيسي الثاني ، و20,000 للحدث الرئيسي الثالث.</span><span class="sxs-lookup"><span data-stu-id="f8652-302">The customer agrees to pay your organization 10,000 for the first milestone, 20,000 for the second milestone, and 20,000 for the third milestone.</span></span> 

<span data-ttu-id="f8652-303">عندما تقوم باعداد عقد المشروع ، فأنت توافق علي فوتره العميل بناء علي الحدث الرئيسي الذي تم إكماله.</span><span class="sxs-lookup"><span data-stu-id="f8652-303">When you set up the project contract, you agree to bill the customer based on the milestone that has been completed.</span></span> <span data-ttu-id="f8652-304">يشتمل اعداد قاعده الفوترة علي الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="f8652-304">The billing rule setup includes the following steps:</span></span>

-   <span data-ttu-id="f8652-305">قم بتعريف المراحل الرئيسية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-305">Define the project milestones.</span></span>
-   <span data-ttu-id="f8652-306">حدد المبلغ الذي سيتم فوتره العميل اليه عند اكتمال كل مرحله رئيسيه.</span><span class="sxs-lookup"><span data-stu-id="f8652-306">Define the amount to invoice the customer when each milestone is completed.</span></span>

<span data-ttu-id="f8652-307">عند اكتمال الحدث الرئيسي الأول في 31 مارس ، ضع علامة علي الحدث الرئيسي كمكتمل ، ثم قم بإنشاء فاتورة ل10,000 وإرساله إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="f8652-307">When the first milestone is completed on March 31, you mark the milestone as completed, and then create an invoice for 10,000 and send it to the customer.</span></span> <span data-ttu-id="f8652-308">لا يمكنك إنشاء فاتورة للحدث الرئيسي حتى يتم تمييز الحدث الرئيسي علي انه مكتمل.</span><span class="sxs-lookup"><span data-stu-id="f8652-308">You can’t create an invoice for a milestone until you have marked the milestone as completed.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a><span data-ttu-id="f8652-309">مثال: إنشاء قاعده فوتره تستند إلى الخدمات بالإضافة إلى رسوم الاداره</span><span class="sxs-lookup"><span data-stu-id="f8652-309">Example: Create a billing rule that is based on services plus a management fee</span></span>

<span data-ttu-id="f8652-310">تقوم مؤسستك ، وهي شركه استشاريه ، بالموافقة علي القيام بأبحاث السوق لتقييم فيابيليتي المنتج الذي يقوم العميل بتطويره.</span><span class="sxs-lookup"><span data-stu-id="f8652-310">Your organization, a management consulting firm, agrees to conduct market research to evaluate the viability of a product that the customer, a retail company, is developing.</span></span> <span data-ttu-id="f8652-311">تحدد شروط الاتفاقية انك ستقدم خدمات مستشارات الاداره الأعلى ، والتي ستقوم بالبحث في أساس الوقت والمواد.</span><span class="sxs-lookup"><span data-stu-id="f8652-311">The terms of the agreement specify that you will provide the services of your top three management consultants, who will conduct the research on a time-and-materials basis.</span></span> <span data-ttu-id="f8652-312">يوافق العميل علي الدفع 100 في الساعة بالإضافة إلى رسوم أداره 10 بالمائة للساعات الاستشارية التي يتم سدادها علي المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-312">The customer agrees to pay 100 per hour, plus a 10 percent management fee for the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="f8652-313">عندما تقوم باعداد عقد المشروع ، قم بإنشاء قاعده فوتره لأضافه رسوم أداره بنسبه 10% إلى الساعات الاستشارية التي يتم فرضها علي المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-313">When you set up the project contract, create a billing rule to add a 10 percent management fee to the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="f8652-314">عند إنشاء فاتورة للعميل ، يتم فوتره العميل إلى 10% من رسوم الاداره بالإضافة إلى تكلفه الساعات الاستشارية.</span><span class="sxs-lookup"><span data-stu-id="f8652-314">When you create an invoice for the customer, the customer is billed a 10 percent management fee plus the cost of the consulting hours.</span></span> <span data-ttu-id="f8652-315">علي سبيل المثال ، إذا كانت المستشارين الثلاثين يعملون في إجمالي 200 ساعة في المشروع ، يتم إنشاء فاتورة لكل 22,000 استنادا إلى الحساب التالي:</span><span class="sxs-lookup"><span data-stu-id="f8652-315">For example, if the three consultants worked a total of 200 hours on the project, an invoice for 22,000 is created based on the following calculation:</span></span>

-   <span data-ttu-id="f8652-316">200 ساعة في 100 في الساعة = 20,000</span><span class="sxs-lookup"><span data-stu-id="f8652-316">200 hours at 100 per hour = 20,000</span></span>
-   <span data-ttu-id="f8652-317">مقابل نسبه أداره 10 بالمائة = 2,000</span><span class="sxs-lookup"><span data-stu-id="f8652-317">10 percent management fee = 2,000</span></span>
-   <span data-ttu-id="f8652-318">مبلغ الفاتورة الإجمالي = 22,000</span><span class="sxs-lookup"><span data-stu-id="f8652-318">Total invoice amount = 22,000</span></span>

<span data-ttu-id="f8652-319">إذا كانت الرسوم خاضعه للعميل ، وقامت بتحديد مجموعه ضريبة مبيعات في عقد المشروع ، يتم إدخال مجموعه ضريبة المبيعات تلقائيا في قاعده فوتره للرسوم.</span><span class="sxs-lookup"><span data-stu-id="f8652-319">If fees are taxable to a customer, and you select a sales tax group in the project contract, the sales tax group is automatically entered in a billing rule for fees.</span></span>

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a><span data-ttu-id="f8652-320">مثال: إنشاء قاعده فوتره لقيمه الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="f8652-320">Example: Create a billing rule for the value of time and materials</span></span>

<span data-ttu-id="f8652-321">تقوم مؤسستك ، بالموافقة علي تقديم خمسه مستشارين فنيين للعمل مع مشروع تطوير برامج لأحد العملاء خلال الأشهر الستة القادمة.</span><span class="sxs-lookup"><span data-stu-id="f8652-321">Your organization, a software consulting firm, agrees to provide five technical consultants to work on a software development project for a customer for the next six months.</span></span> <span data-ttu-id="f8652-322">يوافق العميل علي الدفع 150 لكل ساعة استشاره ، بالإضافة إلى تكلفه الموارد التي توفرها المكتب.</span><span class="sxs-lookup"><span data-stu-id="f8652-322">The customer agrees to pay 150 for each consulting hour, plus the cost of office supplies.</span></span> <span data-ttu-id="f8652-323">ترسل مؤسستك فاتورة إلى العميل في نهاية كل شهر.</span><span class="sxs-lookup"><span data-stu-id="f8652-323">Your organization sends an invoice to the customer at the end of each month.</span></span> 

<span data-ttu-id="f8652-324">عندما تقوم باعداد عقد المشروع ، فأنت توافق علي فوتره العميل كل شهر من الوقت والمواد الموجودة بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-324">When you set up the project contract, you agree to bill the customer each month for time and materials on the project.</span></span> <span data-ttu-id="f8652-325">يمكنك إنشاء قاعده فوتره تتضمن المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="f8652-325">You create a billing rule that includes the following information:</span></span>

-   <span data-ttu-id="f8652-326">الفترة الزمنية للعقد هي سته أشهر.</span><span class="sxs-lookup"><span data-stu-id="f8652-326">The contract period is six months.</span></span>
-   <span data-ttu-id="f8652-327">يتم حساب الوقت الاستشاري بمعدل 150 في الساعة.</span><span class="sxs-lookup"><span data-stu-id="f8652-327">Consulting time is calculated at a rate of 150 per hour.</span></span>
-   <span data-ttu-id="f8652-328">وتتم فوتره تجهيزات المكتب بالتكلفة ، ولا يجب ان تتجاوز التكلفة الاجماليه للمشروع 10,000.</span><span class="sxs-lookup"><span data-stu-id="f8652-328">Office supplies are invoiced at cost, and the total cost for the project must not exceed 10,000.</span></span>
-   <span data-ttu-id="f8652-329">يمكنك إنشاء فاتورة عميل في نهاية كل شهر في التقويم اثناء المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-329">You create a customer invoice at the end of each calendar month during the project.</span></span>

<span data-ttu-id="f8652-330">خلال الشهر الأول ، يتم تسجيل إجمالي 800 ساعة بواسطة المستشارين في المشروع.</span><span class="sxs-lookup"><span data-stu-id="f8652-330">During the first month, a total of 800 hours are recorded by the consultants on the project.</span></span> <span data-ttu-id="f8652-331">تكلفه الموارد التي تتحمل المكتب التي يتم تحميلها إلى المشروع هو 2,000.</span><span class="sxs-lookup"><span data-stu-id="f8652-331">The cost of office supplies that are charged to the project is 2,000.</span></span> <span data-ttu-id="f8652-332">لذلك ، في نهاية الشهر ، تقوم بإنشاء فاتورة بمبلغ 122000 ، والتي يتم حسابها على أنها 800 ساعة مقابل 150 ساعة في الساعة ، بالإضافة إلى 2000 لمستلزمات المكاتب.</span><span class="sxs-lookup"><span data-stu-id="f8652-332">Therefore, at the end of the month, you create an invoice for 122,000, which is calculated as 800 hours at 150 per hour, plus 2,000 for office supplies.</span></span>





[!INCLUDE[footer-include](../includes/footer-banner.md)]