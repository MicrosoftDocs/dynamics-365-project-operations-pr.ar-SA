---
title: نظرة عامة على أبعاد التسعير
description: يوفر هذا الموضوع معلومات حول أبعاد التسعير في Dynamics 365 Project operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: ec2e350e0e4c28ea1c9540d70c83fdf0a75dc408
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128447"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="46f67-103">نظرة عامة على أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="46f67-103">Pricing dimensions overview</span></span>

<span data-ttu-id="46f67-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="46f67-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="46f67-105">الأبعاد المستخدمة في الموارد البشرية لإعداد التسعير والتكاليف تنقسم إلى فئتين:</span><span class="sxs-lookup"><span data-stu-id="46f67-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="46f67-106">أشخاص</span><span class="sxs-lookup"><span data-stu-id="46f67-106">People</span></span>
- <span data-ttu-id="46f67-107">العمل المخطط</span><span class="sxs-lookup"><span data-stu-id="46f67-107">Planned work</span></span>

<span data-ttu-id="46f67-108">ولهذا السبب، هناك نوعان من قيم أبعاد التسعير المتوفرة:</span><span class="sxs-lookup"><span data-stu-id="46f67-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="46f67-109">**مجموعات الخيارات**: الأبعاد التي تمثل تعدادًا ثابتًا لمجموعة من القيم.</span><span class="sxs-lookup"><span data-stu-id="46f67-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="46f67-110">**القيم المستندة إلى الكيانات**: الأبعاد التي يمكن أن تكون مجموعة متنوعة من القيم.</span><span class="sxs-lookup"><span data-stu-id="46f67-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="46f67-111">أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="46f67-111">Pricing dimensions</span></span>

<span data-ttu-id="46f67-112">يُشحن Dynamics 365 Project Operations مع مجموعة افتراضية من أبعاد التسعير.</span><span class="sxs-lookup"><span data-stu-id="46f67-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="46f67-113">يمكنك عرض أبعاد التسعير هذه عن طريق الانتقال إلى **عمليات المشروع** > **المعلمات**.</span><span class="sxs-lookup"><span data-stu-id="46f67-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="46f67-114">في سجل المعلمات، في علامة التبويب **أبعاد التسعير المستندة إلى المبلغ**، تحقق من أن الدور، **msdyn_resourcecategory** والوحدة التنظيمية للموارد، **msdyn_organizationalunit** يشتملان على الحقلين **قابل للتطبيق على المبيعات** **قابل للتطبيق على التكلفة** معينين إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="46f67-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="46f67-115">مع تمكين هذه الحقول، سيتيح لك إمكانية إعداد السعر والتكلفة لكل مجموعة دور ووحدة تنظيمية.</span><span class="sxs-lookup"><span data-stu-id="46f67-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

<span data-ttu-id="46f67-116">إذا كنت بحاجة إلى أسعار أو تكلفه للموارد الخاصة بك باستخدام سمات إضافية، فيمكنك إنشاء حقول وكيانات وأبعاد مخصصة.</span><span class="sxs-lookup"><span data-stu-id="46f67-116">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span>

## <a name="pricing-human-resource-time"></a><span data-ttu-id="46f67-117">وقت المورد البشري للتسعير</span><span class="sxs-lookup"><span data-stu-id="46f67-117">Pricing human resource time</span></span>
<span data-ttu-id="46f67-118">غالبًا ما تكون كيفية قيام المؤسسة بتسعير وقت الموارد البشرية اعتبارًا استراتيجيًا مهمًا يؤثر بشكل مباشر على ربحية المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="46f67-118">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="46f67-119">اعمل مع الفرق المالية ورؤساء التدريب عندما تكون مؤسستك جاهزة لتحديد كيف تريد إعداد فاتورة ومعدلات تكلفة لوقت الموارد البشرية.</span><span class="sxs-lookup"><span data-stu-id="46f67-119">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="46f67-120">تشمل الاعتبارات الأخرى للتسعير ما إذا كان يجب إعادة استخدام الحقول أو الكيانات التي لا تمثل أبعادًا للتسعير حاليًا ولكن يتم تطبيقها كبعد تسعير لمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="46f67-120">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="46f67-121">تعتبر الحقول مثل **فئة المعاملات** (**msdyn_transactioncategory**) و **المورد القابل للحجز** (**bookableresource**) أمثلة على أبعاد المرشحين.</span><span class="sxs-lookup"><span data-stu-id="46f67-121">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="46f67-122">ضع في اعتبارك ما إذا كان يجب أن يكون بُعد التسعير الخاص بك عبارة عن جدول أو مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="46f67-122">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="46f67-123">إذا كنت تتوقع تغييرات في قيم البعد الذي يتجاوز 10 أو 12 وتحتاج إلى سمات إضافية على هذه القيم ، فيمكنك إنشاء كيان بدلاً من مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="46f67-123">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="46f67-124">تتطلب المحافظة على مجموعة خيارات ، مثل إضافة القيم أو إزالتها ، مسؤولًا أو مطورًا ، بينما يمكن لمعظم المستخدمين إضافة صفوف جديدة إلى جدول.</span><span class="sxs-lookup"><span data-stu-id="46f67-124">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="46f67-125">يوضح المثال التالي معدلات الفاتورة التي تم إعدادها بناءً على الدور ووحدة توفير الموارد التي ينتمي إليها المورد.</span><span class="sxs-lookup"><span data-stu-id="46f67-125">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="46f67-126">تعتمد معدلات التكلفة عادة على نطاق مرتب الموظف ووحدة المؤسسة التي ينتمي إليها.</span><span class="sxs-lookup"><span data-stu-id="46f67-126">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="46f67-127">في هذا المثال ، ستبدو جداول معدل الفاتورة ومعدل التكلفة كما يلي.</span><span class="sxs-lookup"><span data-stu-id="46f67-127">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="46f67-128">**نموذج أسعار الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="46f67-128">**Sample bill rates**</span></span>

