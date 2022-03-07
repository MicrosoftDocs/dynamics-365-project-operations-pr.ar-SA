---
title: نظرة عامة على أوضاع إدارة الموارد
description: يوفر هذا الموضوع معلومات حول وظيفة إدارة الموارد في Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 5c0f98a6f08129ebef9b6d3fed1cc85969aa347c815a643d3c8dd639b42c0e8c
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "7008210"
---
# <a name="resource-management-modes-overview"></a>نظرة عامة على أوضاع إدارة الموارد

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_


يدعم Dynamics 365 Project Operations وضعين حتى تتمكن من تنفيذ سير مهام الحجز الإجمالي. يتم تعريف وضع الإدارة كمعلمة مشروع ويمكن تعديلها إذا احتاج العمل الخاص بك إلى التغيير.    

## <a name="central-mode"></a>الوضع المركزي
بالنسبة للمؤسسات التي تقوم بالتخصيص المركزي للموارد بشأن المشاريع، يوفر الوضع المركزي طريقة لضمان أن مديري المشروع يمكنهم تعريف متطلبات الموارد على مستوى المشروع. يتم تفويض استيفاء متطلبات الموارد إلى مدير موارد. يمكن لمديري المشاريع قبول أو رفض الموارد المقترحة من قبل مدير الموارد.

![الوضع مركزي.](./media/resource-management-central.png)

لإدارة الموارد من خلال الوضع المركزي، راجع:

- [تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد](/dynamics365/project-service/assign-generic-bookable-resource)
- [حجز موارد مسماة من متطلبات الموارد](/dynamics365/project-service/book-named-resource)
- [إرسال طلب المورد](/dynamics365/project-service/submit-resource-request)
- [استيفاء طلب موارد](/dynamics365/project-service/resource-management-fulfill-requests)
- [قبول مورد مشروع مقترح أو رفضه من طلب مورد](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>الوضع المختلط
في المؤسسات التي تتطلب مرونة في تخصيص الموارد، يقوم الوضع المختلط بتمكين مديري المشاريع ومديري الموارد من القدرة على حجز الموارد.

![الوضع مختلط.](./media/resource-management-hybrid.png)

بالإضافة إلى عملية الوضع المركزي المدعومة، راجع الموضوعات التالية لإدارة كافة تدفقات الحجز المدعومة الأخرى في الوضع المختلط:

حجز مورد مباشرة إلى مشروع:
- [حجز موارد مسماة قابل للحجز إلى فريق مشروع وتعيين المهام](/dynamics365/project-service/assign-named-bookable-resource)

حجز مورد ممن متطلبات الموارد:
- [تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد](/dynamics365/project-service/assign-generic-bookable-resource)
- [حجز موارد مسماة من متطلبات الموارد](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]