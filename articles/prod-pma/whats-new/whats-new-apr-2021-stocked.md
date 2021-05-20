---
title: الجديد أو المتغير في Project Operations، أبريل 2021 للسيناريوهات المستندة إلى المنتجات المخزنة/الإنتاج
description: يوفر هذا الموضوع معلومات حول تحديثات الجودة المتوفرة في إصدار أبريل 2021 من Project Operations للسيناريوهات المستندة إلى المنتجات المخزنة/الإنتاج‬.
author: andchoi
manager: tfehr
ms.date: 04/22/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: andchoi
ms.openlocfilehash: 2e2e3c1c717b5296964e0921aeec4999dd2f6e29
ms.sourcegitcommit: 69fadd3ce475d6aed2e1ed81a15becb28f020eb9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2021
ms.locfileid: "5935548"
---
# <a name="whats-new-or-changed-in-project-operations-april-2021-for-stockedproduction-based-scenarios"></a>الجديد أو المتغير في Project Operations، أبريل 2021 للسيناريوهات المستندة إلى المنتجات المخزنة/الإنتاج

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى المنتجات المخزنة/الإنتاج_

ينطبق هذه الموضوع على مكونات وإصدارات Dynamics 365 Project Operations التالية:

- إدارة المشاريع والمحاسبة في الإصدار 10.0.18 من بيئة Dynamics 365 Finance
 
### <a name="quality-updates"></a>التحديثات الإصلاحية
                                                                                                                                                                                  
