---
title: سجلات جدولة المشاريع
description: يوفر هذا الموضوع معلومات وعينات ستساعدك على استخدام سجلات جدولة المشاريع في تعقب حالات الفشل المرتبطة بخدمة جدولة المشاريع وواجهات برمجة التطبيقات لجدولة المشاريع.
author: ruhercul
ms.date: 11/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1c5632a880fa30d1b863c326b22e3d930c9564dc
ms.sourcegitcommit: 844ec8eacd0fc10d1659b437cc5cbb4480ec9e1e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/01/2021
ms.locfileid: "7877620"
---
# <a name="project-scheduling-logs"></a>سجلات جدولة المشاريع

_**تنطبق على:** ‏Project Operations للسيناريوهات المستندة إلى الموارد/منتجات غير مخزنة، التوزيع الخفيف - التعامل مع الفواتير الأولية_، _Project for the Web_

يستخدم تطبيق Microsoft Dynamics 365 Project Operations عرض [Project for the Web](https://support.microsoft.com/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) كمحرك الجدولة الرئيسي له. بدلاً من استخدام واجهات برمجة تطبيق ويب Microsoft Dataverse القياسية، تستخدم أداة Project Operations واجهات برمجة التطبيقات لجدولة المشاريع الجديدة لإنشاء وتحديث وحذف مهام المشروع وتخصيصات الموارد، وتبعيات المهام، ومستخدمي المشاريع، وأعضاء فرق المشاريع. ومع ذلك، عند إنشاء أو تحديث أو حذف عمليات تعمل برمجيًا على كيانات هيكل تنظيم العمل (WBS)، قد تحدث أخطاء. لتعقب هذه الأخطاء ومحفوظات العمليات، تم تنفيذ سجلين إداريين جديدين: **مجموعة العمليات** و **خدمة جدولة المشاريع (PSS)**. للوصول إلى هذه السجلات، انتقل إلى **إعدادات** \> **تكامل الجدولة**.

يبين الرسم التوضيحي التالي نموذج البيانات لسجلات جدولة المشاريع.

![نموذج البيانات لسجلات جدولة المشاريع](media/LOGDATAMODEL.jpg)

## <a name="operation-set-log"></a>سجل مجموعة العمليات

يتعقب سجل مجموعة العمليات تنفيذ مجموعة عمليات تُستخدم لتشغيل واحدة أو أكثر من عمليات الإنشاء أو التحديث أو الحذف في دفعة واحدة على المشاريع أو مهام المشاريع أو تعيينات الموارد أو تبعيات المهام أو مجموعات المشاريع أو أعضاء فرق المشاريع. يعرض الحقل **العملية في الحالة** الحالة الإجمالية لمجموعة عمليات. يتم الحصول على تفاصيل حمولة مجموعة العمليات في سجلات تفاصيل مجموعة العمليات ذات الصلة.

### <a name="operation-set"></a>مجموعة العمليات

يعرض الجدول التالي الحقول المرتبطة بالكيان **مجموعة العمليات**.

| اسم المخطط            | الوصف                                                                                                   | DisplayName            |
|-----------------------|--------------------------------------------------------------------------------------------------------------|------------------------|
| msdyn_completedon     | التاريخ/الوقت الذي اكتملت فيه أو فشلت مجموعة العمليات.                                                | CompletedOn            |
| msdyn_correlationid   | قيمة **correlationId** الخاص بالطلب.                                                                  | CorrelationId          |
| msdyn_description     | وصف مجموعة العمليات.                                                                        | الوصف             |
| msdyn_executedon      | التاريخ/الوقت الذي تم فيه تشغيل السجل.                                                                       | تاريخ التنفيذ            |
| msdyn_operationsetId  | المعرف الفريد لمثيلات الكيان.                                                                   | OperationSet           |
| msdyn_Project         | المشروع المتعلق بمجموعة العمليات.                                                            | Project                |
| msdyn_projectid       | قيمة **projectId** الخاص بالطلب.                                                                      | ProjectId (مهمل) |
| msdyn_projectName     | غير قابل للتطبيق.                                                                                              | غير قابل للتطبيق         |
| msdyn_PSSErrorLog     | المعرف الفريد لسجل أخطاء خدمة جدولة المشاريع المقترن بمجموعة العمليات. | سجل أخطاء PSS          |
| msdyn_PSSErrorLogName | غير قابل للتطبيق.                                                                                              | غير قابل للتطبيق         |
| msdyn_status          | حالة مجموعة العمليات.                                                                             | الحالة                  |
| msdyn_statusName      | غير قابل للتطبيق.                                                                                              | غير قابل للتطبيق         |
| msdyn_useraadid       | معرف كائن Azure Active Directory (Azure AD) للمستخدم الذي ينتمي إليه هذا الطلب.                     | UserAADID              |

### <a name="operation-set-detail"></a>تفاصيل مجموعة العمليات

يعرض الجدول التالي الحقول المرتبطة بالكيان **تفاصيل مجموعة العمليات**.

| اسم المخطط                 | الوصف                                                                                  | DisplayName           |
|----------------------------|---------------------------------------------------------------------------------------------|-----------------------|
| msdyn_cdspayload           | حقول Dataverse المتسلسلة للطلب.                                            | CdsPayload            |
| msdyn_entityname           | اسم الكيان للطلب.                                                     | EntityName            |
| msdyn_httpverb             | أسلوب الطلب.                                                                         | HTTPVerb (مهمل) |
| msdyn_httpverbName         | غير قابل للتطبيق.                                                                             | غير قابل للتطبيق        |
| msdyn_operationset         | المعرف الفريد لمجموعة العمليات التي ينتمي إليها السجل.                      | OperationSet          |
| msdyn_operationsetdetailId | المعرف الفريد لمثيلات الكيان.                                                  | تفصيل OperationSet   |
| msdyn_operationsetName     | غير قابل للتطبيق.                                                                             | غير قابل للتطبيق        |
| msdyn_operationtype        | نوع العملية لتفاصيل مجموعة العمليات.                                             | OperationType         |
| msdyn_operationtypeName    | غير قابل للتطبيق.                                                                             | غير قابل للتطبيق        |
| msdyn_psspayload           | حقول خدمة جدولة المشاريع المتسلسلة للطلب.                           | PssPayload            |
| msdyn_recordid             | معرف سجل الطلب.                                                       | معرّف السجل             |
| msdyn_requestnumber        | رقم ينشأ تلقائيًا يحدد الأمر الذي تم استلام الطلبات فيه. | رقم الطلب        |

## <a name="project-scheduling-service-error-logs"></a>سجلات أخطاء خدمة جدولة المشاريع

تقوم سجلات أخطاء خدمة جدولة المشاريع بالتقاط حالات الفشل التي تحدث عندما تحاول خدمة جدولة المشاريع إجراء عملية **حفظ** أو **فتح**. هناك ثلاثة سيناريوهات مدعومة يتم فيها إنشاء هذه السجلات:

- فشل الإجراءات التي بدأها المستخدم بشكل خطير (على سبيل المثال، لا يمكن إنشاء تعيين نظرًا لعدم وجود امتيازات).
- لا يمكن لخدمة جدولة المشاريع برمجيًا إنشاء أو تحديث أو حذف أو تنفيذ أية عملية متتالية أخرى على كيان ما.
- يواجه المستخدم أخطاء عند فشل فتح سجل (على سبيل المثال، عند فتح مشروع أو تحديث معلومات أحد أعضاء الفريق).

### <a name="project-scheduling-service-log"></a>سجل خدمة جدولة المشاريع

يعرض الجدول التالي الحقول التي تم تضمينها في سجل خدمة جدولة المشاريع.

| اسم المخطط          | الوصف                                                                     | DisplayName    |
|---------------------|--------------------------------------------------------------------------------|----------------|
| msdyn_CallStack     | مكدس الاستدعاءات للاستثناء.                                               | تكدس الاستدعاءات     |
| msdyn_correlationid | معرف ارتباط الخطأ.                                               | CorrelationId  |
| msdyn_errorcode     | حقل يتم استخدامه لتخزين رمز خطأ Dataverse أو رمز خطأ HTTP. | رمز الخطأ     |
| msdyn_HelpLink      | رابط وثائق المساعدة العامة.                                       | ارتباط التعليمات      |
| msdyn_log           | السجل من خدمة جدولة المشاريع.                                   | سجل            |
| msdyn_project       | المشروع المقترن بسجل الأخطاء.                             | Project        |
| msdyn_projectName   | اسم المشروع في حالة استمرار حمولة مجموعة العمليات. | غير قابل للتطبيق |
| msdyn_psserrorlogId | المعرف الفريد لمثيلات الكيان.                                     | سجل أخطاء PSS  |
| msdyn_SessionId     | معرف جلسة عمل المشروع.                                                        | معرَّف جلسة العمل     |

## <a name="error-log-cleanup"></a>تنظيف سجل الأخطاء

بشكل افتراضي، يمكن تنظيف كل من سجلات أخطاء خدمة جدولة المشاريع وسجل مجموعة العمليات كل 90 يومًا. سيتم حذف أي سجلات مضى عليها أكثر من 90 يومًا. ومع ذلك، فمن خلال تغيير قيمة الحقل **msdyn_StateOperationSetAge** على صفحة **معلمات المشروع**، يمكن للمسؤولين ضبط نطاق التنظيف بحيث يتراوح بين يوم واحد و120 يومًا. تتوفر عدة أساليب لتغيير هذه القيمة:

- تخصيص الكيان **معلمة المشروع** من خلال إنشاء صفحة مخصصة وإضافة الحقل **‏‫عمر مجموعة العمليات التي انتهت صلاحيتها‬**.
- استخدام التعليمة البرمجية للعميل التي تستخدم [مجموعة تطوير برامج WebApi (SDK)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord).
- استخدام تعليمات SDK البرمجية للخدمة التي تستخدم أسلوب Xrm SDK **updateRecord** (مرجع واجهة برمجة تطبيقات العميل) في التطبيقات التي تستند إلى النموذج. تتضمن Power Apps وصفًا ومعلمات مدعومة لأسلوب **updateRecord**.

    ```C#
    Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter').then(function (response) {
        parameter = response.entities[0];
        var staleOperationValue = prompt("All records older than (x) days will be deleted, please enter X between 1 to 90 days", 1)
        var newData = {};
        newData.msdyn_projectparameterid = parameter.msdyn_projectparameterid;
        newData.msdyn_staleoperationsetage = parseInt(staleOperationValue);
        Xrm.WebApi.updateRecord("msdyn_projectparameter", parameter.msdyn_projectparameterid, newData).then(
            function success(result) {
                console.log("Project Parameter: Stale Operation Expiry is set to: " + newData.msdyn_staleoperationsetage);
                // perform operations on record update
                Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter')
                .then(function (response2) { console.log("Confirmed Project Parameter: Stale Operation Expiry is set to: " + response2.entities[0].msdyn_staleoperationsetage) });
            },
            function (error) {
                console.log("Failed to Update Project Ednpoint with error: " + error.message);
            // handle error conditions
            }
        );
    });
    ```
