---
title: ربط القيم الفعلية بالسجلات الأصلية
description: يشرح هذا الموضوع كيفية ربط القيم الفعلية بالسجلات الأصلية مثل إدخال الوقت أو إدخال المصروفات أو سجلات استخدام المواد.
author: rumant
ms.date: 03/25/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b5a70d2c2b3f98028b4e4998ed25ab73a275c66e4b8137eb573b943658a1a41e
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "6991740"
---
# <a name="link-actuals-to-original-records"></a>ربط القيم الفعلية بالسجلات الأصلية

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_


في Dynamics 365 Project Operations، تشكل *حركة الأعمال* مفهوما مجردًا لا يتم تمثيله بواسطة كيان. ومع ذلك، تم تصميم بعض الحقول والعمليات الشائعة الموجودة في الكيانات لاستخدام مفهوم حركات الأعمال. تستخدم الكيانات التالية هذا المفهوم:

- تفاصيل بند عرض الأسعار‬
- تفاصيل شروط التعاقد
- بنود التقدير
- سطور دفتر اليومية
- القيم الفعلية

من هذه الكيانات، يتم تعيين **تفاصيل بند عرض الأسعار** و **تفاصيل شروط التعاقد** و **بنود التقديرات** إلى مرحلة التقدير في دورة حياه المشروع. يتم تعيين **سطور دفتر اليومية** و **القيم الفعلية** إلى مرحلة التنفيذ في دورة حياة المشروع.

يتعرف Project Operations على السجلات في هذه الكيانات الخمسة كحركات أعمال. والفرق الوحيد هو أن السجلات الموجودة في الكيانات التي تم تعيينها إلى مرحلة التقدير تعتبر تنبؤات مالية، بينما تعتبر السجلات الموجودة في الكيانات التي يتم تعيينها إلى مرحلة التنفيذ حقائق مالية حدثت بالفعل.

## <a name="concepts-that-are-unique-to-business-transactions"></a>المفاهيم الفريدة لحركات الأعمال
تعتبر المفاهيم التالية فريدة لمفهوم حركات الأعمال:

- ‏‫نوع الحركة
- فئة الحركة
- أصل الحركة
- اتصال الحركة

### <a name="transaction-type"></a>‏‫نوع الحركة

يمثل نوع الحركة التوقيت وسياق التأثير المالي على مشروع. ويتم تمثيله بواسطة مجموعة خيارات تحتوي على القيم المدعمة التالية في Project Operations:

  - التكلفة
  - عقد المشروع
  - مبيعات غير مفوترة
  - المبيعات المفوترة
  - مبيعات بين المؤسسات
  - تكلفة وحدة تعيين الموارد

### <a name="transaction-class"></a>فئة الحركة

تمثل فئة الحركة الأنواع المختلفة للتكاليف التي تم تكبدها في المشاريع. ويتم تمثيله بواسطة مجموعة خيارات تحتوي على القيم المدعمة التالية في Project Operations:

  - الوقت
  - المصروفات
  - المواد
  - رسوم
  - الأحداث الرئيسية
  - ضريبة

عادة ما يتم استخدام قيمة **المرحلة الرئيسية** بواسطة منطق الأعمال الخاص بالفوترة ثابتة السعر في Project Operations.

### <a name="transaction-origin"></a>أصل المعاملة

**أصل الحركة** هو كيان يخزن أصل كل حركة عمل. مع التقدم الذي يحصل في تنفيذ المشروع، ستؤدي كل حركة عمل إلى نشوء حركة عمل أخرى ستنشئ بدورها حركة عمل أخرى وهكذا. تم تصميم كيان أصل الحركة لتخزين بيانات حول أصل كل حركة للمساعدة في إعداد التقارير وقابلية التعقب. 

### <a name="transaction-connection"></a>اتصال الحركة

**اتصال الحركة** هو كيان يقوم بتخزين العلاقة بين اثنين من حركات الأعمال المماثلة، مثل التكلفة وقيم المبيعات الفعلية ذات الصلة، أو عمليات إلغاء الحركات التي يتم تشغيلها بواسطة أنشطة الفوترة مثل تأكيد الفاتورة أو تصحيحات الفاتورة.

يساعدك **أصل الحركة** و **اتصال الحركة** معًا في المحافظة على تعقب العلاقات بين حركات الأعمال والإجراءات التي تؤدي إلى إنشاء حركة عمل معينة.

### <a name="example-how-transaction-origin-works-with-transaction-connection"></a>مثال: كيف يعمل أصل الحركة مع اتصال الحركة

يوضح المثال التالي المعالجة النموذجية لإدخالات الوقت في دورة حياة مشروع Project Operations.

> ![معالجة وإدخالات الوقت في دورة حياة خدمه Project Service.](media/basic-guide-17.png)
 
