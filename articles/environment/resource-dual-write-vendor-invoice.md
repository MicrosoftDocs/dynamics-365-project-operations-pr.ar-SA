---
title: تكامل فاتورة المورّد
description: يوفر هذا الموضوع معلومات حول تكامل فواتير الموردين في Project Operations.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 07839436c3777b0554e0721d250bff643e38c088
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955694"
---
# <a name="vendor-invoice-integration"></a><span data-ttu-id="e748a-103">تكامل فاتورة المورّد</span><span class="sxs-lookup"><span data-stu-id="e748a-103">Vendor invoice integration</span></span>

<span data-ttu-id="e748a-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="e748a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e748a-105">يمكن تسجيل عملية الشراء المرتبطة بالمشروع في Dynamics 365 Project Operations من خلال الانتقال إلى **الحسابات الدائنة** > **الفواتير** > **فواتير المورد المعلقة** واستخدام مستند فاتورة المورد المعلقة.</span><span class="sxs-lookup"><span data-stu-id="e748a-105">Project-related procurement in Dynamics 365 Project Operations can be recorded by going to **Accounts Payable** > **Invoices** > **Pending vendor invoices** and using a pending vendor invoice document.</span></span> <span data-ttu-id="e748a-106">لمزيد من المعلومات، راجع [شراء مواد غير مخزنة باستخدام فاتورة مورد معلقة](../procurement/pending-vendor-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="e748a-106">For more information, see [Purchase non-stocked materials using a pending vendor invoice](../procurement/pending-vendor-invoices.md).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e748a-107">قبل استخدام الوظيفة الموضحة في هذا الموضوع، راجع التكوينات المطلوبة وطبقها.</span><span class="sxs-lookup"><span data-stu-id="e748a-107">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="e748a-108">لمزيد من المعلومات، راجع [تمكين مواد غير مخزنة وفواتير المورد المعلقة](../procurement/configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="e748a-108">For more information, see [Enable non-stocked materials and pending vendor invoices](../procurement/configure-materials-nonstocked.md).</span></span>

<span data-ttu-id="e748a-109">في Project Operations، يتم ترحيل فواتير المورد المتعلقة بالمشروع باستخدام قواعد الترحيل الخاصة:</span><span class="sxs-lookup"><span data-stu-id="e748a-109">In Project Operations, project-related vendor invoices are posted using special posting rules:</span></span>

- <span data-ttu-id="e748a-110">لا يتم ترحيل التكلفة المرتبطة بالمشروع (بما في ذلك الضريبة غير القابلة للاسترداد) على الفور إلى حساب تكلفة المشروع في دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="e748a-110">Project-related cost (including non-recoverable tax) isn't immediately posted to the project cost account in the general ledger.</span></span> <span data-ttu-id="e748a-111">بدلا من ذلك، يتم ترحيل التكلفة إلى **حساب تكامل الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e748a-111">Instead, the cost is posted to the **Procurement integration account**.</span></span> <span data-ttu-id="e748a-112">يتم تكوين هذا الحساب في **إدارة المشاريع والمحاسبة** > **الإعداد** > **معلمات إدارة المشاريع والمحاسبة** في علامة التبويب **Project Operations في Dynamics 365 Customer engagement**</span><span class="sxs-lookup"><span data-stu-id="e748a-112">This account is configured in **Project management and accounting** > **Setup** > **Project management and accounting parameters** on the **Project Operations on Dynamics 365 Customer engagement** tab.</span></span>
- <span data-ttu-id="e748a-113">تقوم الكتابة المزدوجة بمزامنة تفاصيل فاتورة المورد مع Microsoft Dataverse باستخدام مخططات الجدول التالية:</span><span class="sxs-lookup"><span data-stu-id="e748a-113">Dual-write synchronizes vendor invoice details to Microsoft Dataverse using the following table maps:</span></span>

     - <span data-ttu-id="e748a-114">**كيان تصدير فاتورة مورد مشروع لتكامل Project Operations (msdyn_projectvendorinvoices)**: يقوم مخطط الجدول هذا بمزامنة معلومات رأس فاتورة المورد.</span><span class="sxs-lookup"><span data-stu-id="e748a-114">**Project Operations integration project vendor invoice export entity (msdyn_projectvendorinvoices)**: This table map synchronizes vendor invoice header information.</span></span> <span data-ttu-id="e748a-115">تتم مزامنة فواتير المورد التي تحتوي على سطر واحد على الأقل يتضمن معرف مشروع إلى Dataverse.</span><span class="sxs-lookup"><span data-stu-id="e748a-115">Only vendor invoices with at least one line that contains a project ID are synchronized to Dataverse.</span></span>
     - <span data-ttu-id="e748a-116">**كيان تصدير سطر فاتورة مورد مشروع لتكامل Project Operations (msdyn_projectvendorinvoicelines)**: يقوم مخطط الجدول هذا بمزامنة معلومات سطر فاتورة المورد.</span><span class="sxs-lookup"><span data-stu-id="e748a-116">**Project Operations integration project vendor invoice line export entity (msdyn_projectvendorinvoicelines)**: This table map synchronizes vendor invoice line information.</span></span> <span data-ttu-id="e748a-117">تتم مزامنة الأسطر التي تحتوي على معرف مشروع فقط إلى Dataverse.</span><span class="sxs-lookup"><span data-stu-id="e748a-117">Only lines that contain a project ID are synchronized to Dataverse.</span></span>

     > [!NOTE]
     > <span data-ttu-id="e748a-118">لا تكون تفاصيل فاتورة المورد في Dataverse قابلة للتحرير.</span><span class="sxs-lookup"><span data-stu-id="e748a-118">Vendor invoice details in Dataverse are not editable.</span></span>

<span data-ttu-id="e748a-119">يتم تسجيل دفتر الأستاذ الفرعي الضريبي ودفتر الأستاذ الفرعي للمورد والترحيلات المالية الأخرى حسب الاقتضاء في Dynamics 365 Finance عند ترحيل فاتورة المورد.</span><span class="sxs-lookup"><span data-stu-id="e748a-119">Tax subledger, vendor subledger, and other financial postings are recorded as applicable in Dynamics 365 Finance when the vendor invoice is posted.</span></span>

![تكامل فاتورة المورّد](media/DW7VendorInvoice.png)

<span data-ttu-id="e748a-121">عند كتابة السجلات إلى كيان **فاتورة المورد** في Dataverse، تبدأ عملية الموافقة التلقائية للسجلات.</span><span class="sxs-lookup"><span data-stu-id="e748a-121">When records are written to a **Vendor invoice** entity in Dataverse, an automated approval process of the records begins.</span></span> <span data-ttu-id="e748a-122">إذا لزم الأمر، يمكن مراجعة حالة عملية الموافقة التلقائية في Dataverse من خلال الانتقال إلى **الإعدادات المتقدمة** > **النظام** > **مهام نظام**.</span><span class="sxs-lookup"><span data-stu-id="e748a-122">If needed, the automated approval process status can be reviewed in Dataverse by going to **Advanced settings** > **System** > **System jobs**.</span></span> <span data-ttu-id="e748a-123">بعد اكتمال الاعتماد، يقوم النظام بإنشاء سجلات فئة معاملة المواد في كيان **القيم الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="e748a-123">After the approval is complete, the system creates material transaction class records in the **Actuals** entity.</span></span>

<span data-ttu-id="e748a-124">ثم تتم معالجة القيم الفعلية المتعلقة بالمواد باستخدام مخطط جدول الكتابة المزدوجة، **القيم الفعلية لتكامل Project Operations (msdyn_actuals)**.</span><span class="sxs-lookup"><span data-stu-id="e748a-124">Material-related actuals are then processed using the dual-write table map, **Project Operations integration actuals (msdyn_actuals)**.</span></span> <span data-ttu-id="e748a-125">للحصول على مزيد من المعلومات، راجع [تقديرات المشروع والقيم الفعلية](resource-dual-write-estimates-actuals.md).</span><span class="sxs-lookup"><span data-stu-id="e748a-125">For more information, see [Project estimates and actuals](resource-dual-write-estimates-actuals.md).</span></span>

<span data-ttu-id="e748a-126">تقوم العملية الدورية **الاستيراد من المرحلة** بإنشاء بنود دفتر يومية لتكامل Project Operations متعلقة بتقرير بفاتورة المورد.</span><span class="sxs-lookup"><span data-stu-id="e748a-126">The periodic process, **Import from staging** creates vendor invoice-related Project Operations integration journal lines.</span></span> <span data-ttu-id="e748a-127">يتخذ حساب المقاصة قيمته الافتراضية من حساب تكامل الشراء.</span><span class="sxs-lookup"><span data-stu-id="e748a-127">The offset account defaults to the procurement integration account.</span></span> <span data-ttu-id="e748a-128">عند ترحيل دفتر يومية التكامل، يتم مسح رصيد الحساب لحركة فاتورة المورد، كما يتم نقل مبلغ السطر إلى حساب تكلفة المشروع.</span><span class="sxs-lookup"><span data-stu-id="e748a-128">When the integration journal is posted, the account balance is cleared for the vendor invoice transaction and the line amount is moved to the project cost account.</span></span> <span data-ttu-id="e748a-129">يتم أيضًا إنشاء معاملات دفتر الأستاذ الفرعي للمشروع لأغراض الفوترة اللاحقة والتعرف على الإيرادات.</span><span class="sxs-lookup"><span data-stu-id="e748a-129">Project subledger transactions are also created for downstream invoicing and revenue recognition purposes.</span></span>
