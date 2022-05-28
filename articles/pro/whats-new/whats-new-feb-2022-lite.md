---
title: الجديد في فبراير 2022 - النشر الخفيف لـ Project Operations
description: يوفر هذا الموضوع معلومات حول تحديثات الجودة المتوفرة في إصدار فبراير 2022 من النشر الخفيف لـ Project Operations.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: af66a5f61adf4f016f3fa547bbdfc75d06b2711b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8574552"
---
# <a name="whats-new-february-2022---project-operations-lite-deployment"></a>الجديد في فبراير 2022 - النشر الخفيف لـ Project Operations

_ينطبق على: النشر الخفيف – من الصفقة إلى الفوترة الأولية_

ينطبق هذا الموضوع على المكونات والإصدارات التالية من Microsoft Dynamics 365 Project Operations:

- Project Operations في بيئة Dataverse الإصدار 4.28.0.120

## <a name="features-included-in-this-release"></a>الميزات المضمنة في هذا الإصدار

اعتبارًا من هذا الإصدار، يمكنك إضافة ما يصل إلى 300 عضو في الفريق إلى مشروع واحد. في السابق، كان الحد الأقصى لعدد أعضاء الفريق هو 150. للحصول على مزيد من المعلومات، راجع [حدود المشروع](../../project-management/create-wbs.md#project-limitations).

## <a name="quality-updates"></a>التحديثات الإصلاحية

| منطقة الميزات | رقم المرجع | تحديث إصلاحي |
| --- | --- | --- |
| الفوترة والتسعير | 2497369 | يجب أن يتبع التصحيح المادي قيمة التاريخ في معلمات **التصحيح**. |
| الفوترة والتسعير | 2498697 | تم تحسين تكوين الأمان لـ **استدعاء إدخال الوقت**. |
| الفوترة والتسعير | 2517455 | يجب عدم السماح بتشغيل إجراء **معلمات سطر الفاتورة المحدثة** عدة مرات متزامنة لنفس الفاتورة. |
| الفوترة والتسعير | 2517465 | تم حظر إجراء **إلغاء تنشيط تفاصيل سطر الفاتورة** نظرا لأنه غير مدعوم. |
| الفوترة والتسعير | 2556660 | تم إصلاح عمليات التحقق من فعالية التاريخ التي تتم على قائمة الأسعار المرفقة بسجل معلمات المشروع. |
| إدارة الفرص | 2369202 | تم تصحيح منطق العمل الذي يتحقق من إمكانية إرفاق قوائم الأسعار التي تحتوي على تواريخ فعالية متداخلة بنفس عقد المشروع. |
| إدارة الفرص | 2385965 | تم تصحيح السلوك في علامة تبويب **العملاء** لصفحة **عقد المشروع** عند تحديد **حفظ وإغلاق**. |