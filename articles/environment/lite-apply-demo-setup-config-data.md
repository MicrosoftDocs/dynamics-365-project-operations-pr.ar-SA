---
title: تطبيق اعداد بيانات العرض التوضيحي وبيانات التكوين
description: يقدم هذا الموضوع معلومات حول كيفية تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين في Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42e02f393e89d20b2a462645f519a3792bee8f2f
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948717"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a>تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين لعملية نشر Project Operations Lite – التعامل مع الفواتير الأولية‬.‬

_**النشر الخفيف - التعامل مع الفواتير الأولية_

1. قم بتنزيل [حزمة البيانات الرئيسية](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip). 
2. انتقل إلى المجلد *ProjOpsDemoDataSetupAndMaster - Integrated CMT*، وقم بتشغيل الملف القابل للتنفيذ *DataMigrationUtility*.
3. في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.

![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. في الصفحة 2 من معالج CMT، حدد **Office 365** على أنه **نوع النشر**.
5. حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و**إظهار الخيارات المتقدمة**‬.
6. حدد منطقة المستأجر، وأدخل بيانات اعتمادك، ثم حدد **تسجيل الدخول**.

![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي اليها، ثم حدد **تسجيل الدخول**.
8. في الصفحة 4، حدد ملف zip، *MasterAndSetupData*، من المجلد الذي تم فك ضغطه، *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.

![ملف مضغوط](./media/3ZipFile.png)

![تحديد ملف](./media/4SelectAFile.png)

9. بعد تحديد ملف zip، حدد **استيراد البيانات**.

![استيراد البيانات](./media/5ImportData.png)

10. ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة. بعد اكتمالها، يمكنك إنهاء معالج CMT. 
11. راجع مؤسستك للحصول على البيانات في الكيانات العشرين التالية:

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
- تفاصيل تكرار الفاتورة
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
