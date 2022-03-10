---
title: خطأ عدم تطابق العملات
description: يوفر هذا الموضع معلومات استكشاف الأخطاء وإصلاحها حول خطأ عدم تطابق العملات الذي يحدث عند حفظ أنواع سجلات محددة.
author: sigitac
ms.date: 12/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 52e33ad3728e1a393e8c7e3ca4e0a4b506d0b774
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903327"
---
# <a name="currency-mismatch-error"></a>خطأ عدم تطابق العملات 

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

عندما تحفظ مشروعًا أو عرض أسعار أو عقدًا أو موردًا قابلاً للحجز، قد تتلقى رسال الخطأ **لا تتطابق عملة الشركة المالكة مع عملة وحدة التعاقد. اختر شركة مالكة أو وحدة تعاقد مختلفة للحصول على عقد مشروع للمتابعة**. يعود سبب ذلك إلى وجود عدم تطابق في العملات بين عملة وحدة التعاقد للسجل وعملة الشركة المالكة.


## <a name="resolution"></a>نوع الحل

لحل هذه المشكلة، قم بما يلي:
- تحقق من عملة وحدة التعاقد لهذا السجل. يمكنك رؤية العملة من خلال فتح سجل الوحدة التنظيمية والتأكد من القيمة في علامة التبويب **عام** في حقل **العملة**.
- تحقق من عملة الشركة المالكة. يمكنك رؤية العملة عن طريق الذهاب إلى **مرتبط** > **دفاتر الأستاذ‬** في سجل الشركة. انقر نقرًا مزدوجًا فوق سجل دفتر الأستاذ المرتبط بالشركة وتحقق من القيمة في علامة التبويب **عام** في حقل **عملة المحاسبة**.

إذا لم تكن العملة التي تم تعيينها في سجل وحدة التعاقد ودفتر الأستاذ متطابقة، فاضبط التكوين أو حدد قيمًا مختلفة عند حفظ السجل. يتطلب النظام وجود تطابق بين هذه السجلات لضمان التدفق الصحيح للفوترة بين الشركات الشقيقة. لمزيد من المعلومات حول التكوينات بين الشركات الشقيقة، راجع [إنشاء حركات بين الشركات الشقيقة](../../project-accounting/create-intercompany-transactions.md).

إذا لم يكن يتوفر لدى سجل الشركة سجل دفتر أستاذ يقترن به، فهذا يشير إلى تكون مفقود عند إعداد البيئة. يجب تصحيح التكوين بواسطة مسؤول النظام. يجب على مسؤول النظام الانتقال إلى **تكوينات الكتابة المزدوجة** وإيقاف **خريطة الكتابة المزدوجة في دفاتر الأستاذ** وإعادة تشغيلها مع المزامنة الأولية لهذه الخريطة ومتطلباتها الأساسية. لمزيد من المعلومات، راجع [إصدارات مخططات الكتابة المزدوجة لـ Project Operations](../../environment/resource-dual-write-maps.md).