---
title: تطوير قوالب المشروع مع نسخ المشروع‬
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء قوالب مشروع باستخدام إجراء "نسخ المشروع" المخصص.
author: stsporen
manager: Annbe
ms.date: 01/21/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 27847575e2d6ec9af77d24f756b13d3aeb0efea7
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286907"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="3130e-103">تطوير قوالب المشروع مع نسخ المشروع‬</span><span class="sxs-lookup"><span data-stu-id="3130e-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="3130e-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="3130e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="3130e-105">يدعم Dynamics 365 Project Operations القدرة علي نسخ مشروع وإرجاع أي تعيينات إلى الموارد العامة التي تمثل الدور.</span><span class="sxs-lookup"><span data-stu-id="3130e-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="3130e-106">يمكن للعملاء استخدام هذه الوظيفة لبناء قوالب المشروع الأساسية.</span><span class="sxs-lookup"><span data-stu-id="3130e-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="3130e-107">عند تحديد **نسخ المشروع**، يتم تحديث حالة المشروع الهدف.</span><span class="sxs-lookup"><span data-stu-id="3130e-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="3130e-108">استخدم **سبب الحالة** لتحديد وقت اكتمال إجراء النسخ.</span><span class="sxs-lookup"><span data-stu-id="3130e-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="3130e-109">يؤدي أيضًا تحديد **نسخ المشروع** إلى تحديث تاريخ بدء المشروع إلى تاريخ البدء الحالي في حال عدم اكتشاف تاريخ مستهدف في كيان المشروع الهدف.</span><span class="sxs-lookup"><span data-stu-id="3130e-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="3130e-110">الإجراء المخصص "نسخ المشروع"</span><span class="sxs-lookup"><span data-stu-id="3130e-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="3130e-111">اسم</span><span class="sxs-lookup"><span data-stu-id="3130e-111">Name</span></span> 

<span data-ttu-id="3130e-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="3130e-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="3130e-113">معلمات الإدخال</span><span class="sxs-lookup"><span data-stu-id="3130e-113">Input parameters</span></span>
<span data-ttu-id="3130e-114">توجد ثلاث معلمات إدخال:</span><span class="sxs-lookup"><span data-stu-id="3130e-114">There are three input parameters:</span></span>

| <span data-ttu-id="3130e-115">المعلمة‬</span><span class="sxs-lookup"><span data-stu-id="3130e-115">Parameter</span></span>          | <span data-ttu-id="3130e-116">النوع</span><span class="sxs-lookup"><span data-stu-id="3130e-116">Type</span></span>   | <span data-ttu-id="3130e-117">القيم</span><span class="sxs-lookup"><span data-stu-id="3130e-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="3130e-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="3130e-118">ProjectCopyOption</span></span>  | <span data-ttu-id="3130e-119">String</span><span class="sxs-lookup"><span data-stu-id="3130e-119">String</span></span> | <span data-ttu-id="3130e-120">**{"removeNamedResources":true}** أو **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="3130e-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="3130e-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="3130e-121">SourceProject</span></span>      | <span data-ttu-id="3130e-122">مرجع الكيان</span><span class="sxs-lookup"><span data-stu-id="3130e-122">Entity Reference</span></span> | <span data-ttu-id="3130e-123">Source Project</span><span class="sxs-lookup"><span data-stu-id="3130e-123">Source Project</span></span> |
| <span data-ttu-id="3130e-124">هدف</span><span class="sxs-lookup"><span data-stu-id="3130e-124">Target</span></span>             | <span data-ttu-id="3130e-125">مرجع الكيان</span><span class="sxs-lookup"><span data-stu-id="3130e-125">Entity Reference</span></span> | <span data-ttu-id="3130e-126">المشروع الهدف</span><span class="sxs-lookup"><span data-stu-id="3130e-126">Target Project</span></span> |


- <span data-ttu-id="3130e-127">**{"clearTeamsAndAssignments":true}**: السلوك الافتراضي لمشروع الويب، وستتم إزالة جميع التعيينات وأعضاء الفريق.</span><span class="sxs-lookup"><span data-stu-id="3130e-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="3130e-128">**{"removeNamedResources":true}** السلوك الافتراضي لـ Project Operations، وستُعاد التعيينات إلى الموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="3130e-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="3130e-129">لمزيد من الإعدادات الافتراضية حول الإجراءات، راجع [استخدام إجراءات API الويب](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="3130e-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="3130e-130">تحديد الحقول المراد نسخها</span><span class="sxs-lookup"><span data-stu-id="3130e-130">Specify fields to copy</span></span> 
<span data-ttu-id="3130e-131">عند استدعاء الإجراء، يبحث **نسخ المشروع** في طريقة عرض المشروع **نسخ أعمدة المشروع** لتحديد الحقول التي يجب نسخها عند نسخ المشروع.</span><span class="sxs-lookup"><span data-stu-id="3130e-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>


### <a name="example"></a><span data-ttu-id="3130e-132">مثال</span><span class="sxs-lookup"><span data-stu-id="3130e-132">Example</span></span>
<span data-ttu-id="3130e-133">يوضح المثال التالي كيفية استدعاء الإجراء المخصص **CopyProject** مع مجموعة المعلمات **RemoveNamedResources**.</span><span class="sxs-lookup"><span data-stu-id="3130e-133">The following example shows how to call the **CopyProject** custom action with the **removeNamedResources** parameter set.</span></span>
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]