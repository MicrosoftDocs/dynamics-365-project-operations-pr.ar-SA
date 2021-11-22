---
title: مجموعات الموافقة في Project Service Automation
description: يوفر موضوع هذا الموضوع معلومات حول مجموعة الموافقات والطلبات والمجموعة الفرعية لهذه العمليات.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 9a7a9efbd8615f4923c6795a16c9cf98a40362b6
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323535"
---
# <a name="approval-sets-in-project-service-automation"></a>مجموعات الموافقة في Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

تعمل الموافقة على تعيين طلبات الموافقة على المجموعات في مجموعات فرعية أصغر من العمليات. يتيح هذا التجميع معالجة الموافقات بالترتيب حسب المشروع كما يتيح إعادة المحاولة والتسلسل. يحسن التجميع وثوقية معالجة الموافقات وتعقبها لعدد كبيرة من الموافقات.

وتشير مجموعات الموافقة إلى حالة المعالجة الإجمالية للسجلات المرتبطة بها. عند معالجة سجل قبول باستخدام مجموعة الموافقة، يتم نقل السجل من **مرسل** إلى **تمت الموافقة** ، وإنه غير مرتبط بمجموعة الموافقة. إذا فشل سجل عند إرساله للموافقة عليه، يظل السجل في حالة **مرسل** ويتم وضع علامة على مجموعة الموافقة كفاشلة. تقوم مجموعة الموافقة بتسجيل رسالة الخطأ الخاصة بالفشل.

## <a name="processing-approvals-and-approval-sets"></a>الموافقات قيد المعالجة ومجموعات الموافقة
تظهر الموافقات التي تم وضعها في قائمة انتظار للمعالجة في طريقة عرض **موافقات قيد الانتظار**. ويحاول النظام معالجة جميع الإدخالات عدة مرات بشكل غير متزامن، بما في ذلك إعادة محاولة الموافقة في حالة فشل المحاولات السابقة.

يسجل الحقل **مجموعة الموافقة مدى الحياة** عدد المحاولات المتبقية لمعالجة المجموعة قبل أن يتم وضع علامة عليها كفاشلة.

## <a name="failed-approvals-and-approval-sets"></a>الموافقات الفاشلة ومجموعات الموافقة
تسرد طريقة عرض **الموافقات الفاشلة** كافة الموافقات التي تتطلب تدخل المستخدم. افتح سجلات مجموعة الموافقة المقترنة لتحديد سبب الفشل.
يضيف تحديد **إعادة المحاولة** إلى فترة مدة بقاء مجموعة الموافقة، وتنقل الموافقة التي تتم إعادة تعيينها إلى حالة **المعالجة**، ومحاولة معالجة السجلات المتبقية.

## <a name="configure-approval-sets"></a>تكوين مجموعات الموافقة

###  <a name="enable-the-approval-sets-feature"></a>تمكين ميزة مجموعات الموافقة
قبل تمكين ميزة مجموعات الموافقة، تحقق من عدم وجود موافقات تتم معالجتها حاليًا.

- انتقل إلى الصفحة **معلمات المشروع** وحدد **التحكم في الميزات** > **تمكين الموافقات الحديثة**.

### <a name="turn-off-the-approval-sets-feature"></a>إيقاف تشغيل ميزة مجموعات الموافقة
قبل إيقاف تشغيل ميزة مجموعات الموافقة، تحقق من عدم وجود موافقات تتم معالجتها حاليًا.

- انتقل إلى الصفحة **معلمات المشروع** وحدد **التحكم في الميزات** > **تعطيل الموافقات الحديثة**.

### <a name="configuring-the-asynchronous-threshold"></a>تكوين الحد غير المتزامن 
عند إنشاء مجموعات الموافقة، يتم نقل المعالجة إلى الخلفية عندما يتجاوز العدد المحدد من السجلات للموافقة الحد المُشار إليه. استخدم الحقل **الحد غير المتزامن** لتكوين الوقت الذي يجب فيه تشغيل معالجة الموافقة بشكل متزامن أو غير متزامن.
القيم الصالحة هي:

  - صفر: ينبغي معالجة كافة الطلبات بشكل غير متزامن. 
  - الأرقام أكبر من صفر: تتم معالجة الموافقات بشكل غير متزامن فقط عندما يتجاوز عدد الموافقات الذي تم إرساله هذه القيمة.

[!INCLUDE[footer-include](../includes/footer-banner.md)]