---
title: إدارة عدة عملاء على بنود عرض أسعار قائم على المنتج
description: يقدم هذا الموضوع معلومات عن كيفية إدارة عدة عملاء على بنود عرض أسعار قائم على المنتج.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ea7f0a8207fc78914783f5b9c919b3243a0bb5a4
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070520"
---
# <a name="manage-multiple-customers-on-project-based-quote-lines"></a>إدارة عدة عملاء على بنود عرض أسعار قائم على المنتج

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

تدعم بنود عرض الأسعار القائم على المشروع سيناريوهات حيث يحتوي كل بند عرض أسعار على قائمة عملاء يدفعون له. قد تكون قائمة العملاء في بند عرض الأسعار القائم على المشروع هي نفسها قائمة العملاء في عرض الأسعار. يمكنك أيضًا تغيير قائمة العملاء لتكون مختلفة. لإنشاء عقد المشروع النهائي عندما يتم الفوز بعرض أسعار المشروع، يتم نسخ قائمة العملاء على بند عرض الأسعار القائم على المشروع إلى شروط التعاقد القائمة على المشروع المناظر. يتم نسخ العملاء على بند عرض الأسعار القائم على المشروع إلى عقد المشروع.

عند فوترة عقد المشروع النهائي، تحتل قائمة العملاء على شروط التعاقد القائمة على المشروع الأولوية على القائمة الموجودة على عقد المشروع. تُستخدم قائمة العملاء على عقد المشروع فقط للإعدادات الافتراضية على شروط تعاقد المشروع الجديدة.

يتم تعيين جميع عملاء عرض الأسعار على علامة تبويب **العملاء** لعرض أسعار المشروع بشكل افتراضي إلى عملاء بند عرض الأسعار على أي بنود عرض أسعار جديدة قائمة على المشروع وتم إنشاؤها لعرض الأسعار. لا ترث بنود عرض الأسعار الموجودة والقائمة على مشروع سجلات عملاء عرض الأسعار الجديدة التي تم إنشاؤها بالاستناد إليها.

## <a name="create-update-or-delete-a-quote-line-customer-record"></a>إنشاء سجل عميل بند عرض أسعار أو تحديثه أو حذفه

يمكنك إنشاء عميل بند عرض أسعار أو تحديثه أو حذفه على علامة التبويب **عملاء بند عرض الأسعار** في الصفحة **بند عرض الأسعار القائم على المشروع**. عندما تضيف عميلاً جديدًا في بند عرض الأسعار القائم على المشروع، يُضاف العميل أيضًا إلى عرض الأسعار الإجمالي كعميل عرض أسعار، مع نسبة مئوية افتراضي لتقسيم الفوترة‬ على عرض الأسعار الإجمالي 0%. يتم نسخ النسبة المئوية لتقسيم الفوترة‬ في عرض الأسعار الإجمالي إلى بنود عرض الأسعار الجديد وإلى عقد المشروع النهائي. ومع ذلك، عند الفوترة من العقد، يتم استخدام النسبة المئوية لتقسيم الفوترة على مستوى بنود عرض الأسعار، وليس النسبة المئوية لتقسيم الفوترة على مستوى العقد الإجمالي. 

يبين الجدول التالي الحقول على سجل عميل بند عرض الأسعار لبند عرض أسعار قائم على المشروع.

| الحقل | الموقع | الوصف والإرشادات | تأثير لاحق |
| --- | --- | --- | --- |
| **العميل** | شبكة قابلة للتحرير على علامة تبويب **عملاء عرض الأسعار** والنموذج الرئيسي ونموذج الإنشاء السريع لعميل بند عرض الأسعار. | يدرج كافة الحسابات النشطة. يتم تأمين هذا الحقل بعد إنشاء السجل. إذا احتجت إلى تحديث الحقل، فاحذف السجل ثم قم بإنشائه من جديد. إذا قمت بتسجيل أي قيم فعلية، فلن تتمكن من حذف السجل. | عند اختيار حساب من القائمة الرئيسية للحسابات التي يجب إضافتها، يُضاف أيضًا عميل بند عرض الأسعار كعميل عرض أسعار. عند الفوز بعرض أسعار، يتم نسخ عملاء بند عرض الأسعار إلى عملاء شروط تعاقد المشروع. |
| **النسبة المئوية لتقسيم الفوترة** | شبكة قابلة للتحرير على علامة تبويب **عملاء عرض الأسعار** والنموذج الرئيسي ونموذج الإنشاء السريع لعميل بند عرض الأسعار. | يمثل هذا الخيار النسبة المئوية لكل حركة مبيعات غير مفوترة والتي ستُنسب إلى عميل بند عرض الأسعار هذا. | يتم نسخه إلى عملاء شروط تعاقد المشروع. |
| **حد يجب عدم تجاوزه** | شبكة قابلة للتحرير على علامة تبويب **عملاء عرض الأسعار** والنموذج الرئيسي ونموذج الإنشاء السريع لعميل بند عرض الأسعار. | يشير هذا الخيار إلى ما إذا كان هناك حد أو حد أقصى يتم التفاوض عليه على المبلغ الإجمالي الذي ستتم فوترته إلى هذا العميل لهذا البند في عرض الأسعار. | يتم نسخه إلى عملاء شروط تعاقد المشروع عند الفوز بعرض أسعار. |
| **الشركة المالكة** | شبكة قابلة للتحرير على علامة تبويب **عملاء عرض الأسعار** والنموذج الرئيسي ونموذج الإنشاء السريع لعميل بند عرض الأسعار. | الكيان القانوني الذي يتم فيه إعداد هذا العميل في الوحدة النمطية **إدارة المشاريع والمحاسبة**. هذا الحقل للقراءة فقط ويتم تعيينه للشركة المالكة لعرض الأسعار نفسه. تمت بالفعل تصفية قائمة العملاء الذين يجب إضافتهم في حقل **الحساب** إلى القائمة من الشركة المالكة في الوحدة النمطية **إدارة المشاريع والمحاسبة** في Project Operations. | تساوي الشركة المالكة مفهوم الكيان القانوني. يتم حساب كافة التكاليف والإيرادات المستحقة من هذا المشروع في دفتر الأستاذ العام للشركة المالكة. |
| **التقريب** | شبكة قابلة للتحرير على علامة تبويب **عملاء عرض الأسعار** والنموذج الرئيسي ونموذج الإنشاء السريع لعميل بند عرض الأسعار. | يشير هذا الخيار إلى ما إذا كان هذا العميل عميل تقريب افتراضي لبند عرض الأسعار هذا القائم على المشروع. | يتم نسخه إلى عملاء عقد المشروع عند الفوز بعرض أسعار. |

## <a name="edit-billing-split-percentages"></a>تحرير النسب المئوية لتقسيم الفوترة

يمكنك تحرير النسب المئوية لتقسيم الفوترة بشكل مباشر. عندما لا يساوي إجمالي النسب المئوية لتقسيم الفوترة 100%، يحدث خطأ. بعد تحرير النسب المئوية لتقسيم الفوترة، قم بتحديث صفحة بند عرض الأسعار لإزالة الخطأ.

استخدم إجراء التوزيع المتساوي على الشبكة الفرعية لعملاء بند عرض الأسعار لتخصيص تقسيم الفوترة على كافة عملاء بنود عرض الأسعار. عند وجود معامل تقريب، سيُضاف إلى عميل التقريب. توضع دائمًا علامة عميل التقريب على أحد عملاء بنود عرض الأسعار، مما يعني أن علامة التقريب لسجل عميل بند عرض الأسعار معينة إلى **نعم**. 