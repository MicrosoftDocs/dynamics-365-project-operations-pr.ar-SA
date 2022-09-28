---
title: استخدام واجهات برمجة التطبيقات لجدولة المشروع لتنفيذ عمليات مع كيانات الجدولة
description: يوفر هذا المقال معلومات وعينات لاستخدام واجهات برمجة التطبيقات (API) لجدولة المشروع.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 159d395efff98f2af780e5ed1e5ab3d6483cba89
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541108"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>استخدام واجهات برمجة التطبيقات لجدولة المشروع لتنفيذ عمليات مع كيانات الجدولة

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_


**كيانات الجدولة**

توفر واجهات برمجة التطبيقات لجدولة المشروع القدرة على تنفيذ عمليات إنشاء وتحديث وحذف باستخدام **كيانات الجدولة**. تُدار هذه الكيانات من خلال محرك جدولة في المشروع للويب. كانت عمليات الإنشاء والتحديث والحذف باستخدام **كيانات الجدولة** مقيدة في إصدارات Dynamics 365 Project Operations السابقة.

يوفر الجدول التالي قائمة كاملة بكيانات جدولة المشروع.

| **اسم الكيان**         | **اسم منطقي للكيان**     |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| مهمة المشروع            | msdyn_projecttask           |
| تبعية مهمة المشروع | msdyn_projecttaskdependency |
| تعيين المورد     | msdyn_resourceassignment    |
| مستودع المشروع          | msdyn_projectbucket         |
| عضو فريق المشروع     | msdyn_projectteam           |
| قوائم اختيار المشروع      | msdyn_projectchecklist      |
| تسمية المشروع           | msdyn_projectlabel          |
| مهمة المشروع المُراد تسميتها   | msdyn_projecttasktolabel    |
| الدورة المتكررة للمشروع‬          | msdyn_projectsprint         |

**OperationSet**

إن OperationSet عبارة نمط وحدة عمل يمكن استخدامه عندما يكون من الضروري معالجة طلبات متعددة تؤثر على الجدولة ضمن حركة.

**واجهات برمجة التطبيقات لجدولة المشروع**

وفيما يلي قائمة بواجهات برمجة التطبيقات لجدولة المشروع.

| **API**                                 | الوصف                                                                                                                        |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **msdyn_CreateProjectV1**               | تُستخدم API هذه لإنشاء مشروع. يتم إنشاء المشروع والحاوية الافتراضية للمشروع على الفور.                         |
| **msdyn_CreateTeamMemberV1**            | تُستخدم API هذه لإنشاء عضو فريق مشروع. يتم إنشاء سجل عضو الفريق على الفور.                                  |
| **msdyn_CreateOperationSetV1**          | تُستخدم API هذه لجدولة طلبات متعددة يجب تنفيذها ضمن حركة.                                        |
| **msdyn_PssCreateV1**                   | تُستخدم API هذه لإنشاء كيان. يمكن أن يكون الكيان أيًا من كيانات جدولة المشروع التي تدعم عملية الإنشاء. |
| **msdyn_PssUpdateV1**                   | تُستخدم API هذه لتحديث كيان. بإمكان الكيان أن يكون عبارة عن أي من كيانات جدولة المشروع التي تدعم عملية التحديث  |
| **msdyn_PssDeleteV1**                   | تُستخدم API هذه لحذف كيان. يمكن أن يكون الكيان أيًا من كيانات جدولة المشروع التي تدعم عملية الحذف. |
| **msdyn_ExecuteOperationSetV1**         | تُستخدم API هذه لتنفيذ جميع العمليات ضمن مجموعة عمليات معينة.                                                 |
| **msdyn_PssUpdateResourceAssignmentV1** | تُستخدم API هذه في تحديث مجموعة العمل المخططة لتعيين الموارد.                                                        |



**استخدام واجهات برمجة التطبيقات لجدولة المشروع مع OperationSet**

