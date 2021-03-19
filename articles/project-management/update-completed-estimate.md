---
title: تحديث التقدير عند الاكتمال
description: يوفر هذا الموضوع معلومات حول تحديث عرض الجهد في مشروع.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 0e63bdb815a6f758c57d055c8c03d92e04700445
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286412"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="aceed-103">تحديث التقدير عند الاكتمال</span><span class="sxs-lookup"><span data-stu-id="aceed-103">Update estimate at completion</span></span>

<span data-ttu-id="aceed-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="aceed-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="aceed-105">من الشائع أن يقوم مدير المشروع بمراجعة التقديرات الأصلية للمهمة.</span><span class="sxs-lookup"><span data-stu-id="aceed-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="aceed-106">عمليات إعادة تخطيط المشروع هي تصور مدير المشروع للتقديرات ، بالنظر إلى الوضع الحالي للمشروع.</span><span class="sxs-lookup"><span data-stu-id="aceed-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="aceed-107">ومع ذلك ، لا نوصي بأن يقوم مديرو المشاريع بتغيير أرقام خط الأساس ، لأن خط الأساس للمشروع يمثل مصدر الحقيقة المحدد لجدول المشروع وتقدير التكلفة ، وقد وافق جميع أصحاب المصلحة في المشروع على ذلك.</span><span class="sxs-lookup"><span data-stu-id="aceed-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="aceed-108">هناك طريقتان يمكن لمدير المشروع من خلالهما إعادة تخطيط الجهود في المهام:</span><span class="sxs-lookup"><span data-stu-id="aceed-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="aceed-109">تجاوز التقدير للإكمال (ETC) الافتراضي مع تقدير جديد للجهد الفعلي المتبقي في المهمة.</span><span class="sxs-lookup"><span data-stu-id="aceed-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="aceed-110">تجاوز النسبة المئوية للتقدم الافتراضي مع تقدير جديد للتقدم الحقيقي في المهمة.</span><span class="sxs-lookup"><span data-stu-id="aceed-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="aceed-111">يؤدي كل من هاتين الطريقتين إلى إعادة حساب التقدير للإكمال للمهمة والتقدير عند الاكتمال (EAC) ونسبة التقدم وتباين الجهد المتوقع في المهمة.</span><span class="sxs-lookup"><span data-stu-id="aceed-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="aceed-112">يتم أيضًا إعادة حساب التقدير عند الاكتمال والتقدير للإكمال والنسبة المئوية للتقدم في مهام الملخص، وتنتج إسقاطًا جديدًا لتباين الجهد.</span><span class="sxs-lookup"><span data-stu-id="aceed-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]