---
title: تغييرات إدارة الموارد (Project Service Automation 3.x)
description: يوفر هذا الموضوع معلومات حول التغييرات التي تتم على منطقة إدارة الموارد.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: bc293e7686b7fd7d50d232cb8b26bfc03eb29c8911b52536d2b0a3a4929730c9
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "7000290"
---
# <a name="resource-management-changes-project-service-automation-3x"></a>تغييرات إدارة الموارد (Project Service Automation 3.x)

[!include [banner](../../includes/psa-now-project-operations.md)]

توفر أقسام هذه الموضوع معلومات حول التغييرات التي تم إجراؤها على منطقة إدارة الموارد في الإصدار 3.x من Dynamics 365 Project Service Automation.

## <a name="project-estimates"></a>تقديرات المشروع

وبدلاً من كون تقديرات المشروع مستندة إلى كيان **msdyn\_projecttask** (**Project Task**)، تستند تقديرات المشروع إلى كيان **msdyn\_resourceassignment** (**تعيين المورد**). أصبحت تعيينات الموارد "مصدر الحقيقة" لجدولة المهام وأسعارها.

## <a name="line-tasks"></a>مهام البنود

في PSA 3. x، مهام البنود قديمة (مهملة). تشير التعيينات الآن إلى المهمة بالكامل بدلاً من مهام البنود.

يوضح المثال التالي كيفية تعيين مهمة تُسمى "مهمة الاختبار" لأعضاء الفريق A وB في الإصدارين السابقين من PSA وفي الإصدار 3.x من PSA.

- **قبل PSA 3.x:**

    - مهمة الاختبار

        - مهمة الاختبار - مهمة البند 1

            - التعيين إلى A

        - مهمة الاختبار - مهمة البند 2

            - التعيين إلى B

- **PSA 3.x:**

    - مهمة الاختبار

        - التعيين إلى A
        - التعيين إلى B

## <a name="unassigned-assignment"></a>التعيين غير المعين

في PSA 3.x، التعيين غير المعين هو تعيين يتم تعيينه لعضو فريق **فارغ** ومورد **فارغ**. يمكن أن تحدث التعيينات غير المعينة في سيناريوهين:

- إذا تم إنشاء مهمة، ولكن لم يتم تعيينها بعد إلى أي عضو من أعضاء الفريق، يتم دومًا إنشاء تعيين غير معين. 
- إذا تمت إزالة كافة المعين لهم في إحدى المهام، ستتم إعادة إنشاء تعيين غير معين لهذه المهمة.

## <a name="scheduling-fields-on-the-project-task-entity"></a>جدولة الحقول في كيان مهمة المشروع

تم إهمال الحقول في كيان **msdyn\_projecttask** أو تم نقلها إلى كيان **msdyn\_resourceassignment** أو تتم الإشارة إليها الآن من كيان **msdyn\_projectteam** (**عضو فريق المشروع**).

| الحقل المهمل في \_projecttask (مهمة المشروع) | حقل جديد في msdyn\_resourceassignment (تعيين المورد) | تعليق |
|---|---|---|
| msdyn\_assignedresources | بلا | |
| msdyn\_assignedteammembers | بلا | |
| msdyn\_numberofresources | بلا | |
| msdyn\_scheduledhours | بلا | |
| msdyn\_effortcontour | msdyn\_plannedwork | تم تغيير تنسيق بنية بيانات منهج كائن JavaScript ‏(JSON) المخزنة في الحقل. |

## <a name="schedule-contour"></a>مخطط الجدولة

يتم تخزين مخطط الجدولة في حقل **العمل المخطط** (**msdyn\_plannedwork**) في كلٍّ من كياني **تعيين المورد** (**msdyn\_resourceassignment**).

### <a name="structure"></a>هيكل

تتكون البنية الجديدة لمخطط الجدولة من شرائح زمنية مرنة يتم تعريفها لكل يوم من الجدولة. تحتوي كل شريحة زمنية على الخصائص التالية:

- **البداية** – بدء ساعات العمل لليوم وفقًا لتقويم المشروع.
- **النهاية** – انتهاء ساعات العمل لليوم وفقًا لتقويم المشروع.
- **الساعات** -عدد الساعات التي تم تعيينها في اليوم.

**مثال**

يستخدم هذا المثال تقويم مشروع حيث يكون يوم العمل من 9 صباحًا إلى 5 مساءً في المنطقة الزمنية UTC-8.

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a>الجدولة التلقائية والجدولة اليدوية

وإذا كانت المهمة مجدولة تلقائيًا، فسيتم تحميل الساعات في المقدمة وقد تنخفض مده المهمة.

**مثال**

تتم جدولة المهمة التالية تلقائيًا لمدة 18 ساعة خلال ثلاثه أيام (من 3 ديسمبر 2018 إلى 5 ديسمبر 2018).

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

وإذا كانت المهمة مجدولة يدويًا، يتم توزيع الساعات بالتساوي على كافة التواريخ.

**مثال**

تتم جدولة المهمة التالية يدويًا لمدة 18 ساعة خلال ثلاثه أيام (من 3 ديسمبر 2018 إلى 5 ديسمبر 2018).

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a>وحدة التعيين

تم إهمال وحده التعيين في PSA 3.x. أصبحت ساعات مجهود المهام مقسومة بشكل متساو في كل يوم، بين كافة الموارد المعينة.

**مثال**

في هذا المثال، يتم تعيين المهمة إلى موردين وتتم جدولتها تلقائيًا لمده 36 ساعة من ثلاثه أيام (من 3 ديسمبر 2018 إلى 5 ديسمبر 2018).

- التعيين 1:

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- التعيين 2:

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a>أبعاد التسعير

في PSA 3.x، تمت إزالة حقول أبعاد التسعير الخاصة بالمورد (مثل **الدور** و **الوحدة التنظيمية**) من كيان **msdyn\_projecttask**. يمكن استرداد هذه الحقول الآن من عضو فريق المشروع المقابل (**msdyn\_projectteam**) في تعيين المورد (**msdyn\_resourceassignment**) عند إنشاء تقديرات المشروع. تمت إضافة الحقل الجديد **msdyn\_organizationalunit** إلى كيان **msdyn\_projectteam**.

| الحقل المهمل في \_projecttask (مهمة المشروع) | حقل من msdyn\_projectteam (عضو فريق المشروع) تم استخدامه بدلاً من ذلك |
|---|---|
| msdyn\_resourcecategory | msdyn\_resourcecategory |
| msdyn\_organizationalunit | msdyn\_organizationalunit |

## <a name="contours"></a>المخططات

تم إهمال حقول مخططات التسعير والتقدير في كيان **msdyn\_projecttask**. وتم نقلها إلى كيان **msdyn\_resourceassignment**.

| الحقل المهمل في \_projecttask (مهمة المشروع) | حقل جديد في msdyn\_resourceassignment (تعيين المورد) |
|---|---|
| msdyn\_costestimatecontour | msdyn\_plannedcostcontour |
| msdyn\_salesestimatecontour | msdyn\_plannedsalescontour |

تمت إضافة الحقول التالية إلى كيان **msdyn\_resourceassignment**:

* msdyn\_plannedcost
* msdyn\_plannedsales

لم يتم تغيير الحقول التالية للتكاليف والمبيعات الفعلية والمتبقية والمخطط لها في كيان **msdyn\_projecttask**:

* msdyn\_plannedcost
* msdyn\_plannedsales
* msdyn\_actualcost
* msdyn\_actualsales
* msdyn\_remainingcost
* msdyn\_remainingsales


[!INCLUDE[footer-include](../../includes/footer-banner.md)]