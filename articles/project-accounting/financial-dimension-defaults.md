---
title: افتراضيات الأبعاد المالية
description: يقدم هذا الموضوع معلومات حول كيفية إعداد الإعدادات الافتراضية للأبعاد المالية.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: aa6771ba5346fd4133b82c3e670badfa7655299f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131867"
---
# <a name="financial-dimension-defaults"></a><span data-ttu-id="16c9e-103">افتراضيات الأبعاد المالية</span><span class="sxs-lookup"><span data-stu-id="16c9e-103">Financial dimension defaults</span></span>

<span data-ttu-id="16c9e-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="16c9e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="16c9e-105">يستخدم Dynamics 365 Project Operations إطار عمل [الأبعاد المالية](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) في Dynamics 365 Finance لتوفير تحليلات إضافية حول حركات المشروع على دفتر الأستاذ الفرعي ودفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="16c9e-105">Dynamics 365 Project Operations uses the [Financial dimensions](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="16c9e-106">يمكن تعيين الأبعاد المالية الافتراضية على عميل أو مصدر تمويل المشروع أو مرحلة رئيسية أو شرط تعاقد المشروع أو مشروع.</span><span class="sxs-lookup"><span data-stu-id="16c9e-106">Default financial dimensions can be set on a customer, project funding source, milestone, project contract line, or project.</span></span>

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="16c9e-107">تحديد الأبعاد المالية الافتراضية لعميل</span><span class="sxs-lookup"><span data-stu-id="16c9e-107">Define default financial dimensions for a customer</span></span>

<span data-ttu-id="16c9e-108">تم تحديد القيم الافتراضية لأبعاد العميل في Finance.</span><span class="sxs-lookup"><span data-stu-id="16c9e-108">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="16c9e-109">أكمل الخطوات التالية لتعيين القيم الافتراضية للأبعاد.</span><span class="sxs-lookup"><span data-stu-id="16c9e-109">Complete the following steps to set dimension defaults.</span></span>

1. <span data-ttu-id="16c9e-110">انتقل إلى **حسابات المقبوضات** > **العملاء** > **جميع العملاء**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-110">Go to **Accounts receivable** > **Customers** > **All customers**.</span></span>
2. <span data-ttu-id="16c9e-111">من صفحة **العملاء**، في علامة التبويب **الأبعاد المالية**، عيّن قيم الأبعاد المالية لعميل محدد.</span><span class="sxs-lookup"><span data-stu-id="16c9e-111">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="16c9e-112">تحديد الأبعاد المالية الافتراضية لعقود المشروع</span><span class="sxs-lookup"><span data-stu-id="16c9e-112">Define default financial dimensions for project contracts</span></span>

<span data-ttu-id="16c9e-113">يتم إنشاء عقود المشروع وصيانتها في Common Data Service (CDS).</span><span class="sxs-lookup"><span data-stu-id="16c9e-113">Project contracts are created and maintained in Common Data Service (CDS).</span></span> <span data-ttu-id="16c9e-114">يتم تعيين سمات المحاسبة الخاصة بعقود المشروع في الوحدة النمطية **إدارة المشاريع والمحاسبة** في Finance.</span><span class="sxs-lookup"><span data-stu-id="16c9e-114">Accounting attributes for project contracts are set in the **Project management and accounting** module in Finance.</span></span>

### <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="16c9e-115">تعيين الأبعاد المالية لمصدر تمويل مشروع</span><span class="sxs-lookup"><span data-stu-id="16c9e-115">Set financial dimensions for a project funding source</span></span>

1. <span data-ttu-id="16c9e-116">انتقل إلى **إدارة المشاريع والمحاسبة** > **المشاريع** > **عقود المشروع**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-116">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="16c9e-117">حدد السجل الذي ترغب في تحديثه، وعلى علامة تبويب **عقد المشروع**، حدد **إظهار المحاسبة الافتراضية**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-117">Select the record you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="16c9e-118">قم بتوسيع **المعلومات ذات الصلة**، وحدد علامة التبويب **مصادر التمويل**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-118">Expand **Related information** and select the **Funding sources** tab.</span></span>
4. <span data-ttu-id="16c9e-119">قم بتعيين القيم الافتراضية للأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="16c9e-119">Set the financial dimension defaults.</span></span> <span data-ttu-id="16c9e-120">لاحظ أنه يتم تعيين الأبعاد المالية الافتراضية من حساب العميل.</span><span class="sxs-lookup"><span data-stu-id="16c9e-120">Notice that the financial dimensions default from the customer account.</span></span>

### <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="16c9e-121">تعيين الأبعاد المالية لشرط تعاقد المشروع</span><span class="sxs-lookup"><span data-stu-id="16c9e-121">Set financial dimensions for a project contract line</span></span>

1. <span data-ttu-id="16c9e-122">انتقل إلى **إدارة المشاريع والمحاسبة** > **المشاريع** > **عقود المشروع**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-122">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="16c9e-123">حدد السجل الذي ترغب في تحديثه، وعلى علامة تبويب **عقد المشروع**، حدد **إظهار المحاسبة الافتراضية**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-123">Select the record you want to update and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="16c9e-124">قم بتوسيع **المعلومات ذات الصلة**، وحدد علامة التبويب **شروط التعاقد**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-124">Expand **Related information** and select the **Contract lines** tab.</span></span>
4. <span data-ttu-id="16c9e-125">قم بتعيين القيم الافتراضية للأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="16c9e-125">Set the financial dimension defaults.</span></span> <span data-ttu-id="16c9e-126">تكون القيم الافتراضية للأبعاد المالية قابلة للتطبيق ويمكن استخدامها فقط مع شروط التعاقد ثابتة السعر (المراحل الرئيسية).</span><span class="sxs-lookup"><span data-stu-id="16c9e-126">The financial dimension defaults are applicable and can be used only with Fixed price (milestone) contract lines.</span></span>

<span data-ttu-id="16c9e-127">تستخدم هذه القيم الافتراضية في الحركات على الحساب وبنود الفواتير التابعة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="16c9e-127">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="16c9e-128">تحديد الأبعاد المالية الافتراضية للمشاريع</span><span class="sxs-lookup"><span data-stu-id="16c9e-128">Define default financial dimensions for projects</span></span>

<span data-ttu-id="16c9e-129">يتم إنشاء المشاريع وصيانتها في CDS.</span><span class="sxs-lookup"><span data-stu-id="16c9e-129">Projects are created and maintained in CDS.</span></span> <span data-ttu-id="16c9e-130">يتم تعيين سمات المحاسبة الخاصة بالمشاريع في الوحدة النمطية **إدارة المشاريع والمحاسبة** في Finance.</span><span class="sxs-lookup"><span data-stu-id="16c9e-130">Accounting attributes for projects are set in the **Project management and accounting** module in Finance.</span></span>

1. <span data-ttu-id="16c9e-131">انتقل إلى **إدارة المشاريع والمحاسبة** > **المشاريع** > **كافة المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-131">Go to **Project management and accounting** > **Projects** > **All projects**.</span></span>
2. <span data-ttu-id="16c9e-132">حدد السجل الذي ترغب في تحديثه، وعلى علامة تبويب **المشروع**، حدد **إظهار المحاسبة الافتراضية**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-132">Select the record that you want to update and on the **Project** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="16c9e-133">قم بتوسيع **المعلومات ذات الصلة**، وحدد علامة التبويب **الإعداد**.</span><span class="sxs-lookup"><span data-stu-id="16c9e-133">Expand **Related information** and select the **Setup** tab.</span></span>
4. <span data-ttu-id="16c9e-134">قم بتعيين القيم الافتراضية للأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="16c9e-134">Set the financial dimension defaults.</span></span> <span data-ttu-id="16c9e-135">لاحظ أنه يتم تعيين الأبعاد المالية الافتراضية من حساب العميل.</span><span class="sxs-lookup"><span data-stu-id="16c9e-135">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="16c9e-136">إذا كان المشروع مقترنًا بشرط تعاقد مع عملاء متعددين لعقد المشروع، فسيتم استخدام العميل الأساسي لتعيين لقيم الافتراضية للأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="16c9e-136">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="16c9e-137">يتم استخدام الأبعاد المالية الافتراضية للمشروع لتعيين الإعدادات الافتراضية لبند دفتر الأستاذ لحركات الوقت والمصروفات والرسوم في **دفتر يومية تكامل Project Operations** في بنود فاتورة المشروع ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="16c9e-137">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration Journal** and on related project invoice lines.</span></span>
