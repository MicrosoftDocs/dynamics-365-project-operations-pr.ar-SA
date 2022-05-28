---
title: الجديد أو المتغير في إصدار التحديث 41، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في تحديث Microsoft Dynamics 365 Project Service Automation الإصدار 41، V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/07/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 649d8bca36fda0a09dc7230ee4d742cadb32f3b3
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580900"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-41-v3"></a>الجديد أو المتغير في إصدار التحديث 41، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. وهو متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو المتغيرة لتحديث Project Service Automation الإصدار 41، V3. يتضمن هذا الإصدار رقم البنية V3.10.62.162 وهو متوفر بشكل عام من خلال تحديث ذاتي في مارس 2022.

## <a name="update-release-41"></a>إصدار التحديث 41

### <a name="bug-fixes"></a>إصلاحات الأخطاء

تم إصلاح المشكلات التالية.

**إدارة المشروع**
- عند محاولة إنشاء مشروع من قالب يستند إلى مشروع تم إنشاؤه من الوظيفة الإضافية لسطح المكتب، يظهر الخطأ التالي، "التحقق من صحة حقل العمل المخطط لتعيين المورد: يجب ألا يكون تاريخ انتهاء شريحة وقت تعيين كل مورد أقدم من تاريخ البدء".

**الوقت والمصروفات**
- عند محاولة حذف إدخال وقت، تظهر رسالة الخطأ التالية، "حدث خطأ غير متوقع من تعليمة ISV البرمجية".

**‏المبيعات**
- عند إنشاء فاتورة لحدث رئيسي ثابت السعر، لا يتم ملء حقلي **الوصف** و **الوصف الخارجي**. 
