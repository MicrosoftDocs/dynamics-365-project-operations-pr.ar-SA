---
title: إعداد معدلات فواتير العمالة
description: يقدم هذا الموضوع معلومات حول كيفية إعداد معدلات فواتير العمالة في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/16/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e6294895857442f3a24a9d73ee07d2b90926a4fb
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070706"
---
# <a name="setting-up-bill-rates-for-labor-rate-billing"></a>إعداد معدلات الفواتير لفوترة معدل العمالة 

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_

تشتمل كل قائمة أسعار على مجموعة من أسعار الأدوار أو معدلات العمالة التي تعتبر فعالة للسياق وسريان التاريخ المضمن على رأس قائمة الأسعار. يمكن إعداد معدلات الفواتير للوقت في Dynamics 365 Project Operations بعملة واحدة فقط، وهي العملة في رأس قائمة الأسعار.

1. لإعداد معدلات فواتير العمالة لقائمة أسعار المبيعات، أنشئ قائمة أسعار تستند إلى رأس قائمة الأسعار. 
2. على علامة التبويب **أسعار الأدوار** ، في الشبكة الفرعية، حدد **‎+ سعر دور جديد**. 
3. في جزء **الإنشاء السريع** ، أدخل مجموعة الدور والوحدة التنظيمية التي تريد إعداد معدل الفاتورة لها.

  يتضمن الجدول التالي الحقول الموجودة على علامة التبويب **عام** وجزء **الإنشاء السريع** لبند سعر الدور الذي ينبغي عليك وضعه في الاعتبار عند إنشاء أسعار الأدوار في قائمه أسعار المبيعات:

  | الحقل | الموقع | الصلة والغرض والإرشاد | تأثير لاحق |
  | --- | --- | --- | --- |
  | الدور | علامة التبويب **عام** وجزء **الإنشاء السريع** | حدد الدور الذي تقوم بتعيين سعر الفاتورة له. | ستتم مطابقة الدور على التقدير أو القيمة الفعلية الواردة في مقابل هذا البند لتعيينه بشكل افتراضي إلى معدل فاتورة الدور. |
  | وحدة تعيين الموارد | علامة التبويب **عام** وجزء **الإنشاء السريع** | حدد الوحدة التنظيمية أو القسم الخاص بالشركة التي يأتي الدور منها. على سبيل المثال، مطور من قسم Robotics في شركة Fabrikam India أو مطور من قسم Software في شركة Fabrikam USA. | ستتم مطابقة وحدة تعيين الموارد على التقدير أو القيمة الفعلية الواردة في مقابل هذا البند لتعيينه بشكل افتراضي إلى معدل فاتورة الدور. |
  | السعر | علامة التبويب **عام** وجزء **الإنشاء السريع** | قم بإعداد معدل الفاتورة لمجموعة شركة تعيين الموارد ووحدة تعيين الموارد للدور. على سبيل المثال، مطور من شركة Fabrikam India لديه معدل فاتورة من 100 دولار أمريكي ومطور من شركة Fabrikam USA لديه معدل فاتورة من 150 دولار أمريكي. | يمثل هذا السعر معدل الفاتورة الافتراضي على السعر لكل وحدة لبند التقدير أو القيمة الفعلية الواردة لفئة حركة الوقت. |
  | ‏‏العملة | علامة التبويب **عام** وجزء **الإنشاء السريع**| بشكل افتراضي، تأتي قيمة العملة من العملة على رأس قائمة أسعار المبيعات. في قائمه أسعار المبيعات، لا يمكن تجاوز العملة. | تمثل هذه العملة الافتراضية على السعر لكل وحدة لبند المبيعات الفعلي الوارد لفئة حركة الوقت. |
  | جدول الوحدات | علامة التبويب **عام** وجزء **الإنشاء السريع** | يتم تعيين جدول الوحدة هذه إلى الوقت بشكل افتراضي، ولا يمكن تغييره على كيان سعر الدور بسبب استخدامه للتعبير عن الأسعار حسب الوحدات الزمنية. | لا يوجد تأثير لاحق لهذا الحقل. |
  | الوحدة | علامة التبويب **عام** وجزء **الإنشاء السريع** | تأتي قيمة الوحدة من حقل **الوحدة الزمنية** على رأس قائمة أسعار المبيعات. ولكن يمكن تجاوز القيمة. على سبيل المثال، مطور من شركة Fabrikam India لديه معدل فاتورة من 100 دولار أمريكي حسب **اليوم في الهند**. مطور من شركة Fabrikam USA لديه معدل فاتورة من 1500 دولار أمريكي حسب‬ **اليوم في الولايات المتحدة**. | عندما يتم تعيين السعر لكل وحدة بشكل افتراضي على بند تقدير أو بند قيمة فعلية وارد، يقوم النظام باستخدام نظام الوحدات والتحويل بالوحدات الأساسية لحساب السعر لكل وحدة. على سبيل المثال، التقدير يساوي 10 من **الأيام في الهند** كأيام عمل لمطور من الهند، والوحدة "يوم في الهند" محددة بعشر ساعات. عندما تقوم بتسعير بند التقدير هذا، يقوم التطبيق بحساب سعر الوحدة على التقدير على أنه 1000 دولار أمريكي/ 10 ساعات = 100 دولار أمريكي للساعة. |


## <a name="transfer-pricing-or-set-up-bill-rates-for-resources-from-other-organizational-units-or-divisions"></a>تحويل التسعير أو إعداد أسعار الفاتورة للموارد من الوحدات التنظيمية أو الأقسام الأخرى 

تستخدم الشركات القائمة على المشاريع الموظفين من مختلف أٌقسام الشركة للعمل على المشروع. ويمكن تنفيذ المشاريع من قسم واحد في حين يأتي الموظفون أو المستشارون من قسم مختلف من أقسام الشركة. كما يمكن أن يتكوّن المشروع من مجموعة من الأشخاص من أقسام مختلفة. في Project Operations، تسمى الشركة التي تملك تسليم المشروع **وحدة التعاقد**. وتمسى كافة الأقسام الأخرى التي توفر الموارد **وحدات تعيين الموارد**. نظرًا للاختلافات في تكاليف العمالة عبر العديد من المناطق الجغرافية وأسواق العمالة في جميع أنحاء العالم، يتم أيضًا إعداد معدلات الفواتير للعمالة بشكل مختلف لمختلف المناطق الجغرافية.

على سبيل المثال، تتم فوترة مطور من شركة Fabrikam India يعمل على مشروع أمريكي بمعدل 100 دولار أمريكي في الساعة. تتم فوترة مطور من شركة Fabrikam US يعمل على مشروع أمريكي بمعدل 150 دولار أمريكي في الساعة.

### <a name="example-set-up-a-bill-rate"></a>مثال: إعداد معدل الفاتورة

1. قم بإنشاء قائمة أسعار مبيعات تسمى *معدلات الفواتير في Fabrikam US* ، وعيّن تاريخ السريان.
2. في قائمة أسعار المبيعات، أدخل معلومات المعدلات التالية:

    | الدور | الوحدة التنظيمية | معدل الفاتورة |
    | --- | --- | --- |
    | المطور | Fabrikam India | 100 دولار أمريكي |
    | المطور | Fabrikam Philippines | 90 دولارًا أمريكيًا |
    | المطور | Fabrikam US | 150 دولارًا أمريكيًا |

3. قم بإرفاق قائمة أسعار المبيعات، **معدلات الفواتير في Fabrikam US** بقائمة أسعار المشروع لعقد المشروع أو بحساب معين.