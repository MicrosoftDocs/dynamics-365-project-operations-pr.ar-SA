---
title: نظرة عامة على ‏‫القيم الفعلية‬
description: يقدم هذا الموضوع معلومات حول القيم الفعلية للمشروع.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 9559cb2dcc38cb8058c5a9a3b97a35019fea486f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070842"
---
# <a name="actuals-overview"></a>نظرة عامة على ‏‫القيم الفعلية‬

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

القيم الفعلية هي مقدار العمل الذي تم إكماله في مشروع. يمكن تتبع العمل الفعلي للمشروع من خلال المستندات المصدر الخاصة به. وتتضمن المستندات المصدر هذه الوقت والمصروفات وإدخالات دفتر اليومية وكذلك الفواتير.

![كيفية تتبع العمل الفعلي للمشروع من خلال مستندات مصدر](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a>إرسال إدخال وقت

في PSA، عند تقديم إدخال وقت لمشروع تم تعيينه إلى بند عقد الوقت والمواد، يتم إنشاء بندي دفتر يومية. ويُخصص بند واحد هو للتكلفة، والبند الآخر للمبيعات غير المفوترة. عند تقديم إدخال وقت لمشروع تم تعيينه إلى بند عقد سعر ثابت، يتم إنشاء بند دفتر يومية للتكلفة فقط. 

يعتمد منطق إدخال الأسعار الافتراضية على سطر دفتر اليومية. يتم نسخ كافة قيم الحقول من إدخال الوقت إلى سطر دفتر اليومية. تتضمن هذه الحقول تاريخ الحركة وبند العقد الذي تم تعيين المشروع له وينتج عن العملة قائمة الأسعار المناسبة. 

تؤدي الحقول التي تؤثر في الأسعار الافتراضية مثل **الدور** و **"وحدة المؤسسة** إلى إدخال سعر مناسب بشكل افتراضي في سطر دفتر اليومية. إذا قمت باضافة حقل مخصص في إدخال الوقت، وتريد أن يتم نشر قيمة الحقل إلى القيم الفعلية، قم بإنشاء الحقل في الكيان "القيم الفعلية"، واستخدم تعيينات الحقول لنسخ الحقل من إدخال الوقت إلى القيمة الفعلية.

## <a name="submitting-an-expense-entry"></a>إرسال إدخال مصروفات

في PSA، عند تقديم إدخال مصروفات لمشروع تم تعيينه إلى بند عقد الوقت والمواد، يتم إنشاء بندي دفتر يومية. ويُخصص بند واحد هو للتكلفة، والبند الآخر للمبيعات غير المفوترة. عند تقديم إدخال مصروفات لمشروع تم تعيينه إلى بند عقد سعر ثابت، يتم إنشاء بند دفتر يومية للتكلفة فقط.

يستند منطق إدخال الأسعار الافتراضية للمصروفات إلى فئة المصروفات التي تم تحديدها في صفحة **إدخال المصروفات**. يتم استخدام تاريخ الحركة وبند العقد الذي تم تعيين المشروع له والعملة جميعًا لتحديد قائمة الأسعار المناسبة. ومع ذلك، بالنسبة للسعر نفسه، يتم تعيين المبلغ الذي ادخله المستخدم مباشرة في بنود دفتر يومية المصروفات المرتبطة بالنسبة للتكلفة والمبيعات بشكل افتراضي.

في الإصدار الحالي من PSA، لا يتوفر الإدخال المستند إلى الفئة للأسعار الافتراضية لكل وحدة في إدخالات المصروفات.

## <a name="using-entry-journals-to-record-costs"></a>استخدام دفاتر يومية الإدخال لتسجيل التكاليف

في PSA، تتيح لك دفاتر يومية الإدخال تسجيل التكلفة أو العائد في فئات المواد أو الرسوم أو الوقت أو المصروفات أو الحركات الضريبية. يحتوي دفتر اليومية علي رأس وبنود وإجراء **تأكيد**. إليك بعض السيناريوهات التي قد تستخدم فيها دفتر اليومية:

- يجب عليك تسجيل التكاليف والمبيعات الفعلية للمواد في أحد المشاريع.
- يجب نقل القيم الفعلية من نظام آخر إلى PSA.
- يجب عليك تسجيل التكاليف التي حدثت في نظام آخ ، مثل تكاليف التدبير أو التقاعد من الباطن.

> [!IMPORTANT]
> يجب ألا يتم استخدام دفاتر اليومية لإنشاء القيم الفعلية إلا بواسطة مستخدم على دراية كاملة بالتأثير المحاسبي الذي تحدثه الأعمال الفعلية على المشروع. وهذا لأن التطبيق لا يتحقق من نوع بند دفتر اليومية، أو التسعير ذي الصلة الذي تم إدخاله في بند دفتر اليومية. ونظرًا لتأثير هذا النوع من دفاتر اليومية، توخ الحذر الكافي بشأن من يتم منحه حق الوصول لإنشاء دفاتر يومية الإدخال.     


## <a name="recording-actuals-based-on-project-events"></a>تسجيل القيم الفعلية استنادا إلى أحداث المشروع

تسجل PSA الحركات المالية التي تحدث أثناء المشروع. تم تسجيل هذه الحركات على أنها **قيم فعليه**. توضح الجداول التالية الأنواع المختلفة من القيم الفعلية التي يتم إنشاؤها، وذلك استنادا إلى ما إذا كان المشروع هو مشروع الوقت والمواد أو أحد المشاريع ثابتة السعر، أو في مرحلة المبيعات الأولية، أو أنه مشروع داخلي.

**ينتمي المورد إلى نفس الوحدة التنظيمية باعتباره وحدة التعاقد الخاصة بالمشروع**

<table>
<thead>
<tr>
<th rowspan="3">حدث</th>
<th colspan="4">مشروع قابل للفوترة أو مبيع</th>
<th rowspan="3">مشروع في مرحلة المبيعات الأولية</th>
<th rowspan="3">مشروع داخلي</th>
</tr>
<tr>
<th colspan="2">الوقت والمواد</th>
<th colspan="2">سعر ثابت</th>
</tr>
<tr>
<th>القيم الفعلية</th>
<th>عملة المعاملة‬</th>
<th>سعر ثابت</th>
<th>عملة المعاملة‬</th>
</tr>
</thead>
<tbody>
<tr>
<td>تم إنشاء إدخال وقت.</td>
<td colspan="6">لا يوجد نشاط في كيان القيم الفعلية</td>
</tr>
<tr>
<td>تم إرسال إدخال وقت.</td>
<td colspan="6">لا يوجد نشاط في كيان القيم الفعلية</td>
</tr>
<tr>
<td rowspan="2">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</td>
<td>القيمة الفعلية للتكلفة</td>
<td>عملة الوحدة المتعاقدة</td>
<td rowspan="2">القيمة الفعلية للتكلفة</td>
<td rowspan="2">عملة الوحدة المتعاقدة
<td rowspan="2">القيمة الفعلية للتكلفة</td>
<td rowspan="2">القيمة الفعلية للتكلفة</td>
</tr>
<tr>
<td>القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="3">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</td>
<td>القيمة الفعلية للتكلفة</td>
<td>عملة الوحدة المتعاقدة</td>
<td rowspan="3">القيمة الفعلية للتكلفة</td>
<td rowspan="3">عملة الوحدة المتعاقدة</td>
<td rowspan="3">القيمة الفعلية للتكلفة</td>
<td rowspan="3">القيمة الفعلية للتكلفة</td>
</tr>
<tr>
<td>القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="2">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</td>
<td>إلغاء مبيعات غير مفوترة</td>
<td>عملة عقد المشروع</td>
<td rowspan="2">المبيعات التي تمت فوترتها للحدث الرئيسي</td>
<td rowspan="2">عملة عقد المشروع</td>
<td rowspan="2">غير قابل للتطبيق</td>
<td rowspan="2">غير قابل للتطبيق</td>
</tr>
<tr>
<td>المبيعات المفوترة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="3">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</td>
<td>إلغاء مبيعات غير مفوترة</td>
<td>عملة عقد المشروع</td>
<td rowspan="3">غير قابل للتطبيق</td>
<td rowspan="3">غير قابل للتطبيق</td>
<td rowspan="3">غير قابل للتطبيق</td>
<td rowspan="3">غير قابل للتطبيق</td>
</tr>
<tr>
<td>المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="2">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</td>
<td>مبيعات مفوترة - إلغاء</td>
<td>عملة عقد المشروع</td>
<td rowspan="5">
<ul>
<li>مبيعات مفوترة للحدث الرئيسي</li>
<li>تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></li>
</ul>
</td>
<td rowspan="5">عملة عقد المشروع</td>
<td rowspan="5">غير قابل للتطبيق</td>
<td rowspan="5">غير قابل للتطبيق</td>
</tr>
<tr>
<td>المبيعات المفوترة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="3">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</td>
<td>مبيعات مفوترة - إلغاء</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>المبيعات المفوترة للكمية الجديدة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</td>
<td>عملة عقد المشروع</td>
</tr>
</tbody>
</table>

**ينتمي المورد إلى وحدة تنظيمية تختلف عن وحدة التعاقد الخاصة بالمشروع**

<table>
<thead>
<tr>
<th rowspan="3">حدث</th>
<th colspan="4">مشروع قابل للفوترة أو مبيع</th>
<th rowspan="3">مشروع في مرحلة المبيعات الأولية</th>
<th rowspan="3">مشروع داخلي</th>
</tr>
<tr>
<th colspan="2">الوقت والمواد</th>
<th colspan="2">سعر ثابت</th>
</tr>
<tr>
<th>القيم الفعلية</th>
<th>عملة المعاملة‬</th>
<th>سعر ثابت</th>
<th>عملة المعاملة‬</th>
</tr>
</thead>
<tbody>
<tr>
<td>تم إنشاء إدخال وقت.</td>
<td colspan="6">لا يوجد نشاط في كيان القيم الفعلية</td>
</tr>
<tr>
<td>تم إرسال إدخال وقت.</td>
<td colspan="6">لا يوجد نشاط في كيان القيم الفعلية</td>
</tr>
<tr>
<td rowspan="4">تمت الموافقة على الوقت، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة أثناء الموافقة.</td>
<td>القيمة الفعلية للتكلفة</td>
<td>عملة الوحدة المتعاقدة</td>
<td rowspan="4">القيمة الفعلية للتكلفة</td>
<td rowspan="4">عملة الوحدة المتعاقدة</td>
<td rowspan="4">القيمة الفعلية للتكلفة</td>
<td rowspan="4">القيمة الفعلية للتكلفة</td>
</tr>
<tr>
<td>القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>تكلفة وحدة تعيين الموارد</td>
<td>عملة وحدة تعيين الموارد</td>
</tr>
<tr>
<td>مبيعات بين المؤسسات</td>
<td>عملة الوحدة المتعاقدة</td>
</tr>
<tr>
<td rowspan="5">تمت الموافقة على الوقت، وحدثت زيادة في الساعات القابلة للفوترة أثناء الموافقة.</td>
<td>القيمة الفعلية للتكلفة</td>
<td>عملة الوحدة المتعاقدة</td>
<td rowspan="5">القيمة الفعلية للتكلفة</td>
<td rowspan="5">عملة الوحدة المتعاقدة</td>
<td rowspan="5">القيمة الفعلية للتكلفة</td>
<td rowspan="5">القيمة الفعلية للتكلفة</td>
</tr>
<tr>
<td>تكلفة وحدة تعيين الموارد</td>
<td>عملة وحدة تعيين الموارد</td>
</tr>
<tr>
<td>مبيعات بين المؤسسات</td>
<td>عملة الوحدة المتعاقدة</td>
</tr>
<tr>
<td>القيمة الفعلية للمبيعات غير المفوترة - خاضعة للرسوم مع الكمية الجديدة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>القيمة الفعلية للمبيعات غير المفوترة - غير خاضعة للرسوم مع الفرق</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="2">تم تأكيد الفاتورة، ولا يحدث تغيير أو زيادة في الساعات القابلة للفوترة.</td>
<td>إلغاء مبيعات غير مفوترة</td>
<td>عملة عقد المشروع</td>
<td rowspan="2">المبيعات التي تمت فوترتها للحدث الرئيسي</td>
<td rowspan="2">عملة عقد المشروع</td>
<td rowspan="2">غير قابل للتطبيق</td>
<td rowspan="2">غير قابل للتطبيق</td>
</tr>
<tr>
<td>المبيعات المفوترة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="3">تم تأكيد الفاتورة، وحدثت زيادة في الساعات القابلة للفوترة.</td>
<td>إلغاء مبيعات غير مفوترة</td>
<td>عملة عقد المشروع</td>
<td rowspan="3">غير قابل للتطبيق</td>
<td rowspan="3">غير قابل للتطبيق</td>
<td rowspan="3">غير قابل للتطبيق</td>
<td rowspan="3">غير قابل للتطبيق</td>
</tr>
<tr>
<td>المبيعات المفوترة - خاضعة للرسوم مع الكمية الجديدة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>المبيعات المفوترة - غير خاضعة للرسوم مع الفرق</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="2">يتم تصحيح فاتورة لزيادة الكمية الخاضعة للرسوم.</td>
<td>مبيعات مفوترة - إلغاء</td>
<td>عملة عقد المشروع</td>
<td rowspan="5">
<ul>
<li>مبيعات مفوترة للحدث الرئيسي</li>
<li>تغيير في حاله الحدث الرئيسي من<strong>مفوتر</strong> إلى <strong>جاهز للفاتورة</strong></li>
</ul>
</td>
<td rowspan="5">عملة عقد المشروع</td>
<td rowspan="5">غير قابل للتطبيق</td>
<td rowspan="5">غير قابل للتطبيق</td>
</tr>
<tr>
<td>المبيعات المفوترة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td rowspan="3">يتم تصحيح فاتورة لتخفيض الكمية الخاضعة للرسوم.</td>
<td>مبيعات مفوترة - إلغاء</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>المبيعات المفوترة للكمية الجديدة</td>
<td>عملة عقد المشروع</td>
</tr>
<tr>
<td>المبيعات غير المفوترة - خاضعة للرسوم مع الفرق</td>
<td>عملة عقد المشروع</td>
</tr>
</tbody>
</table>