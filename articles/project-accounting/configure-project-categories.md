---
title: تكوين فئات المشروعات
description: يقدم هذا الموضوع معلومات حول إعدادات فئات المشروع.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b7adf61a82714a0148d9c8b1d2b2b37fd611c1cf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287492"
---
# <a name="configure-project-categories"></a><span data-ttu-id="19205-103">تكوين فئات المشروعات</span><span class="sxs-lookup"><span data-stu-id="19205-103">Configure project categories</span></span>

<span data-ttu-id="19205-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="19205-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="19205-105">يقدم Project Operations إمكانيات فعالة لتصنيف الإيرادات والمصروفات على المشروعات.</span><span class="sxs-lookup"><span data-stu-id="19205-105">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="19205-106">توفر الفئات القدرة على الإبلاغ عن حركات المشروع وتحليلها، وتعزيز الترحيل إلى دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="19205-106">Categories provide the ability to report on and analyze project transactions, and drive posting to the general ledger.</span></span>

<span data-ttu-id="19205-107">يوضح المخطط التالي الارتباط بين فئات الحركات والفئات المشتركة وفئات المشروع.</span><span class="sxs-lookup"><span data-stu-id="19205-107">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span> 

<span data-ttu-id="19205-108">تعتبر فئات الحركات التجميع الأساسي لحركات المشروع.</span><span class="sxs-lookup"><span data-stu-id="19205-108">Transaction categories are the basic grouping for project transactions.</span></span> <span data-ttu-id="19205-109">يوجد داخل هذا التجميع مجموعة من الفئات المشتركة التي يمكن مشاركتها عبر التطبيقات والوحدات النمطية.</span><span class="sxs-lookup"><span data-stu-id="19205-109">Within that grouping, there is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="19205-110">إذا نظرنا إلى التفاصيل، تعتبر فئات المشروع مستوى المشروعات الأكثر دقة.</span><span class="sxs-lookup"><span data-stu-id="19205-110">Getting even further into specifics, project categories are the most granular level of categories.</span></span> <span data-ttu-id="19205-111">تتعلق فئات المشروع بالكيان القانوني والوحدة النمطية والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="19205-111">Project categories are specific to legal entity, module, and application.</span></span>

![الارتباط بين فئات الحركات والفئات المشتركة وفئات المشروع](media/project-categories.png)

## <a name="transaction-categories"></a><span data-ttu-id="19205-113">فئات الحركات</span><span class="sxs-lookup"><span data-stu-id="19205-113">Transaction categories</span></span>

<span data-ttu-id="19205-114">تمثل فئات الحركات التجميع الأساسي لحركات المشروع وهي لا تتعلق بنوع الشركة أو الحركة.</span><span class="sxs-lookup"><span data-stu-id="19205-114">Transaction categories represent the basic grouping for project transactions and are not company or transaction type-specific.</span></span> <span data-ttu-id="19205-115">على سبيل المثال، تستخدم شركة Contoso Robotics فئات التصميم والسفر والتثبيت وحركة الخدمة لتجميع حركات المشروع.</span><span class="sxs-lookup"><span data-stu-id="19205-115">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group Project transactions.</span></span>

<span data-ttu-id="19205-116">يتم تحديد فئات الحركات في الوحدة النمطية Project Operations.</span><span class="sxs-lookup"><span data-stu-id="19205-116">Transaction categories are defined in the Project Operations module.</span></span> 
1. <span data-ttu-id="19205-117">انتقل إلى **الإعدادات** \> **فئات الحركات** لفتح النموذج.</span><span class="sxs-lookup"><span data-stu-id="19205-117">Go to **Settings** \> **Transaction Categories** to open the form.</span></span> 
2. <span data-ttu-id="19205-118">قم بإنشاء فئة حركة جديدة إما بتحديد **جديد** أو بتحديد **استيراد من Excel**.</span><span class="sxs-lookup"><span data-stu-id="19205-118">Create a new transaction category either by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="19205-119">الفئات المشتركة</span><span class="sxs-lookup"><span data-stu-id="19205-119">Shared categories</span></span>

