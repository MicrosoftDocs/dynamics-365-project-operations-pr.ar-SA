---
title: مراحل المشروع
description: يقدم هذا الموضوع معلومات حول مراحل المشروع المتوفرة في Microsoft Dynamics Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 554ad63bc44cbe5a1fe91eb47fedbb74bbedd4b6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070771"
---
# <a name="project-stages"></a>مراحل المشروع

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

يتم تصميم مراحل المشروع لتعكس حالة المشروع أثناء تقدمه. يمكن استخدام التخصيصات لتحديث المراحل تلقائيًا باستخدام عمليات سير عمل الأعمال أو Power Automate أو ملحقات المكونات الإضافية.

يتم تعريف المراحل التالية في سير إجراءات العمل‬ الافتراضي:

- جديدة
- اقتباس
- الخطة
- تسليم
- تم
- إقفال 

## <a name="new"></a>جديدة

عند إنشاء مشروع، يتم تعيين مرحلة المشروع إلى **جديد**. إذا تم إنشاء المشروع من قالب، فقد يحتوي على جدول وتقدير وبيانات الفريق. وبخلاف ذلك، فهو مخطط للمشروع، ويجب إدخال المكونات المتبقية.

## <a name="quote"></a>عرض الأسعار

عند ربط مشروع بعرض أسعار أو عند قيامك بإنشاء مشروع من عرض أسعار، فإنه يتم تعيين مرحلة المشروع إلى **عرض أسعار** ، ويتم تحديث تواريخ البدء والانتهاء المقدرة. عندما يكون المشروع في مرحلة **عرض الأسعار** ، تعرض علامة التبويب **المبيعات** في **كيان المشروع** تفاصيل عرض الأسعار.

## <a name="plan"></a>الخطة

عندما تفوز بعرض أسعار مقترن بمشروع، ويتم نقل الشروع إلى مرحلة **العقد** ، فإنه يتم تحديث مرحلة المشروع إلى **الخطة**. عندما يكون المشروع في مرحلة **الخطة** ، تعرض صفحة **كيان المشروع** تفاصيل العقد.

## <a name="deliver"></a>تسليم

عند اكتمال خطة المشروع، وتكون مستعدًا لبدء المشروع، يتعين علي مدير المشروع تحديث مرحلة المشروع إلى **التسليم** لإظهار أن المشروع قد بدأ.

## <a name="complete"></a>‏‫مكتمل‬ 

عند اكتمال العمل الخاص بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **مكتمل**. ومن خلال تحديث مرحلة المشروع إلى **مكتمل** ، يشير مدير المشروع إلى أن العمل قد تم بنسبة 100 بالمائة، ولكنه تم فتح المشروع بحيث يمكن تسجيل أي إدخالات زمنية أو مصروفات معلقة.

## <a name="close"></a>إغلاق

عندما يتم تسجيل جميع الحركات الخاصة بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **الإغلاق**. وعند هذه النقطة، لا يمكن تسجيل أي حركات، ويتم تعيين المشروع للقراءة فقط.