1. يؤدي إرسال إدخال الوقت إلى إنشاء سطرين من أسطر دفتر اليومية: أحدهما للتكلفة والأخر للمبيعات غير المفوترة.
2. تتسبب الموافقة النهائية على إدخال الوقت في إنشاء قيمتين فعليتين: قيمة فعلية للتكلفة وأخرى للمبيعات غير المفوترة.
3. عند إنشاء فاتورة مشروع جديدة، يتم إنشاء حركة بند الفاتورة باستخدام بيانات من القيمة الفعلية للمبيعات غير المفوترة. 
4. عند تأكيد الفاتورة، يتم إنشاء قيمتين فعليتين جديدتين: قيمة فعلية لإلغاء المبيعات غير المفوترة وقيمة فعلية للمبيعات المفوترة.

ينشئ كل واحد من هذه الأحداث سجلاً في الكيانين **أصل الحركة** و **اتصال الحركة**. تساعد هذه السجلات الجديدة في إنشاء محفوظات العلاقات بين السجلات التي يتم إنشاؤها عبر تفاصيل إدخال الوقت ودفتر اليومية والقيم الفعلية وسطر الفاتورة.

يُظهر الجدول التالي السجلات في كيان **أصل الحركة** لسير العمل.

| حدث                        | القيمة الأصلية                   | نوع الأصل                       | المعاملة                       | نوع المعاملة         |
|------------------------------|--------------------------|-----------------------------------|-----------------------------------|--------------------------|
| إرسال إدخال الوقت        | معرف GUID لسجل إدخال الوقت   | إدخال الوقت                        | المعرف الفريد العمومي لسجل سطر دفتر اليومية (التكلفة)   | سطر دفتر اليومية             |
| معرف GUID لسجل إدخال الوقت       | إدخال الوقت               | المعرف الفريد العمومي لسجل سطر دفتر اليومية (المبيعات)  | سطر دفتر اليومية                      |                          |
| الموافقة على الوقت                | المعرف الفريد العمومي لسجل سطر دفتر اليومية | سطر دفتر اليومية                      | المعرف الفريد العمومي لسجل المبيعات غير المفوترة        | فعلي                   |
| معرف GUID لسجل إدخال الوقت       | إدخال الوقت               | المعرف الفريد العمومي لسجل المبيعات غير المفوترة        | فعلي                            |                          |
| المعرف الفريد العمومي لسجل سطر دفتر اليومية     | سطر دفتر اليومية             | المعرف الفريد العمومي لسجل القيم الفعلية للتكلفة           | فعلي                            |                          |
| معرف GUID لسجل إدخال الوقت       | إدخال الوقت               | المعرف الفريد العمومي لسجل القيم الفعلية للتكلفة           | فعلي                            |                          |
| إنشاء فاتورة             | معرف GUID لسجل إدخال الوقت   | إدخال الوقت                        | المعرف الفريد العمومي لحركة بند الفاتورة     | حركة بند الفاتورة |
| المعرف الفريد العمومي لسجل سطر دفتر اليومية     | سطر دفتر اليومية             | المعرف الفريد العمومي لحركة بند الفاتورة     | حركة بند الفاتورة          |                          |
| تأكيد الفاتورة         | المعرف الفريد العمومي لبند الفاتورة        | بند الفاتورة                      | المعرف الفريد العمومي لسجل المبيعات المفوترة          | فعلي                   |
| المعرف الفريد العمومي لفاتورة                 | الفاتورة                  | المعرف الفريد العمومي لسجل المبيعات المفوترة          | فعلي                            |                          |
| المعرف الفريد العلمومي لتفاصيل بند الفاتورة     | تفاصيل بند الفاتورة      | المعرف الفريد العمومي لسجل المبيعات المفوترة          | فعلي                            |                          |
| معرف GUID لسجل إدخال الوقت       | إدخال الوقت               | المعرف الفريد العمومي لسجل المبيعات المفوترة          | فعلي                            |                          |
| المعرف الفريد العمومي لسجل سطر دفتر اليومية     | سطر دفتر اليومية             | المعرف الفريد العمومي لسجل المبيعات المفوترة          | فعلي                            |                          |
| معرف GUID لسجل إدخال الوقت       | إدخال الوقت               | المعرف الفريد العمومي لإلغاء مبيعات غير مفوترة      | فعلي                            |                          |
| المعرف الفريد العمومي لسجل سطر دفتر اليومية     | سطر دفتر اليومية             | المعرف الفريد العمومي لإلغاء مبيعات غير مفوترة      | فعلي                            |                          |
| تصحيح فاتورة المسودة     | المعرف الفريد العمومي لـ ILD قديم             | حركة بند الفاتورة          | المعرف الفريد العمومي لـ ILD للتصحيح               | حركة بند الفاتورة |
| المعرف الفريد العمومي لـ IL القديم                  | بند الفاتورة             | المعرف الفريد العمومي لـ ILD للتصحيح               | حركة بند الفاتورة          |                          |
| المعرف الفريد العمومي لفاتورة قديمة             | الفاتورة                  | المعرف الفريد العمومي لـ ILD للتصحيح               | حركة بند الفاتورة          |                          |
| معرف GUID لسجل إدخال الوقت       | إدخال الوقت               | المعرف الفريد العمومي لـ ILD للتصحيح               | حركة بند الفاتورة          |                          |
| المعرف الفريد العمومي لسجل سطر دفتر اليومية     | سطر دفتر اليومية             | المعرف الفريد العمومي لـ ILD للتصحيح               | حركة بند الفاتورة          |                          |
| تصحيح فاتورة مؤكدة | المعرف الفريد العمومي لـ ILD قديم             | حركة بند الفاتورة          | المعرف الفريد العمومي لقيمة فعلية لمبيعات مفوترة ملغاة | فعلي                   |
| المعرف الفريد العمومي لـ IL القديم                  | بند الفاتورة             | المعرف الفريد العمومي لقيمة فعلية لمبيعات مفوترة ملغاة | فعلي                            |                          |
| المعرف الفريد العمومي لفاتورة قديمة             | الفاتورة                  | المعرف الفريد العمومي لقيمة فعلية لمبيعات مفوترة ملغاة | فعلي                            |                          |
| معرف GUID لسجل إدخال الوقت       | إدخال الوقت               | المعرف الفريد العمومي لقيمة فعلية لمبيعات مفوترة ملغاة | فعلي                            |                          |
| المعرف الفريد العمومي لسجل سطر دفتر اليومية     | سطر دفتر اليومية             | المعرف الفريد العمومي لقيمة فعلية لمبيعات مفوترة ملغاة | فعلي                            |                          |
| المعرف الفريد العمومي لـ ILD قديم                 | حركة بند الفاتورة | المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة    | فعلي                            |                          |
| المعرف الفريد العمومي لـ IL القديم                  | بند الفاتورة             | المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة    | فعلي                            |                          |
| المعرف الفريد العمومي لفاتورة قديمة             | الفاتورة                  | المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة    | فعلي                            |                          |
| معرف GUID لسجل إدخال الوقت       | إدخال الوقت               | المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة    | فعلي                            |                          |
| المعرف الفريد العمومي لسجل سطر دفتر اليومية     | سطر دفتر اليومية             | المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة    | فعلي                            |                          |
| المعرف الفريد العمومي لـ ILD للتصحيح          | حركة بند الفاتورة | المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة    | فعلي                            |                          |
| المعرف الفريد العمومي لـ IL تصحيحي           | بند الفاتورة             | المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة    | فعلي                            |                          |
| المعرف الفريد العمومي لتصحيح الفاتورة      | الفاتورة                  | المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة    | فعلي                            |                          |