نظرًا لاستخدام السجلات مع كل من **CreateProjectV1** و **CreateTeamMemberV1** على الفور، لا يمكن استخدام واجهات برمجة التطبيقات هذه في **OperationSet** بشكل مباشر. ومع ذلك، يمكنك استخدام واجهة برمجة التطبيقات لإنشاء السجلات المطلوبة، وإنشاء  **OperationSet**، ثم استخدام هذه السجلات المنشأة مسبقًا في **OperationSet**.

**العمليات المدعومة**

| **كيان الجدولة**   | **‏إنشاء** | **تحديث** | **حذف** | **اعتبارات هامة**                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------|------------|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| مهمة المشروع            | نعم         | نعم         | نعم         | يمكن تحرير حقول **Progress** و **EffortCompleted** و **EffortRemaining** في Project for the Web، ولكن لا يمكن تحريرها في Project Operations.                                                                                                                                                                                             |
| تبعية مهمة المشروع | نعم         | لا          | نعم         | لا يتم تحديث سجلات تبعية مهمة المشروع. بدلاً من ذلك، يمكن حذف سجل قديم، ويمكن إنشاء سجل جديد.                                                                                                                                                                                                                                 |
| تعيين الموارد     | نعم         | نعم\*      | نعم         | العمليات مع الحقول التالية غير مدعومة: **BookableResourceID** و **Effort** و **EffortCompleted** و **EffortRemaining** ة **PlannedWork**. لا يتم تحديث سجلات تعيين الموارد. بدلاً من ذلك، يمكن حذف السجل القديم، ويمكن إنشاء سجل جديد. تم توفير API منفصلة لتحديث خطوط تعيين الموارد. |
| مستودع المشروع          | نعم         | نعم         | نعم         | يتم إنشاء الحاوية الافتراضية باستخدام واجهة برمجة تطبيقات **CreateProjectV1**. تمت إضافة دعم إنشاء حاويات المشروع وحذفها في تحديث الإصدار 16.                                                                                                                                                                                                   |
| عضو فريق المشروع     | نعم         | نعم         | نعم         | بالنسبة لعملية الإنشاء، استخدم واجهة برمجة التطبيقات **CreateTeamMemberV1**.                                                                                                                                                                                                                                                                                           |
| Project                 | نعم         | نعم         |            | العمليات مع الحقول التالية غير مدعومة: **StateCode** و **BulkGenerationStatus** و **GlobalRevisionToken** و **CalendarID** و **Effort** و **EffortCompleted** و **EffortRemaining** و **Progress** و **Finish** و **TaskEarliestStart** و **Duration**.                                                                                       |
| قوائم اختيار المشروع      | نعم         | نعم         | نعم         |                                                                                                                                                                                                                                                                                                                                                         |
| تسمية المشروع           | لا          | نعم         | لا          | يمكن تغيير أسماء بطاقات التسميات. هذه الميزة متاحة فقط لـ Project for the Web.                                                                                                                                                                                                                                                                      |
| مهمة المشروع المُراد تسميتها   | نعم         | لا          | نعم         | هذه الميزة متاحة فقط لـ Project for the Web.                                                                                                                                                                                                                                                                                                  |
| الدورة المتكررة للمشروع‬          | نعم         | نعم         | نعم         | يجب أن يكون حقل **البدء** أقدم من حقل **الإنهاء**. لا يمكن أن تتداخل الدورات المتكررة لنفس المشروع مع بعضها البعض. هذه الميزة متاحة فقط لـ Project for the Web.                                                                                                                                                                    |




خاصية المعرف اختيارية. إذا تم توفيرها، يحاول النظام استخدامها ويلقي استثناءً إذا لم يكن من الممكن استخدامها. إذا لم يتم توفيرها، سيقوم النظام بإنشائها.

**القيود والمشاكل المعروفة**

فيما يلي قائمة بالقيود والمشاكل المعروفة:

