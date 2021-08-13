---
title: نظرة عامة على بنود عرض الأسعار القائم على المشروع
description: يقدم هذا الموضوع معلومات حول استخدام بنود عروض الأسعار المستندة إلى المشروع لعمل المشروع.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 2f2d38c7fb3bc3ec26cf64525ef8275adecafd7fc48e97d6daef595d341c045d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "7001550"
---
# <a name="project-based-quote-lines-overview"></a>نظرة عامة على بنود عرض الأسعار القائم على المشروع 

_**ينطبق على:** نشر خفيف - التعامل مع الفواتير الأولية‬، Project Operations لسيناريوهات الموارد/المنتجات غير المخزنة_

تم تصميم بنود عرض الأسعار المستندة إلى المشروع للمساعدة في تقدير عمل المشروع بأحد المشاركات. يتم توسيع بنية سطر عرض الأسعار المستند إلى المشروع لتقديرات المشروع بالمفاهيم التالية:

- أسلوب الفوترة
- تعيين المشروع والمهمة
- فئات الحركات المضمنة
- حد يجب عدم تجاوزه
- إعداد الخضوع للرسوم
- التقدير باستخدام تفاصيل بند عرض الأسعار
- عملاء بند عرض الأسعار

يوفر الجدول التالي معلومات حول الحقول الموجودة في علامة التبويب **عام** في بند عرض الأسعار المستند إلى المشروع. وتساعد هذه الحقول في إعداد الأساس لتقدير تفصيلي من القاعدة إلى القمة لعمل المشروع.

