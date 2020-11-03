---
title: بنود الفرصة المستندة إلى المشروع (احترافي)
description: يقدم هذا الموضوع معلومات حول بنود الفرصة المستندة إلى مشروع. (احترافي)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a688b9bed5a38e7b5947cbcee1e3cb8ab211e98
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070569"
---
# <a name="project-based-opportunity-lines-pro"></a>بنود الفرصة المستندة إلى المشروع (احترافي)

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_

تتوفر بنود الفرص المستندة إلى المشروع في الفرص المستندة إلى المشروع فقط. تتميز سجلات الفرصة المستندة إلى مشروع بأن حقل **النوع** بها تم تعيينه إلى **يستند إلى العمل**.

بنود الفرصة المستندة إلى مشروع هي عناصر البنود التي سيتم تسليمها إلى العميل باستخدام مشروع. ومع ذلك، لا يمكن ربط مشروع ببند فرصة يستند إلى مشروع. يمكن أن ترتبط المشاريع بعناصر البنود من مرحلة **عرض الأسعار** وما يليها لأن الفرصة عادة ما تكون في مرحلة مبكرة في دورة حياه الصفقة. يتم اتخاذ قرار تحديد عدد المشروعات التي سيتم استخدامها لتسليم العمل للعميل لاحقًا في مرحلة المبيعات. يمكنك استخدام مرحلة الفرصة لتحديد مكونات التسليم المنفصلة الخاصة بالعميل. يمكن تأجيل القرارات المتعلقة بالعدد الفعلي للمشاريع المستخدمة لتسليم هذه المكونات إلى أن يتم التعرف على مزيد من المعلومات حول العمل نفسه.

فيما يلي الحقول الموجودة في بند الفرصة المستندة إلى مشروع:

| **الحقل** | **الموقع** | **الصلة والغرض والإرشاد** | **تأثير لاحق** |
| --- | --- | --- | --- |
| نوع المنتج | علامة التبويب عام (مخفية) | يمكنك تحديد واحد من الخيارات التالية:</br>- خدمة تستند إلى مشروع (تتوفر فقط عند تثبيت Dynamics 365 Project Operations)</br>- المنتج (تتوفر فقط عند تثبيت Dynamics 365 Sales) | يتم تعيين قيمة هذا الحقل إلى **خدمة تستند إلى مشروع** عند إنشاء بند فرصة تستند إلى مشروع من شبكة البنود المستندة إلى المشروع في الفرصة. <br> إذا قمت بتغيير هذه القيمة أو تجاوزتها، فلن يتم تمكين وظيفة المشروع على عناصر البنود المستندة إلى مشروع الخاصة بك. |
| الفرصة | علامة التبويب عام | هذا الحقل للقراءة فقط ويشير إلى سجل الفرصة الأصل الذي ينتمي إليه عنصر البند هذا. | لا يوجد تأثير لاحق من هذا الحقل. |
| اسم | علامة التبويب عام | يمكن استخدام حقل النص القابل للتحرير هذا في إعطاء تعريف قصير لعنصر البند. | يتم ترحيل هذه القيمة إلى بند عرض الأسعار عند إنشاء عرض أسعار من هذه الفرصة. |
| موازنة العميل | علامة التبويب عام | ويمكن استخدام حقل العملة القابل للتحرير هذا لتعقب المبلغ الذي يرغب العميل في إنفاقه على عنصر البند هذا. | يتم ترحيل هذه القيمة إلى الحقل المقابل في بند عرض الأسعار عند إنشاء عرض أسعار من هذه الفرصة. |
| أسلوب الفوترة | علامة التبويب عام | يحتوي هذا الحقل القابل للتحرير على القيم التالية:</br>- الوقت والمادة.</br>- سعر ثابت | يتم ترحيل هذه القيمة إلى الحقل المقابل في بند عرض الأسعار عند إنشاء عرض أسعار من هذه الفرصة. بعد إنشاء بند عرض الأسعار، يتم تأمين الحقل ولا يمكن تغييره. قم بتعيين قيمة هذا الحقل بأقصى قدر ممكن من الدقة. إذا كنت بحاجة إلى تغيير قيمة هذا الحقل في بند عرض الأسعار، فقم بحذف بند عرض الأسعار ثم قم بإعادة إنشائه. |