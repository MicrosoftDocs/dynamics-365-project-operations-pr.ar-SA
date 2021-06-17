---
title: تكامل Microsoft Project Client
description: يمكن أن يكون تخطيط جدول المشروع والحفاظ عليه أمرًا معقدًا ، لذلك يحتاج مديرو المشاريع إلى استخدام الأدوات التي تساعدهم في إدارة هذه المهمة. يوفر التكامل مع Microsoft Project Client الدعم لفتح وإدارة هيكل تقسيم عمل المشروع.
author: Yowelle
ms.date: 12/11/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: 032d726bb6206c563b573f30d13fe2697a13c949
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999430"
---
# <a name="microsoft-project-client-integration"></a>تكامل Microsoft Project Client

[!include [banner](../includes/banner.md)]

يمكن أن يكون تخطيط جدول المشروع والحفاظ عليه أمرًا معقدًا ، لذلك يحتاج مديرو المشاريع إلى استخدام الأدوات التي تساعدهم في إدارة هذه المهمة. يوفر التكامل مع Microsoft Project Client الدعم لفتح وإدارة هيكل تقسيم عمل المشروع. يمكن لمدير المشروع نشر أي تغييرات مرة أخرى إلى هيكل تنظيم عمل مشروع Dynamics 365 Finance.

> [!NOTE]
> إذا كنت تستخدم تحديث يوليو (الإصدار 10.0.4)، فيجب عليك تثبيت قاعدة المعارف 4054797 و4055884.

## <a name="configure-the-microsoft-project-client-add-in"></a>تكوين الوظيفة الإضافية لـ Microsoft Project Client
لتمكين التكامل مع Microsoft Project Client، يلزم تثبيت الوظيفة الإضافية لـ Microsoft Dynamics 365 في تطبيق Microsoft Project الخاص بعميل المستخدم. ويتم ذلك من خلال فتح **مساحة عمل إدارة المشاريع**.

•   انقر فوق **تكوين الوظيفة الإضافية لعميل المشروع** من قسم **الارتباطات** > **الإعداد** في مساحة العمل.

•   انقر **فتح**، ثم انقر فوق **تشغيل** عند المطالبة.

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a>فتح وتحرير مسودة هيكل تنظيم العمل الحالي في Microsoft Project Client
إذا كان مشروع في Dynamics 365 Finance يشتمل على هيكل تنظيم عمل تم إنشاؤه بالفعل، يمكن فتح هيكل تنظيم العمل في تطبيق Microsoft Project Client إذا كان هيكل تنظيم العمل في حالة مسودة. للفتح من صفحة **المشروع**، انقر فوق **فتح في Microsoft Project** علامة التبويب **خطة**. يمكن أيضًا فتح هذه الصفحة من تطبيق Microsoft Project Client عن طريق النقر فوق **فتح** في علامة التبويب **Microsoft Dynamics 365**. حدد **الكيان القانوني** و **المشروع** من القائمة.

> [!NOTE]
> إذا كنت تستخدم Internet Explorer كمستعرض، فستحتاج إلى النقر فوق **حفظ** للفتح يدويًا من الموقع الذي يتم تنزيل الملف إليه. أو انقر فوق **حفظ وفتح** لفتح الملف في Microsoft Project Client. لا تقم بإعادة تسميه اسم الملف عند الحفظ.

قبل إجراء أي تعديلات على الملف باستخدام Microsoft Project Client، تحتاج إلى سحبه. انقر فوق **سحب** في علامة التبويب **Microsoft Dynamics 365**. سيمنع هذا المستخدمين الآخرين من تحرير هيكل تنظيم العمل من داخل Finance في نفس الوقت. لنشر هيكل تنظيم العمل بعد إكمال أي تعديلات، انقر فوق **إيداع** في علامة التبويب **Microsoft Dynamics 365**.

إذا تمت إضافة فريق مشروع بالفعل إلى المشروع في Finance ، فسيتم ملء قائمة الموارد بأعضاء الفريق. إذا لم تتم إضافة فريق المشروع إلى المشروع بعد، يمكنك تحديد الموارد وبناء الفريق داخل Microsoft Project Client عن طريق النقر فوق الزر **موارد** في علامة التبويب **Microsoft Dynamics 365**. 

ستتم مزامنة البيانات التالية مره أخرى إلى Finance كجزء من عمليه الإيداع:

•   اسم المهمة

•   تاريخ البدء

•   تاريخ الانتهاء

•   الأنشطة السابقة

•   أسماء الموارد

•   الفئة

•   فئة المورد

•   ساعات العمل

•   الملاحظات

•   الأولوية

> [!NOTE]
> إذا قمت بإضافة أي أعمدة أخرى إلى ملف Microsoft Project Client الخاص بك، فلن يتم حفظها في الملف ولن يتم عرضها عند فتح الملف مرة أخرى.

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a>إنشاء هيكل تنظيم العمل لمشروع موجود باستخدام Microsoft Project Client
لإنشاء هيكل تنظيم عمل جديد باستخدام Microsoft Project Client، اتبع الخطوات التالية:


1.  افتح Microsoft Project Client.

2.  في علامة التبويب **Microsoft Dynamics 365**، انقر فوق **فتح**.

3.  حدد **الكيان القانوني** للمشروع.

4.  حدد **المشروع**.

5.  انقر فوق **سحب** في علامة التبويب **Microsoft Dynamics 365**.

6.  عندما تكون جاهزًا للنشر إلى Finance، انقر فوق **إيداع** في علامة التبويب **Microsoft Dynamics 365**.

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a>استبدال هيكل تنظيم العمل لمشروع موجود باستخدام Microsoft Project Client
لإنشاء هيكل جديد لتنظيم العمل باستخدام Microsoft Project Client واستبدال هيكل تقسيم العمل الحالي لمشروع موجود، اتبع الخطوات التالية:

1.  افتح Microsoft Project Client.

2.  قم بإنشاء الجدول الزمني في Microsoft Project Client.

3.  في علامة التبويب **Microsoft Dynamics 365**، انقر فوق **حفظ التغييرات** > **استبدال المشروع الموجود**.

4.  حدد **الكيان القانوني** للمشروع.

5.  حدد **المشروع**.

6.  انقر فوق **موافق**.

## <a name="create-a-new-project-from-within-microsoft-project-client"></a>إنشاء مشروع جديد من داخل Microsoft Project Client


1.  افتح Microsoft Project Client.

2.  قم بإنشاء الجدول الزمني في Microsoft Project Client.

3.  في علامة التبويب **Microsoft Dynamics 365**، انقر فوق **حفظ التغييرات** > **حفظ إلى مشروع جديد**.

4.  حدد **الكيان القانوني** للمشروع.

5.  أدخل **معرف المشروع**، إذا لزم الأمر.

6.  أدخل **اسم المشروع**.

7.  حدد **نوع المشروع**، و **مجموعة المشاريع**، و **معرف عقد المشروع**. بدلاً من ذلك، يمكنك إنشاء عقد مشروع جديد بالنقر فوق **جديد**.

8.  حدد **التقويم** الذي سيتم استخدامه لتعيين الموارد.

11. انقر فوق **موافق**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]