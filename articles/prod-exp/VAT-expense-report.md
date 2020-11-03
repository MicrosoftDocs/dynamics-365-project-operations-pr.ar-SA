---
title: استرداد ضريبة القيمة المضافة
description: يوضح هذا الموضوع كيفية استرداد المبالغ المستردة على حركات ضريبة القيمة المضافة (VAT).
author: saraschi2
manager: AnnBe
ms.date: 02/26/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d1be96521cdb486dd5a702cded615d3e1015b364
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070686"
---
# <a name="vat-recovery"></a>استرداد ضريبة القيمة المضافة 

[!include [banner](../includes/banner.md)]

لاستلام مبالغ مستردة في حركات الضريبة ذات القيمة المضافة (VAT) المؤهلة، يجب أن تقوم الشركة أو المؤسسة بتعيين المعلومات الدقيقة وتجميعها والتحقق منها وإرسالها. تشتمل هذه العملية على العديد من المهام، وقد تتضمن العديد من الموظفين أو الأدوار، وذلك وفقًا لحجم الشركة.

لاسترداد ضريبة القيمة المضافة باستخدام إدارة المصروفات، يجب إكمال المتطلبات الأساسية التالية:

- يجب إنشاء أكواد الضريبة للبلاد/المناطق التي تم تخصيصها لفئات المصروفات.
- يجب إنشاء مجموعة ضريبة مبيعات لكل كود ضريبة.
- يجب إنشاء كود ضريبة مبيعات صنف لكل مجموعة ضريبة مبيعات.

بعد اكتمال المتطلبات الأساسية، يتبع الموظفون الخطوات التالية لطلب استرداد القيمة النقدية لحركات ضريبة القيمة المضافة.

1. في تقرير المصروفات، أدخل معلومات الضرائب حول حركات بطاقات الائتمان لتحديد مبالغ ضريبة القيمة المضافة المؤهلة للاسترداد.
2. تأكد من اكتمال كافة معلومات الضريبة، ثم قم بترحيل تقرير المصروفات.
3. قم بمعالجة المصروفات المؤهلة لاسترداد ضريبة القيمة المضافة الدولية.
4. أرسل بيانات استرداد ضريبة القيمة المضافة إلى مورد الجهة الخارجية لإبلاغ عن مستحقات الاسترداد الدولي.
5. قم بمعالجة المصروفات لاسترداد ضريبة القيمة المضافة المحلية.

توفر الأقسام التالية أمثلة توضح كيفية استكمال موظفي Contoso كل خطوة.

## <a name="on-an-expense-report-enter-tax-information-about-credit-card-transactions-to-identify-eligible-vat-refunds"></a>في تقرير المصروفات، أدخل معلومات الضرائب حول حركات بطاقات الائتمان لتحديد مبالغ ضريبة القيمة المضافة المؤهلة للاسترداد.

عادت نانسي، وهي مندوبة مبيعات في شركة Contoso والتي تقيم في الولايات المتحدة، مؤخرًا من رحلة مبيعات إلى المملكة المتحدة. أثناء الرحلة، تكبدت نانسي بعض المصروفات الشخصية عبر بطاقة الائتمان مقابل الوجبات. يجب أن تقوم نانسي الآن بإنشاء تقرير مصروفات لتسوية مصروفاتها.

عندما تدخل نانسي معلومات في تقرير المصروفات، فإنها تحدد **المملكة المتحدة** في حقل **البلد/المنطقة** في صفحة **تحرير تقرير المصروفات**. بعد ذلك تجري تصفية قائمة مجموعات ضريبة المبيعات لكي تظهر فقط المجموعات التي تنطبق على المملكة المتحدة. تحدد نانسي مجموعة ضريبة المبيعات **المملكة المتحدة 001** ثم تحدد مجموعة ضريبة المبيعات لصنف **الوجبات**. بعد ذلك، تضيف نانسي حركة جديدة لتسجيل إقامتها. نظرًا لوجود فقط مجموعة ضريبة مبيعات واحدة ومجموعة ضريبة مبيعات لصنف واحد للتسجيل في الدفتر في المملكة المتحدة، سيتم ملء هذه المعلومات تلقائيًا في تقرير المصروفات لنانسي.

بحسب نهج شركة Contoso، يجب أن تحتوي كافة المصروفات على إيصال مطابق. وبالتالي، عندما تحفظ نانسي تقرير المصروفات، فإنها تتلقى رسالة تنص على أنه يجب عليها إرفاق إيصال لكل حركة قامت بإدراجها في تقرير المصروفات الخاص بها. تتحقق نانسي من أنها قامت بإرفاق صورة رقمية لكل إيصال عملية حركة بتقرير المصروفات الخاص بها ثم أرسلت التقرير للاعتماد. بعد ذلك أرسلت إيصالات ورقية إلى فريق المعالجة بالمكتب الخلفي. سيرسل هذا الفريق بيانات استرداد ضريبة القيمة المضافة إلى مورد الجهات الخارجية الذي يقوم بالإبلاغ عن مستحقات استرداد ضريبة القيمة المضافة الدولية لشركة Contoso.

