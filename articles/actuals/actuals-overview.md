---
title: العمل الفعلي
description: يوفر هذا المقال معلومات حول كيفية العمل مع القيم الفعلية في Microsoft Dynamics 365 Project Operations.
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
ms.openlocfilehash: 2551b7d6d20df170c913e302e734583135265529
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8924782"
---
# <a name="actuals"></a>العمل الفعلي

_**ينطبق على:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

تمثل القيم الفعلية تقدم الجدول والماليات الذي تمت مراجعته والموافقة عليه في أحد المشروعات. يتم إنشاؤها عند الموافقة على إدخالات الوقت والمصروفات واستخدام المواد وإدخالات دفتر اليومية والفواتير.

> [!IMPORTANT]
> لا ينبغي تحرير أو حذف البيانات الفعلية من النظام. بخلاف ذلك، قد تتأثر النزاهة المالية وأي تكامل مع الأنظمة المالية والمحاسبية الأخرى سلبًا. يتيح لك Microsoft Dynamics 365 Project Operations استخدام عكس القيم الفعلية واستبدالها لتحرير القيم الفعلية في نقاط مختلفة في دورة حياة عملية الأعمال لمشاريعك.

## <a name="recording-actuals-based-on-project-events"></a>تسجيل القيم الفعلية استنادا إلى أحداث المشروع

تسجل Project Operations المعاملات المالية التي تحدث أثناء دورة حياة مشاركة المشروع كحسابات فعلية. يختلف إنشاء القيم الفعلية في أحداث مختلفة في دورة الحياة، اعتمادًا على ما إذا كان ارتباط المشروع يستخدم نموذج فوترة الوقت والمواد أو نموذج فوترة السعر الثابت، وما إذا كان في مرحلة ما قبل البيع أو مشروع داخلي.

توضح المقالات التالية التأثير على جدول "القيم الفعلية" في أحداث مختلفة باختلافات مختلفة:

- [تأثير القيم الفعلية في الوقت وفي مشاركة المواد](ActualsonTM.md)
- [التأثير الفعلي في ارتباط ثابت السعر](ActualonFP.md)
- [تأثير القيم الفعلية خلال مرحلة ما قبل البيع للمشاركة](ActualonPreSales.md)
- [تأثير القيم الفعلية لمشروع داخلي](ActualonInternal.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
