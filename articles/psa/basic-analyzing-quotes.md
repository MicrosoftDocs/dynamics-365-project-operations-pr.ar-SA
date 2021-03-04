---
title: تحليل عروض أسعار المشروع
description: يوفر هذا الموضوع معلومات حول تحليل عروض أسعار المشروع.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 361a940261811467c46222c3d58c9504434ec882
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145207"
---
# <a name="analysis-of-project-quotes"></a>تحليل عروض أسعار المشروع

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

يحلل Dynamics 365 Project Service Automation عروض أسعار المشروع لتقدير الربحية. كما يحلل أيضًا مدى انسجام عرض الأسعار مع توقعات العملاء بشأن تاريخ التسليم أو تاريخ الاكتمال، وحول budget.tions.

## <a name="profitability-analysis"></a>تحليل الربحية

يحلل Project Service Automation الربحية باستخدام إجمالي هامش الربح وإجمالي هامش الربح المعدل.

- يتم حساب إجمالي هوامش الربح باستخدام المعادلات التالية:

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- يتم حساب إجمالي هامش الربح المعدل باستخدام المعادلة التالية:

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

وإذا كانت القيم الخاصة بإجمالي هامش الربح وإجمالي هامش الربح المعدل تختلف بهامش عريض، سيتم تصنيف جزء كبير من العمل في عرض الأسعار على أنه غير خاضع للرسوم.

## <a name="analysis-of-customer-expectations"></a>تحليل توقعات العميل

يمكنك تحليل عروض الأسعار وإنشاء مخططات لتوقعات العملاء حول الجدول والميزانية إذا قمت بإدخال قيم للحقول التالية:

- حقل **تاريخ التسليم المطلوب** في رأس عرض الأسعار.
- حقل **موازنة العميل** لكل بند عرض الأسعار (للبنود المستندة إلى المشروع والبنود المستندة إلى المنتج).

ويتم تحليل توقعات العملاء المتعلقة بالجدولة عن طريق مقارنة أحدث تاريخ انتهاء لتفاصيل بند عرض الأسعار مع تاريخ التسليم المطلوب عبر كافة بنود عرض الأسعار في عرض الأسعار.

يتم تحليل توقعات العملاء المتعلقة بالموازنة عن طريق مقارنة مجموع موازنة العميل الإجمالية بمبلغ عرض الأسعار عبر كافة بنود عرض الأسعار.


[!INCLUDE[footer-include](../includes/footer-banner.md)]