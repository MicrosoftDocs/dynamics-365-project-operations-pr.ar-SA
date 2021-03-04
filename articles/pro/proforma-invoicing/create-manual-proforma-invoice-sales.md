---
title: إنشاء فاتورة أولية يدوية - خفيف
description: يوفر هذا الموضوع معلومات حول إنشاء فاتورة أولية يدوية في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5a924de6efc377e28a20e038e7deac04616b95aa
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764487"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="e9536-103">إنشاء فاتورة أولية يدوية - خفيف</span><span class="sxs-lookup"><span data-stu-id="e9536-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="e9536-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="e9536-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e9536-105">في Dynamics 365 Project Operations ، يمكن إنشاء فواتير أولية يدويًا حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="e9536-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="e9536-106">يمكنك إنشاء فاتورة أولية من صفحة قائمة **عقود المشروع** أو من صفحة تفاصيل **عقد المشروع**.</span><span class="sxs-lookup"><span data-stu-id="e9536-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="e9536-107">صفحة قائمة عقود المشروع</span><span class="sxs-lookup"><span data-stu-id="e9536-107">Project Contracts list page</span></span>

<span data-ttu-id="e9536-108">من صفحة قائمة **عقود المشروع**، حدد عقد مشروع واحدًا أو أكثر، وأنشئ فواتير لجميع السجلات المحددة.</span><span class="sxs-lookup"><span data-stu-id="e9536-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="e9536-109">يتحقق النظام لمعرفة ما إذا كانت عقود المشروع المحددة تحتوي على تراكم **جاهز للفوترة** مؤرخ قبل تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="e9536-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="e9536-110">بالنسبة إلى هذه العقود، ينشئ النظام مسودات فواتير أولية.</span><span class="sxs-lookup"><span data-stu-id="e9536-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="e9536-111">إذا تضمن عقد المشروع عدة عملاء، فقد تكون هناك فاتورة واحدة لكل عميل، وفواتير متعددة لكل عقد مشروع.</span><span class="sxs-lookup"><span data-stu-id="e9536-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="e9536-112">تتوفر كافة فواتير المشروع التي تم إنشاؤها في صفحة **الفاتورة** في قسم **الفوترة** في منطقة **المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="e9536-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="e9536-113">صفحة تفاصيل عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="e9536-113">Project Contract details page</span></span>

<span data-ttu-id="e9536-114">يمكن إنشاء فاتورة أولية أيضًا من صفحة تفاصيل **عقد المشروع**.</span><span class="sxs-lookup"><span data-stu-id="e9536-114">A proforma invoice can also be created from the **Project Contract** details page.</span></span> <span data-ttu-id="e9536-115">يتحقق النظام من أن عقد المشروع يحتوي على تراكم **جاهز للفوترة** مؤرخ قبل تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="e9536-115">The system verifies the project contract has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="e9536-116">من هذه العقود، ينشئ النظام مسودة فواتير أولية تستند إلى عدد العملاء في كل شرط تعاقد.</span><span class="sxs-lookup"><span data-stu-id="e9536-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="e9536-117">عند إنشاء فاتورة أولية واحدة، تفتح صفحة **الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="e9536-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="e9536-118">إذا تم إنشاء فواتير متعددة لعقد هذا المشروع، يتم فتح صفحة قائمة **الفواتير** لعرض كافة الفواتير التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="e9536-118">If multiple invoices are created for that project contract, the **Invoices** list page opens to show all of the created invoices.</span></span>
