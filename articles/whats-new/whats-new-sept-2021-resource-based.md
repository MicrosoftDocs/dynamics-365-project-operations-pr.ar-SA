---
title: ما الجديد سبتمبر 2021 - Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة
description: يوفر هذا الموضوع معلومات حول تحديثات الجودة المتوفرة في إصدار سبتمبر 2021 من Project Operations للسيناريوهات المستندة إلى الموارد/غير المخزنة.
author: sigitac
ms.date: 09/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 06f23630ef0205394f376e5bb93a29ae8a9eab15
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582878"
---
# <a name="whats-new-september-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>ما الجديد سبتمبر 2021 - Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة

*ينطبق على: Project Operations للسيناريوهات المستندة إلى الموارد/المنتجات غير المخزنة‬*

ينطبق هذه الموضوع على مكونات وإصدارات Dynamics 365 Project Operations التالية:

   -  Project Operations في إصدار بيئة Microsoft Dataverse  4.14.0.99.
   - إدارة المشاريع والمحاسبة في بيئة Dynamics 365 Finance، إصدار 10.0.20.

## <a name="project-operations-dual-write-maps-updates"></a>تحديثات مخططات ‏‫الكتابة المزدوجة في Project Operations

لا توجد تحديثات لخرائط الكتابة المزدوجة في Project Operations لهذا الإصدار. للحصول على القائمة والإصدارات الحالية لخرائط الكتابة المزدوجة في Project Operations، راجع [إصدارات خرائط الكتابة المزدوجة لـ Project Operations](../environment/resource-dual-write-maps.md).

قم بتشغيل أحدث إصدار من الخريطة في بيئتك وتمكين جميع خرائط الجدول ذات الصلة أثناء تحديث حل Project Operations Dataverse وإصدار حل Finance. قد لا تعمل بعض الميزات والإمكانات بشكل صحيح إذا لم يتم تنشيط أحدث إصدار من المخطط. يمكنك رؤية الإصدار النشط من الخريطة في صفحة **الكتابة المزدوجة** في العمود **الإصدار**. لتنشيط إصدار جديد من المخطط، حدد **إصدارات مخطط الجدول** ثم حدد الإصدار الأخير ثم احفظ الإصدار المحدد. إذا قمت بتخصيص مخطط جدول جاهز، فأعد تطبيق التغييرات. مزيد من المعلومات، راجع [إدارة دورة حياة التطبيقات](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

إذا واجهت مشكلة في بدء تشغيل الخريطة، فاتبع الإرشادات الموجودة في قسم [مشكلة أعمدة الجدول المفقودة على الخرائط](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) في دليل استكشاف الأخطاء وإصلاحها للكتابة المزدوجة.

## <a name="quality-updates"></a>التحديثات الإصلاحية

### <a name="project-operations-on-dataverse"></a>Project Operations على Dataverse

| **منطقة الميزات** | **رقم المرجع** | **تحديث إصلاحي** |
| --- | --- | --- |
| الوقت والمصروفات | 1811407 | تم تعديل دور أمان "موافق على المشروع" لموافقات إدخال المصروفات. |
| الوقت والمصروفات | 1811438 | تم تعديل الدور الأمني للموافق على المشروع لإلغاء الموافقة على إدخال الوقت. |
| الوقت والمصروفات | 2370126 | تم تحديث رمزي **مهمة المشروع** و **الدور** في كيان **إدخال الوقت**. |
| الوقت والمصروفات | 2379879 | تم تصحيح وظيفة **نسخ الأسبوع** في إدخال الوقت عند استخدام Dynamics 365 للهاتف. |
| الفوترة والتسعير | 2371906 | يجب ألا يكون المبلغ الإجمالي للفاتورة الأولية قابلاً للتعديل في Project Operations لعمليات النشر القائمة على الموارد. |
| الفوترة والتسعير | 2385802 | تم إصلاح الخطأ الذي يحدث مع الساعات الفعلية السلبية عند تحديث إجماليات المشروع. |
| الفوترة والتسعير | 2389675 | تحسين سلوك تأكيد الفاتورة الأولية. يجب أن يأخذ كيان الوظائف طويلة المدى في الاعتبار النشاط المطلوب لكتابة نتائج التأكيد للمحاسبة. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>إدارة المشاريع والمحاسبة في Dynamics 365 Finance

| منطقة الميزات | رقم المرجع | تحديث إصلاحي |
| --- | --- | --- |
| السفر والمصروفات | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | المبالغ في حركات ضريبة البائع والمبيعات التي تم ترحيلها من مصروف تم إنشاؤه من حركة بطاقة ائتمان غير صحيحة. |
| السفر والمصروفات | [4620366](https://fix.lcs.dynamics.com/Issue/Details?kb=4620366&amp;bugId=579485&amp;dbType=3&amp;qc=e864789bd95505ea624c537d585bf113c2de60b97c88439d44693dbd85aa8e92) | يتم إنشاء بنود التسوية الخاطئة عند إنشاء دفتر اليومية للدفع. |
| السفر والمصروفات | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | المبالغ في حركات ضريبة المبيعات التي تم ترحيلها من المصاريف التي تم إنشاؤها من معاملة بطاقة الائتمان غير صحيحة. |
| السفر والمصروفات | [4621765](https://fix.lcs.dynamics.com/Issue/Details?kb=4621765&amp;bugId=587306&amp;dbType=3&amp;qc=6fbfad0123d4e95eaf8d5a5a2f6c354577c991b7905c852ab02d1f94e728a876) | قد يستغرق حذف بند مصروفات وقتًا طويلاً. |
| محاسبة المشروع | [4623737](https://fix.lcs.dynamics.com/Issue/Details?kb=4623737&amp;bugId=598109&amp;dbType=3&amp;qc=4101fc5865201e21815299f2ff11ae46d5d5370510868df86c25ee09a8ca1a0c) | بعد تطبيق قاعدة المعارف 4619395، لا يتم دعم تغيير التسلسل الرقمي إلى **مستمر** وعندما تقوم بترحيل تقدير، يحدث الخطأ التالي، "لا يدعم النظام الإعداد "المستمر" للتسلسل الرقمي Proj_X." |
| محاسبة المشروع | [4623332](https://fix.lcs.dynamics.com/Issue/Details?kb=4623332&amp;bugId=586034&amp;dbType=3&amp;qc=2f64bb1977c4a9c9dd2ce9de7e72230b86eca14b6295c5bbfb614ea97ad81caf) | قد يفشل ترحيل فاتورة المورد مع ظهور رسالة الخطأ التالية، "لا تتوازن الحركات على الإيصال وفقًا لـ 17/5/2021. (عملة المحاسبة: 0.00 - عملة إعداد التقارير: 0.01)." |
