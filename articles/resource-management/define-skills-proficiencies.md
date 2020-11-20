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
ms.openlocfilehash: 8738a4743554704ef76807c81fdefcd74e668e1b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124757"
---
# <a name="define-skills-and-proficiencies"></a><span data-ttu-id="0bde5-103">تحديد المهارات والكفاءات</span><span class="sxs-lookup"><span data-stu-id="0bde5-103">Define skills and proficiencies</span></span>

<span data-ttu-id="0bde5-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="0bde5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0bde5-105">المهارات هي خصائص الموارد التي تمت مشاركتها بين Dynamics 365 Project Operations و Dynamics 365 Field Service، إن وُجدت.</span><span class="sxs-lookup"><span data-stu-id="0bde5-105">Skills are resource characteristics that are shared between Dynamics 365 Project Operations and if present, Dynamics 365 Field Service.</span></span> 

- <span data-ttu-id="0bde5-106">للاحتفاظ بمستودع المهارات في عمليات المشروع، انتقل إلى **موارد** \> **مهارات الموارد**.</span><span class="sxs-lookup"><span data-stu-id="0bde5-106">To maintain the repository of skills in Project Operations, go to **Resources** \> **Resource Skills**.</span></span> 

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="0bde5-107">استخدام نماذج الكفاءة لتصنيف الموارد</span><span class="sxs-lookup"><span data-stu-id="0bde5-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="0bde5-108">يتم تصنيف مهارات الموارد بواسطة نماذج كفاءة.</span><span class="sxs-lookup"><span data-stu-id="0bde5-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="0bde5-109">توجد التصنيفات الفردية في نموذج الكفاءة.</span><span class="sxs-lookup"><span data-stu-id="0bde5-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="0bde5-110">لإنشاء نموذج كفاءة، انتقل إلى **الموارد**\>**نماذج الكفاءة**، ثم حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="0bde5-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="0bde5-111">في نموذج التصنيف الجديد، حدد الحد الأدنى لقيمة التصنيف والقيمة القصوى للتصنيف والكيان الذي يتم تصنيفه.</span><span class="sxs-lookup"><span data-stu-id="0bde5-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="0bde5-112">في الشبكة الفرعية **قيم التصنيف**، يمكنك تحديد قيم التصنيف المختلفة، من الحد الأدنى إلى الحد الأقصى.</span><span class="sxs-lookup"><span data-stu-id="0bde5-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>


<span data-ttu-id="0bde5-113">يتم عرض قيم التصنيف هذه في عوامل تصفية **متطلبات الموارد**، و **لوحة الجدولة**، و **مساعد الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="0bde5-113">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>
