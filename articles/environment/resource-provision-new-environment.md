---
title: تزويد بيئة جديدة
description: يوفر هذا الموضوع معلومات حول كيفية تزويد بيئة Project Operations جديدة.
author: sigitac
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 45700371c50e3b5a840df45fc24fa8a5b4584b61
ms.sourcegitcommit: 87b7a8d793c19c50f3765b8d788cde24a6a0ca24
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949346"
---
# <a name="provision-a-new-environment"></a>تزويد بيئة جديدة

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يوفر هذا الموضوع معلومات حول كيفية تزويد بيئة Dynamics 365 Project Operations جديدة للسيناريوهات المستندة إلى المورد/المنتجات غير المخزنة.

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a>تمكين التزويد التلقائي Project Operations في مشروع LCS

استخدم الخطوات التالية لتمكين سير عمل التزويد التلقائي لـ Project Operations لمشروع LCS الخاص بك.

1. انتقل إلى [LCS](https://lcs.dynamics.com/v2) وحدد تجانب **إدارة ميزة المعاينة**.
2. في قائمة **ميزة المعاينة**، قم بتحديد **Project Operations** وحدد **تمكين ميزة المعاينة** لتمكين Project Operations.

> [!NOTE]
> يتم تنفيذ هذه الخطوة مرة واحدة فقط لكل مشروع LCS.

## <a name="provision-a-project-operations-environment"></a>تزويد بيئة Project Operations

1. افتح Dynamics 365 Finance جديد [في بيئة عرض توضيحي](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) أو نشر [بيئة الحماية / الإنتاج](https://docs.microsoft.com/edynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure). 
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

![إعدادات النشر](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> حدد **موافقة** للإقرار بشروط الخدمة ثم حدد **تم** للرجوع إلى إعدادات التوزيع.

![الموافقة على التوزيع](./media/2DeploymentConsent.png)

7. أكمل الحقول المطلوبة المتبقية في المعالج وقم بتأكيد التوزيع. يختلف وقت تزويد البيئة على حسب نوع البيئة. قد تستغرق عملية التزويد ست ساعات.

  بعد اكتمال التوزيع بنجاح، سيتم عرض البيئة بالحالة **تم نشرها**.

8. للتأكد من أنه تم نشر البيئة بنجاح، حدد **تسجيل الدخول** وقم بتسجيل الدخول إلى البيئة للتأكيد.

![تفاصيل بيئة ](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a>تطبيق بيانات العرض التوضيحي لـ Finance في Project Operations (خطوة اختيارية)

طبق بيانات العرض التوضيحي لـ Finance في Project Operations على الإصدار 10.0.13 من البيئة المستضافة على السحابة كما هو موضح في [هذه المقالة](resource-apply-finance-demo-data.md).

## <a name="apply-updates-to-the-finance-environment"></a>تطبيق التحديثات على بيئة Finance

تتطلب Project Operations بيئة Finance بإصدار تطبيق رقم**10.0.13 (10.0.569.20009)** أو الأعلى.

قد تحتاج إلى تطبيق تحديثات الجودة على بيئة Finance لديك لاستلام هذا الإصدار.

1. في LCS، في صفحة **تفاصيل البيئة**، في قسم **التحديثات المتوفرة**، حدد **عرض التحديث**.

![عرض التحديثات](./media/5ViewUpdates.png)

2. في صفحة **التحديثات الثنائية**، حدد **حفظ الحزمة.**

![حفظ الحزمة](./media/6SavePackage.png)

3. انقر فوق **تحديد الكل** ثم حدد **حفظ الحزمة**.

![مراجعة التحديثات وحفظها](./media/7ReviewAndSaveUpdates.png)

4. أدخل اسمًا ووصفًا للحزمة، ثم حدد **حفظ**. تبعًا لاتصال الإنترنت، قد تستغرق هذه العملية بعض الوقت.

![تحميل الحزمة إلى مكتبة الأصول](./media/8UploadPackageToAssetsLibrary.png)

5. بعد حفظ الحزمة، حدد **تم** وقم بحفظ هذه الحزمة في مكتبة الأصول في مشروع LCS الخاص بك.

قد يستغرق حفظ الحزمة والتحقق من صحتها ~ 15 دقيقة.

6. لتطبيق التحديث، انتقل إلى صفحة **تفاصيل البيئة** في LCS وحدد **الصيانة** > **تطبيق التحديثات**.

![صيانة البيئات](./media/9MaintainEnvironment.png)

7. في قائمة التحديثات، قم بتحديد الحزمة التي قمت بإنشائها، وقم بتحديد **تطبيق**.

![تطبيق التحديثات](./media/10ApplyUpdates.png)

ستستغرق عملية "صيانة البيئة" بعض الوقت. بعد انتهائها، ستعود البيئة إلى حالة تم نشرها.

![البيئة المنشورة](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a>إنشاء اتصال كتابة مزدوج 

1. في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.
2. تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات**.
3. بعد اكتمال الارتباط، حدد **ربط بـ CDS للتطبيقات‏‎** مرة أخرى. ستتم إعادة توجيهك إلى الكتابة المزدوجة في Finance.

![ربط بـ CDS](./media/12LinktoCDS.png)

4. حدد **تطبيق الحل** للوصول إلى الكيانات التي سيتم تعيينها في التكامل.

![تطبيق الحلول](./media/13ApplySolutions.png)

5. حدد كلا الحلين، **Dynamics 365 Finance and Operations خريطة كيان الكتابة المزدوجة** و**خرائط كيان الكتابة المزدوجة في Dynamics 365 Project Operations**، ثم حدد **تطبيق**.

![تأكيد الحلول](./media/14ConfirmSolutions.png)

بعد تطبيق الحلول، يتم تطبيق كيانات الكتابة المزدوجة على البيئة.

![تطبيق الحلول](./media/15ApplyingSolutions.png)

بعد تطبيق الكيانات، يتم سرد كافة التعيينات المتوفرة في البيئة.

![خرائط الكتابة المزدوجة](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a>تحديث كيانات البيانات بعد التحديث

1. في Finance، انتقل إلى مساحة عمل **إدارة البيانات**.

![مساحة عمل إدارة البيانات](./media/16DataManagement.png)

2. حدد تجانب **معلمات إطار العمل**.

![معلمات إطار العمل](./media/17FrameworkParameters.png)

3. في صفحة **إعدادات الكيان**، حدد **تحديث قائمة الكيانات**.

![تحديث قائمة الكيانات](./media/18RefreshEntityList.png)

سيستغرق التحديث مدة 20 دقيقة تقريبًا. وستتلقى تحذيرًا عند اكتماله.

![تأكيد التحديث](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a>تشغيل خرائط ‏‫الكتابة المزدوجة في Project Operations

1. في مشروع LCS الخاص بك، انتقل إلى صفحة **تفاصيل البيئة**.
2. تحت **Common Data Service معلومات البيئة**، حدد **ربط بـ CDS للتطبيقات.** بعد تحديد الارتباط، ستتم إعادة توجيهك إلى قائمة الكيانات الموجودة في التعيينات.
3. ابدأ الخرائط كما هو موضح في الجدول التالي. تأكد من اتباع التسلسل كما هو موضح.

| **تعيين الكيان** | **تحديث الكيان** | **المزامنة الأولية** | **أصل المزامنة الأولية** | **تشغيل المتطلبات الأساسية** | **المزامنة الأولية للمتطلبات الأساسية** |
| --- | --- | --- | --- | --- | --- |
| **أدوار موارد المشروع لجميع الشركات (bookableresourcecategories)** | Yes | ‏‏نعم | Common Data Service | Yes | ‏‫غير متوفر‬ |
| **الكيانات القانونية (cdm\_الشركات)** | Yes | ‏‏نعم | تطبيقات Finance and Operations | Yes | ‏‫غير متوفر‬ |
| **القيم الفعلية لتكامل Project Operations(msdyn\_القيم الفعلية)** | Yes | Yes | ‏‫غير متوفر‬ | ‏‏نعم | Yes |
| **بنود عقد المشروع (salesorderdetails)** | Yes | Yes | ‏‫غير متوفر‬ | Yes | Yes |
| **كيان التكامل لعلاقات معاملات المشروع (msdyn\_transactionconnections)** | Yes | Yes | ‏‫غير متوفر‬ | Yes | ‏‫غير متوفر‬ |
| **المراحل الرئيسية لبنود تعاقد التكامل مع Project Operations (msdyn\_contractlinesscheduleofvalues)** | Yes | Yes | ‏‫غير متوفر‬ | Yes | ‏‫غير متوفر‬ |
| **كيان تكامل Project Operations لتقديرات المصروفات (msdyn\_estimateslines)** | Yes | Yes | ‏‫غير متوفر‬ | Yes | ‏‫غير متوفر‬ |
| **كيان تكامل Project Operations لتقديرات الساعات (msdyn\_resourceassignments)** | Yes | Yes | ‏‫غير متوفر‬ | Yes | ‏‫غير متوفر‬ |
| **كيان تصدير مصروفات مشروع لتكامل Project Operations (msdyn\_مصروفات)** | ‏‏نعم | Yes | ‏‫غير متوفر‬ | Yes | ‏‫غير متوفر‬ |
| **كيان تكامل Project Operations لتقديرات الساعات (msdyn\_resourceassignments)** | ‏‏نعم | Yes | ‏‫غير متوفر‬ | Yes | ‏‫غير متوفر‬ |

4. لتحديث الكيان، حدد اسم الخريطة، ثم حدد **تحديث الكيانات**. 
5. تابع تشغيل الخريطة بعد اكتمال التحديث.

![تحديث الخريطة‬](./media/20RefreshMapping.png)

قبل تمكين الخريطة التالية، تحقق من أن الخريطة الموجودة في الجدول بالحالة **تشغيل**. قد يستغرق تشغيل الخرائط بعدد كبير من المتطلبات المسبقة بعض الوقت.

لتشغيل خريطة بالمتطلبات المسبقة، قم بتمكين تبديل **إظهار خرائط الكيانات المرتبطة**. إذا كان الجدول يشير إلى أن **المزامنة الأولية للمتطلبات الأساسية** بالقيمة **لا**، فتحقق من أن علامة **المزامنة الأولية** قيد **الإيقاف** في كافة خرائط المتطلبات الأساسية قبل تشغيلها.

![تشغيل الخريطة](./media/21RunMap.png)

6. تحقق من صحة كافة الخرائط ذات الصلة بالمشروع وأنها بالحالة تشغيل.

![كل الخرائط قيد التشغيل](./media/22AllMapsRunning.png)

تم الآن تزويد بيئة Project Operations وتكوينها.
