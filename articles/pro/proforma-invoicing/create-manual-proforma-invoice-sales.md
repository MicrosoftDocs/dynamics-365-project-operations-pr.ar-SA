---
title: إنشاء فاتورة أولية يدوية
description: يوفر هذا الموضوع معلومات حول إنشاء فاتورة أولية يدوية في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5e93206737507bf6698a9746815c790d3dfc904
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/20/2020
ms.locfileid: "4070873"
---
# <a name="creating-a-manual-proforma-invoice"></a><span data-ttu-id="c59b0-103">إنشاء فاتورة أولية يدوية</span><span class="sxs-lookup"><span data-stu-id="c59b0-103">Creating a manual proforma invoice</span></span>

<span data-ttu-id="c59b0-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="c59b0-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c59b0-105">في Dynamics 365 Project Operations، يمكنك إنشاء فواتير أولية يدويًا كما تقتضي الحاجة.</span><span class="sxs-lookup"><span data-stu-id="c59b0-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="c59b0-106">يمكنك إنشاء فاتورة أولية من صفحة قائمة **عقود المشروع** أو من صفحة تفاصيل **عقد المشروع**.</span><span class="sxs-lookup"><span data-stu-id="c59b0-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="c59b0-107">صفحة قائمة عقود المشروع</span><span class="sxs-lookup"><span data-stu-id="c59b0-107">Project Contracts list page</span></span>

<span data-ttu-id="c59b0-108">من صفحة قائمة **عقود المشروع** ، حدد عقد مشروع واحدًا أو أكثر، وأنشئ فواتير لجميع السجلات المحددة.</span><span class="sxs-lookup"><span data-stu-id="c59b0-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="c59b0-109">يتحقق النظام لمعرفة ما إذا كانت عقود المشروع المحددة تحتوي على تراكم **جاهز للفوترة** مؤرخ قبل تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="c59b0-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="c59b0-110">بالنسبة إلى هذه العقود، ينشئ النظام مسودات فواتير أولية.</span><span class="sxs-lookup"><span data-stu-id="c59b0-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="c59b0-111">إذا تضمن عقد المشروع عدة عملاء، فقد تكون هناك فاتورة واحدة لكل عميل، وفواتير متعددة لكل عقد مشروع.</span><span class="sxs-lookup"><span data-stu-id="c59b0-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="c59b0-112">تتوفر كافة فواتير المشروع التي تم إنشاؤها في صفحة **الفاتورة** في قسم **الفوترة** في منطقة **المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="c59b0-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="c59b0-113">صفحة تفاصيل عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="c59b0-113">Project Contract details page</span></span>

<span data-ttu-id="c59b0-114">يمكن أيضًا إنشاء فاتورة أولية من صفحة تفاصيل **عقد المشروع** ، التي تقوم بإنشاء الفاتورة لعقد المشروع المحدد هذا.</span><span class="sxs-lookup"><span data-stu-id="c59b0-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="c59b0-115">يتحقق النظام من وجود تراكم **جاهز للفوترة** في عقد المشروع مؤرخ قبل تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="c59b0-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="c59b0-116">من هذه العقود، ينشئ النظام مسودة فواتير أولية تستند إلى عدد العملاء في كل شرط تعاقد.</span><span class="sxs-lookup"><span data-stu-id="c59b0-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="c59b0-117">عند إنشاء فاتورة أولية واحدة، تفتح صفحة **الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="c59b0-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="c59b0-118">إذا كانت هناك فواتير متعددة تم إنشاؤها لعقد المشروع هذا، تفتح صفحة قائمة **الفواتير** لعرض كافة الفواتير التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="c59b0-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
