---
title: ملاحظات المطور للموافقات
description: يوفر هذا المقال معلومات مطور إضافية للعمل مع الموافقات.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: df3e27f95bffb9c169644fa3e42ff1e9b2b6ff54
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8924736"
---
# <a name="developer-notes-for-approvals"></a>ملاحظات المطور للموافقات

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

يتضمن Dynamics 365 Project Operations منطق التحقق من الصحة الذي يضمن انتقال السجلات الصحيح من خلال مراحل الموافقة. يضمن الانتقال الصحيح للسجلات: 

  - إنشاء كافة صفوف الداعمة في الجداول ذات الصلة، مثل دفاتر اليومية والقيم الفعلية.
  - توضع على الموافق علامة **الموافق على المشروع** في المشروع قبل المتابعة.


[!INCLUDE[footer-include](../includes/footer-banner.md)]