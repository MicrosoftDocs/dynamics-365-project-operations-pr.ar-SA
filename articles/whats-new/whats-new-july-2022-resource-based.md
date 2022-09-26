---
title: الجديد في يوليو 2022 - Project Operations للسيناريوهات المستندة إلى المنتجات غير المخزنة/الإنتاج
description: يوفر هذا المقال معلومات عن تحديثات الجودة المتوفرة في إصدار يونيو 2022 من Microsoft Dynamics 365 Project Operations للسيناريوهات المستندة إلى موارد/غير مخزنة.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: e63b29741dbaa400a2176ff8b4c35c6d64dfeab4
ms.sourcegitcommit: 7ed8e77a92917f2d242988ca02bd7de9571cce5e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/02/2022
ms.locfileid: "9403935"
---
# <a name="whats-new-july-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>الجديد في يوليو 2022 - Project Operations للسيناريوهات المستندة إلى المنتجات غير المخزنة/الإنتاج

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

ينطبق هذا المقال على المكونات والإصدارات التالية من Microsoft Dynamics 365 Project Operations:

- Project Operations في بيئة Dataverse الإصدار 4.44.0.22
- إدارة المشاريع والمحاسبة في بيئة Dynamics 365 Finance، الإصدار 10.0.28

## <a name="project-operations-dual-write-maps-updates"></a>تحديثات مخططات ‏‫الكتابة المزدوجة في Project Operations

لا توجد تحديثات لخرائط الكتابة المزدوجة في Project Operations لهذا الإصدار. للحصول على القائمة والإصدارات الحالية لخرائط الكتابة المزدوجة في Project Operations، راجع [إصدارات خرائط الكتابة المزدوجة لـ Project Operations](../environment/resource-dual-write-maps.md).

