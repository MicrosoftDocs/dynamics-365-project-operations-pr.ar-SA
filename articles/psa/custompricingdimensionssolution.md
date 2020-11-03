---
title: إنشاء حلول مخصصة لأبعاد التسعير
description: يشرح هذا الموضوع كيفية إنشاء حل مخصص عند إنشاء أبعاد تسعير مخصصة.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 3e437fce5b9f1fb330a713788e24100a4fe02948
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070653"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a>إنشاء حلول مخصصة لأبعاد التسعير

> [!IMPORTANT]
> يجب أن تكون كافة تغييرات أبعاد التسعير المخصصة في حل منفصل. يوفر هذه الممارسة الجيدة المهمة المرونة في المستقبل لتحديث التغييرات أو إزالتها حسب الحاجة، والتي تساعد في إعادة استخدام عملك، وتسهل نقل هذه التغييرات إلى مثيل آخر. بعد إجراء كافة التغييرات المطلوبة، يمكنك تصدير هذا الحل **كحل مُدار** واستيراده إلى مثيلات أخرى لإعادة استخدام إعداد تسعيرك.

1. حدد **الإعدادات** > **الحلول** ، ثم حدد **جديد**. 
2. قم بتسميه الحل، **\<your organization name> أبعاد التسعير** ، وأدخل المعلومات المطلوبة المتبقية، ثم حدد **حفظ**.

> ![إنشاء حل مخصص لأبعاد التسعير](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a>إضافة جميع الكيانات المطلوبة والمكونات ذات الصلة إلى حل أبعاد التسعير
ستحتاج إلى إضافة كيانات Project Service التالية إلى حل التسعير الخاص بك. أكمل الخطوات الواردة في هذا الإجراء لإجراء بعض التغييرات الهامة في المخطط في حل التسعير لكي تصبح الكيانات على علم بأبعاد التسعير الجديدة.

1. حدد **الإعدادات** > **حلول** ، وانقر نقرًا مزدوجًا فوق **\<your organization name> أبعاد التسعير**. 
2. في مستكشف الحلول، في جزء التنقل الأيسر، حدد **إضافة الموجود** > **الكيانات**.
3. في مربع حوار **مكونات الحل** ، حدد الكيانات التالية:

- فعلي
- المورد القابل للحجز
- سطر التقدير
- مهمة المشروع
- تفاصيل بند الفاتورة
- سطر دفتر اليومية
- تفاصيل بنود عقد المشروع
- عضو فريق المشروع
- تفاصيل بند عرض الأسعار‬
- رفع سعر الدور
- سعر الدور 
- إدخال الوقت 

> ![إضافة الكيانات الموجودة إلى حل أبعاد التسعير](media/Existing-entities-to-PD-solution.png)

> ![حدد مكونات الحل](media/Dimension-Components.png)

> [!NOTE]
> تأكد من تضمين كافة النماذج وطرق العرض لكل من الكيانات المحددة.

4. عند مطالبتك بتضمين أية كيانات تابعة للكيانات المحددة، حدد **لا**.

> ![لا تقم بتضمين كافة المكونات ذات الصلة.](media/Do-not-include-required.png)

