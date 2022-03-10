---
title: الجديد في نوفمبر 2021 - Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬
description: يوفر هذا الموضوع معلومات حول تحديثات الجودة المتوفرة في إصدار نوفمبر 2021 من Project Operations للسيناريوهات المستندة إلى موارد/ منتجات غير مخزنة.
author: sigitac
ms.date: 11/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: fb9dad5b04ef2933ed8a8d8211f888f13df5ba40
ms.sourcegitcommit: 9d20e7738cce195d344f5925a115741a1ce3ca36
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/21/2021
ms.locfileid: "7942869"
---
# <a name="whats-new-november-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>الجديد في نوفمبر 2021 - Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬

*ينطبق على: Project Operations للسيناريوهات المستندة إلى الموارد/المنتجات غير المخزنة‬*

ينطبق هذا الموضوع على المكونات والإصدارات التالية من Microsoft Dynamics 365 Project Operations:

- Project Operations في إصدار بيئة Dataverse ‏4.26.0.145 أو 4.26.0.150 أو 4.26.0.155
- إدارة المشاريع والمحاسبة في بيئة Dynamics 365 Finance، إصدار 10.0.22

## <a name="features-included-in-this-release"></a>الميزات المضمنة في هذا الإصدار

تم تضمين الميزات التالية في هذا الإصدار:

- الآن تدعم واجهات برمجة التطبيقات لجدولة المشاريع القدرة على إنشاء وحذف مستودعات المشروع.

## <a name="project-operations-dual-write-maps-updates"></a>تحديثات مخططات ‏‫الكتابة المزدوجة في Project Operations

لا توجد تحديثات لخرائط الكتابة المزدوجة في Project Operations لهذا الإصدار. للحصول على القائمة والإصدارات الحالية لخرائط الكتابة المزدوجة في Project Operations، راجع [إصدارات خرائط الكتابة المزدوجة لـ Project Operations](/dynamics365/project-operations/environment/resource-dual-write-maps).

