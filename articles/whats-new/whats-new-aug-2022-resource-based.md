---
title: الجديد في أغسطس 2022 - Project Operations للسيناريوهات المستندة إلى المنتجات غير المخزنة/الموارد
description: يوفر هذا المقال معلومات حول التحديثات الإصلاحية المتوفرة في إصدار أغسطس 2022 من Microsoft Dynamics 365 Project Operations للسيناريوهات المستندة إلى موارد/غير مخزنة.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 4042dca72a33f48e04e51af2a3cfd2da83146afd
ms.sourcegitcommit: 7ed8e77a92917f2d242988ca02bd7de9571cce5e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/02/2022
ms.locfileid: "9403840"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>الجديد في أغسطس 2022 - Project Operations للسيناريوهات المستندة إلى المنتجات غير المخزنة/الموارد

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

ينطبق هذا المقال على المكونات والإصدارات التالية من Microsoft Dynamics 365 Project Operations:

- Project Operations في بيئة Dataverse الإصدار 4.45.0.53
- إدارة المشاريع والمحاسبة في بيئة Dynamics 365 Finance، الإصدار 10.0.28

## <a name="project-operations-dual-write-maps-updates"></a>تحديثات مخططات ‏‫الكتابة المزدوجة في Project Operations

لا توجد تحديثات لخرائط الكتابة المزدوجة في Project Operations لهذا الإصدار. للحصول على القائمة والإصدارات الحالية لخرائط الكتابة المزدوجة في Project Operations، راجع [إصدارات خرائط الكتابة المزدوجة لـ Project Operations](../environment/resource-dual-write-maps.md).

قم دائمًا بتشغيل أحدث إصدار من الخريطة في بيئتك، وتمكين جميع خرائط الجدول ذات الصلة أثناء تحديث حل Project Operations Dataverse وإصدار حل Finance. قد لا تعمل بعض الميزات والإمكانات بشكل صحيح إذا لم يتم تنشيط أحدث إصدار من الخريطة. يمكن عرض الإصدار النشط من المخطط في عمود **الإصدار** في الصفحة **الكتابة المزدوجة**. لتنشيط إصدار جديد من المخطط، حدد **إصدارات مخطط الجدول** ثم حدد الإصدار الأخير ثم احفظ الإصدار المحدد. إذا كنت قد قمت بتخصيص خريطة جداول جاهزة للاستخدام، فأعد تطبيق التغييرات. مزيد من المعلومات، راجع [إدارة دورة حياة التطبيقات](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

إذا واجهت مشكلة في بدء تشغيل الخريطة، فاتبع الإرشادات الموجودة في قسم [مشكلة أعمدة الجدول المفقودة على الخرائط](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) في دليل استكشاف الأخطاء وإصلاحها للكتابة المزدوجة.

## <a name="quality-updates"></a>التحديثات الإصلاحية

### <a name="project-operations-on-dataverse"></a>Project Operations على Dataverse

| منطقة الميزات | رقم المرجع | تحديث إصلاحي |
| --- | --- | --- |
| إدارة الفرص | 2762089  | خطأ في المعالجة أثناء إغلاق العقد على أنه مفقود إذا تم تعطيل الحفظ التلقائي في المؤسسة.|
|تخطيط المشاريع وتعقبها | 2767841  | يعمل قياس تتبع الاستخدام على تحديث سيناريوهات إنشاء أو تحديث كيان المشروع.|
|الفوترة والتسعير | 2771072  | معالجة استثناء مرجعي فارغ عند التعامل أثناء عرض أسعار الفوز.|
|الفوترة والتسعير | 2844181  |فشل في الحصول على معرف الارتباط وحظر إنشاء فاتورة.|
|الفوترة والتسعير | 2852836  | القيم الفعلية للشركات الشقيقة مفقودة للمصروفات بين الشركات التي تم إنشاؤها وموافقتها في CE.|


### <a name="project-management-and-accounting-in-finance"></a>إدارة المشاريع والمحاسبة في Finance

للحصول على معلومات حول إصلاحات الأخطاء المضمنة في هذا التحديث، سجل دخولك إلى Microsoft Dynamics Lifecycle Services (LCS)، واستعرض [مقال KB (قاعدة المعارف)](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).
