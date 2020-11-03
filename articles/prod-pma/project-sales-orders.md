---
title: أوامر مبيعات المشروع لمشاريع الوقت والمواد
description: توضح هذه الموضوع كيفيه إنشاء أوامر مبيعات تستند إلى المشروع لمشاريع الوقت والمواد.
author: Yowelle
manager: AnnBe
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: 3653a6869dab323be88f1fd0f9fd0f2cb35c456f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070629"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="1d28a-103">أوامر مبيعات المشروع لمشاريع الوقت والمواد</span><span class="sxs-lookup"><span data-stu-id="1d28a-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="1d28a-104">توضح هذه الموضوع كيفيه إنشاء أمر توريد لأحد المشروعات.</span><span class="sxs-lookup"><span data-stu-id="1d28a-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="1d28a-105">لا يمكن إنشاء أوامر المبيعات إلا لمشاريع من نوع **الوقت والمواد**.</span><span class="sxs-lookup"><span data-stu-id="1d28a-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="1d28a-106">إذا كان مشروع الوقت والمواد يحتوي علي العديد من مصادر التمويل في عقد المشروع، فيجب تمكين المعلمة **السماح بأوامر المبيعات الخاصة بالمشروعات التي تحتوي علي العديد من موارد التمويل** في صفحة **معاملات المحاسبة وإدارة المشروعات**.</span><span class="sxs-lookup"><span data-stu-id="1d28a-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="1d28a-107">يتوفر الدعم لأوامر مبيعات المشروع مع مصادر التمويل المتعددة من البدء ب10.0.2 إصدار التطبيق واعلي.</span><span class="sxs-lookup"><span data-stu-id="1d28a-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="1d28a-108">ستتم أزاله المحددة التي يتم بها تمكين الدعم لأوامر مبيعات المشروع التي لها مصادر تمويل متعددة في موجه إصدار 2020 ابريل ، والذي بعده يتم تمكين الوظيفة بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="1d28a-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="1d28a-109">يمكنك إنشاء أوامر مبيعات قائمة على المشروع بطريقتين:</span><span class="sxs-lookup"><span data-stu-id="1d28a-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="1d28a-110">انتقل إلى المشروع نفسه.</span><span class="sxs-lookup"><span data-stu-id="1d28a-110">Go to the project itself.</span></span> <span data-ttu-id="1d28a-111">في جزء الإجراء، حدد **إدارة > مهام العناصر > أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="1d28a-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="1d28a-112">ستتحول معلومات المشروع بشكل افتراضي إلى أمر المبيعات من المشروع.</span><span class="sxs-lookup"><span data-stu-id="1d28a-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="1d28a-113">إذا كان لعقد المشروع أكثر من مصدر تمويل ، ستحتاج إلى تحديد مصدر التمويل لتعيين العميل لأمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="1d28a-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="1d28a-114">إذا كان هناك مصدر تمويل واحد فقط للمشروع ، فسيتم تعيين العميل تلقائيًا.</span><span class="sxs-lookup"><span data-stu-id="1d28a-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="1d28a-115">انتقل إلى صفحة **قوائم أمر المبيعات** وقم بإنشاء أمر توريد جديد.</span><span class="sxs-lookup"><span data-stu-id="1d28a-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="1d28a-116">ستحتاج إلى تحديد المشروع لأمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="1d28a-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="1d28a-117">بعد تحديد المشروع ، سيتم تعيين العميل من مصدر التمويل أو ستحتاج إلى تحديد مصدر التمويل إذا كان عقد المشروع يحتوي على مصادر تمويل متعددة.</span><span class="sxs-lookup"><span data-stu-id="1d28a-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>