-   لا يمكن استخدام واجهات برمجة تطبيقات جدولة المشروع إلا بواسطة **المستخدمين الذين لديهم ترخيص Microsoft Project**. لا يمكن استخدامها بواسطة:
    -   مستخدمي التطبيق
    -   مستخدمي النظام
    -   مستخدمي التكامل
    -   المستخدمين الآخرين الذين ليس لديهم الترخيص المطلوب
-   تتضمن كل **OperationSet** مئة عملية كحدٍ أقصى.
-   بإمكان كل مستخدم أن يحصل على عشر **OperationSet** مفتوحة كحدٍ أقصى.
-   يدعم Project Operations في الوقت الحالي 500 مهمة إجمالية كحد أقصى على مشروع.
-   يتم عد كل عملية تحديث مخطط تعيين موارد كعملية واحدة.
-   يمكن لكل قائمة بالمخططات المحدثة أن تحتوي على 100 شريحة وقت كحد أقصى.
-   في الوقت الحالي، لا تتوفر حالة فشل **OperationSet** وسجلات الفشل.
-   توجد 400 دورة متكررة كحد أقصى لكل مشروع.
-   [القيود والحدود على المشاريع والمهام](/project-for-the-web/project-for-the-web-limits-and-boundaries).
-   التسميات متاحة فقط لـ Project for the Web حاليًا.

**معالجة الخطأ**

-   لمراجعة الأخطاء التي تم إنشاؤها من مجموعات العمليات، انتقل إلى **الإعدادات** \> **تكامل الجدول** \> **مجموعات العمليات**.
-   لمراجعة الأخطاء التي تم إنشاؤها من خدمة جدولة المشروع، انتقل إلى **إعدادات** \> **‏‫تكامل الجدولة** \> **سجلات أخطاء PSS**.

**تحرير مخططات تعيين الموارد**

على عكس جميع واجهات API الأخرى لجدولة المشروع التي تقوم بتحديث الكيان، إن واجهة API تعيين الموارد هي المسؤولة وحدها عن التحديثات لحقل واحد، msdyn_plannedwork، في كيان واحد، msydn_resourceassignment.

وضع الجدولة المحدد هو:

-   **وحدات ثابتة**
-   تقويم المشروع هو 9-5 مساءً من 9 إلى 5 مساءً بتوقيت المحيط الهادئ، الإثنين، الثلاثاء، الخميس، الجمعة (لا يوجد أيام عمل أيام الأربعاء)
-   وتقويم الموارد هو 9-1 مساء بتوقيت المحيط الهادئ من الإثنين إلى الجمعة

هذه المهمة لمدة أسبوع واحد، أربع ساعات في اليوم. هذا لأن تقويم المورد من 9-1 بتوقيت المحيط الهادي، أو أربع ساعات في اليوم.

| &nbsp;     | المهمة | تاريخ البدء | تاريخ الانتهاء  | الكمية | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| عامل 9-1 |  T1  | 6/13/2022  | 6/17/2022 | 20       | 4         | 4         | 4         | 4         | 4         |

على سبيل المثال، إذا كنت تريد أن يعمل العامل ثلاث ساعات فقط كل يوم في هذا الأسبوع ويسمح له بساعة واحدة للقيام بمهام أخرى.

#### <a name="updatedcontours-sample-payload"></a>حمولة عينة المخططات المحدثة:

```json
[{

"minutes":900.0,

"start":"2022-06-13T00:00:00-07:00",

"end":"2022-06-18T00:00:00-07:00"

}]
```

هذا هو التعيين بعد تشغيل واجهة API لتحديث جدولة المخططات.

| &nbsp;     | المهمة | تاريخ البدء | تاريخ الانتهاء  | الكمية | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| عامل 9-1 | T1   | 6/13/2022  | 6/17/2022 | 15       | 3          | 3          | 3          | 3          | 3          |


**سيناريو نموذجي**

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

** عينات إضافية

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
