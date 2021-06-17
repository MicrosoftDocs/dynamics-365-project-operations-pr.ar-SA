---
title: تطبيق إعداد العرض التوضيحي وبيانات التكوين - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين في Project Operations.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7729b4a9ef5f498b78af298f7233d7dd45434bb3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997135"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>تطبيق إعداد العرض التوضيحي وبيانات التكوين لـ Project Operations - خفيف 

_**النشر الخفيف - التعامل مع الفواتير الأولية_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a>المتطلبات الأساسية

قبل بدء التكوين، يجب أن تتوفر لديك بيئة Common Data Service (CDS) تم تزويدها لـ Dynamics 365 Project Operations.


## <a name="instructions"></a>إرشادات

1. قم بتنزيل [حزمة البيانات الرئيسية](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip). 
2. انتقل إلى المجلد *ProjOpsSampleSetupData - CE only CMT* وقم بتشغيل الملف القابل للتنفيذ *DataMigrationUtility*.
3. في الصفحة 1 من معالج ترحيل تكوين (CMT) Common Data Service، حدد **استيراد البيانات** ثم حدد **متابعة**.

    ![ترحيل التكوين](./media/1ConfigurationMigration.png)

4. في الصفحة 2 من معالج CMT، حدد **Microsoft 365** على أنه **نوع النشر**.
5. حدد خانتي الاختيار **عرض قائمة بالمؤسسات المتاحة** و **إظهار الخيارات المتقدمة**‬.
6. حدد منطقة المستأجر، وأدخل بيانات اعتمادك، ثم حدد **تسجيل الدخول**.

   ![تسجيل الدخول إلى التكوين](./media/2ConfigurationSignin.png)

7. في الصفحة 3، من قائمة المؤسسات على المستأجر، حدد المؤسسة التي ترغب في استيراد بيانات العرض التوضيحي اليها، ثم حدد **تسجيل الدخول**.
8. في الصفحة 4، حدد الملف المضغوط، *SampleSetupAndConfigData* من المجلد المفكوك الحزمة *ProjOpsSampleSetupData - CE only CMT*.

   ![ملف مضغوط](./media/3ZipFile.png)

   ![تحديد ملف](./media/4SelectAFile.png)

9. بعد تحديد ملف zip، حدد **استيراد البيانات**.

   ![استيراد البيانات](./media/5ImportData.png)

10. ستعمل عملية الاستيراد لمدة عشر دقائق تقريبًا حسب سرعة الشبكة. بعد اكتمالها، يمكنك إنهاء معالج CMT. 
11. راجع مؤسستك للحصول على البيانات في 18 كيان التالي:

    -   عملة
    -   الحساب
    -   الوحدة التنظيمية
    -   ‏‫جهة الاتصال‬
    -   الوحدة
    -   مجموعة وحدات
    -   قائمة الأسعار
    -   قائمة أسعار معلمات المشروع 
    -   معدل تكرار الفاتورة
    -   فئة المورد القابل للحجز
    -   فئة المعاملة
    -   فئة المصروفات
    -   سعر الدور
    -   سعر فئة المعاملة
    -   ‏‫الخاصية‬
    -   المورد القابل للحجز
    -   تعيين فئة المورد القابل للحجز
    -   خاصية المورد القابل للحجز

    ![اكتمال الاستيراد](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
