---
title: نظرة عامة على أبعاد التسعير
description: يقدم هذا الموضوع معلومات حول أبعاد التسعير في Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 11/30/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 33f55976eafedd046fba952ab6381c297ab4e271
ms.sourcegitcommit: 13a4e58eddbb0f81aca07c1ff452c420dbd8a68f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/30/2020
ms.locfileid: "4650168"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="0ea79-103">نظرة عامة على أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="0ea79-103">Pricing dimensions overview</span></span>

<span data-ttu-id="0ea79-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="0ea79-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0ea79-105">الأبعاد المستخدمة في الموارد البشرية لإعداد التسعير والتكاليف تنقسم إلى فئتين:</span><span class="sxs-lookup"><span data-stu-id="0ea79-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="0ea79-106">أشخاص</span><span class="sxs-lookup"><span data-stu-id="0ea79-106">People</span></span>
- <span data-ttu-id="0ea79-107">العمل المخطط</span><span class="sxs-lookup"><span data-stu-id="0ea79-107">Planned work</span></span>

<span data-ttu-id="0ea79-108">ولهذا السبب، هناك نوعان من قيم أبعاد التسعير المتوفرة:</span><span class="sxs-lookup"><span data-stu-id="0ea79-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="0ea79-109">**مجموعات الخيارات**: الأبعاد التي تمثل تعدادًا ثابتًا لمجموعة من القيم.</span><span class="sxs-lookup"><span data-stu-id="0ea79-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="0ea79-110">**القيم المستندة إلى الكيانات**: الأبعاد التي يمكن أن تكون مجموعة متنوعة من القيم.</span><span class="sxs-lookup"><span data-stu-id="0ea79-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="0ea79-111">أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="0ea79-111">Pricing dimensions</span></span>

<span data-ttu-id="0ea79-112">يتم شحن Dynamics 365 Project Operations بمجموعة افتراضية من أبعاد التسعير.</span><span class="sxs-lookup"><span data-stu-id="0ea79-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="0ea79-113">يمكنك عرض أبعاد التسعير هذه عن طريق الانتقال إلى **عمليات المشروع** > **المعلمات**.</span><span class="sxs-lookup"><span data-stu-id="0ea79-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="0ea79-114">في سجل المعلمات، في علامة التبويب **أبعاد التسعير المستندة إلى المبلغ**، تحقق من أن الدور، **msdyn_resourcecategory** والوحدة التنظيمية للموارد، **msdyn_organizationalunit** يشتملان على الحقلين **قابل للتطبيق على المبيعات** **قابل للتطبيق على التكلفة** معينين إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="0ea79-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="0ea79-115">مع تمكين هذه الحقول، سيتيح لك إمكانية إعداد السعر والتكلفة لكل مجموعة دور ووحدة تنظيمية.</span><span class="sxs-lookup"><span data-stu-id="0ea79-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

![لقطة شاشة لمعلمات Project Service مع تمييز "قابل للتطبيق على المبيعات"](media/PS-OOB-parameters.png)

<span data-ttu-id="0ea79-117">إذا كنت بحاجة إلى أسعار أو تكلفه للموارد الخاصة بك باستخدام سمات إضافية، فيمكنك إنشاء حقول وكيانات وأبعاد مخصصة.</span><span class="sxs-lookup"><span data-stu-id="0ea79-117">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="0ea79-118">لمزيد من المعلومات، راجع المواضيع التالية:</span><span class="sxs-lookup"><span data-stu-id="0ea79-118">For more information, see the following topics.</span></span> 
  
  > [!NOTE]
  > <span data-ttu-id="0ea79-119">يجب إكمال الإجراءات بالترتيب الذي تم سردها به.</span><span class="sxs-lookup"><span data-stu-id="0ea79-119">The procedures must be completed in the order they are listed.</span></span>

