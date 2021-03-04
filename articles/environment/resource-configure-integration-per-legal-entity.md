---
title: تكوين تكامل Project Operations لكل كيان قانوني
description: يقدم هذا الموضوع معلومات حول إعداد التكامل حسب الكيان القانوني في Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5d2bb415362a088e01253fbe54f9f06569b4a921
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122867"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a>تكوين تكامل Project Operations لكل كيان قانوني 

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يرشدك هذا الموضوع عبر الخطوات المطلوبة لتكوين Dynamics 365 Project Operations لكل كيان قانوني.

## <a name="enable-feature-keys-in-dynamics-365-finance"></a>تمكين مفاتيح الميزات في Dynamics 365 Finance

أكمل الخطوات التالية لتمكين الميزات المطلوبة.

1. في Dynamics 365 Finance، انتقل إلى مساحة عمل **إدارة الميزات**.
2. في **قائمة الميزات**، ابحث عن الميزات التالية وقم بتمكينها:
  
    - **تمكين شروط تعاقد متعددة لمشروع**
    - **تمكين Project Operations على Dynamics 365 Customer Engagement**

> [!NOTE]
> إذا لم تظهر **مفاتيح الميزات** مدرجة، فتحقق من ان إصدار Finance يفي بالحد الأدنى من متطلبات الإصدار (إصدار التطبيق 10.0.13 مع تطبيق جميع تحديثات الجودة أو إصدار أعلى). حدد **التحقق من وجود تحديثات** لتحديث قائمة الميزات.

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a>تعريف سيناريو نشر Project Operations لكيان قانوني

يمكنك تمكين Project Operations على Dynamics 365 Customer Engagement على مستوى الكيان القانوني. يمكنك الحصول على كيان قانوني واحد يستخدم Project Operations على Dynamics 365 Customer Engagement للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬. في نفس البيئة، يمكن أن يكون لديك كيان قانوني آخر يستخدم Project Operations لسيناريوهات المنتجات المخزنة/أوامر الإنتاج‬.

1. في Dynamics 365 Finance، انتقل إلى **إدارة المشاريع والمحاسبة** > **الإعداد‏‎** > **معلمات إدارة المشاريع والمحاسبة العمومية**.
2. في قائمة الكيانات القانونية المتاحة، حدد الكيانات التي سيتم فيها تمكين العديد من شروط التعاقد وProject Operations على ميزات Dynamics 365 Customer Engagement. اترك الكيانات القانونية التي ستستخدم Project Operations لسيناريوهات المنتجات المخزنة/أوامر الإنتاج‬ من دون تحديدها.

> [!NOTE]
> لا يمكن تحديد الكيان القانوني الا إذا لم يكن لديه أي مشاريع موجودة.

## <a name="configure-project-management-and-accounting-parameters"></a>تكوين معلمات إدارة المشاريع والمحاسبة

يحتاج كل كيان قانوني يستخدم Project Operations على Dynamics 365 Customer Engagement إلى مجموعة من المعلمات الافتراضية. يتم تكوين هذه المعلمات على علامة تبويب **Project Operations** في صفحة **معلمات إدارة المشاريع والمحاسبة‬**. المعلمات هي:

  - **الإعدادات الافتراضية لنوع الفوترة**: يستخدم Project Operations مجموعة ثابتة من الإعدادات الافتراضية لنوع الفوترة التي يجب تعيها إلى خصائص البنود في Finance. أنشئ سجلاً لكل نوع فوترة: **غير محدد** و **خاضع للرسوم** و **غير خاضع للرسوم** و **تكميلي‬** و **غير متوفر**.
  - **الإعدادات الافتراضية لفئة المشروع**: حدد الإعدادات الافتراضية لفئة المشروع التي يجب استخدامها لكل نوع حركة. سيتم استخدام هذه الإعدادات الافتراضية في **دفتر يومية تكامل Project Operations** وفي التقديرات التي لم يتم فيها تحديد فئة مشروع للقيمة الفعلية للمشروع.
  - **التنبؤات**: حدد نموذج التنبؤ الذي سيتم استخدامه لتقديرات الوقت والمصروفات.


[!INCLUDE[footer-include](../includes/footer-banner.md)]