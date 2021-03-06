---
title: الفواتير المصححة
description: يقدم هذا الموضوع معلومات حول الفواتير المصححة.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e14da1c07d5b697de6caf1b9041c30581ecff102
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898065"
---
# <a name="corrected-invoices"></a>الفواتير المصححة

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

يمكن تحرير الفواتير المؤكدة. عندما تقوم بتحرير فاتورة مؤكدة، يتم إنشاء مسودة فاتورة مُصححة. نظرًا لأن الافتراض هو أنك تريد إلغاء جميع المعاملات والكميات من الفاتورة الأصلية، فمن ثم تتضمن الفاتورة المصححة جميع المعاملات من الفاتورة الأصلية، وتكون جميع الكميات الموجودة بها صفر (0).

عندما لا تتطلب المعاملات تصحيحًا، فيمكنك إزالتها من مسودة الفاتورة المُصححة. لإلغاء أو إرجاع كمية جزئية فقط، يمكنك تحرير حقل الكمية في تفاصيل البند. إذا قمت بفتح تفاصيل بند الفاتورة، فيمكنك الاطلاع على كمية الفاتورة الأصلية. يمكنك بعد ذلك تحرير كمية الفاتورة الحالية حتى تكون أقل من أو أكبر من كمية الفاتورة الأصلية.

عندم تقوم بتأكيد فاتورة تصحيحية، يتم إلغاء القيمة الفعلية للمبيعات المفوترة الأصلية، وإنشاء القيمة الفعلية للمبيعات المفوترة الجديدة. إذا تم تخفيض الكمية، سيتسبب الفرق في إنشاء قمة فعلية لمبيعات غير مفوترة جديدة أيضًا. على سبيل المثال، إذا كان المبيعات الأصلية المفوتر لمدة ثماني ساعات، وكانت تفاصيل بند الفاتورة المُصححة تحتوي على كمية مخفضة تبلغ ست ساعات، فسيتم إلغاء بند المبيعات الأصلي المفوتر ويتم إنشاء عمليتين فعليتين جديدتين:

- قيمة فعلية لمبيعات تمت فوترتها لست ساعات.
- قيمة فعلية لمبيعات غير مفوترة للساعتين المتبقيتين. ويمكن أن يتم فوترة هذه الحركة لاحقا أو وضع علامة عليها على أنها غير خاضعة للرسوم، وذلك وفقا لعمليات التفاوض مع العميل.
