---
title: ما الجديد في أكتوبر 2021 - نشر Project Operations الخفيف
description: يوفر هذا المقال معلومات حول التحديثات الإصلاحية المتوفرة في إصدار أكتوبر 2021 من النشر الخفيف لـ Project Operations.
author: sigitac
ms.date: 10/05/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 7199853bea7e8e99a2a1ce19d6ce88736edb38f8
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921930"
---
# <a name="whats-new-october-2021---project-operations-lite-deployment"></a>ما الجديد في أكتوبر 2021 - نشر Project Operations الخفيف

_ينطبق على: النشر الخفيف – من الصفقة إلى الفوترة الأولية_

ينطبق هذا المقال على مكونات وإصدارات Dynamics 365 Project Operations التالية:

  - Project Operations على بيئة Microsoft Dataverse الإصدار 4.25.0.91


## <a name="features-included-in-this-release"></a>الميزات المضمنة في هذا الإصدار

تم تضمين الميزات التالية في هذا الإصدار:

[إدارة العقود من الباطن](../subcontracting/managing-subcontracts-overview.md): توفر هذه الميزة القدرة على إنشاء عقد من الباطن مع البائع، وتفصيل جميع المشتريات كبنود في العقد من الباطن، وضبط الأسعار، وإقران جهات الاتصال.


## <a name="quality-updates"></a>التحديثات الإصلاحية

| **منطقة الميزات** | **رقم المرجع** | **تحديث إصلاحي** |
| --- | --- | --- |
| الفوترة والتسعير | 2209402 | تم تصحيح عمليات التحقق التي كانت تمنع إصدار فواتير للمبالغ المحتجزة عند تأكيد عقد المشروع. |
| إدارة الفرص | 2227414 | تم نسخ حقول **المنتج**، و **الكتابة**، و **IsProductOverriden** إلى تفاصيل بند عرض الأسعار وتفاصيل شروط التعاقد. |
| الفوترة والتسعير | 2338357 | يجب أن تختلف العملة الموجودة في سجل استخدام المواد عن عملة المشروع عند تحديد المشروع. |
| الوقت والمصروفات | 2414777 | يجب أن يكون إلغاء الموافقة عندما يكون لإدخال المصروفات أو الوقت أكثر من موافقة على مشروع مقترن. |
