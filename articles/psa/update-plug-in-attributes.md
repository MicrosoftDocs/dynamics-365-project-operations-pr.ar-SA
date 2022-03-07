---
title: تحديث سمات المكونات الإضافية لتشمل أبعاد التسعير الجديدة
description: يقدم هذا الموضوع معلومات حول تحديث سمات الوظيفة الإضافيه لأبعاد التسعير.
author: Rumant
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: d04561fb6bcbc64f6ad3ea922bff1912824be64c6bb2b18cddd95e9b1b5c7850
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "6988770"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a>تحديث سمات المكونات الإضافية لتشمل أبعاد التسعير الجديدة

[!include [banner](../includes/psa-now-project-operations.md)]

> [!NOTE]
> إذا لم تكن تستخدم ميزات التعاقد وعروض الأسعار في Project Service Automation (PSA)، يمكنك تخطي هذه الموضوع.

يفترض هذا الموضوع أنك أكملت الإجراءات الموجودة في المواضيع، و[إنشاء الحقول والكيانات المخصصة](create-custom-fields-entities.md)، و[إضافة حقول مخصصة إلى إعداد الأسعار وكيانات المعاملات](field-references.md)، و[إعداد الحقول المخصصة كأبعاد تسعير](set-up-pricing-dimensions.md). إذا لم تقم بإكمال هذه الإجراءات، فقم بالرجوع إلى الحالة السابقة وإكمالها ثم عد إلى هذا الموضوع.

عند إنشاء تفصيل بند عرض الأسعار في صفحة **بند عرض الأسعار** لبند عرض أسعار المشروع، يقوم النظام بإنشاء بندين للتقدير في الخلفية -- بند لجانب التكلفة للتقدير والآخر لجانب المبيعات. هذا هو نفس الشيء بالنسبة لبنود عقد المشروع.

عندما تقوم بإجراء تغيير على الكمية أو الحقل في جانب التكلفة، يتم نشر هذا التغيير لجانب المبيعات. ويعد ذلك ممكنًا بسبب المكونات الاضافيه التالية التي يجب إعاده تسجيلها بعد التغيير إلى أبعاد التسعير.

- PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.
- PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.

توضح الخطوات التالية عملية تسجيل المكونات الاضافيه.

1. افتح **PluginRegistrationTool** وقم بالاتصال بالمثيل الخاص بك على الإنترنت.
2. انقر فوق **بحث**، وابحث عن المكون الإضافي المراد تحديثه.

 ![لقطة شاشة لشجرة البحث.](media/PRT-1.png)

3. بعد العثور على المكون الإضافي، حدده ثم انقر فوق **تحديد في النموذج الرئيسي**.

4. حدد خطوة المكون الإضافي المراد تحديثها، وانقر بزر الماوس الأيمن، ثم حدد **تحديث**.

 ![لقطة شاشة للمكون الإضافي المراد تحديثه.](media/PRT-2.png)
 
5. في نافذة التحديث، انقر فوق علامة القطع (**...**) في سمات التصفية.

 ![لقطة شاشة لمعلومات تكوين الخطوة الحالية للتحديث.](media/PRT-3.png)
 
6. حدد خانات اختيار سمات التسعير.

 ![لقطة شاشة تظهر تحديد خانة الاختيار لسمات التسعير.](media/PRT-4.png)

7. انقر فوق **موافق** لإغلاق الصفحة، ثم حدد **تحديث الخطوة**.

 ![لقطة شاشة تظهر زر "تحديث الخطوة".](media/PRT-5.png)
 
8. كرر هذه العملية للمكون الإضافي الثاني، **PreOperationQuoteLineDetail - تحديث msdyn_quotelinetransaction**.

9. أغلق أداة تسجيل المكون الإضافي.



[!INCLUDE[footer-include](../includes/footer-banner.md)]