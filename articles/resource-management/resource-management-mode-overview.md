---
title: نظرة عامة على أوضاع إدارة الموارد
description: يوفر هذا الموضوع معلومات حول وظائف إدارة الموارد في Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 73ba6190e2e366f22372102d14d26f6d71ba0bc1
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4118502"
---
# <a name="resource-management-modes-overview"></a>نظرة عامة على أوضاع إدارة الموارد

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_


يدعم Dynamics 365 Project Operations وضعين لكي تقوم بتنفيذ سير مهام الحجز الكلية. يتم تعريف وضع الإدارة كمعلمة مشروع ويمكن تعديلها إذا احتاج العمل الخاص بك إلى التغيير.    

## <a name="central-mode"></a>الوضع المركزي
بالنسبة للمؤسسات التي تقوم بالتخصيص المركزي للموارد بشأن المشاريع، يوفر الوضع المركزي طريقة لضمان أن مديري المشروع يمكنهم تعريف متطلبات الموارد على مستوى المشروع. يتم تفويض استيفاء متطلبات الموارد إلى مدير موارد. يمكن لمديري المشاريع قبول أو رفض الموارد المقترحة من قبل مدير الموارد.

![الوضع المركزي](./media/resource-management-central.png)

لإدارة الموارد من خلال الوضع المركزي، راجع:

- [تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [حجز موارد مسماة من متطلبات الموارد](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [إرسال طلب المورد](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [استيفاء طلب موارد](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [قبول مورد مشروع مقترح أو رفضه من طلب مورد](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>الوضع المختلط
في المؤسسات التي تتطلب مرونة في تخصيص الموارد، يقوم الوضع المختلط بتمكين مديري المشاريع ومديري الموارد من القدرة على حجز الموارد.

![الوضع المختلط](./media/resource-management-hybrid.png)

بالإضافة إلى عملية الوضع المركزي المدعومة، راجع الموضوعات التالية لإدارة كافة تدفقات الحجز المدعومة الأخرى في الوضع المختلط:

حجز مورد مباشرة إلى مشروع:
- [حجز موارد مسماة قابل للحجز إلى فريق مشروع وتعيين المهام](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

حجز مورد ممن متطلبات الموارد:
- [تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [حجز موارد مسماة من متطلبات الموارد](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]