قم دائمًا بتشغيل أحدث إصدار من الخريطة في بيئتك، وتمكين جميع خرائط الجدول ذات الصلة أثناء تحديث حل Project Operations Dataverse وإصدار حل Finance. قد لا تعمل بعض الميزات والإمكانات بشكل صحيح إذا لم يتم تنشيط أحدث إصدار من الخريطة. يمكن عرض الإصدار النشط من المخطط في عمود **الإصدار** في الصفحة **الكتابة المزدوجة**. لتنشيط إصدار جديد من المخطط، حدد **إصدارات مخطط الجدول** ثم حدد الإصدار الأخير ثم احفظ الإصدار المحدد. إذا كنت قد قمت بتخصيص خريطة جداول جاهزة للاستخدام، فأعد تطبيق التغييرات. مزيد من المعلومات، راجع [إدارة دورة حياة التطبيقات](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

إذا واجهت مشكلة في بدء تشغيل الخريطة، فاتبع الإرشادات الموجودة في قسم [مشكلة أعمدة الجدول المفقودة على الخرائط](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) في دليل استكشاف الأخطاء وإصلاحها للكتابة المزدوجة.

## <a name="quality-updates"></a>التحديثات الإصلاحية

### <a name="project-operations-on-dataverse"></a>Project Operations على Dataverse

| منطقة الميزات | رقم المرجع | تحديث إصلاحي |
| --- | --- | --- |
| التوزيع والتكوين | 2761472  | يتم معالجة خطأ تثبيت Project Operations. |
| الفوترة والتسعير | 2746940  | يجب أن يكون الحد الأقصى لطول اسم شرط التعاقد من الباطن هو 100 حرف. |
| الفوترة والتسعير | 2739162  | يجب أن يكون العملاء قادرين على رؤية أزرار الشريط في طريقة عرض خطوط الشبكة للقيم الفعلية. |
| تخطيط المشاريع وتعقبها | 2730318  | التحقق من الصحة المحدث للأحرف غير المدعومة في موضوع المشروع. |
| الفوترة والتسعير | 2705361  | يجب تضمين القيم الفعلية للمبيعات التي تم فوترتها جزئيًا في حقول تعقب المشروع. |
| الفوترة والتسعير | 2675880  | منع اتصال مشروع بشرط تعاقد غير مستند إلى العمل. |
| الفوترة والتسعير | 2664396  | في حالة حفظ قائمة أسعار عرض الأسعار من دون عرض أسعار، يجب أن يظهر إشعار بالخطأ لأن عرض الأسعار لا يمكن أن يكون فارغًا. |
| الفوترة والتسعير | 2184019  | ينبغي عدم عرض علامة التبويب **الفوترة المستندة إلى المهام** للمشاريع التي ليس لها عقود داعمة أو عرض أسعار. |
| الوقت والمصروفات | 2754459  | عندما تكون الجدولة المتكررة لسير مهام السحابة غير نشطة، فاعرض الشعار وتجاوز المعالجة غير المتزامنة. |
| الفوترة والتسعير | 2724391  | يتم طرح استثناء خطأ عندما يفقد قاعدة فوترة تقسيم عقد المشروع قيمة العميل. |
| الفوترة والتسعير | 2708638  | لم يتم العثور على السجل أثناء البحث باستخدام البحث في الشبكة في استخدامات المواد والموافقات على استخدامات المواد.|
| الفوترة والتسعير | 2686977  | امنع التحقق من صحة سطر الفاتورة أثناء إنشاء الفاتورة. |
| الفوترة والتسعير | 2683032  | لا يتم توسيع نسخ الأدوار والفئات المسؤولة لما يتجاوز عدد 5000 سجل.|
| الفوترة والتسعير | 2673363  | يحدث تلف في ‏‫النسبة المئوية لاستهلاك التكلفة‬ في المشروع عندما تكون كل من تقديرات الجهد والمصروفات القيم الفعلية موجودة لمشروع ما. |

### <a name="project-management-and-accounting-in-finance"></a>إدارة المشاريع والمحاسبة في Finance

للحصول على معلومات حول إصلاحات الأخطاء المضمنة في هذا التحديث، سجل دخولك إلى Microsoft Dynamics Lifecycle Services (LCS)، واستعرض [مقال KB (قاعدة المعارف)](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).

## <a name="features-turned-on-by-default-in-upcoming-release"></a>يتم تشغيل الميزات افتراضيًا في الإصدار القادم

يسرد الجدول التالي الميزات المشغلة افتراضيًا في الإصدار 10.0.29. يمكن إيقاف تشغيل معظم الميزات التي يتم تشغيلها تلقائيًا في [إدارة الميزات](/dynamics365/fin-ops-core/fin-ops/get-started/feature-management/feature-management-overview). في المستقبل، قد يتم إزالة بعض الميزات التي يتم تشغيلها تلقائيًا من ميزة إدارة الميزات وقد تصبح إلزامية. ويضمن هذا التغيير أن العملاء يستخدمون الوظيفة الحالية، ومن ثم يمكن أن تقوم التحسينات بالبناء على الوظيفة الحالية عند إضافتهم. لن يتم تمكين الميزات تلقائيًا أبدًا في أقل من عام واحد ما لم تكن محددة على أنها أساسية.

| اسم الميزة | تاريخ التمكين | ‬‏‫تمت إضافة الميزة‬‏‫ | حالة الميزة | وحدة نمطية |
| --- | --- | --- |--- |--- |
| تمكين تعديل العمل بالساعة بناءً على التغيير في تخصيص قاعدة التمويل | 16 سبتمبر 2022 | 7 اكتوبر 2020 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| ميزة إلغاء فاتورة الدفع المقدم لأمر الشراء الخاص بالمشروع | 16 سبتمبر 2022 | 6 اكتوبر 2021 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| حذف بنود مقترح الفاتورة عند استخدام Project Operations للسيناريوهات المستندة إلى المورد/غير المخزنة | 16 سبتمبر 2022 | 6 اكتوبر 2021 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| ضبط المحاسبة على معاملة مشروع مرحلة | 16 سبتمبر 2022 | 10 مايو 2020 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| تمكين إعداد المحاسبة الافتراضية للمشروع | 16 سبتمبر 2022 | 19 فبراير 2020 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| تمكين شروط تعاقد متعددة لمشروع | 16 سبتمبر 2022 | 29 يونيو 2020 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| اجعل دفاتر يومية ساعات المشروع للقراءة فقط إذا كانت حالة الموافقة الحالية لا تسمح بالتحرير | 16 سبتمبر 2022 | 6 اكتوبر 2021 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| تمكين بنود مبيعات المزامنة من بنود الشراء عند تحديث بنود الشراء وعند تشغيل معلمة إدارة تغيير أمر الشراء | 16 سبتمبر 2022 | 7 اكتوبر 2020 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| تمكين Project Operations على Dynamics 365 Customer Engagement | 16 سبتمبر 2022 | 29 يونيو 2020 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |
| ميزة التصحيح التلقائي لمعاملات المشروع | 16 سبتمبر 2022 | 13 يوليو 2020 | التشغيل بشكل افتراضي | إدارة المشروعات ومحاسبتها |

## <a name="features-that-become-mandatory-in-the-upcoming-release"></a>الميزات التي ستصبح إلزامية في الإصدار القادم

يسرد الجدول التالي الميزات الإلزامية من الإصدار 10.0.29 فصاعدًا.

| اسم الميزة | تاريخ التمكين | ‬‏‫تمت إضافة الميزة‬‏‫ | حالة الميزة | وحدة نمطية |
| --- | --- | --- | --- | --- |
| حساب القيمة الملتزم بدفعها في مصدر التمويل دون تقريب سعر الصرف | 16 سبتمبر 2022 | 14 يونيو 2020 | إلزامي | إدارة المشروعات ومحاسبتها |
| تمكين ترحيل تعديل المشروع بنفس حساب دفتر الأستاذ كمعاملة أصلية | 16 سبتمبر 2022 | 14 يونيو 2020 | إلزامي | إدارة المشروعات ومحاسبتها |
| تفاصيل المبلغ الملتزم بدفعه بعقد المشروع | 16 سبتمبر 2022 | 31 ‏‏أغسطس 2019 | إلزامي | إدارة المشروعات ومحاسبتها |
| تمكين الفرز حسب المورد خلال إنشاء مقترح فاتورة المشروع | 16 سبتمبر 2022 | 31 ‏‏أغسطس 2019 | إلزامي | إدارة المشروعات ومحاسبتها |