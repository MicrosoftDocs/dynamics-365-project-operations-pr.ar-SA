---
title: استخدام الوظيفة الإضافية Project Service لتخطيط عملك في Microsoft Project | MicrosoftDocs
description: يوفر هذا الموضوع معلومات حول كيفية إضافة وتكوين واستخدام الوظيفة الإضافية لـ Microsoft project لـ Microsoft project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
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
ms.openlocfilehash: 9556feac5481e20bde1c9624c0eccc05385eaa94
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145972"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a>استخدام الوظيفة الإضافية Project Service Automation لتخطيط عملك في Microsoft Project

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

يسهّل [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] عملية التخطيط للمشاريع، بما في ذلك التقديرات. يمكنك تعريف العمل لكي تكون قيمة التكاليف والجهود والمبيعات واضحة عند تقديم الاقتراح النهائي.  

 يمكنك الآن تثبيت [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] والقيام بأعمال التخطيط في بيئة [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] المألوفة. استخدم قدرات التخطيط والإدارة الفعالة من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ثم قم بتحديث خطة مشروعك في Project Service Automation.  

> [!IMPORTANT]
> - لاستخدام ميزة إدارة المستندات في SharePoint لتخزين ملفات [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] لمشاريع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، سيحتاج مسؤول [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] إلى تشغيل إدارة المستندات. 
> - يتوافق [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] فقط مع [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.  

## <a name="download-and-install-the-add-in"></a>تنزيل الوظيفة الإضافية وتثبيتها  
 تأكد من أن معلومات تسجيل الدخول إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] جاهزة. سوف تحتاج إلى هذه المعلومات للاتصال من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] بميزة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  من مركز التنزيل ، يمكنك تنزيل الوظيفة الإضافية للإصدار المدعوم من Project Service، إما [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) أو [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  انقر فوق ارتباط التنزيل.  

3.  عند اكتمال التنزيل، انقر فوق **نعم** لتثبيت الوظيفة الإضافية.  

## <a name="configure-the-add-in"></a>تكوين الوظيفة الإضافية  

1. افتح [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وانقر فوق علامة التبويب **Project Service**.  

2. انقر فوق **Connect**.  

3. أدخل معلومات تسجيل الدخول، ثم انقر فوق **تسجيل الدخول**.  

   يمكنك الآن بدء استخدام الوظيفة الإضافية.  

## <a name="read-from-a-template"></a>القراءة من قالب  
 يمكنك القراءة من قالب أنشأته في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ونسخه إلى [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] لبدء تخطيط المشروع. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [إنشاء قالب مشروع (Project Service Automation)](../psa/create-project-template.md)  

1.  من علامة التبويب **Project Service**، انقر فوق **قراءة** > **قالب مشروع Project Service Automation**.  

2.  اختر قالب مشروع من القائمة وانقر فوق **فتح**.  

    > [!NOTE]
    >  بشكل افتراضي، يتم تعيين المهام المنسوخة من القالب إلى Project على أنها مجدولة يدويًا.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>تعيين أدوار [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى موارد المشروع  

1.  افتح مشروعًا، ثم انقر فوق شريط **المهام**.  

2.  انقر فوق قائمة **مخطط جانت**، ثم اختر **ورقة الموارد**.  

3.  على ورقة الموارد، انقر فوق القائمة المنسدلة **دور موارد Project Service** واختر دور Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>تعيين موارد للمشروع  

1.  من علامة التبويب Project Service، حدد صفًا، ثم انقر فوق **البحث عن موارد**.  

2.  على شاشة **حجز مورد**، حدد المورد الذي تريد استخدامه للمشروع.  

3.  انقر فوق **حجز**، ثم انقر فوق **موافق**.  

## <a name="publish-your-project"></a>نشر المشروع  
عند اكتمال عملية تخطيط المشروع، الخطوة التالية هي استيراد المشروع ونشره في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

سيتم استيراد المشروع إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. يتم تطبيق عملية إنشاء الفريق والتسعير. افتح المشروع في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للتأكد من إنشاء الفريق وتقديرات المشروع وهيكل تنظيم العمل. يبين الجدول التالي المكان حيث يمكن العثور على النتائج:


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **مخطط جانت**   | استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **هيكل تنظيم العمل**. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **ورقة الموارد** |   استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **أعضاء فريق المشروع**.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **الاستخدام**    |    استيراد إلى شاشة [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **تقديرات المشروع**.     |

**لاستيراد مشروعك ونشره**  
1. من علامة التبويب **Project Service**، انقر فوق **نشر** > **مشروع جديد في Project Service Automation**.  

2. في مربع الحوار **نشر في مشروع جديد في Project Service**، أدخل **اسم المشروع** وحدد **العميل**.  

3. حدد **‏‫ربط خطة المشروع بـ Project Service Automation‬** بشكل اختياري لربط ملف خطة Project بـ Project Service Automation.  

4. انقر فوق **نشر**.  

   يؤدي ربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى جعل ملف Project الملف الرئيسي وإلى تعيين هيكل تنظيم العمل في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للقراءة فقط.  لإجراء التغييرات على خطة المشروع، تحتاج إلى إجرائها في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ونشرها كتحديثات إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>تحرير مشروع تم استيراده  
 لإجراء تغييرات على خطة مشروع تم استيراده إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، يمكنك التحديد من ضمن خيارين:  

- فتح الملف الرئيسي وتحريره في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- إلغاء ارتباط الملف الرئيسي وتحريره في Project Service بشكل مباشر. بشكل افتراضي، يكون المشروع الذي يتم تحميله من [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] مؤمنًا ويمكن تحريره فقط في Project. لتحرير الملف في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، يجب إلغاء ارتباط الملف.  

### <a name="edit-in-pn_microsoft_project"></a>تحرير في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. من القائمة الرئيسية، انقر فوق **Project Service** > **المشاريع**.  

2. من قائمة المشاريع، افتح المشروع الذي قمت بإنشائه في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. انقر فوق **فتح في MS Project** من الشريط. سيؤدي ذلك إلى فتح الملف الرئيسي المرتبط في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>إلغاء ارتباط ملف وتحريره في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service  

1. من القائمة الرئيسية، انقر فوق **Project Service** > **المشاريع**.  

2. من قائمة المشاريع، افتح المشروع الذي قمت بإنشائه في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. انقر فوق **إلغاء الارتباط بـ MS Project** من الشريط.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>تحميل ملف مشروع إلى SharePoint أو مجموعات Office  
 يمكنك تحميل ملف مشروع إلى SharePoint والعثور عليه ضمن "المستندات المقترنة" لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] الخاص بك.  يجب أن تطلب من المسؤول تكوين إدارة مستندات في SharePoint وتشغيلها لكيان المشروع. 

 يمكنك أيضًا تحميل ملف Project إلى [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] إذا قمت بإعداد مجموعات Office.

### <a name="upload-a-file-for-sharepoint"></a>تحميل ملف لـ SharePoint  

1. من القائمة الرئيسية، انقر فوق **Project Service** > **تحميل**.  

2. حدد **إلى مستندات مشروع Project Service Automation**.  

3. في مربع الحوار **تمكين الفتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**، حدد **نعم** أو **لا**.  

   - عندما تنقر فوق **نعم**، ستتمكن من تحديد الزر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** في Project Service Automation وتشغيل [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وتحميل ملف المشروع من مكتبة مستندات SharePoint.  

   - عندما تنقر فوق **لا**، لن يعمل الارتباط الخاص بالزر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**.  

4. يمكن العثور على ملف [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] تحت **المستندات** لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] المعين.  

### <a name="upload-a-file-for-office-groups"></a>تحميل ملف لمجموعات Office  

1. من القائمة الرئيسية، انقر فوق **Project Service** > **تحميل**.  

2. حدد **إلى مستندات مشروع Project Service Automation**.  

3. في مربع الحوار **تمكين الفتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**، حدد **نعم** أو **لا**.  

   - عندما تنقر فوق **نعم**، ستتمكن من تحديد الزر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** في Project Service Automation وتشغيل [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] وتحميل ملف المشروع من مكتبة مستندات SharePoint.  

   - عندما تنقر فوق **لا**، لن يعمل الارتباط الخاص بالزر **فتح في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**.  

4. يمكن العثور على ملف [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] تحت **المستندات** لمشروع [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] المعين.  

## <a name="publish--your-project-as-a-template"></a>نشر مشروعك كقالب  
 يمكنك حفظ مشروعك وإعادة استخدامه عن طريق حفظه كقالب مشروع في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  تعتبر قوالب المشروع بمثابة خطط مشروع قابلة لإعادة الاستخدام في [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [إنشاء قالب مشروع (Project Service Automation)](../psa/create-project-template.md)  

1. من علامة التبويب **Project Service**، انقر فوق **نشر** > **قالب مشروع جديد في Project Service Automation**.  

2. في مربع الحوار **نشر في مشروع جديد في قلب Project Service**، أدخل **اسم قالب المشروع**.  

3. بشكل اختياري، حدد **ربط خطة المشروع بـ Project Service Automation‬** لربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. انقر فوق **نشر**.  

يؤدي ربط ملف Project بـ [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] إلى جعل ملف Project الملف الرئيسي وإلى تعيين هيكل تنظيم العمل في قالب [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] للقراءة فقط.  لإجراء التغييرات على خطة المشروع، تحتاج إلى إجرائها في [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ونشرها كتحديثات إلى [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

## <a name="read-a-resource-loaded-schedule"></a>قراءة جدول تحميل الموارد

عند قراءة مشروع من Project Service Automation ، لا تتم مزامنة تقويم المورد مع عميل سطح المكتب. إذا كانت هناك اختلافات في مدد المهمة أو الجهد أو الانتهاء ، فربما يرجع ذلك إلى أن الموارد وعميل سطح المكتب ليس لهما نفس تقويم قالب ساعة العمل المطبق على المشروع.


## <a name="data-synchronization"></a>مزامنة البيانات

يوضح الجدول التالي كيفية مزامنة البيانات بين Project Service Automation والوظيفة الإضافية لسطح مكتب Microsoft Project.

| **كيان.** | **الحقل** | **Microsoft Project إلى Project Service Automation** | **Project Service Automation إلى Microsoft Project** |
| --- | --- | --- | --- |
| مهمة المشروع | تاريخ الاستحقاق | ● | - |
| مهمة المشروع | الجهود التقديرية | ● | - |
| مهمة المشروع | معرف عميل MS Project | ● | - |
| مهمة المشروع | المهمة الأصل | ● | - |
| مهمة المشروع | Project | ● | - |
| مهمة المشروع | مهمة المشروع | ● | - |
| مهمة المشروع | اسم مهمة المشروع | ● | - |
| مهمة المشروع | وحدة تعيين الموارد ‏‫(ميزة مهملة في الإصدار 3.0)‬ | ● | - |
| مهمة المشروع | المدة المجدولة | ● | - |
| مهمة المشروع | تاريخ البدء | ● | - |
| مهمة المشروع | معرف WBS | ● | - |

| **كيان.** | **الحقل** | **Microsoft Project إلى Project Service Automation** | **Project Service Automation إلى Microsoft Project** |
| --- | --- | --- | --- |
| عضو الفريق | معرف عميل MS Project | ● | - |
| عضو الفريق | اسم المنصب | ● | - |
| عضو الفريق | المشروع | ● | ● |
| عضو الفريق | فريق المشروع | ● | ● |
| عضو الفريق | وحدة تعيين الموارد | - | ● |
| عضو الفريق | الدور | - | ● |
| عضو الفريق | ساعات العمل | غير مُزامن | غير مُزامن |

| **كيان.** | **الحقل** | **Microsoft Project إلى Project Service Automation** | **Project Service Automation إلى Microsoft Project** |
| --- | --- | --- | --- |
| تعيين المورد | من تاريخ | ● | - |
| تعيين المورد | ساعات‬ | ● | - |
| تعيين المورد | معرف عميل MS Project | ● | - |
| تعيين المورد | العمل المخطط | ● | - |
| تعيين المورد | Project | ● | - |
| تعيين المورد | فريق المشروع | ● | - |
| تعيين المورد | تعيين المورد | ● | - |
| تعيين المورد | مهمة | ● | - |
| تعيين المورد | إلى التاريخ | ● | - |

| **كيان.** | **الحقل** | **Microsoft Project إلى Project Service Automation** | **Project Service Automation إلى Microsoft Project** |
| --- | --- | --- | --- |
| تبعيات مهمة المشروع | تبعية مهمة المشروع | ● | - |
| تبعيات مهمة المشروع | نوع الارتباط | ● | - |
| تبعيات مهمة المشروع | مهمة النشاط السابق | ● | - |
| تبعيات مهمة المشروع | Project | ● | - |
| تبعيات مهمة المشروع | المهمة اللاحقة | ● | - |

### <a name="see-also"></a>راجع أيضًا  
 [دليل مدير المشروع](../psa/project-manager-guide.md)
