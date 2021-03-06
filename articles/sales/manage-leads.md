---
title: إدارة العملاء المتوقعين
description: يقدم هذا الموضوع معلومات حول إدارة العملاء المتوقعين المستندين إلى المشروع.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a10be42f4ae1ecc8ae5613ed8fdc669304e0ec72
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898605"
---
# <a name="manage-leads"></a>إدارة العملاء المتوقعين

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يمكن إدارة العملاء المتوقعين المستندين إلى المشروع وتأهيلهم في Project Operations. تتضمن عملية إدارة العملاء المتوقعين إنشاء عملاء متوقعين على أساس العمل وتأهيل هؤلاء العملاء المتوقعين. 

## <a name="project-sales-leads"></a>العملاء المتوقعون لمبيعات المشروع

في قسم **المبيعات**، في الجزء الأيسر من التنقل، افتح صفحة قائمة **العملاء المتوقعين** لعرض قائمة بكافة سجلات العملاء المتوقعين في النظام. قائمة العملاء المتوقعين الموضحة هي قائمة تستند إلى العمل والأنواع الأخرى من العملاء المتوقعين الذين يمكن إنشاؤهم إذا كان لديك أيضً تطبيقات Dynamics 365 Sales أو Dynamics 365 Field Service.

يمكنك إنشاء طريقة عرض مُصفاة لرؤية العملاء المتوقعين المستندين إلى المشروع فقط من خلال إنشاء عامل تصفية لقيمة **النوع**. على سبيل المثال، يمكنك اختيار إظهار العملاء المتوقعين المستندين إلى العمل فقط.

## <a name="create-a-new-lead-for-a-project-based-deal"></a>إنشاء عميل متوقع جديد لصفقة مستندة إلى مشروع

عندما يكون العميل المتوقع المستند إلى المشروع مؤهلا، يتم إنشاء فرصة وحساب. تعتبر الفرصة المستندة إلى المشروع نقطة البداية للأنشطة التي تهدف إلى المبيعات في مرحلة الفرصة. تتضمن الفرص المستندة إلى المشروع إمكانيات فريدة والتي تكون مطلوبة لعمل المشروع البيع. وتتضمن هذه الإمكانيات:

- أساليب فوترة الوقت والمواد والسعر الثابت
- قوائم أسعار بتواريخ سريان متعددة للموارد البشرية والمصروفات والمواد التي يتم تكبدها في المشروعات

كي يقوم العميل المتوقع المؤهل بإنشاء فرصة تلقائيًا، قم بتعيين سمة **النوع** إلى **معتمد على العمل** عند إنشاء العميل المتوقع. إذا اخترت نوعًا مختلفًا، فلن يقوم العميل المتوقع بإنشاء فرصة مستندة إلى المشروع عندما يكون مؤهلا. إذا لم يتم إنشاء الفرصة المستندة إلى المشروع، فلن تكون الإمكانات الخاصة بالمشروع متوفرة في عمليات المبيعات اللاحقة.

يتضمن الجدول التالي معلومات الحقل المهمة لأحد العملاء المتوقعين، والآثار اللاحقة لتلك الحقول.
 
| **الحقل** | **الموقع** | **الصلة والغرض والإرشاد** | **تأثير لاحق** |
| --- | --- | --- | --- |
| موضوع | علامة التبويب عام | يجب أن يحتوي الحقل النصي على وصف موجز للصفقة. | سيكون موضوع العميل المتوقع الموضوع الافتراضي للفرصة واسم عرض الأسعار وعقد المشروع. |
| النوع | علامة التبويب عام | يشتمل حقل مجموعة الخيارات هذا على الخيارات التالية:</br>- المستند إلى العمل (متوفر فقط عند تثبيت Project Operations)</br>- المستند إلى البند (يتوفر فقط عند تثبيت Project Operations وSales)</br>- يستند إلى صيانة الخدمة (يكون متوفرًا عند تثبيت Field Service) | عند تعيين قيمة هذا الحقل إلى **يستند إلى العمل** في العميل المتوقع، يتم تأهيل العميل المتوقع لإنشاء فرصة تستند إلى المشروع. تكون الفرصة المستندة إلى المشروع مطلوبة لتمكين كافة الوظائف والملحقات الخاصة بالمشروع في عملية المبيعات اللاحقة لهذه الصفقة. |
| الاسم الأول | علامة التبويب عام | الاسم الأول لجهة اتصال العميل المحتمل | عند تأهيل العميل المتوقع، يتم إنشاء حساب وجهة اتصال وفرصة. الاسم الأول لجهة الاتصال هو القيمة التي تم تعيينها هنا. |
| اسم العائلة | علامة التبويب عام | اسم العائلة لجهة اتصال العميل المحتمل | عند تأهيل العميل المتوقع، يتم إنشاء حساب وجهة اتصال وفرصة. اسم عائلة جهة الاتصال هو القيمة التي تم تعيينها هنا. |
| الشركة | علامة التبويب عام | اسم شركة العميل المحتمل | عند تأهيل العميل المتوقع، يتم إنشاء حساب وجهة اتصال وفرصة. اسم الحساب الذي تم إنشاؤه هو القيمة التي تم تعيينها هنا. |
| ‏‏العملة | علامة التبويب تفاصيل | عملة العميل المحتمل | عند تأهيل العميل المتوقع، يتم إنشاء حساب وجهة اتصال وفرصة. عملة الحساب الذي تم إنشاؤه هو القيمة التي تم تعيينها هنا. |

