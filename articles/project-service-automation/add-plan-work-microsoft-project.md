---
title: استخدام الوظيفة الإضافية Project Service لتخطيط عملك في Microsoft Project | MicrosoftDocs
description: يوفر هذا الموضوع معلومات حول كيفية إضافة وتكوين واستخدام الوظيفة الإضافية لـ Microsoft project لـ Microsoft project Service.
author: ruhercul
manager: kfend
ms.service: Dynamics 365 Project Service Automation
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: efd589e0-8233-4abf-bf7e-5c1e83c4daea
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 0ad503ff0c27f1543d15b60714c2be46b8487d18
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748618"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a><span data-ttu-id="6d894-103">استخدام الوظيفة الإضافية Project Service Automation لتخطيط عملك في Microsoft Project</span><span class="sxs-lookup"><span data-stu-id="6d894-103">Use the Project Service Automation Add-in to plan your work in Microsoft Project</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="6d894-104">يسهّل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] عملية التخطيط للمشاريع، بما في ذلك التقديرات.</span><span class="sxs-lookup"><span data-stu-id="6d894-104">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes it easier for you to do your project planning, including estimates.</span></span> <span data-ttu-id="6d894-105">يمكنك تعريف العمل لكي تكون قيمة التكاليف والجهود والمبيعات واضحة عند تقديم الاقتراح النهائي.</span><span class="sxs-lookup"><span data-stu-id="6d894-105">You can define the work so that costs, effort, and sales value are clear as the final proposal is submitted.</span></span>  

 <span data-ttu-id="6d894-106">يمكنك الآن تثبيت [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] والقيام بأعمال التخطيط في بيئة [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] المألوفة.</span><span class="sxs-lookup"><span data-stu-id="6d894-106">Now you can install the [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] and do your planning work in the familiar environment of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span> <span data-ttu-id="6d894-107">استخدم قدرات التخطيط والإدارة الفعالة من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ثم قم بتحديث خطة مشروعك في Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="6d894-107">Use the robust planning and management capabilities of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and then update your project plan in Project Service Automation.</span></span>  

> [!IMPORTANT]
> - <span data-ttu-id="6d894-108">لاستخدام ميزة إدارة المستندات في SharePoint لتخزين ملفات [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] لمشاريع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، سيحتاج مسؤول [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] إلى تشغيل إدارة المستندات.</span><span class="sxs-lookup"><span data-stu-id="6d894-108">To use SharePoint document management to store your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] files for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] projects, your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] admin will need to turn on document management.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="6d894-109">[تمكين إدارة مستندات SharePoint لكيانات محددة](../admin/enable-sharepoint-document-management-specific-entities.md)</span><span class="sxs-lookup"><span data-stu-id="6d894-109">[Enable SharePoint document management for specific entities](../admin/enable-sharepoint-document-management-specific-entities.md)</span></span>  
> - <span data-ttu-id="6d894-110">يتوافق [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] فقط مع [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span><span class="sxs-lookup"><span data-stu-id="6d894-110">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] is only compatible with [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span></span>  

## <a name="download-and-install-the-add-in"></a><span data-ttu-id="6d894-111">تنزيل الوظيفة الإضافية وتثبيتها</span><span class="sxs-lookup"><span data-stu-id="6d894-111">Download and install the add-in</span></span>  
 <span data-ttu-id="6d894-112">تأكد من أن معلومات تسجيل الدخول إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] جاهزة.</span><span class="sxs-lookup"><span data-stu-id="6d894-112">Have your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sign-in information ready.</span></span> <span data-ttu-id="6d894-113">سوف تحتاج إلى هذه المعلومات للاتصال من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] بميزة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-113">You will need this information to connect from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

