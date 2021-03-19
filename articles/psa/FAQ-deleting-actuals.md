---
title: لماذا لا يمكنني حذف سجلات من كيان القيم الفعلية؟
description: يقدم هذا الموضوع معلومات حول سبب عدم تمكنك من حذف السجلات من كيان القيم الفعلية.
author: JPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
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
ms.openlocfilehash: e3122c5d9495b3ff9a683f477e719ce0c228a84d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286052"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a>لماذا لا يمكنني حذف سجلات من كيان القيم الفعلية؟

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

لا يتيح لك Project Service Automation (PSA) حذف القيم الفعلية لأنها تعمل كمصدر لحقيقة الحركات التي لها تبعات مالية على الأنظمة من الخادم، مثل دفتر الأستاذ العام. وإذا كان من الممكن حذف القيم الفعلية، فيمكن التشكيك في نزاهة حركات التقارير المالية. لإنشاء مسار تدقيق، يجب على العملاء استخدام دفاتر اليومية لإنشاء حركات تعويض.



[!INCLUDE[footer-include](../includes/footer-banner.md)]