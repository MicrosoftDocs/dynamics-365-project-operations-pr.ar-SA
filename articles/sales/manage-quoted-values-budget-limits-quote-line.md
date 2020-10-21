---
title: بنود عروض الأسعار المستندة إلى المشروع
description: يقدم هذا الموضوع معلومات حول استخدام بنود عروض الأسعار المستندة إلى المشروع لعمل المشروع.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 06a47c45dc3b3b174658e2fba14d3d2050aabf85
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906051"
---
# <a name="project-based-quote-lines"></a>بنود عروض الأسعار المستندة إلى المشروع

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

تم تصميم بنود عرض الأسعار المستندة إلى المشروع للمساعدة في تقدير عمل المشروع بأحد المشاركات. يتم توسيع بنية سطر عرض الأسعار المستند إلى المشروع لتقديرات المشروع بالمفاهيم التالية:

- أسلوب الفوترة
- تعيين المشروع
- فئات الحركات المضمنة
- حد يجب عدم تجاوزه
- إعداد الخضوع للرسوم
- التقدير باستخدام تفاصيل بند عرض الأسعار
- عملاء بند عرض الأسعار

يوفر الجدول التالي معلومات حول الحقول الموجودة في علامة التبويب **عام** في بند عرض الأسعار المستند إلى المشروع. وتساعد هذه الحقول في إعداد الأساس لتقدير تفصيلي من القاعدة إلى القمة لعمل المشروع.

