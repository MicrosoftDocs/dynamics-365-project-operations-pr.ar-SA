---
title: نظرة عامة على أوضاع إدارة الموارد
description: يوفر هذا المقال معلومات حول وظيفة إدارة الموارد في Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: dd50d12686a6ad17f6a95ccf0c2f1447cc470bf7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928416"
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

بالإضافة إلى عملية الوضع المركزي المدعوم، راجع المقالات التالية لإدارة كافة عمليات سير عمل الحجوزات المدعومة الأخرى في الوضع المختلط:

حجز مورد مباشرة إلى مشروع:
- [حجز موارد مسماة قابل للحجز إلى فريق مشروع وتعيين المهام](/dynamics365/project-service/assign-named-bookable-resource)

حجز مورد ممن متطلبات الموارد:
- [تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد](/dynamics365/project-service/assign-generic-bookable-resource)
- [حجز موارد مسماة من متطلبات الموارد](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]