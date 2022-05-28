---
title: ترقية الاعتبارات المتعلقة بالموافقات الحديثة
description: يغطي الموضوع النقاط التي يجب على المسؤولين أخذها في الاعتبار عند قيامهم بتمكين وظيفة الموافقات الحديثة.
author: stsporen
ms.date: 01/31/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: a3757f057a801318feccde9be3e49c7b40fa8fcb
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8578370"
---
# <a name="upgrade-considerations-for-modern-approvals"></a>ترقية الاعتبارات المتعلقة بالموافقات الحديثة 

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

كجزء من إصدار الموجة 1 في أبريل 2022، سيتم تمكين وظيفة الموافقات الحديثة افتراضيًا. تعمل هذه الوظيفة على تحسين موثوقية منطق الموافقة وتضمن أنه يمكنك تحديد السبب في حالة فشل منطق الموافقة.

كجزء من هذا التغيير، يتم تحديث تغييرات الحالة الخاصة بالموافقات على المشروع. ينتقل الوضع الآن مباشرة من **تم الإرسال** إلى **تمت الموافقة**. **معلّقة** لم تعد إحدى حالات الموافقات. لتحديد ما إذا كانت الموافقة معلّقة، تحقق من أن الموافقة جزء من مجموعة الموافقة، وقم بمراجعة حالة مجموعة الموافقة المرفقة.

## <a name="before-you-upgrade"></a>قبل الترقية

قبل الترقية إلى الموافقات الحديثة، تأكد من عدم وجود موافقات معلّقة. لا تستخدم الموافقات الحديثة الحالة **معلّقة**. لذلك، لن تتم معالجة أية موافقات لا تزال عليها علامة **معلّقة** بعد الترقية.

## <a name="after-you-upgrade"></a>بعد الترقية

بعد الترقية إلى الموافقات الحديثة، يجب على المسؤول التحقق من تمكين تدفق السحابة الذي يعالج الموافقات.

1. تسجيل الدخول إلى [flow.microsoft.com](https://flow.microsoft.com).
2. في أعلى يمين الصفحة، قم بتبديل البيئة لديك إلى البيئة التي قمت بتحديثها.
3. حدد **الحلول** لسرد الحلول المثبتة في البيئة.
4. في قائمة الحلول، حدد **Project Operations** أو **Project Service**.
5. قم بتغيير عامل التصفية من **الكل** إلى **تدفقات السحابة**.
6. تحقق من تعيين خيار **Project Service – جدولة مجموعات الموافقة على المشروع بشكل متكرر** إلى **تشغيل**. إذا لم يكن كذلك، فحدد سير العمل، ثم قم بتحديد **تشغيل**.
7. تحقق من أن المعالجة تتم كل خمس دقائق من خلال مراجعة قائمة **وظائف النظام** في منطقة **الإعدادات**.

## <a name="short-term-rollback"></a>العودة للحالة السابقة على المدى القصير

إذا لم تتمكن من استيعاب التغييرات، أو إذا واجهت مشكلة خطيرة مع هذه الميزة، فيمكنك الرجوع مؤقتًا إلى تدفق الموافقة الأصلية عن طريق تنفيذ الخطوات التالية:
1. قم بتسجيل الدخول إلى بيئتك وتحقق من عدم وجود موافقات معلقة.
2. انتقل إلى **الإعدادات** > **معلمات المشروع**.
3. حدد **التحكم في الميزات** ثم حدد **الموافقات الحديثة** لإيقاف تشغيل الميزة.

## <a name="removing-the-feature-flag"></a>إزالة علامة الميزة

في تحديث الموجة 2 من إصدار أكتوبر 2022، ستتم إزالة القدرة على إيقاف تشغيل هذه الميزة.

[!INCLUDE[footer-include](../includes/footer-banner.md)]