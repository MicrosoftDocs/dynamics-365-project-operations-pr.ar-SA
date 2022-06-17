---
title: ما الجديد أو المتغير في إصدار التحديث 37، الإصدار 3 من Project Service Automation
description: يسرد هذا المقال الميزات والإصلاحات المتوفرة في إصدار التحديث 37، الإصدار 3 من Microsoft Dynamics 365 Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 11/01/2021
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
ms.openlocfilehash: bdbb125b4f41bb9970f5bd8a01cf0bb863c34738
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922482"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-37-v3"></a>ما الجديد أو المتغير في إصدار التحديث 37، الإصدار 3 من Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام. وهو متوافق مع Dynamics 365 9.x. لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).

يسرد هذا المقال الميزات والإصلاحات الجديدة أو المتغيرة في إصدار التحديث 37، الإصدار 3 من Project Service Automation. يحتوي هذا الإصدار على عدد من الإصدار V3.10.58.120، ويتوفر بشكل عام من خلال التحديث الذاتي في نوفمبر 2021.

## <a name="update-release-37"></a>إصدار التحديث 37

### <a name="bug-fixes"></a>إصلاحات الأخطاء

تم إصلاح المشكلات التالية.

**الوقت والمصروفات**
- يتعذر على المستخدمين حذف إدخال وقت عن طريق مسح الخلية.
- تتضمن طريقة عرض **الموافقات الفاشلة الخاصة بي** على موافقات المشروع التي تحتوي على حالة **مرسلة**.

**إدارة المشروع**
- يتلقى المستخدمون خطأ استثنائي مرجعي فارغ عند فتح مشروع في الوظيفة الإضافية لسطح مكتب Microsoft إذا كان اسم موقع عضو فريق المشروع فارغًا.
- لا يوجد زر **حفظ** على الصفحة **مهمة المشروع** بحيث لا يمكن للمستخدمين حفظ التغييرات على سجلات المهام.
- يتعذر على المستخدمين حذف مشروع يحتوي على مهمة مقترنة بعرض أسعار في الحالة **Won**.

**‏المبيعات**
- يتم تحديث الحقل **العملة** على الصفحة **المشروع** لمطابقة عملة القالب المطبق.
- يتم حساب التكلفة بشكل غير صحيح على المهام التي تحتوي على عملات متعددة.
