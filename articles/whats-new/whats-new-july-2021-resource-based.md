---
title: الجديد في يوليو 2021 - Project Operations للسيناريوهات المستندة إلى المنتجات غير المخزنة/الإنتاج
description: يوفر هذا الموضوع معلومات حول تحديثات الجودة المتوفرة في إصدار يوليو 2021 من Project Operations للسيناريوهات المستندة إلى المنتجات غير المخزنة/الموارد.
author: sigitac
ms.date: 07/07/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5dbf9c7158ce7d9e568e270791e7e7aaf8ce731d
ms.sourcegitcommit: 3abf1e67938d91bd826b025ae3187cd313f556b9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/07/2021
ms.locfileid: "6433502"
---
# <a name="whats-new-july-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>الجديد في يوليو 2021 - Project Operations للسيناريوهات المستندة إلى المنتجات غير المخزنة/الإنتاج

*ينطبق على: Project Operations للسيناريوهات المستندة إلى الموارد/المنتجات غير المخزنة‬*

ينطبق هذه الموضوع على مكونات وإصدارات Dynamics 365 Project Operations التالية:

   -  Project Operations في إصدار بيئة Microsoft Dataverse  4.12.0.148.
   - إدارة المشاريع والمحاسبة في إصدار بيئة Dynamics 365 Finance  10.0.20.

## <a name="features-included-in-this-release"></a>الميزات المضمنة في هذا الإصدار

تم تضمين الميزات التالية في هذا الإصدار:

- قدرة المسؤولين على عرض سجلات PSS وسجلات مجموعة العمليات من قائمة الإعدادات. يتم تخزين السجلات لمدة 90 يومًا.

## <a name="project-operations-dual-write-maps-updates"></a>تحديثات مخططات ‏‫الكتابة المزدوجة في Project Operations

لا توجد تحديثات لخرائط الكتابة المزدوجة في Project Operations لهذا الإصدار.

للحصول على القائمة والإصدارات الحالية لخرائط الكتابة المزدوجة في Project Operations، راجع [إصدارات خرائط الكتابة المزدوجة لـ Project Operations](../environment/resource-dual-write-maps.md).

