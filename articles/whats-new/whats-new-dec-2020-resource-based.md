---
title: الجديد في ديسمبر 2020 - Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬
description: يوفر هذا الموضوع معلومات حول التحديثات الإصلاحية المتوفرة في إصدار ديسمبر 2020 من Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة.‬
author: sigitac
manager: tfehr
ms.date: 12/04/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: f80922877f3d3d0e1149c2aa690f881bcf927b11
ms.sourcegitcommit: 5791f6347e800fc4f6c76e7460947cb6824edebe
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "4700664"
---
# <a name="whats-new-december-2020---project-operations-for-resourcenon-stocked-based-scenarios"></a>الجديد في ديسمبر 2020 - Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

ينطبق هذه الموضوع على مكونات وإصدارات Dynamics 365 Project Operations التالية:

- Project Operations على بيئة Dataverse الإصدار 4.5.0.134
- إدارة المشاريع والمحاسبة في الإصدار 10.0.15 من بيئة Dynamics 365 Finance

## <a name="features-included-in-this-release"></a>الميزات المضمنة في هذا الإصدار
تم تضمين الميزات التالية في هذا الإصدار:

  - [الفوترة بين الشركات الشقيقة](../project-accounting/intercompany-invoicing-overview.md) 
  - [سلف ومقدمات أتعاب العملاء](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)

## <a name="updates-to-project-operations-for-resource-non-stocked-based-scenarios"></a>تحديثات Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة

### <a name="project-operations-on-dataverse"></a>Project Operations على Dataverse

| منطقة الميزات                    | رقم المرجع | تحديث إصلاحي                                                                                                                                               |
|---------------------------------|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| الفوترة والتسعير             | 1986009          | تشتمل سطور دفتر اليومية التي تم إنشاؤها يدويا علي أداء غير متسق عند التاكيد قبل المشروع المرتبط بشروط تعاقد أو غير مرتبطة به.                     |
| الفوترة والتسعير             | 2028174          | ينبغي ان يتبع تحديث تفاصيل سطر الفاتورة منطق دفتر يوميه التصحيح                                                                                  |
| الفوترة والتسعير             | 2028315          | إصلاحات سلوك الشبكة المتداخلة القابلة للتحرير                                                                                                                        |
| الفوترة والتسعير             | 2031070          | يجب ان يتبع تعديل تفاصيل سطر الفاتورة التصحيحي منطق دفتر يوميه التصحيح                                                                              |
| الفوترة والتسعير             | 2034186          | يجب ان يكون قادرا علي تحديث مشروع في سطر العقد                                                                                                        |
| الفوترة والتسعير             | 2034206          | يجب تعيين حاله التسوية اثناء عمليه العكس الفعلي عند إلغاء ارتباط مشروع من سطر عقد                                                        |
| الفوترة والتسعير             | 2040871          | السماح بتحديثات خلايا مجموعة الوحدة والوحدة على شبكة تقديرات المصروفات                                                                                       |
| الفوترة والتسعير             | 2053754          | عدم وضع علامة علي القيم الفعلية التي تم إنشاؤها من عمليات تحرير الفواتير بحاله التسوية وحاله الفوترة                                                                |
| الفوترة والتسعير             | 2057874          | تم إنشاء اتصال المعاملة الصحيح اثناء تحرير تفاصيل سطر الفاتورة                                                                                     |
| الفوترة والتسعير             | 2057875          | أصول المعاملات الصحيحة التي تم إنشاؤها أثناء تحرير تفاصيل سطر الفاتورة                                                                                        |
| الفوترة والتسعير           | 2057944          | تعيين الحالة "غير محدد" كمخصصه للأخطاء الفعلية غير الجاهزة للفوترة من أحد تصحيحات الفاتورة                                             |
| الفوترة والتسعير           | 2066169          | قم بتحديث تاريخ المحاسبة لسجل المبيعات غير المفوتر السالب عند الدمج باستخدام الكتابة المزدوجة                                                            |
| الفوترة والتسعير           | 2067622          | يجب ان يتم عرض أيقونه المعالجة اثناء إنشاء الاحداث الرئيسية                                                                                                |
| الفوترة والتسعير           | 2067624          | يجب وضع علامة على المبلغ المتعاقد عليه كعمل موصى به عند إنشاء الأحداث الرئيسية                                                                      |
| الفوترة والتسعير           | 2086880          | زر إخفاء **الاقتراح** على الشريط الخاص ببنود عرض الأسعار المستندة إلى المشروع                                                                                                |
| الفوترة والتسعير           | 2098140          | عرض زر **الفاتورة الصحيحة** للبيئات المتكاملة                                                                                             |
| التوزيع والتكوين  | 2101152          | يجب ان تحتوي البيئة الجديدة التي تم إنشاؤها باستخدام قالب Project Operations من مركز إدارة Power Platform علي جميع عمليات التثبيت اللاحقة التي تم تنفيذها               |
| إدارة الفرص        | 2086601          | ينبغي الا يتم نسخ الأدوار والفئات التي تم إلغاء تنشيطها إلى الأدوار الخاضعة للرسوم والفئات الخاضعة للرسوم في بنود عرض الأسعار وبنود العقد |
| تخطيط المشاريع وتعقبها | 1949065          | تعمل امكانيه رؤية البيانات بشكل صحيح في 200% التكبير/التصغير                                                                                                                   |
| تخطيط المشاريع وتعقبها | 2046317          | القدرة على إعادة تسمية كيان المشروع في Project Operations                                                                                   |
| تخطيط المشاريع وتعقبها | 2057171          | رسالة خطا محدثه عندما يكون حقل **تاريخ بدء المشروع** فارغًا في صفحة **المشروع**                                                           |
| تخطيط المشاريع وتعقبها | 2057197          | نسخه سطر التقدير مع مرجع المهمة غير مدعومة                                                                                                     |
| تخطيط المشاريع وتعقبها | 2060687          | تحذير المنطقة الزمنيه يختفي الآن بعد مده معينه                                                                                                      |
| إدارة الموارد           | 1832887          | يجب أن يكون معرف فئة المورد الافتراضي ثابتًا لضمان تحميل البيانات القابلة للتكرار لـ Dataverse وبيئات Finance                                                 |
| الوقت والمصروفات              | 2081793          | يجب تعيين **اسم فئة المصروفات** إلى حقل **وصف فئة المصروفات** في تطبيقات Finance and Operations                                                  |
| الوقت والمصروفات              | 2034882          | الزر **جديد** يُعرض مرتين علي شريط الأوامر لإدخالات الوقت عند تثبيت Dynamics 365 Field Service                                          |
| الوقت والمصروفات              | 2056028          | تحديث صفحة **تحرير الوقت** لتضمين خط زمني                                                                                                              |
| الوقت والمصروفات              | 1983747          | مخطط الإدخال الزمني عرض بيانات اضافيه                                                                                                                   |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>إدارة المشاريع والمحاسبة في Dynamics 365 Finance

