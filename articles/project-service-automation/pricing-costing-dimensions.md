---
title: الصفحة الرئيسية لأبعاد التسعير والتكلفة
description: يوفر هذا الموضوع نظرة عامة على أبعاد التسعير.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 425d7bb8-9015-4f67-b9c9-cf3602e9afe8
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 2379d0d2e038f28a1a8df87a851e9bf7db7fe33f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748636"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="7dd01-103">الصفحة الرئيسية لأبعاد التسعير والتكلفة</span><span class="sxs-lookup"><span data-stu-id="7dd01-103">Pricing and costing dimensions home page</span></span>

<span data-ttu-id="7dd01-104">الأبعاد المستخدمة في الموارد البشرية لإعداد التسعير والتكاليف تنقسم إلى فئتين:</span><span class="sxs-lookup"><span data-stu-id="7dd01-104">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="7dd01-105">أشخاص</span><span class="sxs-lookup"><span data-stu-id="7dd01-105">People</span></span>
- <span data-ttu-id="7dd01-106">العمل المخطط</span><span class="sxs-lookup"><span data-stu-id="7dd01-106">Planned work</span></span>

<span data-ttu-id="7dd01-107">ولهذا السبب، هناك نوعان من قيم أبعاد التسعير المتوفرة في Project Service Automation (PSA):</span><span class="sxs-lookup"><span data-stu-id="7dd01-107">Because of this, there are two types of pricing dimension values available in Project Service Automation (PSA):</span></span> 

- <span data-ttu-id="7dd01-108">**مجموعات الخيارات** - الأبعاد التي تمثل تعدادًا ثابتًا لمجموعه من القيم.</span><span class="sxs-lookup"><span data-stu-id="7dd01-108">**Option sets** - Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="7dd01-109">**القيم المستندة إلى الكيانات** - الأبعاد التي يمكن أن تكون مجموعة متنوعة من القيم.</span><span class="sxs-lookup"><span data-stu-id="7dd01-109">**Entity-based values** - Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="7dd01-110">أبعاد التسعير</span><span class="sxs-lookup"><span data-stu-id="7dd01-110">Pricing dimensions</span></span>