قم بتشغيل أحدث إصدار من الخريطة في بيئتك وتمكين جميع خرائط الجدول ذات الصلة أثناء تحديث حل Project Operations Dataverse وإصدار حل Finance. قد لا تعمل بعض الميزات والإمكانات بشكل صحيح إذا لم يتم تنشيط أحدث إصدار من المخطط. يمكنك رؤية الإصدار النشط من الخريطة في صفحة **الكتابة المزدوجة** في العمود **الإصدار**. تنشيط إصدار جديد من الخريطة عن طريق تحديد **إصدارات خريطة الجدول**، وتحديد أحدث إصدار، ثم حفظ الإصدار المحدد. إذا قمت بتخصيص مخطط جدول جاهز، فأعد تطبيق التغييرات. مزيد من المعلومات، راجع [إدارة دورة حياة التطبيقات](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

إذا واجهتك مشكلة عند بدء تشغيل الخريطة، اتبع التعليمات الموجودة في قسم [مشكلة أعمدة الجدول المفقودة على الخرائط](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) في دليل استكشاف الأخطاء وإصلاحها للكتابة المزدوجة.

## <a name="quality-updates"></a>التحديثات الإصلاحية

### <a name="project-operations-on-dataverse"></a>Project Operations على Dataverse

| **منطقة الميزات**              | **رقم المرجع** | **تحديث إصلاحي**                                                                                                                                                                                             |
|-------------------------------|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| الفوترة والتسعير           | 2224046              | يمكن تحرير حقل **فئة الحركة** في علامة التبويب **تفاصيل بند عرض الأسعار**، ولكن يتم إغلاقه إذا كنت تعمل من صفحة **تفاصيل بند عرض الأسعار**.                                                                     |
| الفوترة والتسعير           | 2224400              | يفشل إجراء **إغلاق عرض الأسعار كمكسب** عندما لا يكون لعرض الأسعار مراحل رئيسية في التاريخ.                                                                                                                                    |
| الفوترة والتسعير           | 2234089              | عندما تقوم بإدخال وصف منتج يدويًا، يتم مسحه بعد إدخال كمية لتقدير المادة.                                                                                                                         |
| الفوترة والتسعير           | 2234100              | لا تتضمن شبكة **إعداد فوترة المهمة** عمود **المواد** والقيمة الخاصة به في علامة التبويب **فوترة المهمة** الخاصة بالمشروع.                                                                                                       |
| الفوترة والتسعير           | 2277409              | لا يكون معرف المنتج متوفرًا في تفاصيل بند العقد لبند نوع المادة.                                                                                                                                        |
| الفوترة والتسعير           | 2281728              | يؤدي إنشاء بند العقد دون داع إلى إعادة تقييم القيم الفعلية مما يتسبب في زيادة كبيرة في حجم البيانات، مما يؤثر على الأداء.                                                                                |
| الفوترة والتسعير           | 2298668              | لا تتم إزالة سطور دفتر اليومية المرتبطة بالمصروفات التي تم استرجاعها وحذفها.                                                                                                                                     |
| الفوترة والتسعير           | 2300192              | عندما يقوم عدة مستخدمين بتحرير فاتورة، فمن الممكن إنشاء تفاصيل بند فاتورة جديد في فاتورة مؤكدة.                                                                                   |
| الفوترة والتسعير           | 2301569              | لا يمكن تصحيح الفواتير إذا تم تطبيق الاحتفاظ بالمبلغ 0\$.                                                                                                                                        |
| الفوترة والتسعير           | 2307965              | تظهر رسالة خطأ إذا تم إنشاء سعر فئة بقيم مفقودة.                                                                                                                           |
| الفوترة والتسعير           | 2326870              | يحدث خطأ في **Microsoft.Dynamics.ProjectService.Plugins.PostInvoiceLineDelete** إذا كان **producttypecode** فارغًا.                                                                            |
| الفوترة والتسعير           | 2332732              | تحدث رسالة خطأ إذا تم إنشاء حدث شروط التعاقد بدون سطر الأمر.                                                                                                                |
| تخطيط المشاريع وتعقبها | 2181094              | تدعم واجهة برمجة تطبيقات جدولة المشروع الآن سجلات PSS وسجلات مجموعة العمليات التي يتم تخزينها لمدة 90 يومًا.                                                                                                                  |
| تخطيط المشاريع وتعقبها | 2254201              | يتم تحديث تسمية **وضع الجدولة** بالتفاصيل التي تصف المنطق الافتراضي.                                                                                                                                      |
| تخطيط المشاريع وتعقبها | 2300252              | يتم تحديث ذاكرة التخزين المؤقت للاستجابة **openProject** وتتضمن مالك الرمز المميز في مفتاح ذاكرة التخزين المؤقت، و **عنوان Url الأساسي**، و **عنوان URL للمقطع** بحيث يمكن دائمًا إعادة إنشاء **عنوان URL للطلب** إذا تغير **عنوان Url الأساسي**. |
| تخطيط المشاريع وتعقبها | 2301312              | تم حذف **msdyn_membershipstatus** من طريقة العرض **عضو فريق المشروع**.                                                                                                                                        |
| تخطيط المشاريع وتعقبها | 2302759              | يتم جلب المنتجات بدون داعٍ في علامات التبويب **‏‫تعيينات الموارد‬** و **التقديرات** و **تقديرات المصروفات**.                                                                                                        |
| تخطيط المشاريع وتعقبها | 2308050              | فشل **CopyProject** مع الخطأ، "فشل الحصول على رمز للتحدث إلى خدمة عن بعد".                                                                                                                           |
| تخطيط المشاريع وتعقبها | 2322650              | تم تحديث طريقة عرض **قائمة مهام المشروع** لعرض تاريخ المهمة بشكل افتراضي.                                                                                                            |
| تخطيط المشاريع وتعقبها | 2327266              | ينشئ **CopyProject** الخطأ، "المفتاح غير موجود في القاموس" عند نسخ التقديرات.                                                                                                      |
| تخطيط المشاريع وتعقبها | 2328123              | يُنشئ **CopyProject** الخطأ، "فشل في الحصول على رمز للتحدث إلى خدمة عن بعد".                                                                                                                          |
| تخطيط المشاريع وتعقبها | 2336258              | ينسخ **CopyProject** بشكل غير صحيح أسماء مواقع الموارد.                                                                                                                                                 |
| الفوترة والتسعير           | 2224476              | لا يتطابق حقل **المورد القابل للحجز** بشكل صحيح مع المستخدم الذي قام بتسجيل الدخول في صفحة **استخدام المواد**.                                                                                                            |
| إدارة الموارد           | 2277249              | يحدث خطأ عند تحديث متطلب مورد غير قائم على المشروع.                                                                                                            |
| إدارة الموارد           | 2323869              | لا يتعرف استخدام المورد بشكل صحيح على الموارد التي تمت تصفيتها.                                                                                                                                             |
| الوقت والمصروفات              | 2176538              | يتم تطبيق عوامل التصفية غير الصحيحة على عنصر التحكم **‏‫إدخال الوقت**.                                                                                                                                                   |
| الوقت والمصروفات              | 2177462              | لا يؤدي حذف إدخال الوقت في الشبكة إلى تحديث حالة الزر **إرسال** و **‏‫استدعاء** و **حذف** و **تحرير الإدخال** كما هو متوقع.                                                                                        |
| الوقت والمصروفات              | 2299985              | لا يحتفظ **TimeEntriesImportFromResourceAssignment** بوقت البدء/الانتهاء من مخططات التعيينات‬.                                                                                                  |
| الوقت والمصروفات              | 2318426              | بعد إرسال إدخال الوقت، لا يزال من الممكن تحرير الحقول المقفلة.                                                                                                                                   |
| الوقت والمصروفات              | 2323749              | يحدث خطأ عند إنشاء مصاريف من علامة التبويب **ذات الصلة** لمورد قابل للحجز.                                                                                                      |
| الوقت والمصروفات              | 2327678              | عند إنشاء إدخال وقت من علامة التبويب **ذات الصلة** لمورد قابل للحجز، لا يتم تمرير المورد الأصلي إلى عنصر التحكم في إدخال الوقت.                                                                            |
| عام                        | 2296857              | تعقب التقدم للوظائف التي تعمل لمدة طويلة.                                                                                                                                                                        |
| عام                        | 2253682              | لا ينبغي تثبيت حل الكتابة المزدوجة لـ Project Operations عندما يتم تثبيت حل الكتابة المزدوجة الأساسي‬ في بيئة بدون حل تزامن الكتابة المزدوجة.                                                |
| عام                        | 2316420              | يفشل التوفير الأساسي لـ Project service في حالة تغيير وحدة عمل مستخدم التطبيق.                                                                                                                     |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>إدارة المشاريع والمحاسبة في Dynamics 365 Finance

| منطقة الميزات                      | رقم المرجع | تحديث إصلاحي                                                                                                                                                                                                                                                                                                                |
|-----------------------------------|------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| إدارة المشروعات ومحاسبتها | 4620267          | لا يمكن تخصيص النماذج لإضافة حقل **الغرض** إلى الصفحات **‬‏‫الحركة المُرحلة في المشروع‬‏‫**، و **إنشاء اقتراح فاتورة**‬‏‫، و **‬‏اقتراح فاتورة‬‏**.                                                                                                                                                                                         |
| إدارة المشروعات ومحاسبتها | 4613449          | عند تحديد معرّف عقد مشروع في Finance، تفتح بيئة Project Operations المتكاملة الصفحة لإنشاء سجل جديد، بدلاً من الصفحة الخاصة بعقود المشروع التي تم إنشاؤها بالفعل.                                                                                                                                           |
| إدارة المشروعات ومحاسبتها | 4614445          | في نشر سيناريو Project Operations المتكامل، لا يمكنك تحرير الحقل **مجموعة ضريبة مبيعات الصنف** في مقترح الفاتورة الذي تم استيراده من المرحلة. يجب أن تكون مجموعة ضريبة مبيعات الصنف قابلة للتحرير لمقترح فاتورة مفتوح لجميع أنواع الحركات بما في ذلك الحساب والساعات والمصروفات والرسوم والأصناف. |
| إدارة المشروعات ومحاسبتها |                  | لا يمكن ترحيل مقترح فاتورة ناتج عن تصحيح حركة زمنية سالبة.                                                                                                                                                                                                                                              |
| إدارة المشروعات ومحاسبتها |                  | تتكرر بنود مقترح الفاتورة بسبب عمليات دورية متعددة **استيراد من مرحلة** تعمل في نفس الوقت.                                                                                                                                                                                                                |
