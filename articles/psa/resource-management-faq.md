---
title: الأسئلة المتداولة حول إدارة الموارد
description: يقدم هذا الموضوع إجابات على الأسئلة المتداولة حول إدارة الموارد.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 20562b98ccc8451ab57dd42fb8c2f9f303811dbe
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283127"
---
# <a name="resource-management-faq"></a>الأسئلة المتداولة حول إدارة الموارد

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a>ما الفرق بين عضو الفريق ومتطلب المورد؟

يمكن تعيين عضو فريق مشروع للمهام، المحجوزة أو المحجوزة بشكل زائد، وتعيينه كقائم بالموافقة. يمكن أن يوجد متطلب المورد دون عضو فريق مشروع، كملاحظة مسودة للطلب. 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a>ما الفرق بين الساعات المقترحة والتي تم حجزها بشكل مبدئي؟

تختلف الساعات المقترحة والساعات المحجوزة بشكل مبدئي في الرؤية. تكون الساعات المقترحة مرئية فقط لمديري الموارد ومدير المشروع الذي قام ببدء الطلب باستخدام طلب مورد. تكون الساعات المحجوزة بشكل مبدئي مرئية لأي شخص يتوفر لديه الوصول إلى لوحه الجدولة.

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a>كيف يمكنني رؤية ساعات المحجوزة بشكل مبدئي للموارد الموجودة في فريق؟

يمكن إجراء الحجوزات المبدئية عند قيامك بحجز متطلب مورد. وتظهر الموارد المحجوزة بشكل مبدئي في فريق المشروع كأعضاء فريق لديهم ساعات ساعات محجوزة بشكل مبدئي. كما تظهر في لوحة الجدولة.

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a>كيف يمكنني تغيير الساعات المطلوبة، وتاريخي البدء والانتهاء، لمورد (عام أو مسمى) قمت بحجزه؟

بعد حجز الموارد، حدد **الاحتفاظ بالحجوزات** لإجراء أي تغييرات مطلوبة.

## <a name="what-resources-types-does-project-service-automation-support"></a>ما أنواع الموارد التي يدعمها Project Service Automation؟

يمثل **المستخدم** و **جهة الاتصال** أنواع الموارد الوحيدة التي يتم دعمها في Dynamics 365 Project Service Automation. على الرغم من أنه يمكنك إنشاء أنواع أخرى من الموارد (على سبيل المثال، **المعدات** و **المجموعات**)، فإنه لا توجد حالة استخدام شاملة مدعومة لها.

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a>ما الفرق بين التعيين والحجز؟

التعيينات هي تعيين الموارد إلى مهام المشروع في جدول المشروع. قد تكون الموارد إما موارد حقيقية أو عامة. الحجوزات هي تخصيص الموارد الثابت أو المبدئي لمشروع. تستهلك الحجوزات الثابتة سعة المورد. وبشكل مثالي، بالنسبة للموارد الحقيقية، يجب أن تتفق الحجوزات والتعيينات، لأنها لا تختلف. ومع ذلك، لا يفرض PSA هذا الاتفاق. تعرض طريقة عرض التسوية أماكن مدير مشروع لا تتفق فيها الحجوزات والتعيينات الخاصة بالمورد.


[!INCLUDE[footer-include](../includes/footer-banner.md)]