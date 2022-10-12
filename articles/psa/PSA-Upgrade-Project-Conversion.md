---
title: تغييرات الميزات لـ Project Service Automation إلى Project Operations
description: يوفر هذا المقال نظرة عامة على تغييرات الميزات لـ Microsoft Dynamics 365 Project Service Automation إلى Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 9869b3ad0fb6429484a26f367e06a0996f110ed8
ms.sourcegitcommit: a2d720ac6d7ddb20a0967fe87992a376b2478208
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/04/2022
ms.locfileid: "9621198"
---
# <a name="feature-changes-for-project-service-automation-to-project-operations"></a>تغييرات الميزات لـ Project Service Automation إلى Project Operations

بعد ترقية مشروع بنجاح من Microsoft Dynamics 365 Project Service Automation 3.X إلى Dynamics 365 Project Operations Lite، لن يكون تحرير مهام المشروع في هيكل تنظيم العمل (WBS) في شبكة المهام ممكنًا. سيكون بمقدور العملاء مراجعة هياكل تنظيم العمل (WBS) فشبكة التعقب حيث تمت إضافة حقول جديدة لتقديم كافة التفاصيل المتعلقة بالمهمة. بالنسبة إلى المشاريع حيث عمليات التحرير في هيكل تنظيم العمل (WBS) مطلوبة، يمكنك تحويل المشاريع المؤهلة بطريقة انتقائية إلى تجربة الجدولة الجديدة في Project for the Web.

## <a name="project-conversion-process"></a>عملية تحويل المشروع

لتحويل مشروع، اتبع هذه الخطوات.

1. افتح الصفحة الرئيسية للمشروع، وحدد **تحويل** في جزء الإجراءات.
1. في مربع رسالة التأكيد، حدد **موافق** لبدء تحويل المشروع. تحدث الإجراءات التالية:

    1. شريط رسائل يظهر على الصفحة الرئيسية للمشروع على "يجري تحويل جدول المشروع. لا يمكنك أدخال تغييرات على المشروع حتى يكتمل التحويل."
    1. يُعاد توجيهك إلى قائمة المشاريع.

    بعد اكتمال تحويل المشروع، تحدث الإجراءات التالية:

    1. يتلقى مدير المشروع المعين إعلامًا على الجانب الأيسر من التطبيق.
    1. يُزال شريط الرسائل الذي يشير إلى أن التحويل في التقدم.
    1. تعرض علامة‏‎ تبويب **الجدول** تجربة الجدولة الجديدة مع Project for the Web. بإمكان أي مستخدم لديه التراخيص وأدوار الأمان المناسبة تحرير هيكل تنظيم العمل (WBS).
    1. يتم تحديث حقل **محرك الجدولة** إلى **Project for the Web**.
    1. يُزال الزر **تحويل** من جزء الإجراءات.

> [!IMPORTANT]
> التحويل المجمع للمشروعات غير مسموح به. سيتم تقييد أي محاولة لتحديث حجم كبير من المشاريع في نفس الوقت. يساعد هذا التقييد على ضمان أداء عالٍ لجميع العملاء.

## <a name="manual-tasks-vs-automatic-tasks"></a>المهام اليدوية في مقابل المهام التلقائية

عند ترقية بيئة من Project Service Automation إلى Project Operations، تُعتبر جميع المهام في هيكل تنظيم العمل (WBS) مجدولة بشكل تلقائي. لا يتوفر مفهوم المهام المجدولة يدويًا في Project for the Web. ومع ذلك، يمكنك تعريف سلوك الجدولة المفضل لمشاريعك باستخدام إعداد [وضع الجدولة](/project-management/scheduling-modes.md) عند إنشاء مشاريع جديدة.

## <a name="restricted-operations-for-pre-conversion-projects"></a>العمليات المقيدة للمشاريع ما قبل التحويل

يوضح هذا القسم الاختلافات الفنية التي يمكن توقعها عندما لا يتم تحويل المشاريع.

### <a name="copy-project"></a>نسخ المشروع

عملية **النسخ** مدعومة فقط على المشاريع المحوّلة. لا يمكن نسخ المشاريع التي تمت ترقيتها قبل التحويل.

### <a name="move-project"></a>نقل المشروع

لن يؤدي تغيير تاريخ بدء مشروع إلى نقل بدء المهام بطريقة متناسبة ما لم يتم تحويل المشروع.

## <a name="frequently-asked-questions"></a>الأسئلة المتداولة

### <a name="what-are-the-differences-between-converted-projects-and-new-projects-that-are-created-after-the-upgrade-has-been-completed"></a>ما هي الاختلافات بين المشاريع المحوّلة والمشاريع الجديدة التي نشأت بعد اكتمال الترقية؟

بالنسبة إلى المشاريع التي يتم تحويلها بعد ترقية البيئة، سيتم تعيين علامة ترشد الجدولة لاحترم تقويم المشروع فقط. يتطابق هذا السلوك مع السلوك في Project Service Automation. ومع ذلك، لن يتم تعيين العلامة للمشاريع الجديدة التي يتم إنشاؤها بعد الترقية. وبالتالي، سيراعي الجدول ساعات عمل الموارد عندما يتم تعيينها إلى مهمة.

### <a name="what-should-i-do-if-my-project-fails-to-be-converted"></a>ما الذي يجب عليّ فعله إذا فشل تحويل مشروعي؟

إذا فشل تحويل مشروعك، فإن الخطوة الأولى هي مراجعة سجلات الأخطاء لتحديد أي مشاكل عامة تتعلق بهيكل تنظيم العمل (WBS) في حال عدم إشارة السجلات إلى خطأ معين يمكن اتخاذ إجراء بشأنه، فاتصل بدعم العملاء لإجراء المزيد من المراجعات على حالتك.

### <a name="how-are-business-closures-handled-in-project-for-the-web"></a>كيف يتم التعامل مع حالات إغلاق الأعمال في Project for the Web؟

لا يراعي Project for the Web حالات إغلاق الأعمال التي تحددها الشركة على مستوى المؤسسة. ومع ذلك، فهو سيحترم أنواع أخرى من أيام الإجازات المحددة في قالب ساعات عمل محدد.

### <a name="what-are-the-limitations-of-project-for-the-web"></a>ما هي قيود Project for the Web؟

راجع [إنشاء هيكل تنظيم العمل: قيود المشروع](/project-management/create-wbs#project-limitations.md).

### <a name="can-i-expect-changes-to-my-cost-and-sales-estimates"></a>هل يمكنني توقع تغييرات على تقديرات التكلفة والمبيعات؟

في الحالات النادرة التي يُعاد فيها إعادة حساب خطوط تعيين الموارد، أو حيث تقع على حدود تاريخ مختلف عن المشروع المصدر، قد ترى اختلافات في تقديرات المبيعات والتكلفة. وكجزء من عملية الترقية، من المتوقع أن يختار العملاء عينة تمثيلية لمجموعة من المشاريع، حتى يتمكنوا من فهم أية تغييرات محتملة في الجدولة.