قم دائمًا بتشغيل أحدث إصدار من الخريطة في بيئتك، وتمكين جميع خرائط الجدول ذات الصلة أثناء تحديث حل Project Operations Dataverse وإصدار حل Finance. قد لا تعمل بعض الميزات والإمكانات بشكل صحيح إذا لم يتم تنشيط أحدث إصدار من الخريطة. يمكن عرض الإصدار النشط من المخطط في عمود **الإصدار** في الصفحة **الكتابة المزدوجة**. لتنشيط إصدار جديد من المخطط، حدد **إصدارات مخطط الجدول** ثم حدد الإصدار الأخير ثم احفظ الإصدار المحدد. إذا كنت قد قمت بتخصيص خريطة جداول جاهزة للاستخدام، فأعد تطبيق التغييرات. مزيد من المعلومات، راجع [إدارة دورة حياة التطبيقات](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

إذا واجهت مشكلة في بدء تشغيل الخريطة، فاتبع الإرشادات الموجودة في قسم [مشكلة أعمدة الجدول المفقودة على الخرائط](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) في دليل استكشاف الأخطاء وإصلاحها للكتابة المزدوجة.

## <a name="quality-updates"></a>التحديثات الإصلاحية

### <a name="project-operations-in-dataverse"></a>Project Operations في Dataverse

| منطقة الميزات | رقم المرجع | تحديث إصلاحي |
| --- | --- | --- |
| الفوترة والتسعير | 2240080 | يجب عدم تكرار حقل **شروط الدفع** في الفاتورة المبدئية. |
| الفوترة والتسعير | 2358236 | يجب أن يسمح تصحيح الفاتورة بتصحيحات ذات بنود سعر صفري. |
| إدارة الموارد | 2410072 | السماح بإعداد مورد مُعيّن لمهمة كمدير مشروع. |
| الفوترة والتسعير | 2430234 | إصلاح مشكلة حساب أداء التكلفة. |
| الوقت والمصروفات | 2436978 | السماح بإدخال الوقت بتنسيق hh:mm. |
| الفوترة والتسعير | 2448623 | السماح بتحديث قوائم الأسعار بعد ربطها بوحدة تنظيمية. |
| الوقت والمصروفات | 2460396 | السماح بحذف إدخال وقت عن طريق مسح الخلية. |
| الفوترة والتسعير | 2467386 | السماح بحذف مشروع له مهمة، حتى عندما تكون المهمة مقترنة بعرض أسعار فائز. |
| الوقت والمصروفات | 2461744 | تحتوي طريقة عرض **الموافقات الفاشلة الخاصة بي** فقط على موافقات المشروع في الحالة **مرسلة**. |
| الوقت والمصروفات | 2464082 | قم بإزالة الارتباط من موافقات المشروع إلى مجموعة الموافقات عند مطابقة حالة هدف. |
| الوقت والمصروفات | 2468108 | يجب ألا تحدد مهمة الجدولة حالة **معالجة** لمجموعة الموافقة. |
| الوقت والمصروفات | 2471503 | احذف مجموعات الموافقة التي عمرها سبعة أيام. |
| الفوترة والتسعير | 2480687 | يجب عدم إزالة مرجع سطر عرض الأسعار عند إنشاء مرحلة رئيسية لسطر عرض الأسعار. |

### <a name="project-management-and-accounting-in-finance"></a>إدارة المشاريع والمحاسبة في Finance

| منطقة الميزات | رقم المرجع | تحديث إصلاحي |
| --- | --- | --- |
| إدارة المشروعات ومحاسبتها | [584732](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584732) | لا يتم عرض مبالغ البائع المحجوزة في معاملات مصروفات المشروع في قائمة المعاملات. |
| إدارة المشروعات ومحاسبتها | [593068](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593068) | يتم تقسيم فاتورة البائع بين الشركات الشقيقة عند تشغيل تكامل فاتورة البائع. |
| إدارة المشروعات ومحاسبتها | [593382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593382) | لا تعمل شروط الدفع في فواتير المشروع كما هو متوقع. |
| إدارة المشروعات ومحاسبتها | [596263](https://fix.lcs.dynamics.com/Issue/Details/?bugId=596263) | عند تحرير استبقاء البائع، يكون لنشر الإيصال سطور إضافية غير صحيحة. |
| إدارة المشروعات ومحاسبتها | [598758](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598758) | يفشل دفتر يومية تكامل Project Operations عند نشره، لأن الأبعاد مفقودة لحساب لا يجري نشره. |
| إدارة المشروعات ومحاسبتها | [602650](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602650) | لا تكون علامة التبويب **المشروع** قابلة للتحرير في فاتورة بائع معلقة عندما يتم تعيين فئة المشتريات إلى العنصر. |
| إدارة المشروعات ومحاسبتها | [605121](https://fix.lcs.dynamics.com/Issue/Details/?bugId=605121) | يكون جزء التنقل مفقودًا في حالة عدم تسجيل الدخول إلى Project Operations Dataverse. |
| إدارة المشروعات ومحاسبتها | [602728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602728) | عند ترحيل إيرادات من فاتورة مشروع في حالة استبقاء مطبقة، لا تحدث مشكلات حيث لا تتم موازنة حركات الإيصال. |
| إدارة المشروعات ومحاسبتها | [603624](https://fix.lcs.dynamics.com/Issue/Details/?bugId=603624) | يؤدي إنشاء تقدير بعد نشر اقتراح فاتورة إلى منع استيراد سطور التصحيح. |
| إدارة المشروعات ومحاسبتها | [606083](https://fix.lcs.dynamics.com/Issue/Details/?bugId=606083) | ليس من الممكن تعديل سجل مراحل رئيسية مفوتر بالكامل. |
| السفر والمصروفات | [575305](https://fix.lcs.dynamics.com/Issue/Details/?bugId=575305) | يمكن رؤية جميع تقارير المصروفات عند البحث عن فئة في تطبيق الأجهزة المحمولة الخاص بالمصروفات. |
| السفر والمصروفات | [583101](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583101) | تم ترحيل مبالغ غير صحيحة في حركات ضريبة البائع والمبيعات من مصروف يتم إنشاؤه من حركة بطاقة مدينة. |
| السفر والمصروفات | [583760](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583760) | يحدث تحذير غير ذات صلة عند تحديث صفحات **تقرير المصروفات**. |
| السفر والمصروفات | [598656](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598656) | يُستخدم المعتمد المؤقت الخطأ عندما تقوم بحذف معتمد مؤقت ثم تعيد إرسال تقرير مصروفات عبر سير العمل. |
| السفر والمصروفات | [612742](https://fix.lcs.dynamics.com/Issue/Details/?bugId=612742) | يحدث خطأ في الترحيل يرتبط بإعداد عدد الأميال. |