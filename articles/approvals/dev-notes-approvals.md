---
title: ملاحظات المطور للموافقات
description: يقدم هذا الموضوع معلومات مطور إضافية حول العمل مع الموافقات.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: a89ea669a262c145b9f391fddc19e79a425fabb5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996775"
---
# <a name="developer-notes-for-approvals"></a>ملاحظات المطور للموافقات

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

يتضمن Dynamics 365 Project Operations منطق التحقق من الصحة الذي يضمن انتقال السجلات الصحيح من خلال مراحل الموافقة. يضمن الانتقال الصحيح للسجلات: 

  - إنشاء كافة صفوف الداعمة في الجداول ذات الصلة، مثل دفاتر اليومية والقيم الفعلية.
  - توضع على الموافق علامة **الموافق على المشروع** في المشروع قبل المتابعة.


[!INCLUDE[footer-include](../includes/footer-banner.md)]