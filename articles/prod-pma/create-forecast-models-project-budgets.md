---
title: إنشاء نماذج تنبؤ لموازنات المشروع
description: يصف هذا الموضوع كيفية إنشاء نموذج تنبؤ للموازنات المتبقية.
author: Yowelle
manager: AnnBe
ms.date: 04/24/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 32a436d240f5535ff15f8bc3b8ba9be2d1d4da17
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070780"
---
# <a name="create-forecast-models-for-project-budgets"></a>إنشاء نماذج تنبؤ لموازنات المشروع 

[!include [banner](../includes/banner.md)]

يصف هذا الموضوع كيفية إنشاء نموذج تنبؤ للموازنات المتبقية. يستخدم المشروع الذي يخضع لمراقبة الموازنة نوعين من الميزانيات: الأصلية والمتبقية. عندما تنشئ موازنة المشروع، يجب عليك تحديد نماذج التنبؤ بالموازنة الأصلية والمتبقية التي تم إنشاؤها في صفحة **نماذج التنبؤ**. يتم إنشاء موازنات المشروع المستندة إلى النماذج المحددة عند الالتزام بموازنة المشروع.

> [!NOTE]
> لا يمكن أن يحتوي نموذج التنبؤ الذي يتم استخدامه لمراقبة الموازنة على نموذج فرعي أو لا يمكن استخدامه كنموذج فرعي.

1. حدد **إدارة المشاريع والمحاسبة‬** > **الإعداد** > **التنبؤات**  > **نماذج التنبؤ**.
2. حدد **جديد** لإنشاء نموذج تنبؤ جديد، ثم ادخل رقم واسم معرف النموذج للنموذج الجديد. 
3. قم بتعيين الخيار **إيقاف** إلى **نعم** لمنع حدوث أي تغييرات على بنود التنبؤ الخاصة بنموذج التنبؤ. 
4. إذا كان ينبغي على بنود التنبؤ التي يقترن بها النموذج إنشاء تنبؤات التدفقات النقدية في دفتر الأستاذ العام، فعيّن الخيار **تضمين في تنبؤات التدفقات النقدية** إلى **نعم.** 
5. لاستخدام تاريخ المشروع كتاريخ الفاتورة، عيّن الخيار **التنبؤ بتاريخ الفاتورة** إلى **نعم**. 
6. في الحقل **نوع الموازنة** ، حدد أحد أنواع النماذج التالية:

   - **الموازنة الأصلية** : استخدام مبالغ الموازنة الأصلية‏‎ التي تم الالتزام بها عند إنشاء الموازنة الأولية والموافقة عليها.
   - **الموازنة المتبقية** : استخدام مبالغ الموازنة المتبقية أثناء فترة عمل المشروع. يتم تقليل الأرصدة في نموذج التنبؤ هذا بواسطة الحركات الفعلية ويتم زيادتها أو خفضها بواسطة مراجعات الموازنة.
   - **التحويل** : استخدام مبالغ الموازنة المحوّلة للمشروع. التحويل هو عملية اختيارية يمكن تشغيلها لتحويل مبالغ الموازنة غير المستخدمة من سنة مالية إلى أخرى.

7. قم بتعيين الخيارات التالية حسب الاقتضاء:

   - قم بتمكين الخيار **التنبؤ بتاريخ الفاتورة‬‏‫** لاستخدام تاريخ المشروع كتاريخ الفاتورة.
   - قم بتمكين الخيار **التنبؤ بواسطة الأعمال قيد التنفيذ** للتنبؤ بالاستناد إلى الأعمال قيد التنفيذ (WIP)، ثم حدد نوع الأعمال قيد التنفيذ. 
   - يمكنك إبقاء **نوع الموازنة** الافتراضي معينًا إلى **بلا** أو يمكنك إدخال نوع جديد. لا يمكن تغيير نوع الموازنة بعد تغيير سجل.     
    > [!NOTE]
    > إذا قمت بتغيير نوع الموازنة الافتراضية، فلن تكون الخيارات الأخرى متوفرة للتحديثات، ولا يمكنك إعادة استخدام نموذج التنبؤ هذا. 
   


 