## <a name="qualify-a-new-project-based-lead"></a>تأهيل عميل متوقع جديد يستند إلى مشروع

ويطلق على العملاء المتوقعين الذين تم تعيين قيمة **النوع** لهم إلى **يستند إلى العمل** اسم العملاء المتوقعين المستندين إلى المشروع. عندما يكون العميل المتوقع المستند إلى المشروع مؤهلا، يتم إنشاء ما يلي:

- حساب يستخدم **حقل الشركة** من العميل المتوقع.
- سجل جهة اتصال مقترن بالحساب استنادا إلى القيم الموجودة في حقول **الاسم الأول** و**اسم العائلة** في العميل المتوقع.
- فرصة مستندة إلى مشروع حيث تم تعيين حقل **النوع** إلى &quot;**معتمد على العمل**.

لمزيد من المعلومات التفصيلية حول تأهيل العملاء المتوقعين، راجع [تأهيل العملاء المتوقعين أو تحويلهم](https://docs.microsoft.com/dynamics365/sales-enterprise/qualify-lead-convert-opportunity-sales).

## <a name="lead-qualification-and-legal-entity-information"></a>تأهيل العميل المتوقع ومعلومات عن الكيان القانوني 

عندما تقوم بتشغيل Project Operations باستخدام وضع النشر، Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬، سيحتاج كل عميل وفرصة إلى تعيين حقل **الشركة المالكة**. وتعد الشركة المالكة بمثابة كيان قانوني في مؤسستك يمتلك تسليم المشروع. يجب تعيين قيمة حقل **الشركة المالكة** لكل عميل، أو حساب لديه نوع علاقة العميل، إلى الكيان القانوني الذي يتعاقد ويتفاوض مع العميل. بإمكان العميل أن يكون موجودًا في كيان قانوني واحد فقط.

عندما إلغاء تأهيل العميل المتوقع، سيكون حقل **الشركة المالكة** لسجلات العميل والفرصة التي تم إنشاؤها معينًا إلى شركة سجل المورد القابل للحجز للمستخدم الحالي.

إذا كان سجل المورد القابل للحجز للمستخدم الحالي فارغًا، فسيتم استخدام قيمة حقل **الشركة المالكة** على سجل المستخدم بشكل افتراضي في سجلات العميل والفرصة.

## <a name="business-process-flow-for-project-based-deals"></a>سير إجراءات العمل للصفقات المعتمدة على المشروع

يتم دعم سير إجراءات العمل التالي للصفقات المعتمدة على المشروعات في Project Operations:

- إجراءات العمل من العميل المتوقع إلى الفرصة
- عملية مبيعات الفرصة

تدعم إجراءات العمل من العميل المتوقع إلى الفرصة المراحل التالية:

| اسم المرحلة | الكيان المعين | الوظائف |
| --- | --- | --- |
| تأهيل | عميل متوقع | تأهيل عميل متوقع لإنشاء حساب وجهة اتصال وفرصة. |
| تطوير | الفرصة | تطوير الفرصة لإضافة المزيد من المعلومات حول العمل المتضمن وحملة الأسهم والمنافسة. |
| اقتراح | الفرصة | تطوير الاقتراح والحصول على موافقة من فريق المراجعة الداخلي. |
| إقفال | الفرصة | الفوز بفرصة لإغلاق الصفقة. |