<span data-ttu-id="7dd01-111">يتم شحن PSA بمجموعة افتراضية من أبعاد التسعير.</span><span class="sxs-lookup"><span data-stu-id="7dd01-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="7dd01-112">يمكنك عرضها عن طريق الانتقال إلى **Project Service** > **المعلمات**.</span><span class="sxs-lookup"><span data-stu-id="7dd01-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="7dd01-113">في سجل المعلمات، في علامة التبويب **أبعاد التسعير المستندة إلى المبلغ**، تحقق من أن الدور، **msdyn_resourcecategory** والوحدة التنظيمية للموارد، **msdyn_organizationalunit** يشتملان على الحقلين **قابل للتطبيق على المبيعات** **قابل للتطبيق على التكلفة** معينين إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7dd01-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="7dd01-114">سيتيح لك ذلك إمكانية إعداد السعر والتكلفة لكل مجموعة دور ووحدة تنظيمية.</span><span class="sxs-lookup"><span data-stu-id="7dd01-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![لقطة شاشة لمعلمات Project Service مع تمييز "قابل للتطبيق على المبيعات"](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="7dd01-116">إذا كنت تستخدم حقول الدور والوحدة التنظيمية الجاهزة كأبعاد تسعير قبل الإصدار 3 من PSA، فلن يكون هناك أي تغيير ملحوظ.</span><span class="sxs-lookup"><span data-stu-id="7dd01-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="7dd01-117">يمكنك متابعة استخدام Project Service كالمعتاد.</span><span class="sxs-lookup"><span data-stu-id="7dd01-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="7dd01-118">إذا كنت بحاجة إلى أسعار أو تكلفه للموارد الخاصة بك باستخدام سمات إضافية، فيمكنك إنشاء حقول وكيانات وأبعاد مخصصة.</span><span class="sxs-lookup"><span data-stu-id="7dd01-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="7dd01-119">لمزيد من المعلومات، راجع الموضوعات التالية، ومع ذلك لاحظ أنه يجب عليك إكمال الإجراءات بالترتيب المذكور أدناه:</span><span class="sxs-lookup"><span data-stu-id="7dd01-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="7dd01-120">إنشاء حقول وكيانات مخصصة</span><span class="sxs-lookup"><span data-stu-id="7dd01-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="7dd01-121">إضافة حقول مخصصة إلى إعداد الأسعار وكيانات المعاملات</span><span class="sxs-lookup"><span data-stu-id="7dd01-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="7dd01-122">إعداد الحقول المخصصة كأبعاد تسعير</span><span class="sxs-lookup"><span data-stu-id="7dd01-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="7dd01-123">تحديث سمات المكونات الإضافية لتشمل أبعاد التسعير الجديدة</span><span class="sxs-lookup"><span data-stu-id="7dd01-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="7dd01-124">وقت المورد البشري للتسعير</span><span class="sxs-lookup"><span data-stu-id="7dd01-124">Pricing human resource time</span></span>
<span data-ttu-id="7dd01-125">غالبًا ما تكون كيفية قيام المؤسسة بتسعير وقت الموارد البشرية اعتبارًا استراتيجيًا مهمًا يؤثر بشكل مباشر على ربحية المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="7dd01-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="7dd01-126">اعمل مع الفرق المالية ورؤساء التدريب عندما تكون مؤسستك جاهزة لتحديد كيف تريد إعداد فاتورة ومعدلات تكلفة لوقت الموارد البشرية.</span><span class="sxs-lookup"><span data-stu-id="7dd01-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="7dd01-127">تشمل الاعتبارات الأخرى للتسعير ما إذا كان يجب إعادة استخدام الحقول أو الكيانات التي لا تمثل أبعادًا للتسعير حاليًا ولكن يتم تطبيقها كبعد تسعير لمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="7dd01-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="7dd01-128">تعتبر الحقول مثل **فئة المعاملات** (**msdyn_transactioncategory**) و**المورد القابل للحجز** (**bookableresource**) أمثلة على أبعاد المرشحين.</span><span class="sxs-lookup"><span data-stu-id="7dd01-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="7dd01-129">يجب عليك أيضًا التفكير فيما إذا كان يجب أن يكون بُعد التسعير الخاص بك جدولًا أو مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="7dd01-129">You should also consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="7dd01-130">إذا كنت تتوقع تغييرات في قيم البعد الذي يتجاوز 10 أو 12 وتحتاج إلى سمات إضافية على هذه القيم ، فيمكنك إنشاء كيان بدلاً من مجموعة خيارات.</span><span class="sxs-lookup"><span data-stu-id="7dd01-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="7dd01-131">تتطلب المحافظة على مجموعة خيارات ، مثل إضافة القيم أو إزالتها ، مسؤولًا أو مطورًا ، بينما يمكن لمعظم المستخدمين إضافة صفوف جديدة إلى جدول.</span><span class="sxs-lookup"><span data-stu-id="7dd01-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="7dd01-132">يوضح المثال التالي معدلات الفاتورة التي تم إعدادها بناءً على الدور ووحدة توفير الموارد التي ينتمي إليها المورد.</span><span class="sxs-lookup"><span data-stu-id="7dd01-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="7dd01-133">تعتمد معدلات التكلفة عادة على نطاق مرتب الموظف ووحدة المؤسسة التي ينتمي إليها.</span><span class="sxs-lookup"><span data-stu-id="7dd01-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="7dd01-134">في هذا المثال ، ستبدو جداول معدل الفاتورة ومعدل التكلفة كما يلي.</span><span class="sxs-lookup"><span data-stu-id="7dd01-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="7dd01-135">**نموذج أسعار الفاتورة**</span><span class="sxs-lookup"><span data-stu-id="7dd01-135">**Sample bill rates**</span></span>

