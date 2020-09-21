---
title: لماذا لا يمكنني حذف سجلات من كيان القيم الفعلية؟
description: يقدم هذا الموضوع معلومات حول سبب عدم تمكنك من حذف السجلات من كيان القيم الفعلية.
author: JPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.prod: Project Service
ms.technology: Applies to all versions of Project Service
ms.assetid: ff504c34-7337-474f-89e8-d8afdd1e0a98
ms.author: Jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5817940933c161dccac0fe549fabacbe57e7077a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748608"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a>لماذا لا يمكنني حذف سجلات من كيان القيم الفعلية؟

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

لا يتيح لك Project Service Automation (PSA) حذف القيم الفعلية لأنها تعمل كمصدر لحقيقة الحركات التي لها تبعات مالية على الأنظمة من الخادم، مثل دفتر الأستاذ العام. وإذا كان من الممكن حذف القيم الفعلية، فيمكن التشكيك في نزاهة حركات التقارير المالية. لإنشاء مسار تدقيق، يجب على العملاء استخدام دفاتر اليومية لإنشاء حركات تعويض.

