---
title: تحديد المهارات والكفاءات
description: يقدم هذا الموضوع معلومات حول كيفية إعداد نماذج الكفاءة لتصنيف الموارد‬.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
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
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d1ef50a3aa297ef439b54d37de629414ca66c820
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279662"
---
# <a name="define-skills-and-proficiencies"></a><span data-ttu-id="0e35d-103">تحديد المهارات والكفاءات</span><span class="sxs-lookup"><span data-stu-id="0e35d-103">Define skills and proficiencies</span></span>

<span data-ttu-id="0e35d-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="0e35d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0e35d-105">المهارات هي خصائص الموارد التي تمت مشاركتها بين Dynamics 365 Project Operations وDynamics 365 Field Service، إن وُجد.</span><span class="sxs-lookup"><span data-stu-id="0e35d-105">Skills are resource characteristics that are shared between Dynamics 365 Project Operations and if present, Dynamics 365 Field Service.</span></span> 

- <span data-ttu-id="0e35d-106">للاحتفاظ بمستودع المهارات في عمليات المشروع، انتقل إلى **موارد** \> **مهارات الموارد**.</span><span class="sxs-lookup"><span data-stu-id="0e35d-106">To maintain the repository of skills in Project Operations, go to **Resources** \> **Resource Skills**.</span></span> 

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="0e35d-107">استخدام نماذج الكفاءة لتصنيف الموارد</span><span class="sxs-lookup"><span data-stu-id="0e35d-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="0e35d-108">يتم تصنيف مهارات الموارد بواسطة نماذج كفاءة.</span><span class="sxs-lookup"><span data-stu-id="0e35d-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="0e35d-109">توجد التصنيفات الفردية في نموذج الكفاءة.</span><span class="sxs-lookup"><span data-stu-id="0e35d-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="0e35d-110">لإنشاء نموذج كفاءة، انتقل إلى **الموارد**\>**نماذج الكفاءة**، ثم حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="0e35d-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="0e35d-111">في نموذج التصنيف الجديد، حدد الحد الأدنى لقيمة التصنيف والقيمة القصوى للتصنيف والكيان الذي يتم تصنيفه.</span><span class="sxs-lookup"><span data-stu-id="0e35d-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="0e35d-112">في الشبكة الفرعية **قيم التصنيف**، يمكنك تحديد قيم التصنيف المختلفة، من الحد الأدنى إلى الحد الأقصى.</span><span class="sxs-lookup"><span data-stu-id="0e35d-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>


<span data-ttu-id="0e35d-113">يتم عرض قيم التصنيف هذه في عوامل تصفية **متطلبات الموارد**، و **لوحة الجدولة**، و **مساعد الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="0e35d-113">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]