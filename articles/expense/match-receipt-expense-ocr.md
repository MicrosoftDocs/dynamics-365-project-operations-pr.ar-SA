---
title: مطابقة إيصال بمصروفات باستخدام OCR
description: يوفر هذا الموضوع معلومات حول معالجة التعرف البصري على الأحرف (OCR) للإيصالات.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 02c1bafbe907a657689b610ae792f88085320903
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896985"
---
# <a name="match-a-receipt-to-an-expense-using-ocr"></a>مطابقة إيصال بمصروفات باستخدام OCR

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

تم تحسين إدخال المصاريف من خلال إدخال معالجة التعرف الضوئي على الأحرف (OCR) للإيصالات. تم تصميم هذه الوظيفة لتحسين تجربة المستخدم عند إنشاء تقارير المصروفات.

## <a name="key-features"></a>الميزات الأساسية

- يقوم النظام باستخراج اسم التاجر والتاريخ والمبلغ الإجمالي من الإيصالات.
- سيحاول النظام مطابقة الإيصالات غير المرفقة بحركات المصروفات غير المرفقة.
- يمكنك إنشاء حركات مصروفات تم إدخالها يدويًا من الإيصالات.

## <a name="attach-receipts-to-an-expense-report"></a>إرفاق إيصالات بتقرير مصروفات

لإرفاق إيصالات بحركات بطاقة الائتمان تلقائيًا عند إنشاء تقرير مصروفات، أكمل الخطوات التالية.

  1. افتح مساحة عمل **إدارة المصروفات** .
  2. في علامة التبويب **الإيصالات** ، تحقق من وجود إيصالات غير مرفقة. يمكنك أيضًا تحميل الإيصالات من علامة التبويب **إيصالات** .
  3. في علامة التبويب **المصروفات** ، تحقق من وجود مصروفات غير مرفقة. وعادة ما يقوم مسؤول المصروفات باستيراد هذه المصروفات من موفر بطاقة الائتمان.
  4. حدد **تقرير مصروفات جديد**. لاحظ أنه يمكنك تضمين المصاريف والإيصالات الآن أيضًا عند إنشاء تقرير المصاريف. إذا أضفت كلاً من المصاريف والإيصالات، فسيتم تشغيل المطابقة التلقائية للإيصالات مقابل النفقات.

## <a name="create-or-match-receipts-to-an-expense-report"></a>إنشاء أو مطابقة إيصالات بتقرير مصروفات
لإنشاء مصروفات أو مطابقة مصروفات من إيصال، أكمل الخطوات التالية.

  1. في تقرير المصروفات، في علامة التبويب **الإيصالات** ، قم بإرفاق إيصال من خلال تحديد **إضافة إيصالات**.
  2. ضمن الصورة التي تم تحميلها من الإيصال، لاحظ خيارات **الإنشاء** و **المطابقة** .

      - حدد **إنشاء** لإنشاء حركة مصروفات تم إدخالها يدويًا وملء القيم التي تم استخراجها من الإيصال.
      - إذا قمت بتحديد **مطابقة**، سيحاول النظام مطابقة المصروفات الحالية بالإيصال.

## <a name="installation"></a>التثبيت

لاستخدام إمكانيات المصروفات المتقدمة هذه، قم بتثبيت الوظيفة الإضافية لخدمة إدارة المصروفات لـ Microsoft Dynamics 365 Finance، وقم بتشغيل الميزات الموجودة في المثيل الخاص بك. يمكنك الوصول إلى الوظيفة الإضافية من مشروعك الخاص في Microsoft Dynamics Lifecycle Services (LCS).

1. قم بتسجيل الدخول إلى LCS، وافتح البيئة المطلوبة.
2. انتقل إلى **التفاصيل الكاملة**.
3. حدد **صيانة** أو قم بالتمرير لأسفل إلى علامة التبويب السريع **الوظائف الإضافية الخاصة بالبيئة** .
4. حدد **تثبيت وظيفة إضافية جديدة**.
5. حدد **خدمة إدارة المصروفات**.
6. اتبع دليل التثبيت، ووافق علي البنود والشروط.
7. حدد **تثبيت**.

في مساحة عمل **إدارة الميزات** ، قم بتشغيل الميزات التالية:

- إعادة صياغة تقارير المصروفات
- المطابقة التلقائية للمصروفات وإنشاءها من الإيصال

عند تشغيل هذه الميزات، تحدث الإجراءات التالية:

- يتم استبدال مساحة عمل **إدارة المصروفات** الموجودة بمساحة العمل الجديدة.
- تتم إضافة عنصر قائمة جديد لرؤية حقل المصروفات.
- لا يزال بإمكانك فتح صفحة **تقارير المصروفات** السابقة من خلال الانتقال إلى **إدارة المصروفات > مصروفاتي > تقارير المصروفات**.
- وتستمر عمليات سير العمل وأي موافقات في الانتقال إلى صفحه تقارير المصروفات الموجودة.
- ستتم معالجة الايصالات من خلال Microsoft Azure Cognitive Services، وسيتم استخراج بيانات التعريف وإضافتها.
- تمت إضافة خيار يتيح لك إنشاء تقرير مصروفات يتضمن الإيصالات غير المرفقة المتطابقة.
- يتيح لك الخيار الذي تمت إضافته إلى تقارير المصاريف إنشاء بند مصروفات من إيصال، أو يحاول مطابقة إيصال موجود ببند مصاريف موجود.

## <a name="frequently-asked-questions"></a>الأسئلة الشائعة

**هل تستخدم Microsoft البيانات الخاصة بي لنماذجها؟**

لا، لقد أنشأت Microsoft نموذجًا عامًا للتعلم الآلي لخدمة معالجة الإيصالات. لا يستند هذا النموذج إلى الايصالات التي قمت بتحميلها.

**أين تتوفر هذه الميزة وأين تتم معالجتها؟**

يتم دعمه حاليًا في الولايات المتحدة.

**إلى أين تذهب إيصالاتي؟**

ستتصل الشركة المالية بالخدمات الإدراكية لاستخراج بيانات الحقل. سوف تحتفظ الخدمات الإدراكية بنسخة من إيصالك لفترة تصل إلى 24 ساعة أثناء حدوث المعالجة. بعد اكتمال المعالجة، ستقوم خدمات الإدراك بإزالة الإيصال. لا تزال الإيصالات مُخزنة في التمويل.

لمزيد من المعلومات، راجع [تمكين فهم الإيصالات باستخدام الإمكانية الجديدة لأداة التعرف على النماذج](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).
