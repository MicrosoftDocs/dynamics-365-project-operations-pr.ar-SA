---
title: تزويد بيئة جديدة
description: يوفر هذا المقال معلومات حول كيفية تزويد بيئة Project Operations جديدة.
author: sigitac
ms.date: 09/13/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 78f40ebe79c038799fbc59902442ad6c23fb94d4
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028481"
---
# <a name="provision-a-new-environment"></a>تزويد بيئة جديدة

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_



يقدم هذا المقال معلومات حول كيفية تزويد بيئة Dynamics 365 Project Operations جديدة للسيناريوهات المستندة إلى الموارد/المنتجات غير المخزنة‬.

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a>تمكين التزويد التلقائي Project Operations في مشروع LCS

استخدم الخطوات التالية لتمكين سير عمل التزويد التلقائي لـ Project Operations لمشروع LCS الخاص بك.

1. انتقل إلى [LCS](https://lcs.dynamics.com/v2) وحدد تجانب **إدارة ميزة المعاينة**.
2. في قائمة **ميزة المعاينة**، حدد **ميزة Project Operations** ثم حدد **تمكين ميزة المعاينة** لتمكين Project Operations.

   > [!NOTE]
   > يتم تنفيذ هذه الخطوة مرة واحدة فقط لكل مشروع LCS.

## <a name="provision-a-project-operations-environment"></a>تزويد بيئة Project Operations

1. افتح Dynamics 365 Finance جديد [بيئة العرض](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) أو توزيع [بيئة اختبار معزولة / الإنتاج](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure). 
2. اتبع خطوات معالج **تزويد البيئة**. 

   > [!IMPORTANT]
   > تأكد من أن إصدار التطبيق المحدد 10.0.13 أو أحدث.

3. لتزويد Project Operations، ضمن **إعدادات متقدمة**، حدد **Common Data Service**. 
4. قم بتمكين **إعداد Common Data Service** من خلال اختيار **نعم** ثم أدخل المعلومات في الحقول المطلوبة:

  - اسم
  - المنطقة
  - اللغة‬
  - ‏‏العملة
 
5. في حقل **قالب Common Data Service**، حدد **Project Operations** 
6. حدد نوع البيئة لعملية التوزيع الخاصة بك. سيتيح لك الإصدار التجريبي الذي يستند إلى الاشتراك نشر بيئة CDS لمدة 30 يومًا. 

     ![إعدادات النشر.](./media/1DeploymentSettings.png)

    > [!IMPORTANT]
    > حدد **موافقة** للإقرار بشروط الخدمة ثم حدد **تم** للرجوع إلى إعدادات التوزيع.
    >
    >![الموافقة على التوزيع.](./media/2DeploymentConsent.png)

7. اختياري - تطبيق بيانات تجريبية على البيئة. انتقل إلى **إعدادات متقدمة**، وحدد **تخصيص تكوين قاعدة بيانات SQL**، ثم قم بتعيين **تحديد مجموعة البيانات لقاعدة بيانات التطبيق** إلى **عرض توضيحي**.
8. أكمل الحقول المطلوبة المتبقية في المعالج وقم بتأكيد التوزيع. يختلف وقت توفير البيئة وفقا لنوع البيئة. قد تستغرق عملية التزويد ست ساعات.

   بعد اكتمال التوزيع بنجاح، سيتم عرض البيئة بالحالة **تم نشرها**.

9. لتأكيد نشر البيئة بنجاح، قم بتحديد **تسجيل الدخول** سجل الدخول إلى البيئة للتأكيد.

    ![تفاصيل البيئة.](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a>تطبيق التحديثات على بيئة Finance

تتطلب Project Operations بيئة Finance بإصدار تطبيق رقم **10.0.13 (10.0.569.20009)** أو الأعلى.

قد تحتاج إلى تطبيق تحديثات الجودة على بيئة Finance لديك لاستلام هذا الإصدار.

1. في LCS، في صفحة **تفاصيل البيئة**، في قسم **التحديثات المتوفرة**، حدد **عرض التحديث**.

    ![عرض التحديثات.](./media/5ViewUpdates.png)

2. في صفحة **التحديثات الثنائية**، حدد **حفظ الحزمة.**

    ![حفظ الحزمة.](./media/6SavePackage.png)

3. انقر فوق **تحديد الكل** ثم حدد **حفظ الحزمة**.

    ![مراجعة التحديثات وحفظها.](./media/7ReviewAndSaveUpdates.png)

4. أدخل اسمًا ووصفًا للحزمة، ثم حدد **حفظ**. تبعًا لاتصال الإنترنت، قد تستغرق هذه العملية بعض الوقت.

    ![تحميل الحزمة إلى مكتبة الأصول.](./media/8UploadPackageToAssetsLibrary.png)

5. بعد حفظ الحزمة، حدد **تم** وقم بحفظ هذه الحزمة في مكتبة الأصول في مشروع LCS الخاص بك.

   قد يستغرق حفظ الحزمة والتحقق من صحتها ~ 15 دقيقة.

6. لتطبيق التحديث، انتقل إلى صفحة **تفاصيل البيئة** في LCS وحدد **الصيانة** > **تطبيق التحديثات**.

    ![صيانة البيئات.](./media/9MaintainEnvironment.png)

7. في قائمة التحديثات، قم بتحديد الحزمة التي قمت بإنشائها، وقم بتحديد **تطبيق**.

    ![تطبيق التحديثات.](./media/10ApplyUpdates.png)

   ستستغرق عملية "صيانة البيئة" بعض الوقت. بعد انتهائها، ستعود البيئة إلى حالة تم نشرها.

    ![البيئة المنشورة.](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a>إنشاء اتصال كتابة مزدوج 

1. في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.
2. تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات**.
3. بعد اكتمال الارتباط، حدد **ربط بـ CDS للتطبيقات‏‎** مرة أخرى. ستتم إعادة توجيهك إلى الكتابة المزدوجة في Finance.

    ![ربط بـ CDS.](./media/12LinktoCDS.png)

4. حدد **تطبيق الحل** للوصول إلى الكيانات التي سيتم تعيينها في التكامل.

    ![تطبيق الحلول.](./media/13ApplySolutions.png)

5. حدد كلا الحلين، **مخطط كيان الكتابة المزدوجة لـ Dynamics 365 Finance and Operations** و **Dynamics 365 Project Operations مخططات كيان الكتابة المزدوجة**، ثم حدد **تطبيق**.

    ![تأكيد الحلول.](./media/14ConfirmSolutions.png)

    بعد تطبيق الحلول، يتم تطبيق كيانات الكتابة المزدوجة على البيئة.

    ![تطبيق الحلول.](./media/15ApplyingSolutions.png)

    بعد تطبيق الكيانات، يتم سرد كافة التعيينات المتوفرة في البيئة.

    ![خرائط الكتابة المزدوجة.](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a>تحديث كيانات البيانات بعد التحديث

1. في Finance، انتقل إلى مساحة عمل **إدارة البيانات**.

    ![مساحة عمل إدارة البيانات.](./media/16DataManagement.png)

2. حدد تجانب **معلمات إطار العمل**.

    ![معلمات إطار العمل.](./media/17FrameworkParameters.png)

3. في صفحة **إعدادات الكيان**، حدد **تحديث قائمة الكيانات**.

    ![تحديث قائمة الكيانات.](./media/18RefreshEntityList.png)

سيستغرق التحديث مدة 20 دقيقة تقريبًا. وستتلقى تحذيرًا عند اكتماله.

  ![تأكيد التحديث.](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a>تحديث إعدادات الأمان على Project Operations في Dataverse

1. انتقل إلى Project Operations في بيئة Dataverse الخاصة بك. 
2. انتقل إلى **الإعدادات** > **الأمان** > **أدوار الأمان**. 
3. في صفحة **أدوار الأمان**، في قائمة الأدوار، حدد **مستخدم تطبيق الكتابة المزدوجة** وحدد علامة التبويب **الكيانات المخصصة**.  
4. تحقق من أن الدور يحتوي على أذونات **القراءة** و **الإلحاق** للكيانات التالية:
      
      - **نوع سعر الصرف للعملة**
      - **مخطط الحسابات**
      - **التقويم المالي**
      - **دفتر الأستاذ**
      - **الشركة**
      - **المصروفات**

5. بعد تحديث دور الأمان، انتقل إلى **الإعدادات** > **الأمان** > **الفرق**، وحدد الفريق الافتراضي في طريق عرض الفريق **مالك العمل المحلي**.
6. حدد **إدارة الأدوار** وتحقق من أن امتياز أمان **مستخدم تطبيق الكتابة المزدوجة** يتم تطبيقه على هذا الفريق.

## <a name="run-project-operations-dual-write-maps"></a>تشغيل خرائط ‏‫الكتابة المزدوجة في Project Operations

1. في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.
2. تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات.** بعد تحديد الارتباط، ستتم إعادة توجيهك إلى قائمة الكيانات الموجودة في التعيينات.
3. ابدأ الخرائط. لمزيد من المعلومات، راجع [إصدارات مخططات الكتابة المزدوجة لـ Project Operations](resource-dual-write-maps.md#project-operations-dual-write-maps)
4. تحقق من صحة كافة الخرائط ذات الصلة بالمشروع وأنها بالحالة تشغيل.

    ![كل الخرائط قيد التشغيل.](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a>تطبيق بيانات التكوين في CDS لـ Project Operations (اختياري)

إذا كنت قد قمت بتطبيق بيانات العرض التوضيحي على بيئة Finance، فراجع [إعداد بيانات التكوين وتطبيقها في Common Data Service لـ Project Operations](resource-apply-pro-setup-config-data.md) لتطبيق بيانات العرض التوضيحي على بيئة CDS.


تم الآن تزويد بيئة Project Operations وتكوينها. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
