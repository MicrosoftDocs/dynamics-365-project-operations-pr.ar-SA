---
title: استخدام واجهات برمجة تطبيقات الجدولة لتنفيذ عمليات مع كيانات الجدولة
description: يوفر هذا الموضوع معلومات و عينات لاستخدام واجهات برمجة تطبيقات الجدولة.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950788"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a>استخدام واجهات برمجة تطبيقات الجدولة لتنفيذ عمليات مع كيانات الجدولة

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

> [!IMPORTANT] 
> تتوفر بعض الوظائف المذكورة في هذا الموضوع أو كلها كجزء من إصدار أولي. إن المحتوى والوظائف خاضعة للتغيير. 

## <a name="scheduling-entities"></a>كيانات الجدولة

توفر واجهات برمجة تطبيقات جدولة القدرة على تنفيذ عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة**. تُدار هذه الكيانات من خلال محرك جدولة في المشروع للويب. كانت عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة** مقيدة في إصدارات Dynamics 365 Project Operations السابقة.

يوفر الجدول التالي قائمة كاملة تتضمن **كيانات الجدولة**.

| اسم الكيان  | اسم منطقي للكيان |
| --- | --- |
| Project | msdyn_project |
| مهمة المشروع  | msdyn_projecttask  |
| تبعية مهمة المشروع  | msdyn_projecttaskdependency  |
| تعيين المورد | msdyn_resourceassignment |
| مستودع المشروع  | msdyn_projectbucket |
| عضو فريق المشروع | msdyn_projectteam |

## <a name="operationset"></a>OperationSet

إن OperationSet عبارة نمط وحدة عمل يمكن استخدامه عندما يكون من الضروري معالجة طلبات متعددة تؤثر على الجدولة ضمن حركة.

## <a name="schedule-apis"></a>واجهات برمجة تطبيقات الجدولة

فيما يلي قائمة بواجهات برمجة تطبيقات الجدولة الحالية.

- **msdyn_CreateProjectV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء مشروع. يتم إنشاء مستودع المشروع والمشروع الافتراضي في الحال.
- **msdyn_CreateTeamMemberV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء عضو فريق مشروع. يتم إنشاء سجل عضو الفريق على الفور.
- **msdyn_CreateOperationSetV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لجدولة طلبات متعددة يجب تنفيذها ضمن حركة.
- **msdyn_PSSCreateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لإنشاء كيان. بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية الإنشاء.
- **msdyn_PSSUpdateV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لتحديث كيان. بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية التحديث.
- **msdyn_PSSDeleteV1**: يمكن استخدام واجهة برمجة التطبيقات هذه لحذف كيان. بإمكان الكيان أن يكون أياً من كيانات الجدولة التي تدعم عملية الحذف.
- **msdyn_ExecuteOperationSetV1**: يتم استخدام واجهة برمجة التطبيقات هذه لتنفيذ جميع العمليات ضمن مجموعة عمليات معينة.

## <a name="using-schedule-apis-with-operationset"></a>استخدام واجهات برمجة تطبيقات لجدولة مع OperationSet

نظرًا لاستخدام السجلات مع كل من **CreateProjectV1** و **CreateTeamMemberV1** على الفور، لا يمكن استخدام واجهات برمجة التطبيقات هذه في **OperationSet** بشكل مباشر. ومع ذلك، يمكنك استخدام واجهة برمجة التطبيقات لإنشاء السجلات المطلوبة، وإنشاء  **OperationSet**، ثم استخدام هذه السجلات المنشأة مسبقًا في **OperationSet**.

## <a name="supported-operations"></a>العمليات المدعومة