1.  <span data-ttu-id="6d894-114">من مركز التنزيل ، يمكنك تنزيل الوظيفة الإضافية للإصدار المدعوم من Project Service، إما [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) أو [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span><span class="sxs-lookup"><span data-stu-id="6d894-114">From the Download Center, download the add-in for your supported version of Project Service, either [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) or [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span></span>  

2.  <span data-ttu-id="6d894-115">انقر فوق ارتباط التنزيل.</span><span class="sxs-lookup"><span data-stu-id="6d894-115">Click the download link.</span></span>  

3.  <span data-ttu-id="6d894-116">عند اكتمال التنزيل، انقر فوق **نعم** لتثبيت الوظيفة الإضافية.</span><span class="sxs-lookup"><span data-stu-id="6d894-116">When the download is complete, click **Yes** to install the add-in.</span></span>  

## <a name="configure-the-add-in"></a><span data-ttu-id="6d894-117">تكوين الوظيفة الإضافية</span><span class="sxs-lookup"><span data-stu-id="6d894-117">Configure the add-in</span></span>  

1. <span data-ttu-id="6d894-118">افتح [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وانقر فوق علامة التبويب **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="6d894-118">Open [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and click the **Project Service** tab.</span></span>  

2. <span data-ttu-id="6d894-119">انقر فوق **Connect**.</span><span class="sxs-lookup"><span data-stu-id="6d894-119">Click **Connect**.</span></span>  

3. <span data-ttu-id="6d894-120">أدخل معلومات تسجيل الدخول، ثم انقر فوق **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="6d894-120">Enter your sign-in information and then click **Sign in**.</span></span>  

   <span data-ttu-id="6d894-121">يمكنك الآن بدء استخدام الوظيفة الإضافية.</span><span class="sxs-lookup"><span data-stu-id="6d894-121">Now you can start using the add-in.</span></span>  

## <a name="read-from-a-template"></a><span data-ttu-id="6d894-122">القراءة من قالب</span><span class="sxs-lookup"><span data-stu-id="6d894-122">Read from a template</span></span>  
 <span data-ttu-id="6d894-123">يمكنك القراءة من قالب أنشأته في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ونسخه إلى [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] لبدء تخطيط المشروع.</span><span class="sxs-lookup"><span data-stu-id="6d894-123">Read from a template that you created in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] and copied into [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to start your project planning.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="6d894-124">[إنشاء قالب مشروع (Project Service Automation)](../project-service/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="6d894-124">[Create a project template (Project Service Automation)](../project-service/create-project-template.md)</span></span>  

1.  <span data-ttu-id="6d894-125">من علامة التبويب **Project Service**، انقر فوق **قراءة** > **قالب مشروع Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="6d894-125">From the **Project Service** tab, click **Read** > **Project Service Automation Project Template**.</span></span>  

2.  <span data-ttu-id="6d894-126">اختر قالب مشروع من القائمة وانقر فوق **فتح**.</span><span class="sxs-lookup"><span data-stu-id="6d894-126">Choose a project template from the list and then click **Open**.</span></span>  

    > [!NOTE]
    >  <span data-ttu-id="6d894-127">بشكل افتراضي، يتم تعيين المهام المنسوخة من القالب إلى Project على أنها مجدولة يدويًا.</span><span class="sxs-lookup"><span data-stu-id="6d894-127">By default, the tasks that are copied from the template into Project are set as manually scheduled.</span></span>  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a><span data-ttu-id="6d894-128">تعيين أدوار [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى موارد المشروع</span><span class="sxs-lookup"><span data-stu-id="6d894-128">Assign [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] roles to project resources</span></span>  

1.  <span data-ttu-id="6d894-129">افتح مشروعًا، ثم انقر فوق شريط **المهام**.</span><span class="sxs-lookup"><span data-stu-id="6d894-129">Open a project and click the **Task** ribbon.</span></span>  

2.  <span data-ttu-id="6d894-130">انقر فوق قائمة **مخطط جانت**، ثم اختر **ورقة الموارد**.</span><span class="sxs-lookup"><span data-stu-id="6d894-130">Click the **Gantt Chart** menu and then choose **Resource Sheet**.</span></span>  

3.  <span data-ttu-id="6d894-131">على ورقة الموارد، انقر فوق القائمة المنسدلة **دور موارد Project Service** واختر دور Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="6d894-131">On the Resource Sheet, click the **Project Service Resource Role** drop-down menu and choose a Project Service Automation role.</span></span>  

## <a name="staff-your-project-with-resources"></a><span data-ttu-id="6d894-132">تعيين موارد للمشروع</span><span class="sxs-lookup"><span data-stu-id="6d894-132">Staff your project with resources</span></span>  

1.  <span data-ttu-id="6d894-133">من علامة التبويب Project Service، حدد صفًا، ثم انقر فوق **البحث عن موارد**.</span><span class="sxs-lookup"><span data-stu-id="6d894-133">From the Project Service tab, select a row and click **Find Resources**.</span></span>  

2.  <span data-ttu-id="6d894-134">على شاشة **حجز مورد**، حدد المورد الذي تريد استخدامه للمشروع.</span><span class="sxs-lookup"><span data-stu-id="6d894-134">On the **Book Resource** screen, select the resource that you want to use for the project.</span></span>  

3.  <span data-ttu-id="6d894-135">انقر فوق **حجز**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="6d894-135">Click **Book** and then click **OK**.</span></span>  

## <a name="publish-your-project"></a><span data-ttu-id="6d894-136">نشر المشروع</span><span class="sxs-lookup"><span data-stu-id="6d894-136">Publish your project</span></span>  
<span data-ttu-id="6d894-137">عند اكتمال عملية تخطيط المشروع، الخطوة التالية هي استيراد المشروع ونشره في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-137">When your project planning is complete, the next step is to import and publish the project in to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

<span data-ttu-id="6d894-138">سيتم استيراد المشروع إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-138">The project will import into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="6d894-139">يتم تطبيق عملية إنشاء الفريق والتسعير.</span><span class="sxs-lookup"><span data-stu-id="6d894-139">The pricing and team generation process are applied.</span></span> <span data-ttu-id="6d894-140">افتح المشروع في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للتأكد من إنشاء الفريق وتقديرات المشروع وهيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="6d894-140">Open the project in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to see that the team, project estimates, and work breakdown structure has been generated.</span></span> <span data-ttu-id="6d894-141">يبين الجدول التالي المكان حيث يمكن العثور على النتائج:</span><span class="sxs-lookup"><span data-stu-id="6d894-141">The following table shows where to find the results:</span></span>


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="6d894-142">**مخطط جانت**</span><span class="sxs-lookup"><span data-stu-id="6d894-142">**Gantt Chart**</span></span>   | <span data-ttu-id="6d894-143">استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **هيكل تنظيم العمل**.</span><span class="sxs-lookup"><span data-stu-id="6d894-143">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Work Breakdown Structure** screen.</span></span> |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="6d894-144">**ورقة الموارد**</span><span class="sxs-lookup"><span data-stu-id="6d894-144">**Resource Sheet**</span></span> |   <span data-ttu-id="6d894-145">استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **أعضاء فريق المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6d894-145">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Team Members** screen.</span></span>   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="6d894-146">**الاستخدام**</span><span class="sxs-lookup"><span data-stu-id="6d894-146">**Use Usage**</span></span>    |    <span data-ttu-id="6d894-147">استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **تقديرات المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6d894-147">Omports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Estimates** screen.</span></span>     |

<span data-ttu-id="6d894-148">**لاستيراد مشروعك ونشره**</span><span class="sxs-lookup"><span data-stu-id="6d894-148">**To import and publish your project**</span></span>  
1. <span data-ttu-id="6d894-149">من علامة التبويب **Project Service**، انقر فوق **نشر** > **مشروع جديد في Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="6d894-149">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project**.</span></span>  

2. <span data-ttu-id="6d894-150">في مربع الحوار **نشر في مشروع جديد في Project Service**، أدخل **اسم المشروع** وحدد **العميل**.</span><span class="sxs-lookup"><span data-stu-id="6d894-150">On **Publish to a new project in Project Service** dialog box, enter the **Project Name** and select the **Customer**.</span></span>  

3. <span data-ttu-id="6d894-151">حدد **‏‫ربط خطة المشروع بـ Project Service Automation‬** بشكل اختياري لربط ملف خطة Project بـ Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="6d894-151">Optionally check the **Link project plan to Project Service Automation** to link the plan Project file to Project Service Automation.</span></span>  

4. <span data-ttu-id="6d894-152">انقر فوق **نشر**.</span><span class="sxs-lookup"><span data-stu-id="6d894-152">Click **Publish**.</span></span>  

   <span data-ttu-id="6d894-153">يؤدي ربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى جعل ملف Project الملف الرئيسي وإلى تعيين هيكل تنظيم العمل في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="6d894-153">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to read-only.</span></span>  <span data-ttu-id="6d894-154">لإجراء التغييرات على خطة المشروع، تحتاج إلى إجرائها في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ونشرها كتحديثات إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-154">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

## <a name="edit-a-project-thats-been-imported"></a><span data-ttu-id="6d894-155">تحرير مشروع تم استيراده</span><span class="sxs-lookup"><span data-stu-id="6d894-155">Edit a project that’s been imported</span></span>  
 <span data-ttu-id="6d894-156">لإجراء تغييرات على خطة مشروع تم استيراده إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، يمكنك التحديد من ضمن خيارين:</span><span class="sxs-lookup"><span data-stu-id="6d894-156">To make changes to a project plan that's been imported into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you have two options:</span></span>  

- <span data-ttu-id="6d894-157">فتح الملف الرئيسي وتحريره في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-157">Open the master file and edit it in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

- <span data-ttu-id="6d894-158">إلغاء ارتباط الملف الرئيسي وتحريره في Project Service بشكل مباشر.</span><span class="sxs-lookup"><span data-stu-id="6d894-158">Unlink the file and edit it directly in Project Service.</span></span> <span data-ttu-id="6d894-159">بشكل افتراضي، يكون المشروع الذي يتم تحميله من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] مؤمنًا ويمكن تحريره فقط في Project.</span><span class="sxs-lookup"><span data-stu-id="6d894-159">By default, a project that’s been uploaded from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] is locked and can only be edited in Project.</span></span> <span data-ttu-id="6d894-160">لتحرير الملف في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، يجب إلغاء ارتباط الملف.</span><span class="sxs-lookup"><span data-stu-id="6d894-160">To edit the file in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], the file has to be unlinked.</span></span>  

### <a name="edit-in-pn_microsoft_project"></a><span data-ttu-id="6d894-161">تحرير في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="6d894-161">Edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span></span>  

1. <span data-ttu-id="6d894-162">من القائمة الرئيسية، انقر فوق **Project Service** > **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="6d894-162">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="6d894-163">من قائمة المشاريع، افتح المشروع الذي قمت بإنشائه في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-163">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="6d894-164">انقر فوق **فتح في MS Project** من الشريط.</span><span class="sxs-lookup"><span data-stu-id="6d894-164">Click **Open in MS Project** from the ribbon.</span></span> <span data-ttu-id="6d894-165">سيؤدي ذلك إلى فتح الملف الرئيسي المرتبط في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-165">This will open the linked master file in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a><span data-ttu-id="6d894-166">إلغاء ارتباط ملف وتحريره في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span><span class="sxs-lookup"><span data-stu-id="6d894-166">Unlink a file and edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span></span>  

1. <span data-ttu-id="6d894-167">من القائمة الرئيسية، انقر فوق **Project Service** > **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="6d894-167">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="6d894-168">من قائمة المشاريع، افتح المشروع الذي قمت بإنشائه في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-168">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="6d894-169">انقر فوق **إلغاء الارتباط بـ MS Project** من الشريط.</span><span class="sxs-lookup"><span data-stu-id="6d894-169">Click **Unlink from MS Project** from the ribbon.</span></span>  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a><span data-ttu-id="6d894-170">تحميل ملف مشروع إلى SharePoint أو مجموعات Office</span><span class="sxs-lookup"><span data-stu-id="6d894-170">Upload a Project file to SharePoint or Office Groups</span></span>  
 <span data-ttu-id="6d894-171">يمكنك تحميل ملف مشروع إلى SharePoint والعثور عليه ضمن "المستندات المقترنة" لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="6d894-171">You can upload your Project file to SharePoint and find it under the Associated Documents for your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  <span data-ttu-id="6d894-172">يجب أن تطلب من المسؤول تكوين إدارة مستندات في SharePoint وتشغيلها لكيان المشروع.</span><span class="sxs-lookup"><span data-stu-id="6d894-172">You need to have your administrator configure SharePoint document management and turn it on for the Project entity.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="6d894-173">[إعداد تكامل SharePoint](../admin/set-up-sharepoint-integration.md)</span><span class="sxs-lookup"><span data-stu-id="6d894-173">[Set up SharePoint integration](../admin/set-up-sharepoint-integration.md)</span></span>  

 <span data-ttu-id="6d894-174">يمكنك أيضًا تحميل ملف Project إلى [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] إذا قمت بإعداد مجموعات Office.</span><span class="sxs-lookup"><span data-stu-id="6d894-174">You can also upload your Project file to [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] if you have Office Groups set up.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="6d894-175">[التعاون مع الزملاء باستخدام مجموعات Office 365](../basics/collaborate-with-colleagues-using-office-365-groups.md)</span><span class="sxs-lookup"><span data-stu-id="6d894-175">[Collaborate with your colleagues using Office 365 Groups](../basics/collaborate-with-colleagues-using-office-365-groups.md)</span></span>  

### <a name="upload-a-file-for-sharepoint"></a><span data-ttu-id="6d894-176">تحميل ملف لـ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6d894-176">Upload a file for SharePoint</span></span>  

1. <span data-ttu-id="6d894-177">من القائمة الرئيسية، انقر فوق **Project Service** > **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="6d894-177">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="6d894-178">حدد **إلى مستندات مشروع Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="6d894-178">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="6d894-179">في مربع الحوار **تمكين الفتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**، حدد **نعم** أو **لا**.</span><span class="sxs-lookup"><span data-stu-id="6d894-179">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="6d894-180">عندما تنقر فوق **نعم**، ستتمكن من تحديد الزر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** في Project Service Automation وتشغيل [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وتحميل ملف المشروع من مكتبة مستندات SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6d894-180">If you click **Yes**, you'll be able select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="6d894-181">عندما تنقر فوق **لا**، لن يعمل الارتباط الخاص بالزر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**.</span><span class="sxs-lookup"><span data-stu-id="6d894-181">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="6d894-182">يمكن العثور على ملف [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] تحت **المستندات** لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] المعين.</span><span class="sxs-lookup"><span data-stu-id="6d894-182">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

### <a name="upload-a-file-for-office-groups"></a><span data-ttu-id="6d894-183">تحميل ملف لمجموعات Office</span><span class="sxs-lookup"><span data-stu-id="6d894-183">Upload a file for Office Groups</span></span>  

1. <span data-ttu-id="6d894-184">من القائمة الرئيسية، انقر فوق **Project Service** > **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="6d894-184">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="6d894-185">حدد **إلى مستندات مشروع Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="6d894-185">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="6d894-186">في مربع الحوار **تمكين الفتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**، حدد **نعم** أو **لا**.</span><span class="sxs-lookup"><span data-stu-id="6d894-186">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="6d894-187">عندما تنقر فوق **نعم**، ستتمكن من تحديد الزر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** في Project Service Automation وتشغيل [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وتحميل ملف المشروع من مكتبة مستندات SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6d894-187">If you click **Yes**, you'll be able to select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="6d894-188">عندما تنقر فوق **لا**، لن يعمل الارتباط الخاص بالزر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**.</span><span class="sxs-lookup"><span data-stu-id="6d894-188">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="6d894-189">يمكن العثور على ملف [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] تحت **المستندات** لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] المعين.</span><span class="sxs-lookup"><span data-stu-id="6d894-189">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

## <a name="publish--your-project-as-a-template"></a><span data-ttu-id="6d894-190">نشر مشروعك كقالب</span><span class="sxs-lookup"><span data-stu-id="6d894-190">Publish  your project as a template</span></span>  
 <span data-ttu-id="6d894-191">يمكنك حفظ مشروعك وإعادة استخدامه عن طريق حفظه كقالب مشروع في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-191">You can save your project and reuse it by saving it as a project template in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  <span data-ttu-id="6d894-192">تعتبر قوالب المشروع بمثابة خطط مشروع قابلة لإعادة الاستخدام في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-192">Project templates are reusable project plans in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="6d894-193">[إنشاء قالب مشروع (Project Service Automation)](../project-service/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="6d894-193">[Create a project template (Project Service Automation)](../project-service/create-project-template.md)</span></span>  

1. <span data-ttu-id="6d894-194">من علامة التبويب **Project Service**، انقر فوق **نشر** > **قالب مشروع جديد في Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="6d894-194">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project Template**.</span></span>  

2. <span data-ttu-id="6d894-195">في مربع الحوار **نشر في مشروع جديد في قلب Project Service**، أدخل **اسم قالب المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6d894-195">On the **Publish to a new project in Project Service template** dialog box, enter the **Project template name**.</span></span>  

3. <span data-ttu-id="6d894-196">بشكل اختياري، حدد **ربط خطة المشروع بـ Project Service Automation‬** لربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-196">Optionally, check the **Link project plan to Project Service Automation** to link the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

4. <span data-ttu-id="6d894-197">انقر فوق **نشر**.</span><span class="sxs-lookup"><span data-stu-id="6d894-197">Click **Publish**.</span></span>  

<span data-ttu-id="6d894-198">يؤدي ربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى جعل ملف Project الملف الرئيسي وإلى تعيين هيكل تنظيم العمل في قالب [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="6d894-198">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] template to read-only.</span></span>  <span data-ttu-id="6d894-199">لإجراء التغييرات على خطة المشروع، تحتاج إلى إجرائها في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ونشرها كتحديثات إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6d894-199">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>

### <a name="see-also"></a><span data-ttu-id="6d894-200">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="6d894-200">See Also</span></span>  
 [<span data-ttu-id="6d894-201">دليل مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="6d894-201">Project Manager Guide</span></span>](../project-service/project-manager-guide.md)