| <span data-ttu-id="7dd01-136">الدور</span><span class="sxs-lookup"><span data-stu-id="7dd01-136">Role</span></span>        | <span data-ttu-id="7dd01-137">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="7dd01-137">Org Unit</span></span>    |<span data-ttu-id="7dd01-138">الوحدة</span><span class="sxs-lookup"><span data-stu-id="7dd01-138">Unit</span></span>      |<span data-ttu-id="7dd01-139">السعر</span><span class="sxs-lookup"><span data-stu-id="7dd01-139">Price</span></span>      |<span data-ttu-id="7dd01-140">العملات</span><span class="sxs-lookup"><span data-stu-id="7dd01-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="7dd01-141">المطور</span><span class="sxs-lookup"><span data-stu-id="7dd01-141">Developer</span></span>   | <span data-ttu-id="7dd01-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="7dd01-142">Contoso US</span></span>  |<span data-ttu-id="7dd01-143">Hour‬</span><span class="sxs-lookup"><span data-stu-id="7dd01-143">Hour</span></span> | <span data-ttu-id="7dd01-144">200</span><span class="sxs-lookup"><span data-stu-id="7dd01-144">200</span></span>|<span data-ttu-id="7dd01-145">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="7dd01-145">USD</span></span>     |
| <span data-ttu-id="7dd01-146">المطور</span><span class="sxs-lookup"><span data-stu-id="7dd01-146">Developer</span></span>   | <span data-ttu-id="7dd01-147">شركة حسني بالهند</span><span class="sxs-lookup"><span data-stu-id="7dd01-147">Contoso India</span></span> |<span data-ttu-id="7dd01-148">Hour‬</span><span class="sxs-lookup"><span data-stu-id="7dd01-148">Hour</span></span>|   <span data-ttu-id="7dd01-149">112</span><span class="sxs-lookup"><span data-stu-id="7dd01-149">112</span></span>|<span data-ttu-id="7dd01-150">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="7dd01-150">USD</span></span>     |


<span data-ttu-id="7dd01-151">**نموذج أسعار التكاليف**</span><span class="sxs-lookup"><span data-stu-id="7dd01-151">**Sample cost rates**</span></span>

| <span data-ttu-id="7dd01-152">نطاق الراتب</span><span class="sxs-lookup"><span data-stu-id="7dd01-152">Salary Band</span></span>     | <span data-ttu-id="7dd01-153">الوحدة التنظيمية</span><span class="sxs-lookup"><span data-stu-id="7dd01-153">Org Unit</span></span>    |<span data-ttu-id="7dd01-154">الوحدة</span><span class="sxs-lookup"><span data-stu-id="7dd01-154">Unit</span></span>      |<span data-ttu-id="7dd01-155">السعر</span><span class="sxs-lookup"><span data-stu-id="7dd01-155">Price</span></span>      |<span data-ttu-id="7dd01-156">العملات</span><span class="sxs-lookup"><span data-stu-id="7dd01-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="7dd01-157">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="7dd01-157">My company_Band1</span></span> | <span data-ttu-id="7dd01-158">Contoso US</span><span class="sxs-lookup"><span data-stu-id="7dd01-158">Contoso US</span></span>  |<span data-ttu-id="7dd01-159">Hour‬</span><span class="sxs-lookup"><span data-stu-id="7dd01-159">Hour</span></span> | <span data-ttu-id="7dd01-160">145</span><span class="sxs-lookup"><span data-stu-id="7dd01-160">145</span></span>|<span data-ttu-id="7dd01-161">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="7dd01-161">USD</span></span>     |
| <span data-ttu-id="7dd01-162">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="7dd01-162">My company_Band2</span></span> | <span data-ttu-id="7dd01-163">شركة حسني بالهند</span><span class="sxs-lookup"><span data-stu-id="7dd01-163">Contoso India</span></span> |<span data-ttu-id="7dd01-164">Hour‬</span><span class="sxs-lookup"><span data-stu-id="7dd01-164">Hour</span></span>|   <span data-ttu-id="7dd01-165">67</span><span class="sxs-lookup"><span data-stu-id="7dd01-165">67</span></span>|<span data-ttu-id="7dd01-166">دولار أمريكي</span><span class="sxs-lookup"><span data-stu-id="7dd01-166">USD</span></span>     |