| كيان الجدولة | ‏إنشاء | تحديث | حذف  | اعتبارات هامة |
| --- | --- | --- | --- | --- |
مهمة المشروع | نعم  | نعم  | نعم  | ‏‫بلا |
| تبعية مهمة المشروع | نعم  | نعم  | | لا يتم تحديث سجلات تبعية مهمة المشروع. بدلاً من ذلك، يمكن حذف سجل قديم ويمكن إنشاء سجل جديد. |
| تعيين الموارد | نعم  | نعم  | | العمليات مع الحقول التالية غير مدعومة: **BookableResourceID** و **Effort** و **EffortCompleted** و **EffortRemaining** ة **PlannedWork**. لا يتم تحديث سجلات تعيين الموارد. بدلاً من ذلك، يمكن حذف السجل القديم ويمكن إنشاء سجل جديد. |
| مستودع المشروع | ‏‫غير متوفر‬ | ‏‫غير متوفر‬ | ‏‫غير متوفر‬ | يتم إنشاء المستودع الافتراضي باستخدام واجهة برمجة التطبيقات **CreateProjectV1**. |
| عضو فريق المشروع | نعم  | نعم  | نعم  | بالنسبة لعملية الإنشاء، استخدم واجهة برمجة التطبيقات **CreateTeamMemberV1**. |
| Project | نعم  | نعم  | ‏‫غير متوفر‬ | العمليات مع الحقول التالية غير مدعومة: **StateCode** و **BulkGenerationStatus** و **GlobalRevisionToken** و **CalendarID** و **Effort** و **EffortCompleted** و **EffortRemaining** و **Progress** و **Finish** و **TaskEarliestStart** و **Duration**. |

يمكن استدعاء واجهات برمجة التطبيقات مع كائنات الكيانات التي تتضمن حقولاً مخصصة.

خاصية المعرف اختيارية. إذا تم توفيرها، يحاول النظام استخدامها ويلقي استثناءً إذا لم يكن من الممكن استخدامها. إذا لم يتم توفيرها، سيقوم النظام بإنشائها.

## <a name="restricted-fields"></a>الحقول المقيدة

يُعرف الجداول التالي الحقول المقيدة من **الإنشاء** و **التحرير.**

### <a name="project-task"></a>مهمة المشروع

| **الاسم المنطقي**                       | **يمكن الإنشاء** | **يمكنه التحرير**     |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | ‏‏لا             | ‏‏لا               |
| msdyn_actualcost_base                  | ‏‏لا             | ‏‏لا               |
| msdyn_actualend                        | ‏‏لا             | ‏‏لا               |
| msdyn_actualsales                      | ‏‏لا             | ‏‏لا               |
| msdyn_actualsales_base                 | ‏‏لا             | ‏‏لا               |
| msdyn_actualstart                      | ‏‏لا             | ‏‏لا               |
| msdyn_costatcompleteestimate           | ‏‏لا             | ‏‏لا               |
| msdyn_costatcompleteestimate_base      | ‏‏لا             | ‏‏لا               |
| msdyn_costconsumptionpercentage        | ‏‏لا             | ‏‏لا               |
| msdyn_effortcompleted                  | ‏‏لا             | ‏‏لا               |
| msdyn_effortestimateatcomplete         | ‏‏لا             | ‏‏لا               |
| msdyn_iscritical                       | ‏‏لا             | ‏‏لا               |
| msdyn_iscriticalname                   | ‏‏لا             | ‏‏لا               |
| msdyn_ismanual                         | ‏‏لا             | ‏‏لا               |
| msdyn_ismanualname                     | ‏‏لا             | ‏‏لا               |
| msdyn_ismilestone                      | ‏‏لا             | ‏‏لا               |
| msdyn_ismilestonename                  | ‏‏لا             | ‏‏لا               |
| msdyn_LinkStatus                       | ‏‏لا             | ‏‏لا               |
| msdyn_linkstatusname                   | ‏‏لا             | ‏‏لا               |
| msdyn_msprojectclientid                | ‏‏لا             | ‏‏لا               |
| msdyn_plannedcost                      | ‏‏لا             | ‏‏لا               |
| msdyn_plannedcost_base                 | ‏‏لا             | ‏‏لا               |
| msdyn_plannedsales                     | ‏‏لا             | ‏‏لا               |
| msdyn_plannedsales_base                | ‏‏لا             | ‏‏لا               |
| msdyn_pluginprocessingdata             | ‏‏لا             | ‏‏لا               |
| msdyn_progress                         | ‏‏لا             | لا (نعم لـ P4W) |
| msdyn_remainingcost                    | ‏‏لا             | ‏‏لا               |
| msdyn_remainingcost_base               | ‏‏لا             | ‏‏لا               |
| msdyn_remainingsales                   | ‏‏لا             | ‏‏لا               |
| msdyn_remainingsales_base              | ‏‏لا             | ‏‏لا               |
| msdyn_requestedhours                   | ‏‏لا             | ‏‏لا               |
| msdyn_resourcecategory                 | ‏‏لا             | ‏‏لا               |
| msdyn_resourcecategoryname             | ‏‏لا             | ‏‏لا               |
| msdyn_resourceorganizationalunitid     | ‏‏لا             | ‏‏لا               |
| msdyn_resourceorganizationalunitidname | ‏‏لا             | ‏‏لا               |
| msdyn_salesconsumptionpercentage       | ‏‏لا             | ‏‏لا               |
| msdyn_salesestimateatcomplete          | ‏‏لا             | ‏‏لا               |
| msdyn_salesestimateatcomplete_base     | ‏‏لا             | ‏‏لا               |
| msdyn_salesvariance                    | ‏‏لا             | ‏‏لا               |
| msdyn_salesvariance_base               | ‏‏لا             | ‏‏لا               |
| msdyn_scheduleddurationminutes         | ‏‏لا             | ‏‏لا               |
| msdyn_scheduledend                     | ‏‏لا             | ‏‏لا               |
| msdyn_scheduledstart                   | ‏‏لا             | ‏‏لا               |
| msdyn_schedulevariance                 | ‏‏لا             | ‏‏لا               |
| msdyn_skipupdateestimateline           | ‏‏لا             | ‏‏لا               |
| msdyn_skipupdateestimatelinename       | ‏‏لا             | ‏‏لا               |
| msdyn_summary                          | ‏‏لا             | ‏‏لا               |
| msdyn_varianceofcost                   | ‏‏لا             | ‏‏لا               |
| msdyn_varianceofcost_base              | ‏‏لا             | ‏‏لا               |

