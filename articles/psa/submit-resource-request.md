---
title: إرسال طلب مورد
description: يوفر هذا الموضوع معلومات حول إرسال طلب لمورد مشروع.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: bcea3d640d7e9ee2b071c55bff9ade3268edb319
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070737"
---
# <a name="submitting-a-resource-request"></a>إرسال طلب مورد

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

يمكنك إرسال متطلب مورد تم إنشاؤه كطلب مورد. ثم يتم إرسال الطلب إلى مدير مورد لاستيفائه.

1. في Project Service Automation (PSA)، في صفحة **المشاريع** ، انقر فوق علامة التبويب **فريق** لعرض قائمة بالموارد القابلة للحجز. 
2. حدد المورد العام الذي يحتوي على متطلب مورد من القائمة ثم انقر فوق **إرسال طلب**.

![إرسال طلب مورد](media/RM-how-to-18.png)

ستتغير حالة طلب عضو الفريق العام إلى **تم الإرسال**.

بعد استيفاء الطلب بواسطة مدير الموارد، سيتم استبدال المورد العام بمورد محدد إذا كان مدير الموارد يفي بالطلب مع حجز مورد مسمي. وبخلاف ذلك، سيظل المورد العام في الفريق وستتغير حالة الطلب إلى **في حاجة إلى المراجعة** ، إذا اقترح مدير المورد موردًا مسمى.