| منطقة الميزات                      | رقم المرجع| تحديث إصلاحي                                                                                                                                                                          |
|-----------------------------------|--------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| إدارة المشاريع والمحاسبة | [534393](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534393) | يحدث خطأ في شبكة **فرز المشروع**.                                                                                                                                                      |
| إدارة المشاريع والمحاسبة | [542850](https://fix.lcs.dynamics.com/Issue/Details/?bugId=542850) | يتم زيادة تقدير المبلغ المتعهد بعد تصحيح سعر الوحدة والكمية في أمر شراء مشروع.                                                                                    |
| إدارة المشاريع والمحاسبة | [543645](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543645) | يتم التصريح عن المتغير **ProjParameters** ولكن لا يتم تعيينه أبدا للتخزين المؤقت للسجل قبل استخدامه.                                                                                     |
| إدارة المشاريع والمحاسبة | [543674](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543674) | يتم حذف جداول **ResRollup** عند تنفيذ مهمة الدُفعة **توزيع موارد المشروع عبر جميع الشركات**.                                                                          |
| إدارة المشاريع والمحاسبة | [544417](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544417) | هناك مشكلة عند تحديث حقل **سعر مبيعات المشروع** في أمر شراء باستخدام الكيان **سطور أمر الشراء V2**.                                                                           |
| إدارة المشاريع والمحاسبة | [547652](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547652) | بناء على أرقام المعرف، لا يمكن إنشاءات مشاريع فرعية.   يحدث الخطأ التالي، “الوظيفة العمومية::int642int تم استدعاؤها بشكل غير صحيح."                                         |
| إدارة المشاريع والمحاسبة | [484274](https://fix.lcs.dynamics.com/Issue/Details/?bugId=484274) | يتلقى العميل حسابات خاطئة عند فوترة أمر شراء بفئة شراء وصنف على نفس الفاتورة.                                                                      |
| إدارة المشاريع والمحاسبة | [509920](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509920) | لا يؤدي تعديل معاملة المشروع بالتكاليف غير المباشرة من قابلة للفوترة إلى غير قابل للفوترة ثم العودة إلى قابلة للفوترة إلى تسوية الأعمال قيد التنفيذ بشكل صحيح.                                       |
| إدارة المشاريع والمحاسبة | [511274](https://fix.lcs.dynamics.com/Issue/Details/?bugId=511274) | تكون مبالغ الفاتورة غير صحيحة عند استخدام الاحتفاظ والخصم الإجمالي في أمر المبيعات.                                                                                          |
| إدارة المشاريع والمحاسبة | [511315](https://fix.lcs.dynamics.com/Issue/Details/?bugId=511315) | لا يتم تغيير اسم العنوان في تفاصيل السطر حتى عند تحديد نوع معاملة مختلف.                                                                           |
| إدارة المشاريع والمحاسبة | [522983](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522983) | التكاليف الملتزم بها مع متطلبات الصنف وأمر الشراء هي غير صحيحة في عملية فوترة أوامر الشراء مع إيصال منتج جزئي وفوترة جزئية.                       |
| إدارة المشاريع والمحاسبة | [524226](https://fix.lcs.dynamics.com/Issue/Details/?bugId=524226) | عند تغيير أبعاد المشروع المالية، فإن رأس أمر الشراء لا يعكس التغييرات.                                                                                                  |
| إدارة المشاريع والمحاسبة | [524979](https://fix.lcs.dynamics.com/Issue/Details/?bugId=524979) | تقرير **مشروع السعر الثابت** الذي تم إنشاؤه فارغ.                                                                                                         |
| إدارة المشاريع والمحاسبة | [529445](https://fix.lcs.dynamics.com/Issue/Details/?bugId=529445) | لا تلتقط الفاتورة مرجع "معرف المشروع" عند مراجعة بنود فواتير المورّدين في صفحة **الدفع عند الاستلام**.                                                                          |
| إدارة المشاريع والمحاسبة | [529982](https://fix.lcs.dynamics.com/Issue/Details/?bugId=529982) | إدخال الجدول الزمني غير صحيح للمستخدم الذي يكون وصوله مقيد لأحد الكيانات القانونية في دور **مدير الموارد البشرية**، حيث لم يتم تعيين الفئة افتراضيًا بشكل صحيح.                                         |
| إدارة المشاريع والمحاسبة | [530008](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530008) | لا يؤخذ في الاعتبار تاريخ المشروع الأصلي في عملية تعديل، مما يتسبب في حدوث خطأ عند تعيين الحقل **استخدام تاريخ التعديل كتاريخ مشروع جديد** إلى **لا**.                                             |
| إدارة المشاريع والمحاسبة | [530788](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530788) | عند حساب تقديرات المشروع باستخدام دفعة، تكون النتائج غير صحيحة.                                                                                                         |
| إدارة المشاريع والمحاسبة | [530834](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530834) | المبلغ المنفق في عقد المشروع لا ينسجم مع المبلغ المستحق على الحساب في المشروع.                                                                             |
| إدارة المشاريع والمحاسبة | [530883](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530883) | يتعذر على أدوار محاسب المشروع ومدير المشروع إنشاء دفاتر يومية ساعات من خلال إعداد مجموعة الموافقة.                                                                                 |
| إدارة المشاريع والمحاسبة | [531974](https://fix.lcs.dynamics.com/Issue/Details/?bugId=531974) | لا يمكن ترحيل دفتر يومي المصروفات المستوردة من Microsoft Excel.                                                                                                                                       |
| إدارة المشاريع والمحاسبة | [532548](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532548) | السماح بعكس معاملات المورد من السيناريوهات المشتركة بين الشركات الشقيقة، بما في ذلك تقارير فواتير الموردين والمصروفات.                                                                     |
| إدارة المشاريع والمحاسبة | [533426](https://fix.lcs.dynamics.com/Issue/Details/?bugId=533426) | لا تقوم عملية تعديل المشروع بتحديث مبلغ المبيعات بشكل صحيح بالتكاليف غير المباشرة.                                                                                                    |
| إدارة المشاريع والمحاسبة | [534869](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534869) | عندما يتم إنشاء إشعار دائن لفاتورة مشروع ثابت السعر وتستخدم وحدة قاعدة فوترة التسليم، لا تكون الوحدات التي تم إصدارها متوفرة لإعادة الفوترة. |
| إدارة المشاريع والمحاسبة | [535428](https://fix.lcs.dynamics.com/Issue/Details/?bugId=535428) | لا يقوم عقد مشروع بعملة مختلفة بحساب عملة المحاسبة بشكل صحيح في دفتر يومية البند أو مقترح الفاتورة.                                                   |
| إدارة المشاريع والمحاسبة | [537158](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537158) | تغيير المشروع في سطر أمر الشراء لنقل متطلب العنصر.                                                                                                                          |
| إدارة المشاريع والمحاسبة | [540603](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540603) | يؤدي الاستيراد إلى موازنة مشروع من التوقعات إلى مبالغ غير صحيحة.                                                                                                                    |
| إدارة المشاريع والمحاسبة | [540622](https://fix.lcs.dynamics.com/Issue/Details/?bugId=5406222) | لا يتم إنشاء إدخالات دفتر الأستاذ العام عند تعديل الحركات من قابلة للفوترة إلى غير قابلة للفوترة.                                                                                            |
| إدارة المشاريع والمحاسبة | [540633](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540633) | لا يتم إنشاء حركات المشروع مع الدفع عند الاستلام عند تشغيل مفتاح الميزة، **تمكين ميزة حساب مبلغ التكلفة لمدة احتجاز فواتير مورّد المشروع**.                  |
| إدارة المشاريع والمحاسبة | [541421](https://fix.lcs.dynamics.com/Issue/Details/?bugId=541421) | مشاكل متعددة في صفحة **إنشاء اقتراح الفاتورة**.                                                                                                                             |
| إدارة المشاريع والمحاسبة | [543390](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543390) | لا تعرض صفحة **كافة المشروعات** قائمة برمز اللغة الجديد.                                                                                                            |
| إدارة المشاريع والمحاسبة | [543803](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543803) | مبلغ الميزانية غير الموافقة عليه في رصيد موازنة المشروع يكون غير صحيح عند مراجعة الموازنة أكثر من مرتين.                                                                |
| إدارة المشاريع والمحاسبة | [543968](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543968) | صفحة **اتفاقية الشراء** غير مرئية في الكيانات القانونية لـ Finance المتكاملة مع Project Operations.                                                                               |
| إدارة المشاريع والمحاسبة | [545456](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545456) | لا يتم تحميل تاريخ الإيصال الصحيح إلى سطور دفتر اليومية بالساعات.                                                                                                            |
| إدارة المشاريع والمحاسبة | [545878](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545878) | في السيناريوهات المعتمدة على الموارد في Project Operations، لا يمكنك تحويل عرض أسعار إلى فائز بسبب خطأ في التكامل.                                                                      |
| إدارة المشاريع والمحاسبة | [546604](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546604) | في Project Operations، تحصل على رسالة خطأ عندما تحاول إنشاء إقران بين شرط تعاقد ومعرف مشروع بسبب التحقق من شروط التعاقد المتراكبة وأنواع الحركات.                        |
| إدارة المشاريع والمحاسبة | [546949](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546949) | صفحة **مجموعات التحقق من صحة الموارد/المشروع** بها مشاكل في الأداء عندما يكون هناك أكثر من 14000 سجل في جدول **ProjValEmplProjSetup**.                                                                     |
| إدارة المشاريع والمحاسبة | [547440](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547440) | بإمكان **ProjCDSProjectContractEntity** تعيين عنوان فاتورة مصدر التمويل من عميل مختلف.                                                                                   |
| إدارة المشاريع والمحاسبة | [547606](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547606) | لا يتوفر البحث القياسي للمورد بعد الإصدار 10.0.15.                                                                                          |
| إدارة المشاريع والمحاسبة | [547831](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547831) | عدم تطابق حساب دفتر الحسابات ونوع النشر في إيصال فاتورة أمر الشراء لعنصر الخدمة. تم تعيين مجموعة المشروع إلى **موازنة** وحساب دفتر الأستاذ العام غير صحيح.                   |
| إدارة المشاريع والمحاسبة | [550030](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550030) | لا يظهر رقم النشاط لفاتورة مورّد معلقة، حتى عند تعيين **حظر تحديد النشاط الأصلي** إلى **لا**.                                            |
| إدارة المشاريع والمحاسبة | [550379](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550379) | عند استخدام مسار التنقل، **المشروع** > **الموازنة** > **المراجعات** > **جديد** > **استيراد**، يقوم النظام بإنشاء مراجعة موازنة مشروع لجميع المشاريع                                                            |
| إدارة المشاريع والمحاسبة | [550577](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550577) | ويحدث النشر الخطأ وإدخالات دفتر الحسابات الأستاذ العام عند تعديل حركة بعملات حركة ومحاسبة مختلفة.                                                                        |
| إدارة المشاريع والمحاسبة | [557376](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557376) | لا يتم تضمين أية أبعاد عند إنشاء فاتورة ترحيل للحركة.                                                                                                   |
| إدارة المشاريع والمحاسبة | [559416](https://fix.lcs.dynamics.com/Issue/Details/?bugId=559416) | يتم استدعاء الأسلوب **PurchTotals.purchNewTotalAmount()** عند إنشاء فاتورة مورد معلقة، والتي لا ترتبط بأي أمر شراء ما يتسبب في مشكلة في الأداء.                    |
| السفر والمصروفات                | [480451](https://fix.lcs.dynamics.com/Issue/Details/?bugId=480451) | هناك خطأ في الترحيل متعلق بإعداد المسافة المقطوعة بالميل.                                                                                                                                          |
| السفر والمصروفات                | [522084](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522084) | لا يعمل **الانفصال إلى شخصي** لمعاملات مصروفات العملة الخارجية.                                                                                                         |
| السفر والمصروفات                | [523938](https://fix.lcs.dynamics.com/Issue/Details/?bugId=523938) | تعرض القائمة المنسدلة لفئة المصروفات الفئات غير الصحيحة بغض النظر عما إذا كان قد تم إعداد **التفويضات** كمورد أم لا.                                         |
| السفر والمصروفات                | [539266](https://fix.lcs.dynamics.com/Issue/Details/?bugId=539266) | لا يمكنك حفظ تقرير حساب بين الشركات الشقيقة نظرًا لخطأ التحقق من صحة المورد/الفئة.                                                                                             |
| السفر والمصروفات                | [532610](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532610) | يتضمن حساب معدل المسافة الخطأ في ترحيل تقرير مصروفات أسطر تقسيم.                                                                                                        |
| السفر والمصروفات                | [537404](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537404) | لا يمكنك ترحيل تقرير مصروفات بين الشركات الشقيقة عندما يتم تضمين ضريبة المبيعات وكان نوع حساب الإزاحة في طريقة الدفع هو **العامل**.                                                   |
| السفر والمصروفات                | [542927](https://fix.lcs.dynamics.com/Issue/Details/?bugId=542927) | التراجع عن التغييرات في كيان بيانات **TrvRequisitionLine** والفهرس الفريد المرتبط بالكيان.                                                                                            |
| السفر والمصروفات                | [543239](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543239) | يتم إضافة تسجيل الدخول في نقاط معينة في تقرير مصروفات لدعم إنشاء وتحديث أسطر المستندات المصدر.                                                                                           |
| السفر والمصروفات                | [544323](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544323) | يتم عرض دفتر يومية دفتر الأستاذ الفرعي الخاطئ في سيناريوهات بين الشركات الشقيقة إذا تم ترحيل ضريبة المبيعات إلى الكيان القانوني الوجهة.                                              |
| السفر والمصروفات                | [546877](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546877) | في Project Operations، لا يتم حذف تقديرات المصروفات من Finance عند حذفها من Dataverse.                                                                                         |
| السفر والمصروفات                | [550575](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550575) | عندما تكون فئة مصروفات فئة غير خاصة بمشروع، لا يتم نسخ البُعد المالي المحدد في صفحة **المصروفات** إلى تقرير المصروفات.                                          |

### <a name="regulatory-updates"></a>التحديثات التنظيمية
لمزيد من المعلومات حول التحديثات التنظيمية لتطبيقات Finance and Operations، راجع [التحديثات التنظيمية](/dynamics365/finance/localizations/regulatory-updates). يمكنك أيضًا تسجيل الدخول إلى LCS وعرض التحديثات التنظيمية المخططة باستخدام أداة البحث عن المشاكل. تتيح لك عملية البحث عن المشاكل بالبحث حسب البلد ونوع الميزة والإصدار.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]