---
title: تكامل فاتورة المشروع
description: يوفر هذا موضوع معلومات حول تكامل الكتابة المزدوجة في Project Operations لفوترة العملاء.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 102a7cdba467a2071119c5b32d2e75e48170c783
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955691"
---
# <a name="project-invoice-integration"></a><span data-ttu-id="f7964-103">تكامل فاتورة المشروع</span><span class="sxs-lookup"><span data-stu-id="f7964-103">Project invoice integration</span></span>

<span data-ttu-id="f7964-104">يوفر هذا موضوع معلومات حول تكامل الكتابة المزدوجة في Project Operations لفوترة العملاء.</span><span class="sxs-lookup"><span data-stu-id="f7964-104">This topic provides information about Project Operations dual-write integration for customer invoicing.</span></span>

<span data-ttu-id="f7964-105">في Project Operations، يدير مدير المشروع تراكم الفاتورة وينشئ فاتورة أولية للعميل في Microsoft Dataverse.</span><span class="sxs-lookup"><span data-stu-id="f7964-105">In Project Operations, the Project manager manages the project billing backlog and creates a proforma invoice for the customer in Microsoft Dataverse.</span></span> <span data-ttu-id="f7964-106">وبناء على هذه الفاتورة الأولية، يقوم موظف حسابات المقبوضات أو محاسب المشروع بإنشاء فاتورة مواجهة للعميل.</span><span class="sxs-lookup"><span data-stu-id="f7964-106">Based on this proforma invoice, the Accounts receivable clerk or Project accountant creates a customer-facing invoice.</span></span> <span data-ttu-id="f7964-107">يضمن تكامل الكتابة التلقائية مزامنة تفاصيل الفاتورة الأولية مع تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="f7964-107">Dual-write integration ensures that the proforma invoice details are synchronized to Finance and Operations apps.</span></span> <span data-ttu-id="f7964-108">وبعد ترحيل الفاتورة المواجهة للعميل، يقوم النظام بتحديث القيم الفعلية للمشروع ذات الصلة في Dataverse بتفاصيل المحاسبة.</span><span class="sxs-lookup"><span data-stu-id="f7964-108">After the customer-facing invoice is posted, the system updates the relevant project actuals in Dataverse with the accounting detail.</span></span> <span data-ttu-id="f7964-109">يوفر الرسم التالي نظرة عامة تصورية رفيعة المستوى لهذا التكامل.</span><span class="sxs-lookup"><span data-stu-id="f7964-109">The following graphic provides a high-level conceptual overview of this integration.</span></span>

   ![تكامل فاتورة المشروع](./media/DW5Invoicing.png)

<span data-ttu-id="f7964-111">بعد أن يؤكد مدير المشروع الفاتورة الأولية في Dataverse، يتم مزامنة معلومات رأس الفاتورة الأولية مع تطبيقات Finance and Operations باستخدام مخطط جدول الكتابة المزدوجة **اقتراح فاتورة المشروع V2 (الفواتير)**.</span><span class="sxs-lookup"><span data-stu-id="f7964-111">After the Project manager confirms the proforma invoice in Dataverse, the proforma invoice header information synchronizes to Finance and Operations apps using the dual-write table map, **Project invoice proposal V2 (invoices)**.</span></span> <span data-ttu-id="f7964-112">وهذا تكامل من جانب واحد من Dataverse إلى تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="f7964-112">This is a one-way integration from Dataverse to Finance and Operations apps.</span></span> <span data-ttu-id="f7964-113">لا يتم دعم إنشاء مقترحات فاتورة المشروع أو حذفها مباشرة في تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="f7964-113">Creating or deleting Project invoice proposals directly in Finance and Operations apps isn't supported.</span></span>

<span data-ttu-id="f7964-114">كما يؤدي تأكيد الفاتورة في Dataverse أيضا إلى إطلاق منطق الأعمال لإنشاء سجلات متعلقة بالفوترة في كيان **القيم الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="f7964-114">Invoice confirmation in Dataverse also triggers the business logic to create billing-related records in the **Actuals** entity.</span></span> <span data-ttu-id="f7964-115">تتم مزامنة هذه السجلات مع Finance and Operations باستخدام مخطط جدول الكتابة المزدوجة **القيم الفعلية لتكامل Project Operations (msdyn\_actuals)**.</span><span class="sxs-lookup"><span data-stu-id="f7964-115">These records are synchronized to Finance and Operations using the dual-write table map, **Project Operations integration actuals (msdyn\_actuals).**</span></span> <span data-ttu-id="f7964-116">للحصول على مزيد من المعلومات، راجع [تقديرات المشروع والقيم الفعلية](resource-dual-write-estimates-actuals.md).</span><span class="sxs-lookup"><span data-stu-id="f7964-116">For more information, see [Project estimates and actuals](resource-dual-write-estimates-actuals.md).</span></span> 

<span data-ttu-id="f7964-117">يتم إنشاء بنود عرض فاتورة المشروع بواسطة العملية الدورية، **مراحل استيراد النموذج**.</span><span class="sxs-lookup"><span data-stu-id="f7964-117">Project invoice proposal lines are created by the periodic process, **Import form staging**.</span></span> <span data-ttu-id="f7964-118">تعتمد هذه العملية على تفاصيل القيم الفعلية للمبيعات التي تمت فوترتها في جدول **مراحل القيمة الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="f7964-118">This process is based on the billed sales actuals details in the **Actuals staging** table.</span></span> <span data-ttu-id="f7964-119">لمزيد من المعلومات، راجع [إدارة مقترحات فواتير المشروع](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals).</span><span class="sxs-lookup"><span data-stu-id="f7964-119">For more information, see [Manage project invoice proposals](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals).</span></span> 