| <span data-ttu-id="46f67-129">الدور</span><span class="sxs-lookup"><span data-stu-id="46f67-129">Role</span></span>        | <span data-ttu-id="46f67-130">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="46f67-130">Org Unit</span></span>    |<span data-ttu-id="46f67-131">الوحدة</span><span class="sxs-lookup"><span data-stu-id="46f67-131">Unit</span></span>      |<span data-ttu-id="46f67-132">السعر</span><span class="sxs-lookup"><span data-stu-id="46f67-132">Price</span></span>      |<span data-ttu-id="46f67-133">العملات</span><span class="sxs-lookup"><span data-stu-id="46f67-133">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="46f67-134">المطور</span><span class="sxs-lookup"><span data-stu-id="46f67-134">Developer</span></span>   | <span data-ttu-id="46f67-135">Contoso US</span><span class="sxs-lookup"><span data-stu-id="46f67-135">Contoso US</span></span>  |<span data-ttu-id="46f67-136">Hour‬</span><span class="sxs-lookup"><span data-stu-id="46f67-136">Hour</span></span> | <span data-ttu-id="46f67-137">200</span><span class="sxs-lookup"><span data-stu-id="46f67-137">200</span></span>|<span data-ttu-id="46f67-138">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="46f67-138">USD</span></span>     |
| <span data-ttu-id="46f67-139">المطور</span><span class="sxs-lookup"><span data-stu-id="46f67-139">Developer</span></span>   | <span data-ttu-id="46f67-140">شركة حسني بالهند</span><span class="sxs-lookup"><span data-stu-id="46f67-140">Contoso India</span></span> |<span data-ttu-id="46f67-141">Hour‬</span><span class="sxs-lookup"><span data-stu-id="46f67-141">Hour</span></span>|   <span data-ttu-id="46f67-142">112</span><span class="sxs-lookup"><span data-stu-id="46f67-142">112</span></span>|<span data-ttu-id="46f67-143">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="46f67-143">USD</span></span>     |


<span data-ttu-id="46f67-144">**نموذج أسعار التكاليف**</span><span class="sxs-lookup"><span data-stu-id="46f67-144">**Sample cost rates**</span></span>

| <span data-ttu-id="46f67-145">نطاق الراتب</span><span class="sxs-lookup"><span data-stu-id="46f67-145">Salary Band</span></span>     | <span data-ttu-id="46f67-146">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="46f67-146">Org Unit</span></span>    |<span data-ttu-id="46f67-147">الوحدة</span><span class="sxs-lookup"><span data-stu-id="46f67-147">Unit</span></span>      |<span data-ttu-id="46f67-148">السعر</span><span class="sxs-lookup"><span data-stu-id="46f67-148">Price</span></span>      |<span data-ttu-id="46f67-149">العملات</span><span class="sxs-lookup"><span data-stu-id="46f67-149">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="46f67-150">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="46f67-150">My company_Band1</span></span> | <span data-ttu-id="46f67-151">Contoso US</span><span class="sxs-lookup"><span data-stu-id="46f67-151">Contoso US</span></span>  |<span data-ttu-id="46f67-152">Hour‬</span><span class="sxs-lookup"><span data-stu-id="46f67-152">Hour</span></span> | <span data-ttu-id="46f67-153">145</span><span class="sxs-lookup"><span data-stu-id="46f67-153">145</span></span>|<span data-ttu-id="46f67-154">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="46f67-154">USD</span></span>     |
| <span data-ttu-id="46f67-155">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="46f67-155">My company_Band2</span></span> | <span data-ttu-id="46f67-156">شركة حسني بالهند</span><span class="sxs-lookup"><span data-stu-id="46f67-156">Contoso India</span></span> |<span data-ttu-id="46f67-157">Hour‬</span><span class="sxs-lookup"><span data-stu-id="46f67-157">Hour</span></span>|   <span data-ttu-id="46f67-158">67</span><span class="sxs-lookup"><span data-stu-id="46f67-158">67</span></span>|<span data-ttu-id="46f67-159">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="46f67-159">USD</span></span>     |
