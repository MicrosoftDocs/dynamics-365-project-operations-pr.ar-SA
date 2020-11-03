---
title: عمليات المبيعات
description: يوفر هذا الموضوع معلومات حول عمليات المبيعات الأساسية.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: f09b30fe6d842faaf896cb97f44b060ec4049213
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070758"
---
# <a name="sales-processes"></a>عمليات المبيعات

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

تختلف عمليات المبيعات المستخدمة في المؤسسة المستندة إلى المشروع عن عمليات المبيعات المستخدمة في المؤسسة المستندة إلى المنتج. يحدث هذا الاختلاف نتيجة لأن دورات المبيعات الخاصة بالمؤسسات المستندة إلى المشروع أطول وتتطلب تقنيات تقديرات مخصصة لتحليل عروض الأسعار وإنشاءها لكل صفقة. يستخدم Dynamics 365 Project Service Automation بعض الوظائف نفسها المستخدمة في عملية المبيعات لمبيعات Dynamics 365 Sales. وإليك بعض الأمثلة:

- يتم استخدام كيان عميل متوقع لتعقب عملية المبيعات.
- ويتم تعقب تأهيل العملاء المتوقعين كفرص مبيعات محتملة. كما يمكن أن تبدأ عملية المبيعات أيضا بفرصة مبيعات.
- يتم الوصول إلى كافة البيانات الاصطناعية ذات الصلة لإحدى الفرص. وتتضمن هذه البيانات الاصطناعية فريق المبيعات والمساهمين والاحتمالات والتصنيف ومراحل المبيعات وعمليات الأعمال.
- ويتم إنشاء عروض أسعار متعددة للفرصة.
- يتخذ عرض الأسعار علامة **مغلق كمكسب** لإنشاء أمر مبيعات. في PSA، يتم تخصيص أمر المبيعات ويُطلق عليه عقد مشروع.

يوضح الرسم التوضيحي التالي عملية مبيعات نموذجية في مؤسسة تستند إلى مشروع.

> ![عملية المبيعات في مؤسسة تستند إلى مشروع](media/basic-guide-1.png)

## <a name="estimating-a-sale"></a>تقدير المبيعات
يمكن تقدير قيمة المبيعات بناء على المشاريع التي تم تسليمها في السابق ومدى تعقيد المشاريع. بالنسبة للمشاريع التي تشكل امتدادات للمشاريع السابقة، أو المشاريع التي تكون فيها خبرة المورد عالية ويتم استخدام قوالب عمل معروفة ، يمكنك استخدام عملية تقدير أبسط. عادة ما يكون للمشاريع الأكثر تعقيدا عملية شراء أطول. بالتالي، يوجد المزيد من المراحل في عملية تقدير المبيعات. وفي بداية العملية، يستخدم فريق المبيعات إدخالات مديري الحسابات وخبراء الموضوع (SME) للبدء في إنشاء تقدير عال المستوي لكل مكون مميز للعمل الذي يتم إنشاء عرض أسعار له. يتم تمثيل المكونات العمل هذه بواسطة بنود عرض الأسعار. 

يمكنك إنشاء تقدير عال المستوى لعرض الأسعار. وفي النهاية، سيتم استبدال هذا التقدير عال المستوى بتقدير أكثر تفصيلا يعتمد على خطة مشروع قمت بإنشائه باستخدام قوالب المشروع القياسية. تساعدك هذه القوالب في بناء جدول وتحديد القيم المالية في عرض الأسعار ومكوناته (بنود عرض الأسعار). 

يمكنك إنشاء عروض أسعار متعددة لمشروع وتجميعها تحت نوع كيان فرصة فردي. وفي النهاية ، يتم وضع علامة **مغلق كمكسب** على أحد عروض الأسعار هذه، ويتم إنشاء عقد مشروع أو بيان من العمل (SOW). يحتفظ عقد المشروع بقيمة التعاقد لكل مكون (شرط التعاقد) والذي يقبله العميل للتسليم. ويتم في العادة إنشاء بيان العمل (SOW) كمستند Microsoft Word. جميع الفواتير التي يتم إرسالها إلى العميل طوال دورة تسليم المشروع تشير إلى عقد المشروع أو SOW.

يمكنك أيضا إنشاء عروض أسعار بديلة تحت نوع كيان فرصة واحدة أو إعداد النظام بحيث يتم إنشاء عقد مشروع عندما يتم الفوز بعرض أسعار. في هذه الحالة، يمكنك إرفاق مستند Word يمثل SOW بسجل عقد المشروع.

![إغلاق عرض أسعار لإنشاء عقد مشروع](media/basic-guide-2.png)

## <a name="configuring-the-sales-process"></a>تكوين عملية المبيعات
يمكنك استخدام سير إجراءات العمل (BPF) في Microsoft Dynamics 365 لتكوين عملية المبيعات الخاصة بك. يمنح سير إجراءات العمل (BPF) فريق المبيعات واجهة مرئية إرشادية يمكنهم استخدامها للانتقال بالصفقات إلى الأمام عبر المراحل التي تكون مناسبة لشركك.

على سبيل المثال، قد يكون لدي شركتك المراحل الستة التالية في عملية المبيعات:

1. تأهيل
2. التقدير
3. المراجعة الداخلية
4. عقد
5. التسليم
6. إغلاق

يتم تمثيل هذه المراحل الستة بشارة الرتبة (\>) التي تحددها للتوسيع في كل نوع من أنواع كيانات الفرصة التي تقوم بإنشاءها.

![تكوين عملية أعمال في Dynamics 365](media/basic-guide-3.png)
 
