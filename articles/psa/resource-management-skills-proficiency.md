---
title: نماذج المهارات والكفاءة
description: يقدم هذا الموضوع معلومات حول كيفية استخدام نماذج المهارات والكفاءة.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: cd243544df062e5801bbfa0a3bd75c4d9a116a6f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070864"
---
# <a name="skills-and-proficiency-models"></a>نماذج المهارات والكفاءة

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

المهارات هي خصائص الموارد التي تمت مشاركتها بين Dynamics 365 Project Service Automation وDynamics 365 Field Service، إن وُجد. 

للاحتفاظ بمستودع المهارات في Project Service Automation، انتقل إلى **الموارد**\>**مهارات الموارد**. 

> ![مهارات الموارد](media/Resource-Management-image84.png)

## <a name="use-proficiency-models-to-rate-resources"></a>استخدام نماذج الكفاءة لتصنيف الموارد

يتم تصنيف مهارات الموارد بواسطة نماذج كفاءة. توجد التصنيفات الفردية في نموذج الكفاءة. 

1. لإنشاء نموذج كفاءة، انتقل إلى **الموارد**\>**نماذج الكفاءة** ، ثم حدد **جديد**.
2. في نموذج التصنيف الجديد، حدد الحد الأدنى لقيمة التصنيف والقيمة القصوى للتصنيف والكيان الذي يتم تصنيفه.
3. في الشبكة الفرعية **قيم التصنيف** ، يمكنك تحديد قيم التصنيف المختلفة، من الحد الأدنى إلى الحد الأقصى.

> ![تحديد التصنيفات الدنيا والقصوى](media/Resource-Management-image85.png)

يتم عرض قيم التصنيف هذه في عوامل تصفية **متطلبات الموارد** ، و **لوحة الجدولة** ، و **مساعد الجدولة**.
