---
title: تطبيق بيانات العرض التوضيحي لـ Project Operations على بيئة مستضافة في سحابة Finance
description: يوضح هذا الموضوع كيفية تطبيق البيانات التجريبية من Project Operations إلى بيئة Dynamics 365 Finance المستضافة على السحابة.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b9af6c71b61840f4ffdf2892d8e7e5bbf0f8df67
ms.sourcegitcommit: 91ad491e94a421f256a378b0f4b26ed48c67bc93
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/22/2020
ms.locfileid: "4096606"
---
# <a name="apply-project-operations-demo-data-to-a-finance-cloud-hosted-environment"></a>تطبيق بيانات العرض التوضيحي لـ Project Operations على بيئة مستضافة في سحابة Finance

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

> [!IMPORTANT]
> ينطبق هذا الموضوع فقط على Microsoft Dynamics 365 Finance الإصدار 10.0.13 ويمكن تنفيذه فقط على بيئة مستضافة على السحابة. أكمل الخطوات الواردة في هذا الموضوع **قبل** تطبيق تحديثات الجودة على البيئة.

1. في مشروع LCS الخاص بك، افتح صفحة **تفاصيل البيئة**. لاحظ أنه يتضمن التفاصيل اللازمة للاتصال بالبيئة باستخدام بروتوكول سطح المكتب البعيد (RDP).

![تفاصيل بيئة ](./media/1EnvironmentDetails.png)

المجموعة الأولى من بيانات الاعتماد المميزة هي بيانات اعتماد الحسابات المحلية وتحتوي على ارتباط تشعبي إلى الاتصال سطح المكتب البعيد. تتضمن بيانات الاعتماد اسم المستخدم وكلمة المرور الخاصة بمسؤول البيئة. يتم استخدام المجموعة الثانية من بيانات الاعتماد لتسجيل الدخول إلى SQL Server في هذه البيئة.

2. قم بالاتصال بالبيئة بواسطة الارتباط التشعبي في **الحسابات المحلية** ، واستخدم **بيانات اعتماد الحساب المحلي** للمصادقة.
3. انتقل إلى **خدمات معلومات الإنترنت** > **مجموعات التطبيقات** > **AOSService** وأوقف الخدمة. أنت توقف الخدمة عند هذه النقطة لكي يمكنك الاستمرار في استبدال قاعدة بيانات SQL.

![إيقاف AOS](./media/2StopAOS.png)

4. انتقل إلى **الخدمات** وأوقف العنصرين التاليين:

- Microsoft Dynamics 365 Unified Operations: خدمة إدارة الدفعات
- Microsoft Dynamics 365 Unified Operations: إطار عمل تصدير واستيراد البيانات

![إيقاف الخدمات](./media/3StopServices.png)

5. افتح Microsoft SQL Server Management Studio. سجل الدخول باستخدام بيانات اعتماد SQL server واستخدم مستخدم وكلمة مرور axdbadmin من صفحة **تفاصيل البيئة** لـ LCS.

![SQL Server Management Studio](./media/4SSMS.png)

6. في مستكشف الكائنات، **قواعد البيانات** وحدد مكان **AXDB**. ستقوم باستبدال قاعدة البيانات بقاعدة البيانات الجديدة الموجودة في [مركز التنزيل](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip). 
7. انسخ الملف المضغوط إلى VM الذي تتصل به عن بعد وقم باستخراج المحتويات المضغوطة.
8. في SQL Server Management Studio، انقر بزر الماوس الأيمن فوق **AxDB** ، ثم حدد **المهام** > **استعادة** > **قاعدة البيانات**.

![استعادة قاعدة البيانات](./media/5RestoreDatabase.png)

9. حدد **الجهاز المصدر** وانتقل إلى الملف الذي تم استخراجه من الملف المضغوط الذي قمت بنسخه.

![الأجهزة المصدر](./media/6SourceDevice.png)

10. حدد **الخيارات** ، ثم حدد **الكتابة فوق قاعدة البيانات الموجودة** و **إغلاق الاتصالات الموجودة بقاعدة البيانات الوجهة**. 
11. حدد **موافق**.

![استعادة الإعدادات](./media/7RestoreSetting.png)

ستتلقى تأكيدًا بأن عملية استعادة AXDB كانت ناجحة. بعد تلقي هذا التأكيد، يمكنك إغلاق SQL Services Management Studio.

12. ارجع إلى **خدمات معلومات الإنترنت** > **مجموعات التطبيقات** > **AOSService** وابدأ AOSService.
13. انتقل إلى **الخدمات** وأبدا الخدمتين اللتين قمت بإيقافهما في وقت سابق.

14. حدد موقع أداة AdminUserProvisioning في VM هذا. ابحث أسفل، K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.
15. قم بتشغيل ملف .ext باستخدام عنوان المستخدم الخاص بك في حقل **عنوان البريد الإلكتروني**. 
16. حدد **إرسال**.

![تزويد المستخدم المسؤول](./media/8AdminUserProvisioning.png)

يستغرق إكمال هذا الإجراء عدة دقائق. ينبغي أن تتلقي رسالة تأكيد بأن المستخدم المسؤول قد تم تحديثه بنجاح.

17. في النهاية، قم بتشغيل موجه الأوامر كمسؤول وتنفيذ iisreset

![إعادة تعيين IIS](./media/9IISReset.png)

18. قم بإغلاق جلسة عمل سطح المكتب البعيد واستخدم صفحة **تفاصيل بيئة** LCS لتسجيل الدخول إلى البيئة للتأكد من أنها تعمل كما هو متوقع.

![Finance and Operations](./media/10FinanceAndOperations.png)
