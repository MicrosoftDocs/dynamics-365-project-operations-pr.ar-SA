---
title: سطور فاتورة البائع للمنتجات
description: يشرح هذا المقال كيفية تسجيل بنود فاتورة المورّد للمنتجات واستخدام الحقول المختلفة لتسجيل مشتريات المنتجات من المورّدين.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: d38a447c576c095a7bbe2f5ed84342a88bf69a9b
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261542"
---
# <a name="vendor-invoice-lines-for-products"></a>سطور فاتورة البائع للمنتجات

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_

يمكن أن تحتوي فاتورة المورد في Microsoft Dynamics 365 Project Operations على بنود فاتورة المورّد للمنتجات (يُشار إليها أيضًا بالمواد). يمكن لمديري المشاريع استخدام بنود فاتورة المورّد للمنتجات لتسجيل تكاليف المنتجات التي تم شراؤها في المشاريع.

قد تشير أو لا تشير بنود فاتورة المورّد للمنتجات إلى شروط التعاقد من الباطن للمواد. إذا كان بند فاتورة المورّد للمنتجات يشير إلى عقد من الباطن، فسيكون مديرو المشروع قادرين على مطابقة المنتجات التي يتم تحرير فواتير بها بواسطة بند فاتورة المورّد والتحقق منها مقابل استخدام المنتجات المشتراة التي تم تسجيلها والتي تمت الموافقة عليها من قبل مديري المشروع.

يوفر الجدول التالي معلومات حول الحقول الموجودة في شروط فاتورة المورد للمنتجات.

| الحقل | الوصف  | التأثير الوظيفي |
| --- | --- | --- |
| Name | اسم بند فاتورة المورّد، للمساعدة في تحديد الهوية. | سيظهر هذا الاسم كأول عمود في كل عمليات البحث التي تستند إلى بنود فاتورة المورّد. |
| الوصف  | وصف مختصر للمنتجات التي يتم فوترتها بواسطة المورد في سطر فاتورة المورّد. | ‏‫بلا |
| العقد من الباطن | العقد من الباطن الذي تم طلب المنتجات فيه في الأصل. | عند تحديد عقد من الباطن لفاتورة المورّد، فإن جميع البنود الموجودة في فاتورة المورد ترث هذا التحديد. لا يمكن أن تحتوي فاتورة المورّد على بنود فاتورة المورد التي تشير إلى عقود من الباطن مختلفة. |
| شروط التعاقد من الباطن | شروط التعاقد من الباطن الذي تم طلب المنتجات فيه. تقتصر قائمة بنود التعاقد من الباطن التي يمكن تحديدها على البنود الموجودة في التعاقد من الباطن المحدد. | عند تحديد بند تعاقد من الباطن في بند فاتورة المورد للمنتجات، فإنه يتم إدخال القيم الافتراضية للحقول **المشروع**، **المهمة** و **المنتج** من الحقول المقابلة في شرط التعاقد من الباطن. وإذا كان شرط التعاقد من الباطن المحدد يتضمن قيم في الحقول **المشروع**، **المهمة** و **المنتج**، فلا يمكن أن تختلف قيم الحقول المقابلة في بند فاتورة المورد عن هذه القيم. |
| تاريخ الحركة | التاريخ الذي سيتم فيه تسجيل التكلفة الفعلية لبند فاتورة المورّد في المشروع. | ‏‫بلا|
| فئة الحركة | عند فوترة المنتجات، ينبغي تعيين هذا الحقل إلى **المواد**. | تشير القيمة **المواد** إلى أنه يتم استخدام بند فاتورة المورد لتسجيل مبلغ الفاتورة للمواد التي تم شراؤها. |
| Project | اسم المشروع الذي تم استخدام المنتجات قيد الفواتير عليه. | هذا الحقل مطلوب ولا يمكن تركه فارغًا. |
| المهمة | اسم مهمة المشروع الذي تم استخدام المنتجات قيد الفواتير عليه. هذا الحقل متاح فقط إذا تم تحديد المشروع. يُعد اختيار مهمة مشروع أمرًا اختياريًا. | إذا تم ترك هذا الحقل فارغًا، فيمكن لمدير المشروع مطابقة بند فاتورة المورد مع المنتج الذي تم شراؤه والمُستخدم في أي مهمة من مهام المشروع. إذا كان بند فاتورة المورد لا يشير إلى شروط التعاقد من الباطن، وتم ترك هذا الحقل فارغًا، فلن يتم ربط التكلفة الفعلية التي تم إنشاؤها بواسطة بند فاتورة المورّد بأي قيم فعلية للمبيعات غير مفوترة. في هذه الحالة، إذا تم إعداد الفوترة المستندة إلى المهام، فلن تتم فوترة التكاليف إلى العميل النهائي. |
| منتج محدد | حدد ما إذا كان المنتج الذي تتم فوترته هو منتج موجود من الكتالوج أو منتج مدرج. | يتم إدخال القيمة الافتراضية من شروط التعاقد من الباطن عند تحديد شرط تعاقد من الباطن. |
| المنتج  | حدد المنتج من الكتالوج. إذا كان المنتج عبارة عن منتج مكتوب، أدخل اسم المنتج. | يستخدم هذا الحقل لإدخال أسعار الشراء الافتراضية للمنتجات الحالية. |
| الكمية | أدخل كمية المواد التي يتم تحرير فاتورة بها بواسطة المورد في بند الفاتورة هذا. | ‏‫بلا |
| مجموعة الوحدات | حدد مجموعة الوحدات للوحدة التي يتم التعبير عن الكمية التي يتم تحرير فواتير بها. | ‏‫بلا |
| الوحدة | القيمة الافتراضية هي الوحدة الأساسية لمجموعة الوحدات المحددة. يمكنك تغيير هذه القيمة للدفع في أي وحدة من مجموعة الوحدات المختارة. | سيتم استخدام مجموعة قيم **المنتج** و **الوحدة** كقيمة افتراضية أو محسوبة لحقل **سعر الوحدة** في بند فاتورة المورد. |
| سعر الوحدة | يستخدم سعر الوحدة الافتراضي مجموعة قيم **المنتج** و **الوحدة** من قائمة أسعار المشروع القابلة للتطبيق على تاريخ معاملة بند فاتورة المورد. | ‏‫بلا |
| المجموع الفرعي | يتم حساب هذا الحقل للقراءة فقط على أنه *الكمية* &times; *سعر الوحدة*، إذا تم إدخال القيم في حقل **الكمية** وحقل **سعر الوحدة**. إذا كان أحد هذين الحقلين فارغًا، فيمكنك إدخال قيمة في هذا الحقل. | ‏‫بلا |
| ضريبة المبيعات | أدخل مبلغ ضريبة المبيعات. | ‏‫بلا |
| المبلغ الإجمالي | المبلغ الإجمالي لبند فاتورة المورّد، بما في ذلك الضرائب. يتم حساب هذا الحقل كـ *الإجمالي الفرعي* + *الضريبة على المبيعات*. | ‏‫بلا |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]