| منطقة الميزات                        | رقم المرجع | تحديث إصلاحي                                                                                                                                                                                                                                                   |
|-------------------------------------|------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| إدارة المشاريع والمحاسبة | [441680](https://fix.lcs.dynamics.com/Issue/Details/?bugId=441680)           | عمليات الضبط المؤمنة لطلب الصنف إرجاع                                                                                                                                                                                                        |
| إدارة المشاريع والمحاسبة | [446498](https://fix.lcs.dynamics.com/Issue/Details/?bugId=446498)           | عدم ظهور ملاحظات النموذج في فواتير المشروع المنسقة                                                                                                                                                                                                          |
| إدارة المشاريع والمحاسبة | [453407](https://fix.lcs.dynamics.com/Issue/Details/?bugId=453407)           | لا يُسمح لـ MEXICO CFDI 33 لفواتير المشروع بتحديث طريقة الدفع من اقتراح الفاتورة                                                                                                                                                           |
| إدارة المشاريع والمحاسبة | [458149](https://fix.lcs.dynamics.com/Issue/Details/?bugId=458149)           | لا يتم الحصول علي المعلمة التي تقوم تلقائيا بتعيين التاريخ المحاسبي إلى فتره مفتوحة في دفتر يومية **التكامل**                                                                                                                                                             |
| إدارة المشاريع والمحاسبة | [470293](https://fix.lcs.dynamics.com/Issue/Details/?bugId=470293)           | لا تظهر عناصر قائمة التنبؤ في صفحة قائمة **المشاريع**                                                                                                                                                                                                      |
| إدارة المشاريع والمحاسبة | [475873](https://fix.lcs.dynamics.com/Issue/Details/?bugId=475873)           | لا يمكن فتح **كشف المشروع** > **الحركات والتنبؤ**                                                                                                                                                                                                      |
| إدارة المشاريع والمحاسبة | [482558](https://fix.lcs.dynamics.com/Issue/Details/?bugId=482558)           | تؤدي إزالة تعيين الموارد وقراءتها إلى مضاعفة إدخالات توقعات المشروع في Finance                                                                                                                                                                   |
| إدارة المشاريع والمحاسبة | [484468](https://fix.lcs.dynamics.com/Issue/Details/?bugId=484468)           | تعذر إنشاء تقديرات المشروع في Dataverse دون وجود سطر عقد في المشروع                                                                                                                                                                 |
| إدارة المشاريع والمحاسبة | [485439](https://fix.lcs.dynamics.com/Issue/Details/?bugId=485439)           | فشل عملية الاستبعاد بسبب عدم توافق الإيصال عندما تكون عملة الشركة مختلفة عن عملة الحركة.                                                                                                                                            |
| إدارة المشاريع والمحاسبة | [488382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488382)           | تصفيه حاله الفاتورة في حركات المشروع المرحلة للمشاريع ثابته الأسعار لا تعمل                                                                                                                                                            |
| إدارة المشاريع والمحاسبة | [505458](https://fix.lcs.dynamics.com/Issue/Details/?bugId=505458)           | يتعذر تحديث تاريخ البدء لمهمة في Dataverse                                                                                                                                                                                                                    |
| إدارة المشاريع والمحاسبة | [507172](https://fix.lcs.dynamics.com/Issue/Details/?bugId=507172)           | يمكن حذف بنود مقترح الفاتورة في السيناريو المتكامل لـ Project Operations                                                                                                                                                                                    |
| إدارة المشاريع والمحاسبة | [509989](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509989)           | يمكن حذف بنود مقترح الفاتورة في السيناريو المتكامل لـ Project Operations                                                                                                                                                                                    |
| إدارة المشاريع والمحاسبة | [510041](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510041)           | منع تمكين ميزة شروط تعاقد متعددة دون تكامل Dataverse                                                                                                                                                                                        |
| إدارة المشاريع والمحاسبة | [510527](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510527)           | تقدير شاشه الإيراد المفوتر هو صفر (0) عند فوتره الحساب = الربح والخسارة                                                                                                                                                                          |
| إدارة المشاريع والمحاسبة | [514364](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514364)           | الأعمال تحت التنفيذ - ترحيل قيمه المبيعات في الشركات الشقيقة اختيار فوتره المشروع حساب غير متوقع                                                                                                                                                                           |
| إدارة المشاريع والمحاسبة | [522799](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522799)           | غير قادر علي أداء التعرف علي الإيرادات/التقييم مع تمكين Project Operations                                                                                                                                                                         |
| السفر والمصروفات                | [378738](https://fix.lcs.dynamics.com/Issue/Details/?bugId=378738)           | يتم إرجاع المصروفات التي تم إدخالها بواسطة المفوض إلى مستخدم المصروفات وليس التفويض                                                                                                                                                                                           |
| السفر والمصروفات                | [409489](https://fix.lcs.dynamics.com/Issue/Details/?bugId=409489)           | تقرير المصروفات سير العمل لا يتم تحديد المستخدم المفوض إرسال سير العمل كمنشئ سير العمل                                                                                                                                                             |
| السفر والمصروفات                | [464658](https://fix.lcs.dynamics.com/Issue/Details/?bugId=464658)           | الابعاد الافتراضية في تجاوزات الكيان القانوني لا تعمل في تقارير المصروفات بين الشركات الشقيقة                                                                                                                                                                    |
| السفر والمصروفات                | [472892](https://fix.lcs.dynamics.com/Issue/Details/?bugId=472892)           | مشكله في حساب خفض الوجبة لليوم الأخير لفئة مصروفات المصروف اليومي الماضي                                                                                                                                                                                    |
| السفر والمصروفات                | [473646](https://fix.lcs.dynamics.com/Issue/Details/?bugId=473646)           | حقل **المبلغ الذي ستتم تسويته** في صفحة **طلب السفر** لا يتم تحديثه بعد حذف عنصر بند مصروفات من تقرير المصروفات المرتبط بطلب السفر                                                                                                       |
| السفر والمصروفات                | [474396](https://fix.lcs.dynamics.com/Issue/Details/?bugId=474396)           | التحقق من صحة تقرير المصروفات لهذا النهج بعد الإرسال إلى سير العمل                                                                                                                                                                                           |
| السفر والمصروفات                | [475777](https://fix.lcs.dynamics.com/Issue/Details/?bugId=475777)            | لا يتم عرض إيصالات مصروفات السفر بشكل صحيح لمفوض الإدخال                                                                                                                                                                                            |
| السفر والمصروفات                | [477714](https://fix.lcs.dynamics.com/Issue/Details/?bugId=477714)            | نوع المصروفات لكل موظف عدم إظهار المصروفات المفصلة عند تعيين لغة المستخدم إلى es-MX                                                                                                                         |
| السفر والمصروفات                | [477831](https://fix.lcs.dynamics.com/Issue/Details/?bugId=477831)            | يتيح تقرير المصروفات إدخال الفئة الفرعية غير الصحيحة لفئة مصروفات                                                                                                                                                                                       |
| السفر والمصروفات                | [478630](https://fix.lcs.dynamics.com/Issue/Details/?bugId=478630)            | لا تعمل تسويه السلفة النقدية بتقرير المصروفات بالشكل المتوقع عندما يكون مبلغ تقرير المصروفات أكبر من مبلغ السلفة النقدية.                                                                                                           |
| السفر والمصروفات                | [486680](https://fix.lcs.dynamics.com/Issue/Details/?bugId=486680)            | مشاكل الأداء مع الاستعلامات المتعلقة بـ ProjProjectLookup. تم حظر العميل لان الاستعلام يستغرق وقتا طويلا لتنفيذه.                                                                                                                     |
| السفر والمصروفات                | [487531](https://fix.lcs.dynamics.com/Issue/Details/?bugId=487531)            | تقارير المصروفات التي تم ترحيلها مع **السماح بتجميع الحركات المستندة إلى حساب الدفع المقابل** و **تصحيح التاريخ المحاسبي عند الترحيل** قيد التشغيل تُظهر تواريخ المحاسبة ولا يتم تجميعها في جدول **التوزيع المحاسبي**، والذي يؤثر علي سجلات ضريبة المبيعات |
| السفر والمصروفات                | [491759](https://fix.lcs.dynamics.com/Issue/Details/?bugId=491759)            | حركات بطاقات الائتمان المستوردة بعمله أجنبيه يؤدي إلى إنشاء حركات مورد غير صحيحه في حاله استخدام **ضريبة القيمة المضافة للتكاليف العكسية** في بنود تقرير المصروفات                                                                                                                     |
| السفر والمصروفات                | [506175](https://fix.lcs.dynamics.com/Issue/Details/?bugId=506175)            | لا يمكن إنشاء تقرير مصروفات بين الشركات الشقيقة في حاله أضافه "معرف المشروع" في "مستوي العنوان"                                                                                                                                                                 |
| السفر والمصروفات                | [509491](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509491)            | إصدار دفع المصروفات عندما يكون مبلغ المصروفات أكبر من مبلغ السلفة النقدية                                                                                                                                                                          |
| السفر والمصروفات                | [509556](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509556)            | معلومات معرف المشروع ضمن تقرير مصروفات بين الشركات الشقيقة فارغه إذا تم تعيين دور المستخدم لمؤسسه معينه                                                                                                                                           |
| السفر والمصروفات                | [513845](https://fix.lcs.dynamics.com/Issue/Details/?bugId=513845)            | سير عمل الترحيل التلقائي لتقرير المصروفات مكتمل لكن لم يتم ترحيل الفاتورة                                                                                                                                                                                          |

### <a name="regulatory-updates"></a>التحديثات التنظيمية
لمزيد من المعلومات حول التحديثات التنظيمية لتطبيقات Finance and Operations، راجع [التحديثات التنظيمية](https://docs.microsoft.com/dynamics365/finance/localizations/regulatory-updates). يمكنك أيضًا تسجيل الدخول إلى LCS وعرض التحديثات التنظيمية المخططة باستخدام أداة البحث عن المشاكل. تتيح لك عملية البحث عن المشاكل بالبحث حسب البلد ونوع الميزة والإصدار.