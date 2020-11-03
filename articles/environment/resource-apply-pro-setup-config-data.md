---
title: إعداد وتطبيق بيانات التكوين في Common Data Service لـ Project Operations
description: يقدم هذا الموضوع معلومات حول إعداد وتطبيق بيانات التكوين في Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5e72b88a4dae1eb89859fdfd55f6d5e6ee5befcd
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070517"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a>إعداد وتطبيق بيانات التكوين في Common Data Service لـ Project Operations

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

## <a name="install-setup-and-configuration-data"></a>تثبيت بيانات الإعداد والتكوين

1. قم بتنزيل وإلغاء حظر وفك ضغط [حزمة بيانات الإعداد والتكوين](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).
2. انتقل إلى المجلد غير المضغوط وقم بتشغيل الملف القابل للتنفيذ، *DataMigrationUtility*.
3. في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.

![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. في الصفحة 2 من معالج CMT، حدد **Microsoft 365** على أنه **نوع النشر**.
5. حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و **إظهار الخيارات المتقدمة** ‬.
6. حدد منطقة المستأجر، وأدخل بيانات اعتمادك، وحدد **تسجيل الدخول**.

![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي إليها، ثم حدد **تسجيل الدخول**.
8. في الصفحة 4، حدد الملف المضغوط *SampleSetupAndConfigData* من المجلد غير المضغوط.

![اختيار الملف المضغوط](./media/3ZipFile.png)

![تحديد ملف](./media/4SelectAFile.png)

9. بعد تحديد ملف zip، حدد **استيراد البيانات**.

![استيراد البيانات](./media/5ImportData.png)

10. ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة. بعد اكتمال الاستيراد، قم بإنهاء معالج CMT. 
11. راجع مؤسستك للحصول على البيانات في 19 كيان التالي:

  - ‏‏العملة
  - الوحدة التنظيمية
  - جهة اتصال
  - مجموعة الضرائب
  - مجموعة العملاء
  - الوحدة
  - مجموعة وحدات
  - قائمة الأسعار
  - قائمة أسعار معلمات المشروع
  - معدل تكرار الفاتورة
  - فئة المورد القابل للحجز
  - فئة المعاملة
  - فئة المصروفات
  - سعر الدور
  - سعر فئة المعاملة
  - ‏‫الخاصية‬
  - المورد القابل للحجز
  - تعيين فئة المورد القابل للحجز
  - خاصية المورد القابل للحجز

![اكتمال الاستيراد](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a>تحديث تكوينات Project Operations

1. انتقل إلى بيئة CE. يمكنك البحث عنها عن طريق فتح [مركز إدارة Power Platform](https://admin.powerplatform.microsoft.com/environments) وتحديد البيئة ثم تحديد **فتح البيئة**. 

![فتح البيئة](./media/7OpenEnvironment.png)

2. انتقل إلى **المشروعات** > **الموارد** ثم حدد **جديد** لإنشاء مورد قابل للحجز للمستخدم الخاص بك.

![الموارد القابلة للحجز](./media/8BookableResources.png)

3. في علامة التبويب **عام** ، حدد المستخدم المسؤول الخاص بك. تحقق من أن المنطقة الزمنية تتطابق مع تلك التي تعيش فيها. 

![مورد جديد قابل للحجز](./media/9NewBookableResource.png)

4. في علامة تبويب **الجدولة** ، في حقل **الشركة** ، قم اختيار شركة **USPM** ، ثم حدد **حفظ**. 

![علامة تبويب الجدولة](./media/10SchedulingTab.png)

5. حدد علامة التبويب **ساعات العمل**.  

![ساعات العمل](./media/11WorkHours.png)

6. انقر نقرًا مزدوجًا فوق أي قيمة في التقويم وحدد **تحرير** > **كافة الأحداث في السلسلة**. 

![تقويم العمل](./media/12WorkCalendar.png)

7. قم بتغيير ساعات العمل إلى يوم عمل من ثمانية (8) ساعات وقم بتعليم عطلات نهاية الأسبوع على أنها أيام بدون عمل، وتأكد من تطابق المنطقة الزمنية مع المنطقة الخاصة بك. 
8. حدد **حفظ وإغلاق**.

![تحديث التقويم](./media/13UpdateCalendar.png)

9. انتقل إلى **الإعدادات** > **قوالب التقويم** وحدد **جديد**.
 
 ![قوالب التقويم](./media/14CalendarTemplates.png)
 
 10. أدخل اسمًا، وحدد مورد القالب الذي قمت بإنشائه، ثم حدد **حفظ**. 
 
 ![حفظ قالب التقويم](./media/15SaveCalendarTemplate.png)
 
 11. انتقل إلى **المعلمات** وانقر نقرًا مزدوجًا فوق السجل. 
 
 ![معلمات المشروع](./media/16ProjectParameters.png)
 
12. قم بتحديث الحقول التالية:

 - **الشركة الافتراضية** : USPM
 - **الوحدة التنظيمية الافتراضية** : Contoso Robotics Global
 - **تكرار الفاتورة** : اليوم السابع واليوم الأخير
 - **قالب ساعة العمل** : قم بالتغيير إلى القالب الذي قمت بإنشائه.

13. حدد **حفظ**. 

![معلمات المشروع المحدثة](./media/17UpdatedProjectParameters.png)