---
title: إنشاء قالب ساعات عمل
description: يصف هذا الموضوع كيفية إنشاء قالب ساعات العمل في Project Service.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 5788378c7e015c4b11182aaf427aca7d1da48b40
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8598932"
---
# <a name="create-a-work-hours-template-project-service"></a>إنشاء قالب ساعات العمل (Project Service)

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

لإنشاء مشروع وإدارته، يجب تطبيق قالب تقويم على المشروع. يحدد قالب التقويم سمات المشروع التالية:

- ساعات العمل، بما في ذلك وقت البدء والانتهاء
- أيام العمل
- استثناءات التقويم مثل الأيام غير المخصصة للعمل

قالب التقويم المطبق على مشروع هو نسخة من قالب التقويم المعرف في إعدادات المؤسسة.

> [!NOTE]
> إذا قمت بتغيير قالب التقويم، فلا يتم نشر هذه التغييرات إلى ساعات عمل المشروع. لتغيير ساعات عمل المشروع، يجب تطبيق قالب جديد.

لإنشاء قالب تقويم لمنظمتك، يوجد متطلبين أساسيين:

- حدد ساعات العمل المطلوبة في القالب باستخدام مورد جديد أو موجود قابل للحجز.
- قم بإنشاء قالب تقويم جديد وإقران القالب بالمورد القابل للحجز.

**تحديد ساعات عمل القالب**

1. انتقل إلى **الموارد** \> **الموارد**.
2. قم بإنشاء مورد جديد للمرجع في قالب التقويم، أو حدد موردًا موجودًا.
3. حدد علامة التبويب **ساعات العمل** للمورد واستكمل الإرشادات في [تعيين ساعات العمل للمورد](/dynamics365/field-service/set-work-hours-resource) لتكوين قواعد التقويم.

**إنشاء قالب تكوين جديد.**

1. انتقل إلى **الإعدادات** \> **قالب التقويم**.
2. حدد **جديد**، وأدخل اسمًا ووصفًا ومورد القالب.


> [!NOTE]
> عند الرجوع إلى مورد في قالب تقويم، يتم ربط نسخة من تقويم المورد مع قالب التقويم. إذا تم تغيير ساعات العمل للقالب المنسوخ، فلا يتم نشر هذه التغييرات إلى قالب التقويم.


### <a name="see-also"></a>راجع أيضًا  
 [إعداد الموارد](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