قد تستخدم المؤسسة الخاصة بك كيانات مختلفة لتمثيل نفس الصفقة أثناء تطورها. في البداية في عملية المبيعات، يتم تمثيل الصفقة بواسطة كيان الفرصة. بمرور الوقت وظهور المزيد من التفاصيل، يمكنك استخدام تقديرات عالية المستوى لإنشاء واحد أو أكثر من عروض الأسعار. إذا تمت مراجعة أحد عروض الأسعار هذه من قبل المساهمين الداخليين والعملاء، فسيمثل كيان عرض الأسعار الصفقة. وبعد أن يقبل العميل عرض الأسعار ، فإن عقد مشروع أو SOW يمثل الصفقة. ولدعم هذا السلوك، يتم بناء سير إجراءات العمل BPF بحيث تكون كل مرحلة في العملية مرتبطة بجدول قاعدة بيانات مختلف.

يمكن تدعيم مرحلة **التأهيل** في عملية المبيعات بواسطة كيان فرصة. ويمكن تدعيم مراحل **التقدير** و **المراجعة الداخلية** بواسطة كيان عرض الأسعار. يمكن تدعيم مراحل **العقد** و **التسليم** و **الإغلاق** بواسطة كيان عقد مشروع.

عندما تقوم بتحريك الصفقات عبر المراحل، تتم مطالبتك بإنشاء سجل الكيان المناسب لمساعدتك وإرشادك خلال العملية. يمكن أن تكون المراحل شرطية. على سبيل المثال، إذا كنت تطلب مراجعة داخلية لعرض أسعار فقط وإذا كان عرض الأسعار يستخدم قائمة أسعار مخصصة، فيمكنك تكوين هذا الشرط في المرحلة الملائمة لعملية الأعمال. عندئذ يتم عرض مرحلة **المراجعة الداخلية** فقط لعروض الأسعار التي تستخدم قائمة أسعار مخصصة. النسبة لكافة الصفقات وعروض الأسعار الأخرى تكون مرحلة **التقدير** متبوعة بمرحلة **العقد**.

> [!NOTE]
> يوجد في PSA صفحات محددة لكيانات الفرص وعروض الأسعار والأوامر والفواتير. يجب أن تقوم بإنشاء فرص project service وعروض الأسعار والأوامر والفواتير باستخدام صفحات معلومات المشروع لهذه الكيانات. إذا استخدمت صفحة أخرى لإنشاء سجل، فلن تتمكن من فتح السجل من صفحة **معلومات المشروع**. إذا أردت فتح سجل من صفحة **معلومات المشروع** ، يجب عليك حذف السجل وإعادة إنشائه باستخدام صفحة **معلومات المشروع**. في صفحة **معلومات المشروع** ، يضمن منطق الأعمال الخاص بكل من أنواع الكيانات هذه أن يتم تعيين حقل **النوع** الخاص بالسجل بشكل صحيح، ويتم تهيئة كافة المفاهيم الإلزامية بشكل صحيح.

> ![معلومات المشروع لأمر جديد](media/basic-guide-4.png)
 
## <a name="differences-between-project-service-automation-and-sales"></a>الاختلافات بين Project Service Automation وSales
على الرغم من أن عملية المبيعات في PSA تستخدم الإمكانات الأساسية لعملية المبيعات في Sales، لكن يوجد بعض الاختلافات الأساسية للتباينات في ممارسات الأعمال الخاصة بالمؤسسات المستندة إلى المشروع. وإليك بعض الأمثلة:

- **عروض أسعار المشروع** - في Project Service Automation، يتم إغلاق عرض الأسعار بعد إنشاء عقد المشروع من عرض الأسعار. في Sales، يمكنك الاحتفاظ بعرض الأسعار مفتوحا بعد الفوز به. والسبب وراء هذا الاختلاف هو أن التطابق بين عرض الأسعار وعقد المشروع أفضل للمؤسسات المستندة إلى المشروع. 
- **التنشيط والمراجعات** – في PSA ، لا يتم دعم التنشيط والمراجعات لعروض أسعار المشروع. في Sales، يمكن تأمين عرض الأسعار لمنع عمليات التحرير الإضافية.
- **إغلاق عرض أسعار كخسارة أو فوز** -في PSA، عند إغلاق عرض أسعار مشروع كفوئز أو خسارة، تبقي الفرصة مفتوحة. ويتم إغلاق كافة عروض الأسعار الأخرى الموجودة في الفرصة باعتبارها خاسره. في Sales، عندما يتم إغلاق عرض أسعار تم الفوز به أو خسارته، تتم مطالبة المستخدم باتخاذ إجراء على الفرصة. واستنادا إلى إدخال المستخدم، قد تكون الفرصة الأساسية مغلقه أو متروكة مفتوحة.

## <a name="tracking-revisions-to-quotes-and-project-plans-in-the-sales-cycle"></a>تعقب مراجعات عروض الأسعار وخطط المشروع في دورة المبيعات
في PSA، لا يمكنك تعقب المراجعات التي يتم اجراؤها على عرض أسعار. بدلا من ذلك، يجب وضع علامة **مغلق كخسارة** على عرض الأسعار الموجود ثم إنشاء عرض أسعار جديد. يمكنك نسخ عرض أسعار أو استنساخ عرض أسعار يستند إلى المشروع باستخدام PSA.

## <a name="tracking-comments-and-approvals-of-quotes-and-project-contracts"></a>تعقب التعليقات والموافقات لعروض الأسعار وعقود المشروع
يمكنك إدارة مراجعة عروض الأسعار وعقود المشروع والموافقة عليها عن طريق استخدام حائط السجلات وعمليات النشر. يمكن لمؤسسك إنشاء مهام سير عمل مخصصة ومكونات إضافية لتعيين إعلامات المراجعة والموافقة على عناصر العمل وإعادة توجيهها وتصعيدها وإدارتها.