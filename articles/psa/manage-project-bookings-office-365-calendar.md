---
title: إدارة المشاريع والحجوزات في تقويم Office 365 الخاص بك
description: كيفية إدارة المشاريع والحجوزات في تقويم Office 365 الخاص بك
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: fd4119693875fb851c7bd3f34287db7d81237140
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070678"
---
# <a name="manage-projects-and-bookings-in-your-calendar-project-service"></a>إدارة المشاريع والحجوزات في تقويمك في (Project Service)

> [!Note]
> مهمل: هذه الميزة تم إهمالها ولم تعد متوفرة.

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] 

يمكنك عرض المواعيد الشخصية والحجوزات الخاصة بأعمال المشروع وتعيينات أوامر عمل Field Service باستخدام تقويم [!INCLUDE[pn_office_365](../includes/pn-office-365.md)].  
  
 من خلال وضع كل شيء في مكانه الصحيح، ستتمكن من إدارة عملك اليومي بسهولة. تتوفر اجتماعاتك ومواعيدك وحجوزاتك ومهامك كلها في تقويمك في [!INCLUDE[pn_office_365](../includes/pn-office-365.md)].  
  
 إذا كنت تستخدم [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]، فيمكنك أيضًا إدخال مواعيدك الشخصية في طريقة عرض إدخال الوقت في Project Service. من شأن ذلك أن يسمح لمدراء المشاريع والموارد بمعرفة ما إذا كنت متوفرًا للعمل على المشاريع. كما أنه يوفر لك الوقت، لأنك لست بحاجة إلى إدخال معلومات حول مواعيدك الشخصية مرتين. يمكنك ببساطة استيراد المواعيد الشخصية من تقويمك إلى طريقة عرض إدخال الوقت في Project Service.‬  
  
 وسيقوم التقويم بمزامنة حجوزات المشروع وأوامر العمل اعتبارًا من اليوم وحتى الأسابيع الأربعة القادمة. لا يمكن تغيير هذا الإعداد.  
  
 تكون المزامنة مدعومة في اتجاه واحد فقط، من PSA إلى تقويم [!INCLUDE[pn_office_365](../includes/pn-office-365.md)]. يمكنك إجراء المزامنة بالترتيب العكسي. 
  
 لمعرفة كيفية استخدام تقويم [!INCLUDE[pn_office_365](../includes/pn-office-365.md)]، راجع [التقويم في Outlook على الويب للعمل](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936).  
  
## <a name="setup"></a>الإعداد  
 قبل أن تتمكن من رؤية حجوزاتك وإدارتها على تقويم [!INCLUDE[pn_office_365](../includes/pn-office-365.md)]، تحتاج إلى إعداد بعض الأشياء.  
  
- يجب أن تتوفر لديك بيانات اعتماد مسؤول النظام أو المسؤول العمومي في [!INCLUDE[pn_office_365](../includes/pn-office-365.md)].  
  
- سيحتاج المسؤول إلى تكوين ملف تعريف خادم البريد الإلكتروني وسيحتاج كل مستخدم إلى تكوين علبة البريد الخاصة به. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [إعداد معالجة البريد الإلكتروني من خلال المزامنة من جانب الخادم](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)  
  
## <a name="turn-on-synchronization-for-your-organization-admin-task"></a>تشغيل المزامنة لمؤسسة (مهمة المسؤول)  
  
1.  من القائمة الرئيسية، انقر فوق **الإعدادات** > **الإدارة**.  
  
2.  انقر فوق **إعدادات النظام**.  
  
3.  انقر فوق علامة التبويب **المزامنة**.  
  
4.  ضمن **حدد إذا ما كان يمكن مزامنة حجز الموارد مع** ، حدد **مزامنة حجز الموارد مع Outlook**.  
  
## <a name="turn-on-synchronization-for-your-user-profile-user-task"></a>تشغيل المزامنة لملف تعريف المستخدم (مهمة المسؤول)  
  
1.  انقر فوق زر **الإعدادات** في الركن العلوي الأيسر من الشاشة.  
  
2.  انقر فوق **خيارات**.  
  
3.  انقر فوق علامة التبويب **المزامنة**  
  
4.  ضمن **مزامنة حجز الموارد مع Outlook** ، حدد **حجز موارد المزامنة مع Outlook**.  
  
## <a name="import-your-personal-appointments-user-task"></a>استيراد المواعيد الشخصية (مهمة المستخدم)  
 يمكنك استيراد المواعيد الشخصية من تقويمك إلى طريقة عرض إدخال الوقت في Project Service Automation.‬  
  
1. افتح تقويم [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] وانقر فوق **استيراد البيانات**.  
  
2. في شاشة عوامل التصفية، حدد **المواعيد من Exchange** ، ثم انقر فوق **تطبيق**.  
  
3. سوف يسحب النظام المواعيد إلى طريقة عرض إدخال الوقت كإدخالات مقترحة من الأسبوع الحالي. لإضافة إدخالات لأسبوع آخر، انقر فوق **السابق** أو **التالي**.  
  
4. حدد الموعد الذي تريد إضافته إلى طريقة عرض إدخال الوقت في Project Service Automation.  
  
5. على المربع المنبثق **إدخال الوقت** ، حدد الخيارات المناسبة لتحويل الموعد إلى طريقة عرض إدخال الوقت في Project Service Automation..  
  
6. انقر فوق **حفظ**.  
  
### <a name="see-also"></a>راجع أيضًا  
 [دليل الوقت والمصروفات والتعاون](../psa/time-expense-collaboration-guide.md)