### <a name="project-task-dependency"></a>تبعية مهمة المشروع

| **الاسم المنطقي**              | **يمكن الإنشاء** | **يمكنه التحرير** |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | ‏‏لا             | ‏‏لا           |
| msdyn_linktypename            | ‏‏لا             | ‏‏لا           |
| msdyn_predecessortask         | نعم            | ‏‏لا           |
| msdyn_predecessortaskname     | نعم            | ‏‏لا           |
| msdyn_project                 | نعم            | ‏‏لا           |
| msdyn_projectname             | نعم            | ‏‏لا           |
| msdyn_projecttaskdependencyid | نعم            | ‏‏لا           |
| msdyn_successortask           | نعم            | ‏‏لا           |
| msdyn_successortaskname       | نعم            | ‏‏لا           |

### <a name="resource-assignment"></a>تعيين الموارد

| **الاسم المنطقي**             | **يمكن الإنشاء** | **يمكنه التحرير** |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | نعم            | ‏‏لا           |
| msdyn_bookableresourceidname | نعم            | ‏‏لا           |
| msdyn_bookingstatusid        | ‏‏لا             | ‏‏لا           |
| msdyn_bookingstatusidname    | ‏‏لا             | ‏‏لا           |
| msdyn_committype             | ‏‏لا             | ‏‏لا           |
| msdyn_committypename         | ‏‏لا             | ‏‏لا           |
| msdyn_effort                 | ‏‏لا             | ‏‏لا           |
| msdyn_effortcompleted        | ‏‏لا             | ‏‏لا           |
| msdyn_effortremaining        | ‏‏لا             | ‏‏لا           |
| msdyn_finish                 | ‏‏لا             | ‏‏لا           |
| msdyn_plannedcost            | ‏‏لا             | ‏‏لا           |
| msdyn_plannedcost_base       | ‏‏لا             | ‏‏لا           |
| msdyn_plannedcostcontour     | ‏‏لا             | ‏‏لا           |
| msdyn_plannedsales           | ‏‏لا             | ‏‏لا           |
| msdyn_plannedsales_base      | ‏‏لا             | ‏‏لا           |
| msdyn_plannedsalescontour    | ‏‏لا             | ‏‏لا           |
| msdyn_plannedwork            | ‏‏لا             | ‏‏لا           |
| msdyn_projectid              | نعم            | ‏‏لا           |
| msdyn_projectidname          | ‏‏لا             | ‏‏لا           |
| msdyn_projectteamid          | ‏‏لا             | ‏‏لا           |
| msdyn_projectteamidname      | ‏‏لا             | ‏‏لا           |
| msdyn_start                  | ‏‏لا             | ‏‏لا           |
| msdyn_taskid                 | ‏‏لا             | ‏‏لا           |
| msdyn_taskidname             | ‏‏لا             | ‏‏لا           |
| msdyn_userresourceid         | ‏‏لا             | ‏‏لا           |

