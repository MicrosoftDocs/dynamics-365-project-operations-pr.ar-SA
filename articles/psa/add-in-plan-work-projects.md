---
title: خطط لعملك في Microsoft Project مع الوظيفة الإضافية Project Service
description: يوفر هذا الموضوع معلومات حول كيفية استخدام الوظيفة الإضافية لـ Microsoft project في Microsoft project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 01/07/2021
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
ms.openlocfilehash: 471d3c421cd9dc39a5864e37ef762b5d08e59762
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285512"
---
# <a name="plan-your-work-in-microsoft-project-with-the-project-service-add-in"></a>خطط لعملك في Microsoft Project مع الوظيفة الإضافية Project Service

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3x](../includes/cc-applies-to-psa-app-3x.md)]

يسهّل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] عملية التخطيط للمشاريع، بما في ذلك التقديرات. يمكنك تعريف العمل لكي تكون قيمة التكاليف والجهود والمبيعات واضحة عند تقديم الاقتراح النهائي.  

يمكنك تثبيت [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] والقيام بأعمال التخطيط في بيئة [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] المألوفة. استخدم قدرات التخطيط والإدارة الفعالة من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ثم قم بتحديث خطة مشروعك في Project Service Automation.  

> [!IMPORTANT]
> - لاستخدام ميزة إدارة المستندات في SharePoint لتخزين ملفات [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] لمشاريع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، سيحتاج مسؤول [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] إلى تشغيل إدارة المستندات. 
> - يتوافق [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] فقط مع [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.  

## <a name="download-and-install-the-add-in"></a>تنزيل الوظيفة الإضافية وتثبيتها  
 تأكد من أن معلومات تسجيل الدخول إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] جاهزة. سوف تحتاج إلى هذه المعلومات للاتصال من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] بميزة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  من مركز التنزيل ، يمكنك تنزيل الوظيفة الإضافية للإصدار المدعوم من Project Service، إما [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) أو [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  حدد ارتباط التنزيل.  

3.  عند اكتمال التنزيل، حدد **نعم** لتثبيت الوظيفة الإضافية.  

## <a name="configure-the-add-in"></a>تكوين الوظيفة الإضافية  

1. افتح [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وحدد علامة التبويب **Project Service**.  

2. حدد **اتصال**.  

3. أدخل معلومات تسجيل الدخول، ثم حدد **تسجيل الدخول**.  

   يمكنك الآن بدء استخدام الوظيفة الإضافية.  

## <a name="read-from-a-template"></a>القراءة من قالب  
 يمكنك القراءة من قالب أنشأته في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ونسخه إلى [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] لبدء تخطيط المشروع. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [إنشاء قالب مشروع (Project Service Automation)](../psa/create-project-template.md)  

1.  من علامة التبويب **Project Service**، حدد **قراءة** > **قالب مشروع Project Service Automation**.  

2.  اختر قالب مشروع من القائمة وحدد **فتح**.  

    > [!NOTE]
    >  بشكل افتراضي، يتم تعيين المهام المنسوخة من القالب إلى Project على أنها مجدولة يدويًا.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>تعيين أدوار [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى موارد المشروع  

1.  افتح مشروعًا، ثم حدد شريط **المهام**.  

2. حدد قائمة **مخطط جانت**، ثم اختر **ورقة الموارد**.  

3. على ورقة الموارد، حدد القائمة المنسدلة **دور موارد Project Service** واختر دور Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>تعيين موارد للمشروع  

1.  من علامة التبويب Project Service، حدد صفًا، ثم حدد **البحث عن موارد**.  

2.  على شاشة **حجز مورد**، حدد المورد الذي تريد استخدامه للمشروع.  

3.  حدد **حجز**، ثم قم بتحديد **موافق**.  

## <a name="publish-your-project"></a>نشر المشروع  
عند اكتمال عملية تخطيط المشروع، الخطوة التالية هي استيراد المشروع ونشره في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

سيتم استيراد المشروع إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. يتم تطبيق عملية إنشاء الفريق والتسعير. افتح المشروع في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للتأكد من إنشاء الفريق وتقديرات المشروع وهيكل تنظيم العمل. يبين الجدول التالي المكان حيث يمكن العثور على النتائج.


|              Microsoft Project                                                           |                      Project Service Automation                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **مخطط جانت**   | استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **هيكل تنظيم العمل**. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **ورقة الموارد** |   استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **أعضاء فريق المشروع**.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **الاستخدام**    |    استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **تقديرات المشروع**.     |

**لاستيراد مشروعك ونشره**  
1. في علامة التبويب **Project Service**، انتقل إلى **نشر** > **مشروع جديد في Project Service Automation**.  

2. في مربع الحوار **نشر في مشروع جديد في Project Service**، أدخل **اسم المشروع** وحدد **العميل**.  

3. اختر **‏‫ربط خطة المشروع بـ Project Service Automation‬** بشكل اختياري لربط ملف خطة Project بـ Project Service Automation.  

4. حدد **نشر**.  

   يؤدي ربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى جعل ملف Project الملف الرئيسي وإلى تعيين هيكل تنظيم العمل في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للقراءة فقط.  لإجراء التغييرات على خطة المشروع، تحتاج إلى إجرائها في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ونشرها كتحديثات إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>تحرير مشروع تم استيراده  
 لإجراء تغييرات على خطة مشروع تم استيراده إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، يمكنك التحديد من ضمن خيارين:  

- فتح الملف الرئيسي وتحريره في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- إلغاء ارتباط الملف الرئيسي وتحريره في Project Service بشكل مباشر. بشكل افتراضي، يكون المشروع الذي يتم تحميله من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] مؤمنًا ويمكن تحريره فقط في Project. لتحرير الملف في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، يجب إلغاء ارتباط الملف.  

### <a name="edit-in-pn_microsoft_project"></a>تحرير في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. من القائمة الرئيسية، انتقل إلى **Project Service** > **المشاريع**.  

2. من قائمة المشاريع، افتح المشروع الذي قمت بإنشائه في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. حدد **فتح في MS Project** من الشريط. سيؤدي ذلك إلى فتح الملف الرئيسي المرتبط في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>إلغاء ارتباط ملف وتحريره في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service  

1. من القائمة الرئيسية، انتقل إلى **Project Service** > **المشاريع**.  

2. من قائمة المشاريع، افتح المشروع الذي قمت بإنشائه في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. حدد **إلغاء الارتباط بـ MS Project** من الشريط.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>تحميل ملف مشروع إلى SharePoint أو مجموعات Office  
 يمكنك تحميل ملف مشروع إلى SharePoint والعثور عليه ضمن "المستندات المقترنة" لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] الخاص بك.  يجب أن تطلب من المسؤول تكوين إدارة مستندات في SharePoint وتشغيلها لكيان المشروع. 

 يمكنك أيضًا تحميل ملف Project إلى [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] إذا قمت بإعداد مجموعات Office.

### <a name="upload-a-file-for-sharepoint"></a>تحميل ملف لـ SharePoint  

1. من القائمة الرئيسية، انتقل إلى **Project Service** > **تحميل**.  

2. حدد **إلى مستندات مشروع Project Service Automation**.  

3. في مربع الحوار **تمكين الفتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**، حدد **نعم** أو **لا**.  

   - عندما تحدد **نعم** ستتمكن من تحديد زر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** في Project Service Automation وتشغيل [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وتحميل ملف المشروع من مكتبة مستندات SharePoint.  

   - إذا قمت بتحديد **لا** ، فلن يعمل الارتباط **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**.  

4. يمكن العثور على ملف [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] تحت **المستندات** لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] المعين.  

### <a name="upload-a-file-for-office-groups"></a>تحميل ملف لمجموعات Office  

1. من القائمة الرئيسية، انتقل إلى **Project Service** > **تحميل**.  

2. حدد **إلى مستندات مشروع Project Service Automation**.  

3. في مربع الحوار **تمكين الفتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**، حدد **نعم** أو **لا**.  

   - عندما تحدد **نعم** ستتمكن من تحديد زر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** في Project Service Automation وتشغيل [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وتحميل ملف المشروع من مكتبة مستندات SharePoint.  

   - إذا قمت بتحديد **لا** ، فلن يعمل الارتباط **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**.  

4. يمكن العثور على ملف [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] تحت **المستندات** لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] المعين.  

## <a name="publish--your-project-as-a-template"></a>نشر مشروعك كقالب  
 يمكنك حفظ مشروعك وإعادة استخدامه عن طريق حفظه كقالب مشروع في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. تعتبر قوالب المشروع بمثابة خطط مشروع قابلة لإعادة الاستخدام في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. لمزيد من المعلومات، راجع [إنشاء قالب مشروع (Project Service Automation)](../psa/create-project-template.md). 

1. في علامة التبويب **Project Service**، انتقل إلى **نشر** > **قالب مشروع جديد في Project Service Automation**.  

2. في مربع الحوار **نشر في مشروع جديد في قلب Project Service**، أدخل **اسم قالب المشروع**.  

3. حدد **ربط خطة المشروع بـ Project Service Automation‬** بشكل اختياري لربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. حدد **نشر**.  

يؤدي ربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى جعل ملف Project الملف الرئيسي وإلى تعيين هيكل تنظيم العمل في قالب [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للقراءة فقط.  لإجراء التغييرات على خطة المشروع، تحتاج إلى إجرائها في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ونشرها كتحديثات إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

## <a name="read-a-resource-loaded-schedule"></a>قراءة جدول تحميل الموارد

عند قراءة مشروع من Project Service Automation ، لا تتم مزامنة تقويم المورد مع عميل سطح المكتب. إذا كانت هناك اختلافات في مدد المهمة أو الجهد أو الانتهاء ، فربما يرجع ذلك إلى أن الموارد وعميل سطح المكتب ليس لهما نفس تقويم قالب ساعة العمل المطبق على المشروع.


## <a name="data-synchronization"></a>مزامنة البيانات
توفر الجداول في هذا القسم معلومات حول مزامنة بيانات الكيان بين Project Service Automation والوظيفة الإضافية لسطح المكتب Microsoft Project.

### <a name="project-task-entity-table"></a>جدول كيان مهمة المشروع
يوضح الجدول التالي كيفية مزامنة بيانات كيان مهمة المشروع بين Project Service Automation والوظيفة الإضافية لسطح مكتب Microsoft Project.

| **كيان.** | **الحقل** | **Microsoft Project إلى Project Service Automation** | **Project Service Automation إلى Microsoft Project** |
| --- | --- | --- | --- |
| مهمة المشروع | تاريخ الاستحقاق | Synchronized | غير متزامنة |
| مهمة المشروع | الجهود التقديرية | Synchronized | غير متزامنة |
| مهمة المشروع | معرف عميل MS Project | Synchronized | غير متزامنة |
| مهمة المشروع | المهمة الأصل | Synchronized | غير متزامنة |
| مهمة المشروع | Project | Synchronized | غير متزامنة |
| مهمة المشروع | مهمة المشروع | Synchronized | غير متزامنة |
| مهمة المشروع | اسم مهمة المشروع | Synchronized | غير متزامنة |
| مهمة المشروع | وحدة تعيين الموارد ‏‫(ميزة مهملة في الإصدار 3.0)‬ | Synchronized | غير متزامنة |
| مهمة المشروع | المدة المجدولة | Synchronized | غير متزامنة |
| مهمة المشروع | تاريخ البدء | Synchronized | غير متزامنة |
| مهمة المشروع | معرف WBS | Synchronized | غير متزامنة |

### <a name="team-member-entity-table"></a>جدول كيانات أعضاء الفريق
يوضح الجدول التالي كيفية مزامنة بيانات كيان عضو الفريق بين Project Service Automation والوظيفة الإضافية لـ Micros.

| **كيان.** | **الحقل** | **Microsoft Project إلى Project Service Automation** | **Project Service Automation إلى Microsoft Project** |
| --- | --- | --- | --- |
| عضو الفريق | معرف عميل MS Project | Synchronized | غير متزامنة |
| عضو الفريق | اسم المنصب | Synchronized | غير متزامنة |
| عضو الفريق | المشروع | Synchronized | Synchronized |
| عضو الفريق | فريق المشروع | Synchronized | Synchronized |
| عضو الفريق | وحدة تعيين الموارد | غير متزامنة | Synchronized |
| عضو الفريق | الدور | غير متزامنة | Synchronized |
| عضو الفريق | ساعات العمل | غير متزامنة | غير متزامنة |

### <a name="resource-assignment-entity-table"></a>جدول كيانات تعيين الموارد
يوضح الجدول التالي كيفية مزامنة بيانات كيان تعيين الموارد بين Project Service Automation والوظيفة الإضافية لـ Micros.

| **كيان.** | **الحقل** | **Microsoft Project إلى Project Service Automation** | **Project Service Automation إلى Microsoft Project** |
| --- | --- | --- | --- |
| تعيين المورد | من تاريخ | Synchronized | غير متزامنة |
| تعيين المورد | ساعات‬ | Synchronized | غير متزامنة |
| تعيين المورد | معرف عميل MS Project | Synchronized | غير متزامنة |
| تعيين المورد | العمل المخطط | Synchronized | غير متزامنة |
| تعيين المورد | Project | Synchronized | غير متزامنة |
| تعيين المورد | فريق المشروع | Synchronized | غير متزامنة |
| تعيين المورد | تعيين المورد | Synchronized | غير متزامنة |
| تعيين المورد | مهمة | Synchronized | غير متزامنة |
| تعيين المورد | إلى التاريخ | Synchronized | غير متزامنة |

### <a name="project-task-dependencies-entity-table"></a>جدول كيانات تبعيات مهام المشروع
يوضح الجدول التالي كيفية مزامنة بيانات كيان تبعيات مهام المشروع بين Project Service Automation والوظيفة الإضافية لـ Micros.

| **كيان.** | **الحقل** | **Microsoft Project إلى Project Service Automation** | **Project Service Automation إلى Microsoft Project** |
| --- | --- | --- | --- |
| تبعيات مهمة المشروع | تبعية مهمة المشروع | Synchronized | غير متزامنة |
| تبعيات مهمة المشروع | نوع الارتباط | Synchronized | غير متزامنة |
| تبعيات مهمة المشروع | مهمة النشاط السابق | Synchronized | غير متزامنة |
| تبعيات مهمة المشروع | Project | Synchronized | غير متزامنة |
| تبعيات مهمة المشروع | المهمة اللاحقة | Synchronized | غير متزامنة |

### <a name="additional-resources"></a>الموارد الإضافية
 [دليل مدير المشروع](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]