## <a name="make-sure-that-all-tax-information-is-complete-and-then-post-the-expense-report"></a>تأكد من اكتمال كافة معلومات الضريبة، ثم قم بترحيل تقرير المصروفات.

يجب على أبريل، وهي منسقة الحسابات الدائنة في شركة Contoso، إدخال أية معلومات ضريبة مفقودة من تقرير مصروفات قبل أن تتمكن من ترحيله. وعليها فتح صفحة **تفاصيل تقرير المصروفات** ومشاهدة تقرير المصروفات المعتمدة لنانسي. بعد ذلك، تفتح أبرل تقرير المصروفات لعرض تفاصيل الحركات. وترى أن نانسي لم تدخل مجموعة ضريبة مبيعات الصنف لإحدى الحركات. ونظرًا لعدم توفير هذه المعلومات، لا يمكن لأبرل ترحيل تقرير المصروفات. وبالتالي، تبحث أبريل في صفحة **تكوينات الضريبة** في إدارة المصروفات، وتعثر على مجموعة ضريبة مبيعات الصنف المناسبة للبلد/المنطقة ونوع الحركة. يمكن لأبرل الآن ترحيل تقرير المصروفات إلى دفتر الأستاذ العام.

وعندما تقوم أبرل بترحيل تقرير المصروفات، يتم إنشاء بند عمل ضريبة القيمة القابلة للاسترداد. تم تعيين بند العمل هذا لعضو في فريق المعالجة بالمكتب الخلفي. تستلم أبرل رسالة تؤكد إتمام عملية الترحيل بنجاح. كما تسرد هذه الرسالة عدد معاملات ضريبة القيمة المضافة التي تم تحديدها للاسترداد.

## <a name="process-expenses-that-are-eligible-for-international-vat-recovery"></a>معالجة المصروفات المؤهلة لاسترداد ضريبة القيمة المضافة الدولية

يتولى أرني، وهو عضو في فريق المعالجة الخلفية لشركة Contoso، مسؤولية التأكد من أن جميع المعلومات المطلوبة لاسترداد ضريبة القيمة المضافة مضمنة في تقارير المصروفات. وهو يفتح صفحة **استرداد ضريبة المصروفات** ويحدد تقرير المصروفات الذي أرسلته نانسي. يتحقق أرني من إرفاق كافة الإيصالات المطلوبة، ومن إدخال مجموعة ضريبة المبيعات وأكواد ضريبة المبيعات للصنف الصحيحة.

وعندما يستلم أرني الإيصالات الورقية من نانسي، يتحقق منها مقابل الإيصالات الرقمية ثم يقوم بتغيير حالة تقرير المصروفات إلى **جاهز للاسترداد**.

## <a name="send-vat-recovery-data-to-the-third-party-vendor-to-file-international-recovery-returns"></a>أرسل بيانات استرداد ضريبة القيمة المضافة إلى مورّد خارجي لإبلاغ عن مستحقات الاسترداد الدولي.

عندما يصبح أرني جاهزًا لإرسال بيانات تقرير المصروفات إلى مورد الجهات الخارجية الذي سيقوم بالإبلاغ عن مرتجعات ضريبة القيمة المضافة، فإنه يفتح صفحة **استرداد ضريبة المصروفات**. ويقوم بتصفية الصفحة بحيث تُظهر فقط تقارير المصروفات التي تم تعليمها على أنها **جاهزة للاسترداد**. بعد ذلك حدد أرني **إبلاغ** &gt; **تصدير إلى Excel**. يتم تصدير معلومات ضريبة القيمة المضافة من تقارير المصروفات إلى ورقة عمل Microsoft Excel. أرسل أرني ورقة العمل هذه إلى مورد الجهة الخارجية وقام بتضمين رسالة توضح أنه تم إرسال إيصالات ورقية بواسطة شركة نقل.

## <a name="process-expenses-for-domestic-vat-recovery"></a>معالجة المصروفات لاسترداد ضريبة القيمة المضافة المحلية

يجب أن يتحقق أرني من أن حركات تقرير المصروفات مؤهلة لاسترداد ضريبة القيمة المضافة، وأنه قد تم إرفاق الإيصالات الرقمية بالتقارير. لبدء معالجة المصروفات المؤهلة للاسترداد المحلي، يفتح أرني صفحة **استرداد ضريبة المصروفات** ويحدد تقرير المصروفات الذي يتطلب التحقق. ويتحقق من أن الإيصالات باسم الشركة بدلا من الموظف. بالنسبة لاسترداد ضريبة القيمة المضافة، يجب أن تكون الإيصالات باسم الشركة. يؤكد أرني بعد ذلك تطبيق مجموعة ضريبة المبيعات وأكواد ضريبة مبيعات الصنف الصحيحة.

عندما يتلقى أرني الإيصالات الورقية، يقوم بتغيير حالة تقرير المصروفات إلى **جاهز للاسترداد**. ويمكنه عندئذ الإبلاغ عن المبلغ المرتجع مع هيئة الضرائب المناسبة. وفي هذه الحالة، هيئة الضرائب المناسبة في الولايات المتحدة هي دائرة الإيرادات الداخلية (IRS).