يُظهر الجدول التالي السجلات في كيان **اتصال الحركة** لسير العمل.

| حدث                          | المعاملة 1                 | دور الحركة 1 | نوع الحركة 1           | الحركة 2                | دور الحركة 2 | نوع الحركة 2 |
|--------------------------------|-------------------------------|--------------------|------------------------------|------------------------------|--------------------|--------------------|
| إرسال إدخال الوقت          | المعرف الفريد العمومي لسطر دفتر اليومية (المبيعات)     | مبيعات غير مفوترة     | msdyn_journalline            | المعرف الفريد العمومي لسطر دفتر اليومية (التكلفة)     | تكلفة               | msdyn_journalline  |
| الموافقة على الوقت                  | المعرف الفريد العمومي للقيم الفعلية غير المفوترة (المبيعات)  | مبيعات غير مفوترة     | msdyn_actual                 | المعرف الفريد العمومي للقيمة الفعلية للتكلفة (التكلفة)       | تكلفة               | msdyn_actual       |
| إنشاء فاتورة               | المعرف الفريد العلمومي لتفاصيل بند الفاتورة      | المبيعات المفوترة       | msdyn_invoicelinetransaction | المعرف الفريد العمومي للقيم الفعلية للمبيعات غير المفوترة   | مبيعات غير مفوترة     | msdyn_actual       |
| تأكيد الفاتورة           | الفريد العمومي الفعلي للقيمة الفعلية الملغاة         | إلغاء          | msdyn_actual                 | المعرف الفريد العمومي مبيعات غير مفوترة أصلية | أصلي           | msdyn_actual       |
| المعرف الفريد العمومي للمبيعات المفوترة              | المبيعات المفوترة                  | msdyn_actual       | المعرف الفريد العمومي للقيم الفعلية للمبيعات غير المفوترة   | مبيعات غير مفوترة               | msdyn_actual       |                    |
| تصحيح فاتورة المسودة       | المعرف الفريد العمومي لحركة بند الفاتورة | استبدال          | msdyn_invoicelinetransaction | المعرف الفريد العمومي للمبيعات المفوترة            | أصلي           | msdyn_actual       |
| تأكيد تصحيح فاتورة     | المعرف الفريد العمومي لإلغاء مبيعات مفوترة    | إلغاء          | msdyn_actual                 | المعرف الفريد العمومي للمبيعات المفوترة            | أصلي           | msdyn_actual       |
| المعرف الفريد العمومي لقيمة فعلية لمبيعات غير المفوترة جديدة | استبدال                     | msdyn_actual       | المعرف الفريد العمومي للمبيعات المفوترة            | أصلي                     | msdyn_actual       |                    |


[!INCLUDE[footer-include](../includes/footer-banner.md)]