---
title: تغييرات الميزة من Project Service Automation إلى Project Operations
description: يوفر هذا المقال نظرة عامة على تغييرات الميزات من Project Service Automation إلى Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 8a6030faf777051ea1003679589af4bdf97322ab
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925334"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>تغييرات الميزة من Project Service Automation إلى Project Operations

سيتم تسليم الترقية من Dynamics 365 Project Service Automation إلى Dynamics 365 Project Operations Lite على ثلاث مراحل. يوفر هذا المقال معلومات حول التغييرات الرئيسية التي يمكن أن تتوقع رؤيتها عند اكتمال الترقية.

| تسليم الترقية | المرحلة 1 <br>(يناير 2022) | المرحلة 2 <br>(موجة أبريل 2022) | المرحلة 3  |
|------------------|------------------------|---------------------------|---------------------------|
| لا تبعية على هيكل تنظيم العمل (WBS) للمشاريع. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| هيكل تنظيم العمل (WBS) مضمن في الحدود المدعومة حاليًا في Project Operations. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| هيكل تنظيم العمل (WBS) خارج الحدود المدعومة حاليًا في Project Operations، بما في ذلك دعم Project Desktop Client. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>إدارة المشروع

ستكون أهم التغييرات في تجربة المستخدم في مجال تخطيط المشروع. يتبنى Project Operations تجربة حديثة جديدة لإدارة هيكل توزيع العمل (WBS) من خلال الاستفادة من إمكانيات الجدولة التي توفرها [Project for the Web](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>الاختلافات في تجربة الجدولة

يلخص الجدول التالي اختلافات الجدولة بين Project Service Automation وProject Operations.

|  جدولة      |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| قوالب المشروع - القدرة على تحديد وتطبيق قوالب المشروع عند إنشاء المشروع  |  &nbsp;    | :heavy_check_mark: |
| تكامل هيكل تنظيم العمل (WBS) للمشروع مع عميل سطح المكتب   |    &nbsp;  | :heavy_check_mark: |
| القيود - لا تبدأ قبل ذلك، وتنتهي في موعد لا يتجاوز  | :heavy_check_mark: |   &nbsp;  |
| الأحداث الرئيسية - المهام ذات المدة الصفرية   | :heavy_check_mark:  |  &nbsp;  |
| ستحترم المهام القائمة على الموارد توافر الموارد المخصصة   | :heavy_check_mark: |  &nbsp;    |
| التحرير على مراحل زمنية - تحرير الخطط والعمل على أساس يومي   |   &nbsp;  | :heavy_check_mark: |
| الجدولة التلقائية / اليدوية - استخدم محرك جدولة المشروع لجدولة المهام تلقائيًا أو يدويًا |  &nbsp; | :heavy_check_mark:  |
| تحرير المشاريع الكبيرة مباشرة في واجهة المستخدم: لا يوجد حد لحجم الخطط القابلة للتحرير  | 500 مهمة كحد أقصى  | :heavy_check_mark:       |
| النسبة المئوية للاكتمال - وضع علامة على تقدم المهمة   | :heavy_check_mark:  |  &nbsp;  |
| [أوضاع جدولة المشروع](../project-management/scheduling-modes.md) - تعريف المشروع على أنه وحدات ثابتة أو جهد ثابت أو مدة ثابتة | :heavy_check_mark: | &nbsp; |
| المخطط الزمني - قم بإنشاء طريقة عرض المخطط الزمني وتخصيصها لعرض تفاصيل الجدول الزمني والتواصل مع أصحاب المصلحة. | :heavy_check_mark:  | &nbsp; |
| المهام المستندة إلى الجهد - جدولة دعم المحرك لجدولة مهمة مستندة إلى الجهد  | :heavy_check_mark:  | &nbsp; |
| مربع حوار **معلومات المهمة** - حفظ تفاصيل المهمة باستخدام مربع حوار | :heavy_check_mark:  |  &nbsp;  |
| السحب والإفلات - مهام متعددة التحديد وتعديل موضعها على WBS | :heavy_check_mark: | &nbsp;  |
| طرق العرض الثابتة المرنة - تحديد طرق عرض أكثر تفصيلاً لسمات المهمة   | :heavy_check_mark:  | &nbsp; |
| فرز WBS وتصفيتها  | :heavy_check_mark:  | &nbsp; |
| عرض اللوحات لتسليم المشروع غير المتدفق  | :heavy_check_mark:   | &nbsp; |
| عرض المخطط الزمني - مخطط جانت التفاعلي المستخدم لتصور WBS وتحريره   | :heavy_check_mark:  | &nbsp; |
| اختصارات لوحة المفاتيح - استخدم اختصارات لوحة المفاتيح للعمليات الشائعة، مثل مسافة بادئة أو إدراج  | :heavy_check_mark:  |  &nbsp; |
| التراجع متعدد المستويات - إجراء تحليل ماذا لو لفهم تأثير التغييرات بشكل كامل عن طريق عكس مجموعة كاملة من العمليات وإعادة تطبيقها | :heavy_check_mark: | &nbsp; |
| قص / نسخ / لصق - التعاون في تطوير الجدول الزمني عن طريق نسخ تفاصيل الجدول الزمني ولصقها بين التطبيقات  | :heavy_check_mark: | &nbsp; |
| قوائم اختيار المهام - أضف ما يصل إلى 20 عنصر من عناصر قائمة الاختيار إلى مهمة ما   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>تخطيط المشروع

تحتوي صفحة **المشروع** في Project Operations على عدد كبير من الاختلافات مقارنة بصفحة **المشروع** في Project Service Automation.

تمت إزالة الإجراءات التالية من صفحة **المشروعات** كجزء من ترقية المرحلة 1:

  - **فتح في MS Project**
  - **إنشاء قالب**
  - **إلغاء ربط المشروع من MS Project**

وتتضمن صفحة **المشروع** في Project Operations علامات التبويب الجديدة التالية.

- **تقديرات المواد**
- **إعداد فوترة المهام**

تمت إزالة علامة تبويب **الحالة** وحقل **الحالة** الآن في علامة تبويب **الملخص** مع وضع الجدولة الخاص بالمشروع.

   ![تحديثات صفحة المشروع.](media/projectform.png)

تمت إعادة تسمية علامة تبويب **الجدولة** إلى علامة تبويب **المهمة** وتتميز بخبرة تخطيط المشروع الجديدة مع Project for the Web.

   ![علامة تبويب مهام المشروع الجديدة.](media/tasktab.png)

## <a name="scheduling-modes"></a>أوضاع الجدولة

قدمت Project Operations ميزة جديدة، [أوضاع الجدولة](../project-management/scheduling-modes.md). سيتم تعيين كافة مشروعات Project Service Automation الموجودة بشكل افتراضي إلى **مدة ثابتة** في Project Operations. ومع ذلك، يمكن إدارة الإعداد الافتراضي للمشروعات الجديدة عن طريق الانتقال إلى **الإعدادات** > **المعلمات** > **المعلمة** > **وضع الجدولة**.

   ![إعدادات معلمات المشروع لوضع الجدولة.](media/projectparameter.png)

## <a name="project-planning-limits"></a>حدود تخطيط المشروع

تعتمد Project Operations على Project for the Web لجميع عمليات جدولة المشروع. يدير Project for the Web هيكل تنظيم العمل باستخدام الحدود الموضحة في الجدول التالي.

| **الحقل**                                          | **حد**             |
|----------------------------------------------------|-----------------------|
| الحد الأقصى لإجمالي المهام لمشروع                  | 500                   |
| الحد الأقصى لإجمالي المدة لمشروع               | 3650 يومًا (10 سنوات)  |
| الحد الأقصى لإجمالي الموارد لمشروع              | 300                   |
| الحد الأقصى لإجمالي الارتباطات (اللاحقة فقط) لمشروع | 600                   |
| الحد الأقصى لإجمالي الحقول المخصصة لمشروع          | 10                    |
| الحد الأقصى لمستوى التدرج الهرمي                            | 10 مستويات             |
| الحد الأقصى للارتباطات (اللاحقة + السابقة)            | 20                    |
| الحد الأقصى لمدة المهمة الطرفية                      | 1250 يومًا             |
| الحد الأقصى لمدة مهمة الملخص                 | 3650 يومًا (10 سنوات)  |
| الحد الأقصى للموارد المعينة لمهمة               | 20 مورد          |
| نطاق التاريخ المعتمد لمهمة                    | 1/1/2000 - 12/31/2149 |
| عناصر قائمة الاختيار                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>التوسع في تخطيط المشروع وتطويره

بعد الترقية إلى Project Operations، يجب عليك استخدام واجهات برمجة تطبيقات جدولة المشروع لتنفيذ عمليات الإنشاء والتحديث والحذف على الكيانات التالية:

|   اسم الكيان           |   اسم منطقي للكيان       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| مهمة المشروع            | msdyn_projecttask           |
| تبعية مهمة المشروع | msdyn_projecttaskdependency |
| تعيين المورد     | msdyn_resourceassignment    |
| مستودع المشروع          | msdyn_projectbucket         |
| عضو فريق المشروع     | msdyn_projectteam           |

إذا كان لديك حاليًا تخصيصات تتضمن هذه الكيانات، فراجع [استخدام واجهات برمجة تطبيقات جدولة المشروع لإجراء عمليات باستخدام كيانات الجدولة](../project-management/schedule-api-preview.md) للحصول على إرشادات التنفيذ.

## <a name="data-model-changes"></a>تغييرات نموذج البيانات

كجزء من مرحلة الترقية 1، هناك تغييرات في نموذج البيانات. هذه التغييرات هي في الأساس تغييرات في الحقول للكيانات الحالية. في المرحلة 1، الكيانات **msydn_project** و **msdyn_projectteam** هي إعادة هيكلة التخصيصات. 

> [!IMPORTANT]
> سيتم تحديث هذا القسم بكيانات إضافية مع اكتمال مراحل الترقية المستقبلية.

تم استبدال الحقول التالية بحقول جديدة.

|   الكيان           |   الاسم المنطقي القديم   |   الاسم المنطقي الجديد    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

تمت إضافة الحقول التالية.

|   الكيان           |   الاسم المنطقي                               |   الوصف  |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | عرض تجميع مبيعات الرسوم الفعلية في المشروع. للاستخدام في Project Service Automation فقط. |
| msdyn_project     | msdyn_actualmaterialcost                     | عرض تجميع تكلفة المواد الفعلية في المشروع. للاستخدام في Project Service Automation فقط. |
| msdyn_project     | msdyn_actualmaterialsales                    | عرض تجميع مبيعات المواد الفعلية في المشروع. للاستخدام في Project Service Automation فقط. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | شروط التعاقد المقترنة بهذا المشروع. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | هذا حقل نظام داخلي، يُستخدم لـ **نسخ المشروع** المرتبط بمعرف الارتباط. للاستخدام في Project Service Automation فقط. |
| msdyn_project     | msdyn_copyprojectsessionid                   | هذا حقل نظام داخلي، يُستخدم لـ **نسخ المشروع** المرتبط بمعرف جلسة العمل. للاستخدام في Project Service Automation فقط. |
| msdyn_project     | msdyn_globalrevisiontoken                    | آخر مزامنة للرمز المميّز لمراجعة xRM العامة من خدمة جدولة المشروع. |
| msdyn_project     | msdyn_msprojectdocument                      | مستند Microsoft Project الذي ينتمي إلى المشروع. |
| msdyn_project     | msdyn_plannedmaterialcost                    | تجميع تكلفة المواد المخططة في المشروع. للاستخدام في Project Service Automation فقط. |
| msdyn_project     | msdyn_plannedmaterialsales                   | تجميع مبيعات المواد المخططة في المشروع. للاستخدام في Project Service Automation فقط. |
| msdyn_project     | msdyn_program                                | البرنامج الذي يرتبط به هذا السجل. |
| msdyn_project     | msdyn_quotelineproject                       | بند عرض الأسعار المقترن بهذا المشروع. |
| msdyn_project     | msdyn_replaylogheader                        | عنوان سجلات إعادة التشغيل. |
| msdyn_project     | msdyn_schedulemode                           | وضع الجدولة الافتراضي المستخدم لجميع المهام في المشروع.  |
| msdyn_project     | msdyn_taskearlieststart                      | تاريخ البدء الأبكر لأي مهمة في المشروع.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | عضو فريق المشروع الذي تم نسخ عضو فريق المشروع هذا منه. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | يشير إلى ما إذا كان سيتم إنشاء متطلب المورد لعضو فريق عام تم إنشاؤه حديثا.  |
| msdyn_projectteam | msdyn_deletestatus                           | حاله الحذف لعضو الفريق لتعقب ما إذا كان هناك طلب حذف تم إرساله إلى خدمة جدولة المشروع وما إذا كانت ترسل الاستجابة مرة أخرى بنجاح وفي إطار الوقت المتوقع. |
| msdyn_projectteam | msdyn_effortcompleted                        | تتعقب مقدار الجهود التي بذلها عضو الفريق لتنفيذ المهام المعينة له. |
| msdyn_projectteam | msdyn_effortremaining                        | تتعقب الجهد الذي يتعين على عضو الفريق إكماله في المهام المعينة له. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | فترة الانتظار من الوقت الذي يرسل فيه عضو الفريق طلب حذف إلى خدمة جدولة المشروع حتى يتم حذف عضو الفريق فعليًا على Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | الطابع الزمني المراد تسجيله عند إرسال طلب حذف عضو الفريق إلى خدمة جدولة المشروع. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | عرض عضو فريق المشروع الذي تم نسخ عضو فريق المشروع هذا منه.  |

## <a name="project-templates"></a>قوالب المشروع

لا يوفر Project Operations دعمًا لقوالب المشروع. ومع ذلك ، يمكنك نسخ الكثير من الوظائف الأساسية باستخدام [واجهة برمجة تطبيقات نسخ المشروع](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>دعم الوظيفة الإضافية لسطح المكتب

لن يتوفر دعم الوظيفة الإضافية لتطبيق Microsoft Project لسطح المكتب في أول مرحلتين من الترقية. وفي المرحلة الثالثة، سيتمكن العملاء الذين لديهم مشروعات أكبر من حدود Project for the Web المدعومة حاليًا من استخدام الوظيفة الإضافة لسطح المكتب.

## <a name="editing-resource-assignment-contours"></a>يتم الآن تحرير مخططات تعيين الموارد

ستكون القدرة على تحرير ملامح تخصيص الموارد متاحة عند توفر المرحلة 2 من الترقية.

## <a name="billing-and-pricing"></a>الفوترة والتسعير

تمت إضافة الميزات الجديدة التالية في Project Operations. هذه الميزات مضافة بطبيعتها ولا تؤثر على نموذج بيانات Project Service Automation.

- [تسجيل استخدام المواد على المشاريع ومهام المشاريع](../material/material-usage-log.md)
- [إدارة التعاقد من الباطن‬](../pro/subcontracting/managing-subcontracts-overview.md)
- [إعداد السلف والعقود المستندة إلى مقدم الأتعاب](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [الحالات وعمليات من الصحة التي يجب ألا يتم تجاوزها في العقد](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [الفوترة القائمة على المهام](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>المكونات المهملة

توثق الجداول التالية جميع الحقول المهملة التي تم نقلها إلى حل المكونات المهملة بعد الترقية. لمزيد من المعلومات والارتباط بالحل، راجع [Dynamics 365 Project Service Automation 3x للمكونات المهملة لـ Project Operations 4x](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>invoicedetail

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinescheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_istemplate                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduleddurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocomplete                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicantsavailable                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hoursrequested                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinescheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransactioncategory.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_name                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>salesorderdetail

| الحقول                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

