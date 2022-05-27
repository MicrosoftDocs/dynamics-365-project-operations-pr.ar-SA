---
title: ملاحظات المطور للموافقات
description: يقدم هذا الموضوع معلومات مطور إضافية حول العمل مع الموافقات.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: c02778c4ed79a8750d207b5870300ebf0f479be7
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8579704"
---
# <a name="developer-notes-for-approvals"></a>ملاحظات المطور للموافقات

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

يتضمن Dynamics 365 Project Operations منطق التحقق من الصحة الذي يضمن انتقال السجلات الصحيح من خلال مراحل الموافقة. يضمن الانتقال الصحيح للسجلات: 

  - إنشاء كافة صفوف الداعمة في الجداول ذات الصلة، مثل دفاتر اليومية والقيم الفعلية.
  - توضع على الموافق علامة **الموافق على المشروع** في المشروع قبل المتابعة.


[!INCLUDE[footer-include](../includes/footer-banner.md)]