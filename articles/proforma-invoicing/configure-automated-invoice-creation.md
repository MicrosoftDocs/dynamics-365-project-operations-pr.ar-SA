---
title: تكوين عملية إنشاء فاتورة تلقائية
description: يقدم هذا الموضوع معلومات حول التشغيل السريع لتكوين النظام بحيث يتم إنشاء الفواتير تلقائيًا.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898110"
---
# <a name="configure-automated-invoice-creation"></a>تكوين عملية إنشاء فاتورة تلقائية

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

أكمل الخطوات التالية لتكوين تشغيل فاتورة تلقائية في عمليات المشروع.

1. الانتقال إلى **إعدادات** \> **الوظائف الدفعية**.
2. قم بإنشاء وظيفة دفعية، وقم بتسميتها **إنشاء فواتير عمليات المشروع**. يجب أن يتضمن اسم الوظيفة الدفعية مصطلح "إنشاء الفواتير."
3. في حقل **نوع الوظيفة**، حدد **بلا**. افتراضيًا، يتم تعيين  خيارات **التكرار اليومي** و**نشط** إلى **نعم**.
4. حدد **تشغيل سير العمل**. في مربع حوار **البحث عن سجل**، ستري ثلاث مهام لسير العمل:

    - ProcessRunCaller
    - ProcessRunner
    - UpdateRoleUtilization

5. حدد **ProcessRunCaller**، ثم حدد **إضافة**.
6. في مربع الحوار التالي، حدد **موافق**. يكون سير عمل **السكون** متبوعًا بسير عمل **العملية**.

    يمكنك أيضا تحديد **ProcessRunner** في الخطوة 5. بعد ذلك، عندما تحدد **موافق**، يكون سير عمل **العملية** متبوعًا بسير عمل **السكون**.

يؤدي سير عمل **ProcessRunCaller** و**ProcessRunner** إلى إنشاء الفواتير. **ProcessRunCaller** يستدعي **ProcessRunner**. **ProcessRunner** هو سير العمل الذي ينشئ الفواتير فعليًا. ويمر بكافة بنود العقد التي يجب إنشاء الفواتير لها، ويقوم بإنشاء الفواتير لهذه البنود. لتحديد شروط التعاقد التي يجب إنشاء الفواتير لها، فإن الوظيفة تبحث عن تواريخ تشغيل الفاتورة لشروط التعاقد. إذا كانت بنود العقد التي تنتمي لأحد العقود لها نفس تاريخ تشغيل الفاتورة، سيتم تجميع الحركات في فاتورة واحدة بها بندين للفاتورة. إذا لم تكن هناك حركات لإنشاء فواتير لها، تتخطى الوظيفة إنشاء الفاتورة.

بعد انتهاء تشغيل **ProcessRunner**، فإنه يستدعي **ProcessRunCaller**، الذي يوفر وقت النهاية، وويتم إغلاقه. بعد ذلك يبدأ **ProcessRunCaller** المؤقت الذي يعمل على مدار 24 ساعة من وقت النهاية المحدد. في نهاية المؤقت، يتم إغلاق **ProcessRunCaller**.

تعتبر وظيفة المعالجة الدفعية لإنشاء الفواتير وظيفة متكررة. إذا تم تشغيل هذه المعالجة الدفعية عده مرات، سيتم إنشاء مثيلات متعددة للوظيفة وتتسبب في حدوث أخطاء. بالتالي، يجب عليك بدء عملية المعالجة الدفعية مرة واحدة فقط، وينبغي إعادة تشغيلها في حالة توقفها عن العمل فقط.

> [!NOTE]
> لا يتم تشغيل الفوترة الدفعية إلا لبنود عقد المشروع التي تم تكوينها بواسطة جداول الفواتير. يجب أن يحتوي بند العقد مع طريقة فوترة بسعر ثابت على مراحل مكوّنة. سيحتاج بند عقد المشروع مع طريقة فوترة الوقت والمواد إلى إعداد جدول فاتورة يستند إلى التاريخ. ينطبق الأمر نفسه على بند العقد المستند إلى المشروع.     
