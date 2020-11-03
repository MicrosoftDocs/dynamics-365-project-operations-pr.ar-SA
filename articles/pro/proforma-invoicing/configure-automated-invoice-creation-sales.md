---
title: تكوين الإنشاء التلقائي للفاتورة الأولية
description: يقدم هذا الموضوع معلومات حول تكون الإنشاء التلقائي للفواتير الأولية.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e146dd510b3795d52d164fc6acf8e5400ba11310
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070553"
---
# <a name="configure-automated-proforma-invoice-creation"></a>تكوين الإنشاء التلقائي للفاتورة الأولية

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_

يمكنك تكوين الإنشاء التلقائي للفواتير في فاتورة تلقائية في Dynamics 365 Project Operations. يقوم النظام بإنشاء مسودة فاتورة أولية استنادًا إلى جدول الفواتير لكل عقد مشروع وشروط تعاقد. يتم تكوين جداول الفواتير على مستوى شروط التعاقد. بإمكان كل بند على عقد أن يتضمن جدول فواتير مميزًا، أو يمكن تضمين جدول الفواتير نفسه على كل بند من بنود العقد.

عندما تنشئ فاتورة، يقوم النظام دائمًا بإنشاء فاتورة واحدة على الأقل لكل عقد مشروع. في بعض الحالات، قد يتم إنشاء فواتير متعددة.

على سبيل المثال، عندما يتضمن العقد عدة عملاء، سيتم إنشاء عدد فواتير مماثلة لعدد العملاء الذين لديهم حركات قابلة للفوترة لإجراء الفوترة على عقد المشروع هذا.

## <a name="understand-how-transactions-are-included-on-an-invoice"></a>كيفية تضمين الحركات في فاتورة 

في بعض الأحيان، يحدد كل شرط من شروط التعاقد المستندة إلى المشروع جدول فواتير منفصلاً. على سبيل المثال، تتضمن خدمات التنفيذ الخاصة بعقد Adatum شروط التعاقد التالية:

- عمل النموذج الأولي وهو سعر ثابت مع مرحلتين رئيسيتين تم إنشاؤهما يدويًا.
- عمل التنفيذ الذي يشتمل على الوقت والذي ستتم فوترته كل أسبوعين‬ أيام الإثنين.
- المصروفات المستحقة التي ينبغي ان تتم فوترها شهريًا في أول يوم إثنين من كل شهر.

تبدو جداول الفواتير التي تم تعريفها في كل من هذين البندين كالجدول التالي:

| شروط التعاقد | تاريخ تشغيل الفاتورة | تاريخ إيقاف العملية | تاريخ المرحلة الرئيسية | مبلغ المرحلة الرئيسية |
| --- | --- | --- | --- | --- |
| عمل النموذج الأولي | الإثنين 5 أكتوبر | - | الإثنين 5 أكتوبر | 5000 دولار أمريكي |
| - | الثلاثاء 3 نوفمبر | - | الثلاثاء 3 نوفمبر | 12,000 دولار أمريكي |
| عمل التنفيذ | الإثنين 5 أكتوبر | الأحد 4 أكتوبر | - | - |
| - | الإثنين 19 أكتوبر | الأحد 18 أكتوبر | - | - |
| - | الإثنين 2 نوفمبر | الأحد 1 نوفمبر | - | - |
| - | الإثنين 16 نوفمبر | الأحد 15 نوفمبر | - | - |
| المصروفات المستحقة | الإثنين 5 أكتوبر | الأحد 4 أكتوبر | - | - |
| - | الإثنين 2 نوفمبر | الأحد 1 نوفمبر | - | - |

في هذا المثال عندما يتم تشغيل الفوترة التلقائية على:

- **4 أكتوبر أو أي تاريخ قبله** : لا يتم إنشاء فاتورة لهذا العقد لأن **جدول الفواتير** لكل شرط من شروط التعاقد لا يسمي الأحد 4 أكتوبر كتاريخ تشغيل الفاتورة.
- **الإثنين 5 أكتوبر** : يتم إنشاء فاتورة لما يلي:

    - عمل النموذج الأولي الذي يتضمن المرحلة الرئيسية، إذا وضعت عليه علامة **جاهز للفوترة**.
    - عمل التنفيذ الذي يتضمن كافة حركات الوقت التي تم إنشاؤها قبل تاريخ وقف الحركة يوم الأحد 4 أكتوبر، والذي تم وضع علامة عليه على أنه **جاهز للفوترة**.
    - المصروفات المستحقة التي تتضمن كافة حركات المصروفات التي تم إنشاؤها قبل تاريخ وقف الحركة يوم الأحد 4 أكتوبر، والذي تم وضع علامة عليها على أنها **جاهزة للفوترة**.
  