### <a name="project-team-member"></a>عضو فريق المشروع

| **الاسم المنطقي**                                 | **يمكن الإنشاء** | **يمكنه التحرير** |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | ‏‏لا             | ‏‏لا           |
| msdyn_creategenericteammemberwithrequirementname | ‏‏لا             | ‏‏لا           |
| msdyn_deletestatus                               | ‏‏لا             | ‏‏لا           |
| msdyn_deletestatusname                           | ‏‏لا             | ‏‏لا           |
| msdyn_effort                                     | ‏‏لا             | ‏‏لا           |
| msdyn_effortcompleted                            | ‏‏لا             | ‏‏لا           |
| msdyn_effortremaining                            | ‏‏لا             | ‏‏لا           |
| msdyn_finish                                     | ‏‏لا             | ‏‏لا           |
| msdyn_hardbookedhours                            | ‏‏لا             | ‏‏لا           |
| msdyn_hours                                      | ‏‏لا             | ‏‏لا           |
| msdyn_markedfordeletiontimer                     | ‏‏لا             | ‏‏لا           |
| msdyn_markedfordeletiontimestamp                 | ‏‏لا             | ‏‏لا           |
| msdyn_msprojectclientid                          | ‏‏لا             | ‏‏لا           |
| msdyn_percentage                                 | ‏‏لا             | ‏‏لا           |
| msdyn_requiredhours                              | ‏‏لا             | ‏‏لا           |
| msdyn_softbookedhours                            | ‏‏لا             | ‏‏لا           |
| msdyn_start                                      | ‏‏لا             | ‏‏لا           |

### <a name="project"></a>Project

| **الاسم المنطقي**                       | **يمكن الإنشاء** | **يمكنه التحرير** |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | ‏‏لا             | ‏‏لا           |
| msdyn_actualexpensecost_base           | ‏‏لا             | ‏‏لا           |
| msdyn_actuallaborcost                  | ‏‏لا             | ‏‏لا           |
| msdyn_actuallaborcost_base             | ‏‏لا             | ‏‏لا           |
| msdyn_actualsales                      | ‏‏لا             | ‏‏لا           |
| msdyn_actualsales_base                 | ‏‏لا             | ‏‏لا           |
| msdyn_contractlineproject              | نعم            | ‏‏لا           |
| msdyn_contractorganizationalunitid     | نعم            | ‏‏لا           |
| msdyn_contractorganizationalunitidname | نعم            | ‏‏لا           |
| msdyn_costconsumption                  | ‏‏لا             | ‏‏لا           |
| msdyn_costestimateatcomplete           | ‏‏لا             | ‏‏لا           |
| msdyn_costestimateatcomplete_base      | ‏‏لا             | ‏‏لا           |
| msdyn_costvariance                     | ‏‏لا             | ‏‏لا           |
| msdyn_costvariance_base                | ‏‏لا             | ‏‏لا           |
| msdyn_duration                         | ‏‏لا             | ‏‏لا           |
| msdyn_effort                           | ‏‏لا             | ‏‏لا           |
| msdyn_effortcompleted                  | ‏‏لا             | ‏‏لا           |
| msdyn_effortestimateatcompleteeac      | ‏‏لا             | ‏‏لا           |
| msdyn_effortremaining                  | ‏‏لا             | ‏‏لا           |
| msdyn_finish                           | نعم            | نعم          |
| msdyn_globalrevisiontoken              | ‏‏لا             | ‏‏لا           |
| msdyn_islinkedtomsprojectclient        | ‏‏لا             | ‏‏لا           |
| msdyn_islinkedtomsprojectclientname    | ‏‏لا             | ‏‏لا           |
| msdyn_linkeddocumenturl                | ‏‏لا             | ‏‏لا           |
| msdyn_msprojectdocument                | ‏‏لا             | ‏‏لا           |
| msdyn_msprojectdocumentname            | ‏‏لا             | ‏‏لا           |
| msdyn_plannedexpensecost               | ‏‏لا             | ‏‏لا           |
| msdyn_plannedexpensecost_base          | ‏‏لا             | ‏‏لا           |
| msdyn_plannedlaborcost                 | ‏‏لا             | ‏‏لا           |
| msdyn_plannedlaborcost_base            | ‏‏لا             | ‏‏لا           |
| msdyn_plannedsales                     | ‏‏لا             | ‏‏لا           |
| msdyn_plannedsales_base                | ‏‏لا             | ‏‏لا           |
| msdyn_progress                         | ‏‏لا             | ‏‏لا           |
| msdyn_remainingcost                    | ‏‏لا             | ‏‏لا           |
| msdyn_remainingcost_base               | ‏‏لا             | ‏‏لا           |
| msdyn_remainingsales                   | ‏‏لا             | ‏‏لا           |
| msdyn_remainingsales_base              | ‏‏لا             | ‏‏لا           |
| msdyn_replaylogheader                  | ‏‏لا             | ‏‏لا           |
| msdyn_salesconsumption                 | ‏‏لا             | ‏‏لا           |
| msdyn_salesestimateatcompleteeac       | ‏‏لا             | ‏‏لا           |
| msdyn_salesestimateatcompleteeac_base  | ‏‏لا             | ‏‏لا           |
| msdyn_salesvariance                    | ‏‏لا             | ‏‏لا           |
| msdyn_salesvariance_base               | ‏‏لا             | ‏‏لا           |
| msdyn_scheduleperformance              | ‏‏لا             | ‏‏لا           |
| msdyn_scheduleperformancename          | ‏‏لا             | ‏‏لا           |
| msdyn_schedulevariance                 | ‏‏لا             | ‏‏لا           |
| msdyn_taskearlieststart                | ‏‏لا             | ‏‏لا           |
| msdyn_teamsize                         | ‏‏لا             | ‏‏لا           |
| msdyn_teamsize_date                    | ‏‏لا             | ‏‏لا           |
| msdyn_teamsize_state                   | ‏‏لا             | ‏‏لا           |
| msdyn_totalactualcost                  | ‏‏لا             | ‏‏لا           |
| msdyn_totalactualcost_base             | ‏‏لا             | ‏‏لا           |
| msdyn_totalplannedcost                 | ‏‏لا             | ‏‏لا           |
| msdyn_totalplannedcost_base            | ‏‏لا             | ‏‏لا           |


