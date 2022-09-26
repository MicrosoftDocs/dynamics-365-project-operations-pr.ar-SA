---
title: سطور فاتورة البائع للمراحل الرئيسية
description: يشرح هذا المال كيفية إنشاء بنود فاتورة المورّد للمراحل الرئيسية في عقد من الباطن.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: f066c2ac7377a989a92a9ae2e9a732d3c979a0db
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2022
ms.locfileid: "9260979"
---
# <a name="vendor-invoice-lines-for-milestones"></a>سطور فاتورة البائع للمراحل الرئيسية

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_

قد تتضمن فاتورة المورد في Microsoft Dynamics 365 Project Operations سطور فاتورة المورد للأحداث الرئيسية المحددة في شرط التعاقد من الباطن. يمكن لمديري المشاريع استخدام سطور فاتورة البائع للمراحل الرئيسية لتسجيل تكاليف الخدمات التي تم شراؤها كتكاليف تستند إلى الأحداث الرئيسية التي يتم تكبدها على الخدمات أو المنتجات التي تم شراؤها للمشروع.

يجب أن تشير سطور فاتورة المورد للأحداث الرئيسية دائمًا إلى شرط تعاقد من الباطن يحتوي على طريقة فوترة بسعر ثابت. عندما يشير سطر فاتورة المورد للأحداث الرئيسية إلى شرط تعاقد من الباطن، سيتمكن مديرو المشاريع من مطابقة التكاليف الأساسية للوقت أو المصروفات أو المواد التي تشير إلى شرط التعاقد من الباطن هذا والتحقق منها مقابل الحدث الرئيسي الذي يقوم المورّد بإصدار فواتير له.

يوفر الجدول التالي معلومات حول الحقول الموجودة في شروط فاتورة المورد للأحداث الرئيسية.

| الحقل | الوصف  | التأثير الوظيفي |
| --- | --- | --- |
| Name | اسم بند فاتورة المورّد، للمساعدة في تحديد الهوية. | سيظهر هذا الاسم كأول عمود في كل عمليات البحث التي تستند إلى بنود فاتورة المورّد. |
| الوصف  | وصف مختصر للخدمات التي يتم فوترتها بواسطة المورد في سطر فاتورة المورّد. | ‏‫بلا |
| العقد من الباطن | العقد من الباطن الذي تم طلب الخدمات فيه في الأصل. | عند تحديد عقد من الباطن لفاتورة المورّد، فإن جميع البنود الموجودة في فاتورة المورد ترث هذا التحديد. لا يمكن أن تحتوي فاتورة المورّد على بنود فاتورة المورد التي تشير إلى عقود من الباطن مختلفة. |
| شروط التعاقد من الباطن | شروط التعاقد من الباطن الذي تم طلب الخدمات فيه. تقتصر قائمة بنود التعاقد من الباطن التي يمكن تحديدها على البنود الموجودة في التعاقد من الباطن المحدد. | عندما يتم تحديد بشرط التعاقد من الباطن في سطر فاتورة المورد للأحداث الرئيسية، فإن الحقول **الدور** و **فئة المعاملة** والحقول ذات الصلة بالمنتج تكون غير ذات صلة وغير متاحة. كما أن حقول **الكمية** و **الوحدة** و **مجموعة الوحدة** ليست ذات صلة بسطور فاتورة المورد المستندة إلى الأحداث الرئيسية. |
| تاريخ الحركة | التاريخ الذي سيتم فيه تسجيل التكلفة الفعلية لبند فاتورة المورّد في المشروع. | ‏‫بلا |
| فئة الحركة | حدد **الحدث الرئيسي** لتسجيل فاتورة مورد لحدث رئيسي مكتمل تم تحديده على شرط تعاقد من الباطن. | ‏‫بلا |
| الأحداث الرئيسية | حدد الحدث الرئيسي الذي تم تحديده في شرط التعاقد من الباطن ذي الصلة الذي تم وضع علامة عليه كـ **جاهز للفوترة**. | يمكن تحديد الأحداث الرئيسية لشرط التعاقد من الباطن التي لها حالة **جاهزة للفوترة** في بند فاتورة المورد. |
| Project | اسم المشروع الذي تم استخدام الخدمات قيد الفواتير عليه. | هذا الحقل مطلوب ولا يمكن تركه فارغًا. |
| المهمة | اسم مهمة المشروع الذي تم استخدام الخدمات قيد الفواتير عليه. هذا الحقل متاح فقط إذا تم تحديد المشروع. يُعد اختيار مهمة مشروع أمرًا اختياريًا. | إذا تم ترك هذا الحقل فارغًا، فيمكن لمدير المشروع مطابقة سطر فاتورة المورد مع فئة المعاملات في شرط التعاقد من الباطن ذي الصلة الذي تم تسجيله في أي مهمة من مهام المشروع. إذا كان بند فاتورة المورد لا يشير إلى شروط التعاقد من الباطن، وتم ترك هذا الحقل فارغًا، فلن يتم ربط التكلفة الفعلية التي تم إنشاؤها بواسطة بند فاتورة المورّد بأي قيم فعلية للمبيعات غير مفوترة. في هذه الحالة، إذا تم إعداد الفوترة المستندة إلى المهام، فقد لا تتم فوترة التكاليف إلى العميل النهائي. |
| مبلغ المرحلة الرئيسية | أدخل قيمة الحدث الرئيسي المحدد في شرط التعاقد من الباطن الجاهز للفوترة. | ‏‫بلا |
| ضريبة المبيعات | أدخل مبلغ ضريبة المبيعات. | ‏‫بلا |
| المبلغ الإجمالي | المبلغ الإجمالي لبند فاتورة المورّد، بما في ذلك الضرائب. يتم حساب هذا الحقل كـ *مبلغ الحدث الرئيسي* + *ضريبة المبيعات*. | ‏‫بلا |

> [!NOTE]
> عند إنشاء سطر فاتورة المورد يشير إلى حدث رئيسي لشرط التعاقد من الباطن، يتم تحديث حالة الحدث الرئيسي للتعاقد من الباطن إلى **تم إنشاء فاتورة العميل**. وبعد ذلك، عند تأكيد فاتورة المورد هذه، يتم تحديث حالة الحدث الرئيسي لشرط التعاقد من الباطن إلى **تم تأكيد فاتورة المورد**.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]