| **الحقل** | **الصلة والغرض والإرشاد** | **تأثير لاحق** |
| --- | --- | --- |
| اسم | اسم بند عرض الأسعار الذي ينبغي أن يساعدك في تحديد المكون المنفصل لعرض الأسعار الذي يتم تقديره. | يتم نسخه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| أسلوب الفوترة | في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل المقابل في بند الفرصة. يتضمن هذا الحقل اثنين من نماذج التعاقد الرئيسية المدعومة من Dynamics 365 Project Operations:</br>- سعر ثابت</br>- الوقت والمادة.| يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| Project | استخدم هذا الحقل الاختياري لتحديد المشروع الذي سيتم استخدامه لتسليم العمل في هذه المشاركة. عندما يتم تعيين مشروع إلى بند عرض الأسعار، فإنه يساعد في إعداد المهام الخاضعة للرسوم وكذلك يساعد في إحضار التقديرات المستندة إلى المشروع لبند عرض الأسعار كتفاصيل بند عرض الأسعار. عند عدم تعيين مشروع لبند عرض أسعار يستند إلى مشروع، يتعين إنشاء التقدير يدويًا عن طريق إنشاء كل تفاصيل بند عرض الأسعار. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| تضمين الوقت | تشير علامة **نعم**/**لا** إلى ما إذا كان حركات الوقت أو تكاليف العمالة في المشروع المحدد مضمنة في التقدير لبند عرض الأسعار هذا أم لا. تشير علامة **لا** إلى أن حركات الوقت أو تكلفة العمالة لن يتم تضمينها في التقدير لبند عرض الأسعار هذا. تشير علامة **نعم** إلى أن حركات الوقت أو تكلفة العمالة سيتم تضمينها في التقدير لبند عرض الأسعار هذا. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| يتضمن المصروفات | تشير علامة **نعم**/**لا** إلى ما إذا كانت تكاليف المصروفات في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا. تشير علامة **لا** إلى أن تكلفة المصروفات لن يتم تضمينها في التقدير لبند عرض الأسعار هذا. تشير علامة **نعم** إلى أن تكلفة المصروفات سيتم تضمينها في التقدير لبند عرض الأسعار هذا. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| تضمين الرسوم | تشير علامة **نعم**/**لا** إلى ما إذا كانت الرسوم في المشروع المحدد سيتم تضمينها في التقدير لبند عرض الأسعار هذا أم لا. تشير علامة **لا** إلى أن الرسوم لن يتم تضمينها في التقدير لبند عرض الأسعار هذا. تشير علامة **نعم** إلى أن الرسوم سيتم تضمينها في التقدير لبند عرض الأسعار هذا. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| المبلغ المعروض | هذا هو المبلغ الذي سيتم وضعه في التسعير للعميل لكل العمل المتوقع في بند عرض الأسعار المستند إلى المشروع هذا. في عرض الأسعار الذي تم إنشاؤه من أحدي الفرص، يتم نسخ هذه القيمة من الحقل **ميزانية العميل** في بند الفرصة. عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من المبلغ الموجود في تفاصيل بند عرض الأسعار. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| الضريبة المقدرة | هذا حقل قابل للتحرير لكي يقوم المستخدم بإضافة مبلغ الضريبة المقدرة في بند عرض الأسعار. عندما يحتوي بند عرض الأسعار المستند إلى المشروع على تفاصيل البند، يكون هذا الحقل مؤمنًا للتحرير ويتم تلخيصه من مبلغ الضريبة الموجود في تفاصيل بند عرض الأسعار. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| ‏‫المبلغ المعروض‬ بعد الضريبة | هذا الحقل هو مبلغ بند عرض الأسعار بعد الضريبة وهو للقراءة فقط. يتم حساب المبلغ الموجود في هذا الحقل *كمبلغ معروض + الضريبة*. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| حد ما يجب ألا يتم تجاوزه | ويكون هذا الحقل قابلا للتحرير ويكون متاحا فقط في بنود عروض الأسعار المستندة إلى المشروع والتي لها أسلوب فوترة **الوقت والمادة**. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |
| موازنة العميل | يكون هذا الحقل قابلا للتحرير ويتم نسخه من الحقل المقابل في بند الفرصة إذا تم إنشاء عرض الأسعار من إحدى الفرص. | يتم نسخ قيمة الحقل هذه إلى بند عقد المشروع الذي تم إنشاؤه من بند عرض الأسعار هذا عندما يتم ربح عرض الأسعار. |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>قواعد التحقق من الصحة للحقول في علامة التبويب عام لبنود عرض الأسعار المستندة إلى المشروع

**القاعدة 1**: يمكن فقط تضمين فئة حركات معينة في المشروع المحدد في بند عرض أسعار واحد يستند إلى مشروع في عرض الأسعار.

**القاعدة 2**: إذا كانت الفرصة تحتوي على عدة عروض أسعار، فيمكن أن يكون هناك بنود عرض أسعار مختلفة والتي تشير إلى نفس المشروع وتتضمن نفس فئة الحركات.

**القاعدة 3**: إذا لم تكن عروض الأسعار تنتمي إلى نفس الفرصة، فلا يمكن أن تتضمن نفس فئة المشروع والحركات.

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p>
                    <strong>الفرصة</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>اقتباس</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>بند عرض الأسعار</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>تضمين الوقت</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>تضمين المصروفات</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>تضمين</strong>
                </p>
                <p>
                    <strong>الرسوم</strong>
                </p>
            </td>
            <td width="54" valign="top">
                <p>
                    <strong>صالح/غير صالح</strong>
                </p>
            </td>
            <td width="308" valign="top">
                <p>
                    <strong>سبب</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
غير صالح </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
انتهاك القاعدة #1. يتم تضمين الوقت والمصروفات والرسوم في المشروع P1 في كل من بنود عرض الأسعار وQL1 و QL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
غير صالح </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
انتهاك القاعدة #1. يتم تضمين الوقت والرسوم في المشروع P1 في كل من بنود عرض الأسعار وQL1 و QL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
صالح </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
يتم تضمين الوقت والرسوم على المشروع P1 في QL1.
يتم تضمين المصروفات في المشروع P1 في QL2.
لا يكون هناك تداخل في ما يتم تضمينه في كل بند عرض الأسعار لذا يكون صالحًا.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
غير صالح </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
انتهاك القاعدة #1 السابقة </p>
                <p>
يتضمن Q1 الوقت والمصروفات والرسوم للمشروع P1 بالكامل.
                </p>
                <p>
يتضمن QL2 الوقت والمصروفات والرسوم للمشروع P1 بالكامل ويتداخل مع ما تم تضمينه في Q1.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="54" valign="top">
                <p>
صالح </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
بناء على القاعد #2، فإن Q1 و Q2 يمثلان عرضا أسعار في نفس الفرصة، لذا يمكنهم التقدير لنفس المكونات الخاصة بأحد المشروعات.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الثاني </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 في Q2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="54" valign="top">
                <p>
صالح </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
بناء على القاعد #3، فإن Q1 و Q2 يمثلان عرضا أسعار لفرص مختلفة، لذا لا يمكنهم التقدير لنفس المكونات الخاصة بنفس المشروع.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O2 </p>
            </td>
            <td width="41" valign="top">
                <p>
ربع السنة الأول </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏نعم </p>
            </td>
            <td width="54" valign="top">
                <p>
غير صالح </p>
            </td>
        </tr>
    </tbody>
</table>

