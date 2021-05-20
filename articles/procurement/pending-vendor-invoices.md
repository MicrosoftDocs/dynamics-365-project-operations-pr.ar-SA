---
title: شراء مواد غير مخزنة باستخدام فاتورة مورد معلقة
description: يوضح هذا الموضوع كيفية تسجيل فواتير الموردين المعلقة.
author: sigitac
manager: tfehr
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7a706f419443dcdf92ce3b247d719943272907d0
ms.sourcegitcommit: 7468d668c48c1d87934aab9a034decd51e56dec6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/13/2021
ms.locfileid: "5880614"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="bdf76-103">شراء مواد غير مخزنة باستخدام فاتورة مورد معلقة</span><span class="sxs-lookup"><span data-stu-id="bdf76-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="bdf76-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="bdf76-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="bdf76-105">عندما تقوم شركة ما بشراء مواد غير خزينة لمشروع، يمكن تسجيل التكلفة فورًا مقابل المشروع.</span><span class="sxs-lookup"><span data-stu-id="bdf76-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="bdf76-106">على سبيل المثال، تقوم شركة Contoso Robotics US بتنفيذ مشروع تجديد للمعدات وتحتاج إلى تراخيص البرامج.</span><span class="sxs-lookup"><span data-stu-id="bdf76-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="bdf76-107">ويتم شراء هذه التراخيص من مورد خارجي.</span><span class="sxs-lookup"><span data-stu-id="bdf76-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="bdf76-108">باستخدام Dynamics 365 Finance، يقوم موظف حسابات المدفوعات بتسجيل مستند فاتورة مورد المعلقة وينسب سمات تكاليف الترخيص مباشرة مقابل مشروع تجديد المعدات.</span><span class="sxs-lookup"><span data-stu-id="bdf76-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="bdf76-109">قبل استخدام الوظيفة الموضحة في هذا الموضوع، راجع التكوينات المطلوبة وطبقها.</span><span class="sxs-lookup"><span data-stu-id="bdf76-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="bdf76-110">لمزيد من المعلومات، راجع [تمكين مواد غير مخزنة وفواتير المورد المعلقة](configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="bdf76-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="bdf76-111">ترحيل فاتورة مورد معلقة متعلقة بالمشروع</span><span class="sxs-lookup"><span data-stu-id="bdf76-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="bdf76-112">يمكن تسجيل فواتير المورد المعلقة في صفحة **فواتير المورد المعلقة** (**حسابات المدفوعات** > **الفواتير** > **فواتير المورد المعلقة**).</span><span class="sxs-lookup"><span data-stu-id="bdf76-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="bdf76-113">أكمل الخطوات التالية لترحيل فاتورة المورد المعلقة المتعلقة بالمشروع:</span><span class="sxs-lookup"><span data-stu-id="bdf76-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="bdf76-114">انتقل إلى **حسابات المدفوعات** > **الفواتير** وحدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="bdf76-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="bdf76-115">في الحقل **حساب الفاتورة**، حدد موردا، وفي الحقل **الرقم**، أدخل تعريف الفاتورة الخاص بالمورد.</span><span class="sxs-lookup"><span data-stu-id="bdf76-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="bdf76-116">أضف سطرا إلى فاتورة المورد، وفي الحقل **رقم العنصر**، حدد العنصر غير المخزن الذي تم شراؤه من المورد.</span><span class="sxs-lookup"><span data-stu-id="bdf76-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="bdf76-117">لا يمكن تسجيل أسطر فواتير المورد التي تستند إلى فئة شراء مقابل المشروع.</span><span class="sxs-lookup"><span data-stu-id="bdf76-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="bdf76-118">أضف الكمية التي تم شراؤها.</span><span class="sxs-lookup"><span data-stu-id="bdf76-118">Add the quantity purchased.</span></span> <span data-ttu-id="bdf76-119">يقوم النظام بتعبئة سعر الوحدة استنادا إلى تكوين أسعار العناصر غير المخزنة.</span><span class="sxs-lookup"><span data-stu-id="bdf76-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="bdf76-120">تحقق من إجمالي المبلغ والتفاصيل المطلوبة الأخرى على السطر.</span><span class="sxs-lookup"><span data-stu-id="bdf76-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="bdf76-121">في تفاصيل السطر، في علامة التبويب **مشروع**، حدد المعرف الخاص بالمشروع الذي سيتم تسجيل هذا العنصر له.</span><span class="sxs-lookup"><span data-stu-id="bdf76-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="bdf76-122">اختياريًا، قم بتحديد رقم النشاط وتحديث فئة المشروع وخاصية السطر.</span><span class="sxs-lookup"><span data-stu-id="bdf76-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="bdf76-123">قم بترحيل فاتورة المورد المعلقة.</span><span class="sxs-lookup"><span data-stu-id="bdf76-123">Post pending vendor invoice.</span></span> <span data-ttu-id="bdf76-124">عند ترحيل الفاتورة، فإن النظام يسجل:</span><span class="sxs-lookup"><span data-stu-id="bdf76-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="bdf76-125">مبلغ رصيد المورد.</span><span class="sxs-lookup"><span data-stu-id="bdf76-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="bdf76-126">مبلغ ضريبة المبيعات.</span><span class="sxs-lookup"><span data-stu-id="bdf76-126">The sales tax amount.</span></span>
    - <span data-ttu-id="bdf76-127">يتم تسجيل التكلفة مقابل المشروع في حساب تكامل الشراء.</span><span class="sxs-lookup"><span data-stu-id="bdf76-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="bdf76-128">المعاملة الفعلية للمشروع في Dataverse.</span><span class="sxs-lookup"><span data-stu-id="bdf76-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="bdf76-129">تتم معالجة هذه المعاملة أيضا باستخدام [دفتر يومية تكامل Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="bdf76-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="bdf76-130">يؤدي ترحيل دفتر اليومية هذا إلى نقل المبلغ من حساب تكامل الشراء إلى حساب تكلفة المشروع.</span><span class="sxs-lookup"><span data-stu-id="bdf76-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
