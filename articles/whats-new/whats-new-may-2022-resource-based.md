---
title: الجديد في مايو 2022 - Project Operations للسيناريوهات المستندة إلى الموارد/ المنتجات غير المخزنة
description: يوفر هذا المقال معلومات حول التحديثات الإصلاحية المتوفرة في إصدار مايو 2022 من Microsoft Dynamics 365 Project Operations للسيناريوهات المستندة إلى موارد/غير مخزنة.
author: sigitac
ms.date: 05/02/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: beb75fc4b721d52cddbdaf2d20194218cefced5e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921378"
---
# <a name="whats-new-may-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>الجديد في مايو 2022 - Project Operations للسيناريوهات المستندة إلى الموارد/ المنتجات غير المخزنة

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

ينطبق هذا المقال على المكونات والإصدارات التالية من Microsoft Dynamics 365 Project Operations:

- Project Operations في بيئة Dataverse الإصدار 4.42.0.70
- إدارة المشاريع والمحاسبة في بيئة Dynamics 365 Finance، الإصدار 10.0.26

## <a name="project-operations-dual-write-maps-updates"></a>تحديثات مخططات ‏‫الكتابة المزدوجة في Project Operations

لا توجد تحديثات لخرائط الكتابة المزدوجة في Project Operations لهذا الإصدار. للحصول على القائمة والإصدارات الحالية لخرائط الكتابة المزدوجة في Project Operations، راجع [إصدارات خرائط الكتابة المزدوجة لـ Project Operations](../environment/resource-dual-write-maps.md).

قم دائمًا بتشغيل أحدث إصدار من الخريطة في بيئتك، وتمكين جميع خرائط الجدول ذات الصلة أثناء تحديث حل Project Operations Dataverse وإصدار حل Finance. قد لا تعمل بعض الميزات والإمكانات بشكل صحيح إذا لم يتم تنشيط أحدث إصدار من الخريطة. يمكن عرض الإصدار النشط من المخطط في عمود **الإصدار** في الصفحة **الكتابة المزدوجة**. لتنشيط إصدار جديد من المخطط، حدد **إصدارات مخطط الجدول** ثم حدد الإصدار الأخير ثم احفظ الإصدار المحدد. إذا كنت قد قمت بتخصيص خريطة جداول جاهزة للاستخدام، فأعد تطبيق التغييرات. مزيد من المعلومات، راجع [إدارة دورة حياة التطبيقات](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

إذا واجهت مشكلة في بدء تشغيل الخريطة، فاتبع الإرشادات الموجودة في قسم [مشكلة أعمدة الجدول المفقودة على الخرائط](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) في دليل استكشاف الأخطاء وإصلاحها للكتابة المزدوجة.

## <a name="quality-updates"></a>التحديثات الإصلاحية
### <a name="project-operations-on-dataverse"></a>Project Operations على Dataverse

| منطقة الميزات | رقم المرجع | تحديث إصلاحي |
| --- | --- | --- |
| إدارة الموارد | 2634019 | تم تحسين رسائل الخطأ لعمليات التحقق من صحة الأعمال عند إضافة أعضاء الفريق العامين كموارد. |
| دليل تخطيط المشاريع وتعقبها | 2648515 | تحديثات مقيدة لـ **ownerid** و **الولاية** و **الحالة** في كيانات الجدولة. |
| الفوترة والتسعير | 2653167 | يجب أن يتبع الفاصل العشري لخطوط شبكة **التقديرات** إعدادات التنسيق في **الخيارات الشخصية**. |
| الفوترة والتسعير| 2662251 | توجد القيم في الحقول **الوحدة الصحيحة** و **مجموعة الوحدة** افتراضيًا عند إنشاء السجلات في تقديرات المواد. |
| الفوترة والتسعير| 2571408 | يتم ختم القيم الفعلية للمبيعات غير المفوترة بمعرف الفاتورة المبدئي عند إنشاء مسودة فاتورة. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>إدارة المشاريع والمحاسبة في Dynamics 365 Finance

للحصول على معلومات حول إصلاحات الأخطاء المضمنة في هذا التحديث، سجل دخولك إلى Microsoft Dynamics Lifecycle Services (LCS)، واستعرض [مقال KB (قاعدة المعارف)](https://fix.lcs.dynamics.com/Issue/Details?bugId=662864).
