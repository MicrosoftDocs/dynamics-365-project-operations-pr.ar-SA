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
ms.openlocfilehash: b9b45e3ae0cd9273af4d2a5cd9cce30502c0aa78
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127142"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a>لماذا لا يمكنني حذف سجلات من كيان القيم الفعلية؟

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

لا يتيح لك Project Service Automation (PSA) حذف القيم الفعلية لأنها تعمل كمصدر لحقيقة الحركات التي لها تبعات مالية على الأنظمة من الخادم، مثل دفتر الأستاذ العام. وإذا كان من الممكن حذف القيم الفعلية، فيمكن التشكيك في نزاهة حركات التقارير المالية. لإنشاء مسار تدقيق، يجب على العملاء استخدام دفاتر اليومية لإنشاء حركات تعويض.

