---
title: شراء مواد غير مخزنة باستخدام فاتورة مورد معلقة
description: يوضح هذا الموضوع كيفية تسجيل فواتير الموردين المعلقة.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b5e6632d73c8a211b1f0d568be8e10ef47be77e2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993761"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="47da9-103">شراء مواد غير مخزنة باستخدام فاتورة مورد معلقة</span><span class="sxs-lookup"><span data-stu-id="47da9-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="47da9-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="47da9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="47da9-105">عندما تقوم شركة ما بشراء مواد غير خزينة لمشروع، يمكن تسجيل التكلفة فورًا مقابل المشروع.</span><span class="sxs-lookup"><span data-stu-id="47da9-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="47da9-106">على سبيل المثال، تقوم شركة Contoso Robotics US بتنفيذ مشروع تجديد للمعدات وتحتاج إلى تراخيص البرامج.</span><span class="sxs-lookup"><span data-stu-id="47da9-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="47da9-107">ويتم شراء هذه التراخيص من مورد خارجي.</span><span class="sxs-lookup"><span data-stu-id="47da9-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="47da9-108">باستخدام Dynamics 365 Finance، يقوم موظف حسابات المدفوعات بتسجيل مستند فاتورة مورد المعلقة وينسب سمات تكاليف الترخيص مباشرة مقابل مشروع تجديد المعدات.</span><span class="sxs-lookup"><span data-stu-id="47da9-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="47da9-109">قبل استخدام الوظيفة الموضحة في هذا الموضوع، راجع التكوينات المطلوبة وطبقها.</span><span class="sxs-lookup"><span data-stu-id="47da9-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="47da9-110">لمزيد من المعلومات، راجع [تمكين مواد غير مخزنة وفواتير المورد المعلقة](configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="47da9-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="47da9-111">ترحيل فاتورة مورد معلقة متعلقة بالمشروع</span><span class="sxs-lookup"><span data-stu-id="47da9-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="47da9-112">يمكن تسجيل فواتير المورد المعلقة في صفحة **فواتير المورد المعلقة** (**حسابات المدفوعات** > **الفواتير** > **فواتير المورد المعلقة**).</span><span class="sxs-lookup"><span data-stu-id="47da9-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="47da9-113">أكمل الخطوات التالية لترحيل فاتورة المورد المعلقة المتعلقة بالمشروع:</span><span class="sxs-lookup"><span data-stu-id="47da9-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="47da9-114">انتقل إلى **حسابات المدفوعات** > **الفواتير** وحدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="47da9-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="47da9-115">في الحقل **حساب الفاتورة**، حدد موردا، وفي الحقل **الرقم**، أدخل تعريف الفاتورة الخاص بالمورد.</span><span class="sxs-lookup"><span data-stu-id="47da9-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="47da9-116">أضف سطرا إلى فاتورة المورد، وفي الحقل **رقم العنصر**، حدد العنصر غير المخزن الذي تم شراؤه من المورد.</span><span class="sxs-lookup"><span data-stu-id="47da9-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="47da9-117">لا يمكن تسجيل أسطر فواتير المورد التي تستند إلى فئة شراء مقابل المشروع.</span><span class="sxs-lookup"><span data-stu-id="47da9-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="47da9-118">أضف الكمية التي تم شراؤها.</span><span class="sxs-lookup"><span data-stu-id="47da9-118">Add the quantity purchased.</span></span> <span data-ttu-id="47da9-119">يقوم النظام بتعبئة سعر الوحدة استنادا إلى تكوين أسعار العناصر غير المخزنة.</span><span class="sxs-lookup"><span data-stu-id="47da9-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="47da9-120">تحقق من إجمالي المبلغ والتفاصيل المطلوبة الأخرى على السطر.</span><span class="sxs-lookup"><span data-stu-id="47da9-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="47da9-121">في تفاصيل السطر، في علامة التبويب **مشروع**، حدد المعرف الخاص بالمشروع الذي سيتم تسجيل هذا العنصر له.</span><span class="sxs-lookup"><span data-stu-id="47da9-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="47da9-122">اختياريًا، قم بتحديد رقم النشاط وتحديث فئة المشروع وخاصية السطر.</span><span class="sxs-lookup"><span data-stu-id="47da9-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="47da9-123">قم بترحيل فاتورة المورد المعلقة.</span><span class="sxs-lookup"><span data-stu-id="47da9-123">Post pending vendor invoice.</span></span> <span data-ttu-id="47da9-124">عند ترحيل الفاتورة، فإن النظام يسجل:</span><span class="sxs-lookup"><span data-stu-id="47da9-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="47da9-125">مبلغ رصيد المورد.</span><span class="sxs-lookup"><span data-stu-id="47da9-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="47da9-126">مبلغ ضريبة المبيعات.</span><span class="sxs-lookup"><span data-stu-id="47da9-126">The sales tax amount.</span></span>
    - <span data-ttu-id="47da9-127">يتم تسجيل التكلفة مقابل المشروع في حساب تكامل الشراء.</span><span class="sxs-lookup"><span data-stu-id="47da9-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="47da9-128">المعاملة الفعلية للمشروع في Dataverse.</span><span class="sxs-lookup"><span data-stu-id="47da9-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="47da9-129">تتم معالجة هذه المعاملة أيضا باستخدام [دفتر يومية تكامل Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="47da9-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="47da9-130">يؤدي ترحيل دفتر اليومية هذا إلى نقل المبلغ من حساب تكامل الشراء إلى حساب تكلفة المشروع.</span><span class="sxs-lookup"><span data-stu-id="47da9-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
