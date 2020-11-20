---
title: الجديد أو المتغير في إصدار التحديث 17، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 12.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: bb93208217972639f91b39b7b6705d9897373ef7
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126782"
---
# <a name="project-service-automation-update-release-17-v3"></a>الإصدار 3 من Project Service Automation، إصدار التحديث 17

يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365. يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.  هذا الإصدار متوافق مع Dynamics 365 9.x. للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث. لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في PSA V3، إصدار التحديث 17. يتضمن هذا الإصدار رقم البنية V3.10.6.34 وهو متوفر بشكل عام من خلال تحديث ذاتي في مارس 2020.


## <a name="update-release-17"></a>إصدار التحديث 17

### <a name="bug-fixes"></a>إصلاحات الأخطاء

**عام**

- ‏‫تم الإصلاح‬: تحديث Project Service Automation لفرض تراخيص Team Member (سيتضمن مركز موارد المشروع بيانات تعريف خطة خدمة Team Member 3.x)
 
**الوقت والمصروفات**

- تم الإصلاح: لا يمكن تغيير تقدير مصروفات من سعر غير صفري إلى صفر (0). تم تجاهل التغيير.

**إدارة المشروع**

- تم الإصلاح: تمت إضافة فحص القيم الفارغة على اسم منصب عضو الفريق.
- تم الإصلاح: تم إهمال الحقل **msdyn_userresourceid** على الكيان **msdyn_resourceassignment**.
- تم الإصلاح: تعالج الآن الترقية من 2.x إلى 3.x حدود المجهود الفارغة على تعيينات المهام.

**المبيعات**

- تم الإصلاح: يعالج **Invoice.PreValidateInvoiceUpdate** الآن سيناريو إعادة تعيين مالكي السجلات بشكل صحيح.
- تم الإصلاح: عندما تكون فئة المعاملة **الوقت**، تكون **UnitGroup** غير قابلة للتحرير لجميع الكيانات، بما فيها **QuoteLineDetails** و **JournalLine** و **InvoiceLineDetail** و **ContractLineDetails**. ومع ذلك، فإن **الوحدة** غير قابلة للتحرير فقط لكل من **JournalLine** و **InvoiceLineDetails**.