| **الحقل** | **الوصف** | **تأثير لاحق** |
| --- | --- | --- |
| الاسم  | اسم بند عرض الأسعار الذي يساعدك في تحديد المكون المنفصل لعرض الأسعار الجاري تقديره. | يتم نسخه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| أسلوب الفوترة | في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل المقابل في بند الفرصة. يتضمن هذا الحقل نموذجين أساسيين للتعاقد يدعمهما Dynamics 365 Project Operations:</br>- سعر ثابت</br>- الوقت والمادة.| يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| Project | استخدم هذا الحقل الاختياري لتحديد المشروع الذي سيتم استخدامه لتسليم العمل في هذه المشاركة. عندما يتم تعيين مشروع إلى بند عرض الأسعار، فإنه يساعد في إعداد المهام الخاضعة للرسوم وكذلك يساعد في إحضار التقديرات المستندة إلى المشروع لبند عرض الأسعار كتفاصيل بند عرض الأسعار. عند عدم تعيين مشروع لبند عرض أسعار يستند إلى مشروع، يتعين إنشاء التقدير يدويًا عن طريق إنشاء كل تفاصيل بند عرض الأسعار. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار.|
| المهام المضمنة | يشير إلى ما إذا كان يتم استخدام بند عرض الأسعار لكافة مهام المشروع أو بعضها للمشروع المحدد. يحتوي هذا الحقل على القيم الممكنة التالية:</br>- كل مهام المشروع</br>- مهام المشروع المحددة فقط</br>القيمة الفارغة في هذا الحقل تكافئ خيار **كافة مهام المشروع**. | عند تحديد الخيار **مهام المشروع المحددة فقط‬** على صفحة المشروع، تسمح لك علامة التبويب **إعداد فوترة المهام** تحديد مهام معينة لربطها ببند عرض الأسعار هذا. يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| تضمين الوقت | تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين حركات الوقت أو تكاليف العمالة على المشروع المحدد في التقدير على بند عرض الأسعار هذا. تشير علامة **لا** إلى أن حركات الوقت أو تكلفة العمالة لن يتم تضمينها في التقدير لبند عرض الأسعار هذا. تشير علامة **نعم** إلى أن حركات الوقت أو تكلفة العمالة سيتم تضمينها في التقدير لبند عرض الأسعار هذا. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| يتضمن المصروفات | تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين تكاليف المصروفات على المشروع المحدد في التقدير على بند عرض الأسعار هذا. تشير علامة **لا** إلى أن تكلفة المصروفات لن يتم تضمينها في التقدير لبند عرض الأسعار هذا. تشير علامة **نعم** إلى أن تكلفة المصروفات سيتم تضمينها في التقدير لبند عرض الأسعار هذا. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| تضمين المواد | تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين تكاليف المواد على المشروع المحدد في التقدير على بند عرض الأسعار هذا. تشير القيمة **نعم** إلى أنه لن يتم تضمين تكاليف المواد في التقدير على بند عرض الأسعار هذا. تشير القيمة **نعم** إلى أنه سيتم تضمين تكاليف المواد في التقدير على بند عرض الأسعار هذا. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| تضمين الرسوم | تشير القيمة **نعم**/**لا** إلى ما إذا كان سيتم تضمين الرسوم على المشروع المحدد في التقدير على بند عرض الأسعار هذا. تشير القيمة **لا** إلى أنه لن يتم تضمين الرسوم في التقدير لبند عرض الأسعار هذا. تشير القيمة **نعم** إلى أنه سيتم تضمين الرسوم في التقدير لبند عرض الأسعار هذا. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| المبلغ المعروض | هذا هو المبلغ الذي سيتم إدراجه في عرض الأسعار للعميل لكل العمل المتوقع في شرط التعاقد القائم على هذا المشروع. في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل **ميزانية العميل** في بند الفرصة. عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من المبلغ الموجود في تفاصيل بند عرض الأسعار. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| الضريبة المقدرة | هذا حقل قابل للتحرير لكي يقوم المستخدم بإضافة مبلغ الضريبة المقدرة في بند عرض الأسعار. عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من مبلغ الضريبة الموجود في تفاصيل بند عرض الأسعار. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| ‏‫المبلغ المعروض‬ بعد الضريبة | هذا الحقل هو مبلغ بند عرض الأسعار بعد الضريبة وهو للقراءة فقط. يتم حساب المبلغ الموجود في هذا الحقل *كمبلغ معروض + الضريبة*. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| حد ما يجب ألا يتم تجاوزه | ويكون هذا الحقل قابلا للتحرير ويكون متاحا فقط في بنود عروض الأسعار المستندة إلى المشروع والتي لها أسلوب فوترة **الوقت والمادة**. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |
| موازنة العميل | يكون هذا الحقل قابلا للتحرير ويتم نسخه من الحقل المقابل في بند الفرصة إذا تم إنشاء عرض الأسعار من إحدى الفرص. | يتم نسخ هذه القيمة إلى شرط تعاقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عند فوز عرض الأسعار. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>قواعد التحقق من الصحة للحقول في علامة التبويب عام لبنود عرض الأسعار المستندة إلى المشروع

**القاعدة 1**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه على **جميع مهام المشروع**، فسيتم تضمين المشروع في بند عرض الأسعار.

**القاعدة 2**: إذا كان حقل **المهام المضمنة** فارغًا، أو إذا تم تعيينه إلى **كافة مهام المشروع**، فيمكن تضمين مشروع وفئة حركة معينة فقط في بند عرض أسعار واحد يستند إلى مشروع في عرض الأسعار.

**القاعدة 3**: إذا تم تعيين حقل **المهام المضمنة** إلى **مهام المشروع المحددة فقط**، فيمكن تضمين مشروع وفئة حركة معينة فقط في عدة بنود عرض أسعار يستند إلى مشروع في عرض الأسعار.

**القاعدة 4**: إذا كانت الفرصة تحتوي على عدة عروض أسعار، فيمكن أن يكون هناك بنود عرض أسعار مختلفة والتي تشير إلى نفس المشروع وتتضمن نفس فئة الحركات.

**القاعدة 5**: إذا لم تكن عروض الأسعار تنتمي إلى نفس الفرصة، فلا يمكن أن تتضمن نفس فئة المشروع والحركات.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p>
                    <strong>الفرصة</strong>
                </p>
            </td>
            <td width="39" valign="top">
                <p>
                    <strong>اقتباس</strong>
                </p>
            </td>
            <td width="40" valign="top">
                <p>
                    <strong>بند عرض الأسعار</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="77" valign="top">
                <p>
                    <strong>المهام المضمنة</strong>
                </p>
            </td>
            <td width="45" valign="top">
                <p>
                    <strong>تضمين الوقت</strong>
                </p>
            </td>
            <td width="46" valign="top">
                <p>
                    <strong>يتضمن المصروفات</strong>
                </p>
            </td>
            <td width="43" valign="top">
                <p>
                    <strong>تضمين المواد</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>تضمين</strong>
                </p>
                <p>
                    <strong>رسوم</strong>
                </p>
            </td>
            <td width="49" valign="top">
                <p>
                    <strong>صالح/غير صالح</strong>
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    <strong>سبب</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
فارغ </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
غير صالح </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
انتهاك القاعدة #2. يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في بنود عرض الأسعار QL1 وQL2. </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
فارغ </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
فارغ </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
لا  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
غير صالح </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
انتهاك القاعدة #2. يتم تضمين الوقت والمواد والرسوم في المشروع P1 في بنود عرض الأسعار QL1 وQL2. </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
فارغ </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
فارغ </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
لا  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
صالح </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
يتم تضمين الوقت والمواد والرسوم في المشروع P1 على QL1 <br>
يتم تضمين المصروفات في المشروع P1 في QL2. <br>
لا يوجد تداخل في ما يتم تضمينه في كل بند عرض أسعار وهو بالتالي صالح.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
فارغ </p>
            </td>
            <td width="45" valign="top">
                <p>
لا  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
لا  </p>
            </td>
            <td width="41" valign="top">
                <p>
لا  </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
المهام المحددة فقط </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
غير صالح </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
انتهاك القاعدة رقم 2 </p>
                <p>
يتضمن Q1 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1 </p>
                <p>
يتضمن QL2 الوقت والمصروفات والرسوم لمشروع P1 بكامله وبالتالي يتداخل مع ما يتضمنه Q1.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
فارغ </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
المهام المحددة فقط </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
صالح </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
حسب القاعدة 3 </p>
                <p>
يتضمن Q1 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1.
                </p>
                <p>
يتضمن QL2 الوقت والمواد والمصروفات والرسوم في مجموعة فرعية من المهام في المشروع P1.
                </p>
                <p>
التحقق الإضافي الوحيد هو حول المجموعة الفرعية من المهام على QL1 التي تختلف عن المجموعة الفرعية للمهام في QL2 لضمان عدم وجود تداخل. يتم ذلك بواسطة النظام عند اقتران المهام.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
المهام المحددة فقط </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
كافة مهام المشروع أو فارغة </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
صالح </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
بحسب القاعدة 5، Q1 وQ2 عبارة عن عرضي أسعار في نفس الفرصة، وبالتالي يقدران المكونات نفسها لمشروع
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الثاني </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
كافة مهام المشروع أو فارغة </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
كافة مهام المشروع أو فارغة </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
غير صالح </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
بحسب القاعدة 4، Q1 وQ2 عبارة عن عرضي أسعار في فرص مختلفة، وبالتالي لا يمكنهما تقدير المكونات نفسها للمشروع نفسه.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O2 </p>
            </td>
            <td width="39" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
كافة مهام المشروع أو فارغة </p>
            </td>
            <td width="45" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="46" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="43" valign="top">
                <p>
نعم  </p>
            </td>
            <td width="41" valign="top">
                <p>
نعم  </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
