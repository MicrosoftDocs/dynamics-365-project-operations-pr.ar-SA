---
title: الأرصدة والفواتير المصححة
description: يوفر هذا الموضوع معلومات حول الفواتير المصححة في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/15/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d2187627439d42b37222dce0a491c62dafc358d5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070755"
---
# <a name="credits-and-corrected-invoices"></a>الأرصدة والفواتير المصححة

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_

يمكن تصحيح فاتورة مشروع مؤكدة لمعالجة التغييرات أو الأرصدة نتيجة التفاوض مع العميل ومدير المشروع.

لإجراء عمليات تحرير على فاتورة مؤكدة، افتح الفاتورة المؤكدة وحدد **تصحيح هذه الفاتورة**. 

> [!NOTE]
> لا يتوفر هذا التحديد ما لم يتم تأكيد فاتورة المشروع.

يتم إنشاء فاتورة مسودة جديدة من الفاتورة المؤكدة. يتم نسخ كافة تفاصيل بنود الفاتورة من الفاتورة المؤكدة في السابق إلى المسودة الجديدة. فيما يلي بعض النقاط الأساسية للتعرف على تفاصيل البنود في الفاتورة الجديدة التي تم تصحيحها:

- يتم تحديث جميع الكميات إلى صفر. يفترض التطبيق أن جميع الأصناف المفوترة مقيدة في الحساب بشكل كامل. عند الضرورة، يمكنك تحديث هذه الكميات يدويًا لتعكس الكمية التي تجري فوترتها، وليس الكمية التي يجري تقييدها في الحساب. استنادًا إلى الكمية التي تقوم بإدخالها، يحتسب التطبيق الكمية المقيدة في الحساب. ويظهر هذا المبلغ في القيم الفعلية التي يتم إنشاؤها عند تأكيد الفاتورة المصححة. إذا كنت تجري تغييرات على مبلغ الضريبة، فيجب عليك إدخال مبلغ الضريبة الصحيح وليس مبلغ الضريبة الذي يجري تقييده في الحساب.
- لا يتم نسخ شروط التعاقد التي تستند إلى المنتج والتي تم تأكيدها في السابق. لا يتم دعم معالجة التصحيحات على فاتورة مشروع تستند إلى منتج.
- تتم دائمًا معالجه تصحيحات المراحل الرئيسية كأرصدة كاملة.
- يمكن تصحيح مقدم الأتعاب أو السلفة إذا تمت فوترة العميل بمبلغ غير صحيح.
- يمكن تصحيح تسويات مقدم الأتعاب والسلف إذا تم استخدام مبلغ غير صحيح للتسوية في مقابل الرسوم في فاتورة مؤكدة سابقًا.

> [!IMPORTANT]
> تم تعيين حقل **التصحيح** إلى **نعم** في تفاصيل بنود الفواتير التي تعتبر تصحيحات لرسوم تمت فوترها في السابق. تتضمن الفواتير ذات تفاصيل بنود فواتير مصححة حقلاً يسمى **لديه تصحيحات** معينًا أيضًا إلى **نعم**.

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a>القيم الفعلية التي تم إنشاؤها عند تأكيد فاتورة تصحيحية:

فيما يلي القيم الفعلية التي تم إنشاؤها بواسطة التطبيق عند تأكيد فاتورة تصحيحية استنادًا إلى العمليات التي تم تنفيذها على مسودة الفاتورة التصحيحية قبل التأكيد.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p>
                    <strong>السيناريو</strong>
                </p>
            </td>
            <td width="808" valign="top">
                <p>
                    <strong>القيم الفعلية المنشأة عند التأكيد</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
تأكيد تصحيح سلفة أو مقدم أتعاب مفوترة.<strong></strong>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات غير مفوترة لمقدم الأتعاب أو السلفة التي تم إنشاؤها للتسوية. يكون هذا المبلغ موجبًا لأنه معد لإلغاء المبلغ السالب الذي تم إنشاؤه عند فوترة السلف أو مقدم الأتعاب.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
يتم إنشاء قيمة فعلية لإلغاء المبيعات المفوترة للمبلغ على السلفة أو مقدم الأتعاب لإلغاء المبيعات الأصلية المفوترة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
يتم إنشاء قيمة فعلية جديدة للمبيعات المفوترة للمبلغ المصحح على مقدم الأتعاب أو بنود الفاتورة المصححة القائمة على السلفة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية للمبيعات غير المفوترة للمبلغ السالب لمقدم الأتعاب أو بنود الفاتورة المصححة القائمة على السلفة، التي سيتم استخدامها للتسوية.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
تأكيد تصحيح سلفة أو مقدم أتعاب تمت تسويته في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات غير مفوترة لمقدم الأتعاب أو السلفة التي تم إنشاؤها للتسوية. يكون هذا المبلغ موجبًا وهو معد لإلغاء المبلغ السالب الذي تم إنشاؤه عند حدوث التسوية السابقة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
القيمة الفعلية لإلغاء مبيعات مفوترة للمبلغ على الفاتورة السابقة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات المفوترة للمبلغ المصحح على مقدم الأتعاب المطبق على الفاتورة المصححة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية للمبيعات غير المفوترة مع مبلغ سالب من السلفة أو مقدم الأتعاب المتبقية والمصححة، التي سيتم استخدامها للتسوية على الفواتير اللاحقة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
فوترة الرصيد الكامل لحركة وقت تمت فوترتها في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات مفوترة للساعات والمبلغ في تفاصيل بند الفاتورة الأصلية للوقت.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات غير المفوترة للساعات والمبلغ في تفاصيل بند الفاتورة الأصلية للوقت.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
فوترة الرصيد الجزئي على حركة الوقت.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات مفوترة للساعات والمبلغ المفوترة على تفاصيل بند الفاتورة الأصلية للوقت.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الساعات والمبلغ على تفاصيل بنود الفاتورة المعدلة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والساعات المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
فوترة الرصيد الكامل لحركة مصروفات تمت فوترتها في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات غير المفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
فوترة الرصيد الجزئي لحركة مصروفات تمت فوترتها في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للمصروفات.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة المصححة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم المبلغ والكمية المتبقية بعد خصم الأرقام المصححة على تفاصيل بنود الفاتورة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
فوترة الرصيد الكامل لحركة رسوم تمت فوترتها في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات مفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للرسوم.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات غير المفوترة للكمية والمبلغ على تفاصيل بند الفاتورة الأصلية للرسوم.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
فوترة الرصيد الجزئي لحركة رسوم تمت فوترتها في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات مفوترة للكمية والمبلغ المفوتر على تفاصيل بند الفاتورة الأصلية للرسوم.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
قيمة فعلية جديدة للمبيعات غير المفوترة تخضع لرسوم الكمية والمبلغ على تفاصيل بنود الفاتورة التصحيحية المعدلة، وإلغاء لها، وقيمة فعلية مكافئة للمبيعات المفوترة.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
فوترة الرصيد الكامل لمرحلة رئيسية تمت فوترتها في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
إلغاء مبيعات مفوترة للمبلغ في تفاصيل بند الفاتورة الأصلية للمرحلة الرئيسية.
                </p>
                <p>
يتم تحديث فاتورة المرحلة الرئيسية أو حالة الفوترة على شروط تعاقد المشروع إلى **جاهزة للفوترة**.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
فوترة الرصيد الجزئي لمرحلة رئيسية تمت فوترتها في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
غير مدعوم </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
الأرصدة والتصحيحات لشروط تعاقد مستندة إلى مشروع تمت فوترتها في وقت سابق.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
غير مدعوم </p>
            </td>
        </tr>
    </tbody>
</table>