<span data-ttu-id="19205-120">يستخدم Dynamics 365 مفهوم الفئات المشتركة لتصنيف المصروفات في تطبيقات مختلفة، مثل Dynamics 365 Finance وDynamics 365 Supply Chain وDynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="19205-120">Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as Dynamics 365 Finance, Dynamics 365 Supply Chain, and Dynamics 365 Project Operations.</span></span> <span data-ttu-id="19205-121">النسبة لكل فئة حركة يتم إنشاؤها، ينشئ Project Operations بشكل تلقائيا أربع فئات مشتركة ذات صلة: الساعات والمصروفات والرسوم والصنف.</span><span class="sxs-lookup"><span data-stu-id="19205-121">For each Transaction category created, Project Operations automatically creates four related Shared categories: Hours, Expense, Fees, and Item.</span></span> <span data-ttu-id="19205-122">يمكنك مراجعة الفئات المشتركة وضبطها من خلال الانتقال إلى **إدارة المشاريع والمحاسبة‬** \> **الإعداد** \> **الفئات** \> **الفئات المشتركة**.</span><span class="sxs-lookup"><span data-stu-id="19205-122">You can review and adjust the shared categories by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="19205-123">فئات المشروع</span><span class="sxs-lookup"><span data-stu-id="19205-123">Project categories</span></span>

<span data-ttu-id="19205-124">تمثل فئات المشروع المستوي الأكثر دقة من تكوين الفئة ويجب تكوينها بشكل منفصل، ولكل شركة من خلال محاسب المشروع.</span><span class="sxs-lookup"><span data-stu-id="19205-124">Project categories represent most granular level of category configuration and must be configured separately, and for each company, by a Project accountant.</span></span>

1. <span data-ttu-id="19205-125">انتقل إلى **إدارة المشاريع والمحاسبة‬‬‏‫** \> **الإعداد** \> **الفئات** \> **فئات المشروع**.</span><span class="sxs-lookup"><span data-stu-id="19205-125">Go to **Project Management and Accounting** \> **Setup** \> **Categories** \> **Project categories**.</span></span>
2. <span data-ttu-id="19205-126">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="19205-126">Select **New**.</span></span>
3. <span data-ttu-id="19205-127">حدد **معرف الفئة** للفئة المشتركة التي أنشأته في القسم السابق.</span><span class="sxs-lookup"><span data-stu-id="19205-127">Select the **Category ID** of the Shared category you created in the previous section.</span></span> <span data-ttu-id="19205-128">يسمح لك Project Operations باستخدام فقط تلك الفئات المشتركة المرتبطة بفئات الحركات.</span><span class="sxs-lookup"><span data-stu-id="19205-128">Project Operations allows using only those shared categories that are associated with transaction categories.</span></span>
4. <span data-ttu-id="19205-129">حدد مجموعة فئات.</span><span class="sxs-lookup"><span data-stu-id="19205-129">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="19205-130">مجموعات الفئات</span><span class="sxs-lookup"><span data-stu-id="19205-130">Category groups</span></span>

<span data-ttu-id="19205-131">تُستخدم مجموعات الفئات لمشاركة الخصائص، بشكل أساسي ملفات تعريف الترحيل، بين فئات المشروع ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="19205-131">Category groups are used to share properties, primarily posting profiles, between related Project categories.</span></span> <span data-ttu-id="19205-132">يجب أن يكون هناك مجموعة فئات واحدة على الأقل لكل نوع حركة ويتم تعيين مجموعة لكلف فئة مشروع.</span><span class="sxs-lookup"><span data-stu-id="19205-132">There must be at least one category group for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="19205-133">يتم تحديد مواصفات الترحيل في Project Operations بواسطة قواعد ملفات تعريف إيرادات وتكلفة المشروع وفئات المشاريع ومجموعات الفئات.</span><span class="sxs-lookup"><span data-stu-id="19205-133">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="19205-134">يمكنك إعداد مجموعات الفئات من خلال الانتقال إلى **إدارة المشاريع والمحاسبة** \> **الإعداد** \> **الفئات** \> **مجموعات الفئات**.</span><span class="sxs-lookup"><span data-stu-id="19205-134">You can set up category groups by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Category groups**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]