- **6 أكتوبر أو أي تاريخ قبل 19 أكتوبر** : لا يتم إنشاء فاتورة لهذا العقد لأن **جدول الفواتير** لكل شرط من شروط التعاقد هذه لا يسمي 6 أكتوبر أو أي تاريخ قبل 19 أكتوبر كتاريخ تشغيل الفاتورة.
- **الإثنين 19 أكتوبر** : يتم إنشا فاتورة لعمل التنفيذ الذي يتضمن كافة حركات الوقت التي تم إنشاؤها قبل تاريخ وقف الحركة يوم الأحد 18 أكتوبر، والذي تم وضع علامة عليها على أنها **جاهزة للفوترة**.
- **الإثنين 2 نوفمبر** : يتم إنشاء فاتورة لما يلي:

    - عمل التنفيذ الذي يتضمن كافة حركات الوقت التي تم إنشاؤها قبل تاريخ وقف الحركة يوم الأحد 1 نوفمبر، والذي تم وضع علامة عليه على أنه **جاهز للفوترة**.
    - المصروفات المستحقة التي تتضمن كافة حركات المصروفات التي تم إنشاؤها قبل تاريخ وقف الحركة يوم الأحد 1 نوفمبر، والذي تم وضع علامة عليها على أنها **جاهزة للفوترة**.

- **الثلاثاء 3 نوفمبر** : يتم إنشاء فاتورة لعمل النموذج الأولي الذي يتضمن المرحلة الرئيسية من 12000 دولار أمريكي، إذا وضعت عليها علامة **جاهزة للفوترة**.

## <a name="configure-automatic-invoicing"></a>تكوين الفوترة التلقائية

أكمل هذه الخطوات لتكوين التشغيل التلقائي للفاتورة.

1. في **Project Operations** ، انتقل إلى **الإعدادات** > **إعداد الفاتورة المتكررة‬**.
2. قم بإنشاء وظيفة دفعية، وقم بتسميتها **إنشاء فواتير Project Operations**. يجب أن يتضمن اسم الوظيفة الدُفعية الكلمات "إنشاء الفواتير."
3. في حقل **نوع الوظيفة** ، حدد **بلا**. افتراضيًا، يتم تعيين الحقلين **التكرار اليومي** و **نشط** إلى **نعم**.
4. حدد **تشغيل سير العمل**. في مربع حوار **البحث عن سجل** ، ستري ثلاث مهام لسير العمل:

- ProcessRunCaller
- ProcessRunner
- UpdateRoleUtilization

5. حدد **ProcessRunCaller** ، ثم حدد **إضافة**.
6. في مربع الحوار التالي، حدد **موافق**. يكون سير عمل **السكون** متبوعًا بسير عمل **العملية**. 

> [!NOTE]
> يمكنك أيضا تحديد **ProcessRunner** في الخطوة 5. بعد ذلك، عندما تحدد **موافق** ، يكون سير عمل **العملية** متبوعًا بسير عمل **السكون**.

يؤدي سير عمل **ProcessRunCaller** و **ProcessRunner** إلى إنشاء الفواتير. **ProcessRunCaller** يستدعي **ProcessRunner**. **ProcessRunner** هو سير العمل الذي ينشئ الفواتير فعليًا. يمر سير العمل عبر جميع شروط التعاقد التي يجب إنشاء الفواتير لها، ويقوم بإنشاء فواتير لشروط التعاقد هذه. لتحديد شروط التعاقد التي يجب إنشاء الفواتير لها، فإن الوظيفة تبحث عن تواريخ تشغيل الفاتورة لشروط التعاقد. إذا كانت بنود العقد التي تنتمي لأحد العقود لها نفس تاريخ تشغيل الفاتورة، سيتم تجميع الحركات في فاتورة واحدة بها بندين للفاتورة. إذا لم تكن هناك حركات لإنشاء فواتير لها، تتخطى الوظيفة إنشاء الفاتورة.

بعد انتهاء تشغيل **ProcessRunner** ، فإنه يستدعي **ProcessRunCaller** ، الذي يوفر وقت النهاية، وويتم إغلاقه. بعد ذلك يبدأ **ProcessRunCaller** تشغيل مؤقت يعمل على مدار 24 ساعة من وقت النهاية المحدد. في نهاية المؤقت، يتم إغلاق **ProcessRunCaller**.

تعتبر وظيفة المعالجة الدفعية لإنشاء الفواتير وظيفة متكررة. إذا تم تشغيل هذه المعالجة الدفعية عدة مرات، سيتم إنشاء مثيلات متعددة للوظيفة وتتسبب في حدوث أخطاء. وبالتالي، يجب عليك بدء عملية المعالجة الدفعية مرة واحدة فقط، ثم إعادة تشغيلها في حالة توقفها عن العمل فقط.

> [!NOTE]
> لا يتم تشغيل الفوترة الدفعية في Project Operations إلا لشروط تعاقد المشروع التي تم تكوينها بواسطة جداول الفواتير. يجب أن يحتوي بند العقد مع طريقة فوترة بسعر ثابت على مراحل مكوّنة. سيحتاج بند عقد المشروع مع طريقة فوترة الوقت والمواد إلى إعداد جدول فاتورة يستند إلى التاريخ.