## <a name="limitations-and-known-issues"></a>القيود والمشاكل المعروفة
فيما يلي قائمة بالقيود والمشاكل المعروفة:

- يمكن استخدام واجهات برمجة تطبيقات الجدولة فقط بواسطة **المستخدمين الذين لديهم ترخيص Microsoft Project.** لا يمكن استخدامها بواسطة:
    - مستخدمي التطبيق
    - مستخدمي النظام
    - مستخدمي التكامل
    - المستخدمين الآخرين الذين ليس لديهم الترخيص المطلوب
- تتضمن كل **OperationSet** مئة عملية كحدٍ أقصى.
- بإمكان كل مستخدم أن يحصل على عشر **OperationSet** مفتوحة كحدٍ أقصى.
- يدعم Project Operations في الوقت الحالي 500 مهمة إجمالية كحد أقصى على مشروع.
- في الوقت الحالي، لا تتوفر حالة فشل **OperationSet** وسجلات الفشل.
- واجهات برمجة تطبيقات الجدولة هي حاليًا في وضع الإصدار الأولي للاستخدام العام. لا تدعم Microsoft استخدام واجهات برمجة التطبيقات هذه في بيئة الإنتاج.
- [القيود والحدود على المشروعات والمهام](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a>معالجة الخطأ

   - لمراجعة الأخطاء التي تم إنشاؤها من مجموعات العمليات، انتقل إلى **الإعدادات** \> **تكامل الجدول** \> **مجموعات العمليات**.
   - لمراجعة الأخطاء التي تم إنشاؤها من خدمة جدولة المشروع، انتقل إلى **الإعدادات** \> **تكامل الجدول** \> **سجلات أخطاء PSS**.

## <a name="sample-scenario"></a>سيناريو نموذجي

في هذا السيناريو، ستقوم بإنشاء مشروع، وعضو فريق، وأربع مهام، وعمليتي تعيين للموارد. بعد ذلك، عليك تحديث مهمة واحدة وتحديث المشروع وحذف مهمة واحدة وحذف تعيين مورد واحد وإنشاء تبعية مهمة.

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>عينات إضافية

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;

    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
