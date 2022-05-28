---
title: القيم الفعلية
description: يوفر هذا الموضوع معلومات حول كيفية التعامل مع القيم الفعلية في Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 02/22/2022
ms.topic: overview
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 3f0cb8c478e2ce6fba589d51d95649f53f62e883
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581268"
---
# <a name="actuals"></a>العمل الفعلي

_**ينطبق على:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

تمثل القيم الفعلية تقدم الجدول والماليات الذي تمت مراجعته والموافقة عليه في أحد المشروعات. يتم إنشاؤها عند الموافقة على إدخالات الوقت والمصروفات واستخدام المواد وإدخالات دفتر اليومية والفواتير.

> [!IMPORTANT]
> لا ينبغي تحرير أو حذف البيانات الفعلية من النظام. بخلاف ذلك، قد تتأثر النزاهة المالية وأي تكامل مع الأنظمة المالية والمحاسبية الأخرى سلبًا. يتيح لك Microsoft Dynamics 365 Project Operations استخدام عكس القيم الفعلية واستبدالها لتحرير القيم الفعلية في نقاط مختلفة في دورة حياة عملية الأعمال لمشاريعك.

## <a name="recording-actuals-based-on-project-events"></a>تسجيل القيم الفعلية استنادا إلى أحداث المشروع

تسجل Project Operations المعاملات المالية التي تحدث أثناء دورة حياة مشاركة المشروع كحسابات فعلية. يختلف إنشاء القيم الفعلية في أحداث مختلفة في دورة الحياة، اعتمادًا على ما إذا كان ارتباط المشروع يستخدم نموذج فوترة الوقت والمواد أو نموذج فوترة السعر الثابت، وما إذا كان في مرحلة ما قبل البيع أو مشروع داخلي.

توضح الموضوعات التالية التأثير على جدول "القيم الفعلية" في أحداث مختلفة باختلافات مختلفة:

- [تأثير القيم الفعلية في الوقت وفي مشاركة المواد](ActualsonTM.md)
- [التأثير الفعلي في ارتباط ثابت السعر](ActualonFP.md)
- [تأثير القيم الفعلية خلال مرحلة ما قبل البيع للمشاركة](ActualonPreSales.md)
- [تأثير القيم الفعلية لمشروع داخلي](ActualonInternal.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
