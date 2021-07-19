---
title: أداء اقتراحات فواتير المشروع
description: يوفر هذا الموضوع معلومات حول تحسينات الأداء لاقتراحات فواتير المشروع.
author: Yowelle
ms.date: 06/16/2021
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ''
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 20121-03-05
ms.dyn365.ops.version: 10.0.18
ms.openlocfilehash: 5a14acf51d277b16896d64c4b12ee00bfb326910
ms.sourcegitcommit: 3a4b181be08ef0428104d72b54a3e61ac2782f14
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/17/2021
ms.locfileid: "6269774"
---
# <a name="project-invoice-proposal-performance"></a><span data-ttu-id="e584c-103">أداء اقتراحات فواتير المشروع</span><span class="sxs-lookup"><span data-stu-id="e584c-103">Project invoice proposal performance</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e584c-104">عند إنشاء اقتراح فاتورة جديد، قد تواجه مشاكل في الأداء مع زيادة عدد المشاريع والمشاريع الفرعية.</span><span class="sxs-lookup"><span data-stu-id="e584c-104">When you create a new invoice proposal you might encounter performance issues as the number of projects and subprojects increase.</span></span> <span data-ttu-id="e584c-105">لتحسين الأداء، تتوفر ميزة تقلل من الوقت اللازم لإنشاء اقتراح فاتورة جديد لحركات المشروع المرحلة.</span><span class="sxs-lookup"><span data-stu-id="e584c-105">To improve performance, a feature is available that reduces the time needed to create a new invoice proposal for posted project transactions.</span></span>

## <a name="enable-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="e584c-106">تمكين تحسين أداء اقتراحات فواتير المشروع</span><span class="sxs-lookup"><span data-stu-id="e584c-106">Enable project invoice proposal performance enhancement</span></span>
<span data-ttu-id="e584c-107">لتمكين ميزة تحسين أداء اقتراحات فواتير المشروع، أكمل الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="e584c-107">To enable the project invoice proposal performance enhancement feature, complete the following steps.</span></span>

1.  <span data-ttu-id="e584c-108">انتقل إلى **إدارة الميزات** > **الكل**.</span><span class="sxs-lookup"><span data-stu-id="e584c-108">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="e584c-109">في قائمة الميزات، حدد موقع **تحسين أداء اقتراحات فواتير المشروع**.</span><span class="sxs-lookup"><span data-stu-id="e584c-109">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="e584c-110">حدد **تمكين الآن**.</span><span class="sxs-lookup"><span data-stu-id="e584c-110">Select **Enable now**.</span></span>
3.  <span data-ttu-id="e584c-111">قم بتحديث المستعرض، ثم أنشئ مقترحًا جديدًا للفاتورة.</span><span class="sxs-lookup"><span data-stu-id="e584c-111">Refresh your browser, and then create a new invoice proposal.</span></span>

## <a name="turn-off-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="e584c-112">إيقاف تشغيل تحسين أداء اقتراحات فواتير المشروع</span><span class="sxs-lookup"><span data-stu-id="e584c-112">Turn off project invoice proposal performance enhancement</span></span>
<span data-ttu-id="e584c-113">أكمل الخطوات التالية لإيقاف تشغيل تحسين أداء اقتراحات فواتير المشروع.</span><span class="sxs-lookup"><span data-stu-id="e584c-113">Complete the following steps to turn off the project invoice proposal performance enhancement.</span></span>

1.  <span data-ttu-id="e584c-114">انتقل إلى **إدارة الميزات** > **الكل**.</span><span class="sxs-lookup"><span data-stu-id="e584c-114">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="e584c-115">في قائمة الميزات، حدد موقع **تحسين أداء اقتراحات فواتير المشروع**.</span><span class="sxs-lookup"><span data-stu-id="e584c-115">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="e584c-116">حدد **تعطيل**.</span><span class="sxs-lookup"><span data-stu-id="e584c-116">Select **Disable**.</span></span>
3.  <span data-ttu-id="e584c-117">قم بتحديث المستعرض.</span><span class="sxs-lookup"><span data-stu-id="e584c-117">Refresh your browser.</span></span>

> [!NOTE]
> <span data-ttu-id="e584c-118">لا يمكن تطبيق أداء مقترح الفاتورة عند تمكين قواعد الفوترة.</span><span class="sxs-lookup"><span data-stu-id="e584c-118">Invoice proposal performance can't be applied when billing rules are enabled.</span></span>
> 
> <span data-ttu-id="e584c-119">أثناء عملية الدُفعات لإنشاء مقترحات الفواتير، سيقوم عدد المهام الفرعية بتقسيم المهام إلى أقصى عدد بناءً على عدد العقود ذات الحركات القابلة للفوترة، بغض النظر عما أدخلته.</span><span class="sxs-lookup"><span data-stu-id="e584c-119">During the batch process to create invoice proposals, the number of subtasks will split the tasks to a maximum number based on the number of contracts with invoiceable transactions, regardless of what you have entered.</span></span> <span data-ttu-id="e584c-120">على سبيل المثال ، إذا أدخلت **3** لعدد المهام الفرعية لإنشاء مقترح الفاتورة دفعة واحدة، وكان هناك عقدين فقط مع حركات قابلة للفوترة، فسيتم إنشاء مهمتين فرعيتين فقط.</span><span class="sxs-lookup"><span data-stu-id="e584c-120">For example, if you enter **3** for the number of subtasks for invoice proposal creation in batch, and there are only two contracts with invoiceable transactions, only two subtasks are created.</span></span>
