---
title: نماذج المهارات والكفاءة
description: يقدم هذا الموضوع معلومات حول كيفية استخدام نماذج المهارات والكفاءة.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/13/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 976650cc71b0cdb75d5ce2d7532cd78bd91d3670
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6008655"
---
# <a name="skills-and-proficiency-models"></a><span data-ttu-id="f7c1c-103">نماذج المهارات والكفاءة</span><span class="sxs-lookup"><span data-stu-id="f7c1c-103">Skills and proficiency models</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="f7c1c-104">المهارات هي خصائص الموارد التي تمت مشاركتها بين Dynamics 365 Project Service Automation وDynamics 365 Field Service، إن وُجد.</span><span class="sxs-lookup"><span data-stu-id="f7c1c-104">Skills are resource characteristics that are shared between Dynamics 365 Project Service Automation and if present, Dynamics 365 Field Service.</span></span> 

<span data-ttu-id="f7c1c-105">للاحتفاظ بمستودع المهارات في Project Service Automation، انتقل إلى **الموارد**\>**مهارات الموارد**.</span><span class="sxs-lookup"><span data-stu-id="f7c1c-105">To maintain the repository of skills in Project Service Automation, go to **Resources** \> **Resource Skills**.</span></span> 

> ![مهارات الموارد](media/Resource-Management-image84.png)

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="f7c1c-107">استخدام نماذج الكفاءة لتصنيف الموارد</span><span class="sxs-lookup"><span data-stu-id="f7c1c-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="f7c1c-108">يتم تصنيف مهارات الموارد بواسطة نماذج كفاءة.</span><span class="sxs-lookup"><span data-stu-id="f7c1c-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="f7c1c-109">توجد التصنيفات الفردية في نموذج الكفاءة.</span><span class="sxs-lookup"><span data-stu-id="f7c1c-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="f7c1c-110">لإنشاء نموذج كفاءة، انتقل إلى **الموارد**\>**نماذج الكفاءة**، ثم حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="f7c1c-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="f7c1c-111">في نموذج التصنيف الجديد، حدد الحد الأدنى لقيمة التصنيف والقيمة القصوى للتصنيف والكيان الذي يتم تصنيفه.</span><span class="sxs-lookup"><span data-stu-id="f7c1c-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="f7c1c-112">في الشبكة الفرعية **قيم التصنيف**، يمكنك تحديد قيم التصنيف المختلفة، من الحد الأدنى إلى الحد الأقصى.</span><span class="sxs-lookup"><span data-stu-id="f7c1c-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>

> ![تحديد التصنيفات الدنيا والقصوى](media/Resource-Management-image85.png)

<span data-ttu-id="f7c1c-114">يتم عرض قيم التصنيف هذه في عوامل تصفية **متطلبات الموارد**، و **لوحة الجدولة**، و **مساعد الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="f7c1c-114">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]