1. [<span data-ttu-id="0ea79-120">إنشاء حل لأبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="0ea79-120">Create a solution for custom pricing dimensions</span></span>](../sales/create-solution-custompd.md)
2. [<span data-ttu-id="0ea79-121">إنشاء حقول وكيانات مخصصة</span><span class="sxs-lookup"><span data-stu-id="0ea79-121">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md)
3. [<span data-ttu-id="0ea79-122">إضافة حقول مخصصة إلى إعداد الأسعار وكيانات الحركات </span><span class="sxs-lookup"><span data-stu-id="0ea79-122">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
4. [<span data-ttu-id="0ea79-123">إعداد الحقول المخصصة كأبعاد تسعير</span><span class="sxs-lookup"><span data-stu-id="0ea79-123">Set up custom fields as pricing dimensions</span></span>](set-up-custom-fields-pricing-dimensions.md)
5. [<span data-ttu-id="0ea79-124">تحديث سمات المكونات الإضافية لتشمل أبعاد التسعير الجديدة</span><span class="sxs-lookup"><span data-stu-id="0ea79-124">Update plug-in attributes to include new pricing dimensions</span></span>](update-plugin-attributes-pd.md)


## <a name="pricing-human-resource-time"></a><span data-ttu-id="0ea79-125">وقت المورد البشري للتسعير</span><span class="sxs-lookup"><span data-stu-id="0ea79-125">Pricing human resource time</span></span>
<span data-ttu-id="0ea79-126">غالبًا ما تكون كيفية قيام المؤسسة بتسعير وقت الموارد البشرية اعتبارًا استراتيجيًا مهمًا يؤثر بشكل مباشر على ربحية المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="0ea79-126">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="0ea79-127">اعمل مع الفرق المالية ورؤساء التدريب عندما تكون مؤسستك جاهزة لتحديد كيف تريد إعداد فاتورة ومعدلات تكلفة لوقت الموارد البشرية.</span><span class="sxs-lookup"><span data-stu-id="0ea79-127">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="0ea79-128">تشمل الاعتبارات الأخرى للتسعير ما إذا كان يجب إعادة استخدام الحقول أو الكيانات التي لا تمثل أبعادًا للتسعير حاليًا ولكن يتم تطبيقها كبعد تسعير لمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="0ea79-128">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="0ea79-129">تعتبر الحقول مثل **فئة المعاملات** (**msdyn_transactioncategory**) و **المورد القابل للحجز** (**bookableresource**) أمثلة على أبعاد المرشحين.</span><span class="sxs-lookup"><span data-stu-id="0ea79-129">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="0ea79-130">ضع في اعتبارك ما إذا كان يجب أن يكون بُعد التسعير الخاص بك عبارة عن جدول أو مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="0ea79-130">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="0ea79-131">إذا كنت تتوقع تغييرات في قيم البعد الذي يتجاوز 10 أو 12 وتحتاج إلى سمات إضافية على هذه القيم ، فيمكنك إنشاء كيان بدلاً من مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="0ea79-131">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="0ea79-132">تتطلب المحافظة على مجموعة خيارات ، مثل إضافة القيم أو إزالتها ، مسؤولًا أو مطورًا ، بينما يمكن لمعظم المستخدمين إضافة صفوف جديدة إلى جدول.</span><span class="sxs-lookup"><span data-stu-id="0ea79-132">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="0ea79-133">يوضح المثال التالي معدلات الفاتورة التي تم إعدادها بناءً على الدور ووحدة توفير الموارد التي ينتمي إليها المورد.</span><span class="sxs-lookup"><span data-stu-id="0ea79-133">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="0ea79-134">تعتمد معدلات التكلفة عادة على نطاق مرتب الموظف ووحدة المؤسسة التي ينتمي إليها.</span><span class="sxs-lookup"><span data-stu-id="0ea79-134">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="0ea79-135">في هذا المثال ، ستبدو جداول معدل الفاتورة ومعدل التكلفة كما يلي.</span><span class="sxs-lookup"><span data-stu-id="0ea79-135">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="0ea79-136">**نموذج أسعار الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="0ea79-136">**Sample bill rates**</span></span>

| <span data-ttu-id="0ea79-137">الدور</span><span class="sxs-lookup"><span data-stu-id="0ea79-137">Role</span></span>        | <span data-ttu-id="0ea79-138">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="0ea79-138">Org Unit</span></span>    |<span data-ttu-id="0ea79-139">الوحدة</span><span class="sxs-lookup"><span data-stu-id="0ea79-139">Unit</span></span>      |<span data-ttu-id="0ea79-140">السعر</span><span class="sxs-lookup"><span data-stu-id="0ea79-140">Price</span></span>      |<span data-ttu-id="0ea79-141">العملات</span><span class="sxs-lookup"><span data-stu-id="0ea79-141">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="0ea79-142">المطور</span><span class="sxs-lookup"><span data-stu-id="0ea79-142">Developer</span></span>   | <span data-ttu-id="0ea79-143">Contoso US</span><span class="sxs-lookup"><span data-stu-id="0ea79-143">Contoso US</span></span>  |<span data-ttu-id="0ea79-144">Hour‬</span><span class="sxs-lookup"><span data-stu-id="0ea79-144">Hour</span></span> | <span data-ttu-id="0ea79-145">200</span><span class="sxs-lookup"><span data-stu-id="0ea79-145">200</span></span>|<span data-ttu-id="0ea79-146">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="0ea79-146">USD</span></span>     |
| <span data-ttu-id="0ea79-147">المطور</span><span class="sxs-lookup"><span data-stu-id="0ea79-147">Developer</span></span>   | <span data-ttu-id="0ea79-148">شركة حسني بالهند</span><span class="sxs-lookup"><span data-stu-id="0ea79-148">Contoso India</span></span> |<span data-ttu-id="0ea79-149">Hour‬</span><span class="sxs-lookup"><span data-stu-id="0ea79-149">Hour</span></span>|   <span data-ttu-id="0ea79-150">112</span><span class="sxs-lookup"><span data-stu-id="0ea79-150">112</span></span>|<span data-ttu-id="0ea79-151">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="0ea79-151">USD</span></span>     |


<span data-ttu-id="0ea79-152">**نموذج أسعار التكاليف**</span><span class="sxs-lookup"><span data-stu-id="0ea79-152">**Sample cost rates**</span></span>

| <span data-ttu-id="0ea79-153">نطاق الراتب</span><span class="sxs-lookup"><span data-stu-id="0ea79-153">Salary Band</span></span>     | <span data-ttu-id="0ea79-154">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="0ea79-154">Org Unit</span></span>    |<span data-ttu-id="0ea79-155">الوحدة</span><span class="sxs-lookup"><span data-stu-id="0ea79-155">Unit</span></span>      |<span data-ttu-id="0ea79-156">السعر</span><span class="sxs-lookup"><span data-stu-id="0ea79-156">Price</span></span>      |<span data-ttu-id="0ea79-157">العملات</span><span class="sxs-lookup"><span data-stu-id="0ea79-157">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="0ea79-158">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="0ea79-158">My company_Band1</span></span> | <span data-ttu-id="0ea79-159">Contoso US</span><span class="sxs-lookup"><span data-stu-id="0ea79-159">Contoso US</span></span>  |<span data-ttu-id="0ea79-160">Hour‬</span><span class="sxs-lookup"><span data-stu-id="0ea79-160">Hour</span></span> | <span data-ttu-id="0ea79-161">145</span><span class="sxs-lookup"><span data-stu-id="0ea79-161">145</span></span>|<span data-ttu-id="0ea79-162">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="0ea79-162">USD</span></span>     |
| <span data-ttu-id="0ea79-163">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="0ea79-163">My company_Band2</span></span> | <span data-ttu-id="0ea79-164">شركة حسني بالهند</span><span class="sxs-lookup"><span data-stu-id="0ea79-164">Contoso India</span></span> |<span data-ttu-id="0ea79-165">Hour‬</span><span class="sxs-lookup"><span data-stu-id="0ea79-165">Hour</span></span>|   <span data-ttu-id="0ea79-166">67</span><span class="sxs-lookup"><span data-stu-id="0ea79-166">67</span></span>|<span data-ttu-id="0ea79-167">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="0ea79-167">USD</span></span>     |
