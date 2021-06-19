---
title: تحديد المهارات والكفاءات
description: يقدم هذا الموضوع معلومات حول كيفية إعداد نماذج الكفاءة لتصنيف الموارد‬.
author: ruhercul
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 982f64677b74f2195eacc287fc07b80c34f7acc0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6015315"
---
# <a name="define-skills-and-proficiencies"></a><span data-ttu-id="83edf-103">تحديد المهارات والكفاءات</span><span class="sxs-lookup"><span data-stu-id="83edf-103">Define skills and proficiencies</span></span>

<span data-ttu-id="83edf-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="83edf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="83edf-105">المهارات هي خصائص الموارد التي تمت مشاركتها بين Dynamics 365 Project Operations وDynamics 365 Field Service، إن وُجد.</span><span class="sxs-lookup"><span data-stu-id="83edf-105">Skills are resource characteristics that are shared between Dynamics 365 Project Operations and if present, Dynamics 365 Field Service.</span></span> 

- <span data-ttu-id="83edf-106">للاحتفاظ بمستودع المهارات في عمليات المشروع، انتقل إلى **موارد** \> **مهارات الموارد**.</span><span class="sxs-lookup"><span data-stu-id="83edf-106">To maintain the repository of skills in Project Operations, go to **Resources** \> **Resource Skills**.</span></span> 

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="83edf-107">استخدام نماذج الكفاءة لتصنيف الموارد</span><span class="sxs-lookup"><span data-stu-id="83edf-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="83edf-108">يتم تصنيف مهارات الموارد بواسطة نماذج كفاءة.</span><span class="sxs-lookup"><span data-stu-id="83edf-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="83edf-109">توجد التصنيفات الفردية في نموذج الكفاءة.</span><span class="sxs-lookup"><span data-stu-id="83edf-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="83edf-110">لإنشاء نموذج كفاءة، انتقل إلى **الموارد**\>**نماذج الكفاءة**، ثم حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="83edf-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="83edf-111">في نموذج التصنيف الجديد، حدد الحد الأدنى لقيمة التصنيف والقيمة القصوى للتصنيف والكيان الذي يتم تصنيفه.</span><span class="sxs-lookup"><span data-stu-id="83edf-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="83edf-112">في الشبكة الفرعية **قيم التصنيف**، يمكنك تحديد قيم التصنيف المختلفة، من الحد الأدنى إلى الحد الأقصى.</span><span class="sxs-lookup"><span data-stu-id="83edf-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>


<span data-ttu-id="83edf-113">يتم عرض قيم التصنيف هذه في عوامل تصفية **متطلبات الموارد**، و **لوحة الجدولة**، و **مساعد الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="83edf-113">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]