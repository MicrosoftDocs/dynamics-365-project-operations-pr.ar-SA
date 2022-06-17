---
title: الجديد أو المتغير في إصدار التحديث 41، الإصدار 3 من Project Service Automation
description: يسرد هذا المقال الميزات والإصلاحات المتوفرة في إصدار التحديث 41، الإصدار 3 من Microsoft Dynamics 365 Project Service Automation.
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
ms.openlocfilehash: 8625ae16e45da30614b3a3eec44193bee0c0b36f
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930532"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-41-v3"></a>الجديد أو المتغير في إصدار التحديث 41، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. وهو متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا المقال الميزات والإصلاحات الجديدة أو المتغيرة في إصدار التحديث 41، الإصدار 3 من Project Service Automation. يتضمن هذا الإصدار رقم البنية V3.10.62.162 وهو متوفر بشكل عام من خلال تحديث ذاتي في مارس 2022.

## <a name="update-release-41"></a>إصدار التحديث 41

### <a name="bug-fixes"></a>إصلاحات الأخطاء

تم إصلاح المشكلات التالية.

**إدارة المشروع**
- عند محاولة إنشاء مشروع من قالب يستند إلى مشروع تم إنشاؤه من الوظيفة الإضافية لسطح المكتب، يظهر الخطأ التالي، "التحقق من صحة حقل العمل المخطط لتعيين المورد: يجب ألا يكون تاريخ انتهاء شريحة وقت تعيين كل مورد أقدم من تاريخ البدء".

**الوقت والمصروفات**
- عند محاولة حذف إدخال وقت، تظهر رسالة الخطأ التالية، "حدث خطأ غير متوقع من تعليمة ISV البرمجية".

**‏المبيعات**
- عند إنشاء فاتورة لحدث رئيسي ثابت السعر، لا يتم ملء حقلي **الوصف** و **الوصف الخارجي**. 
