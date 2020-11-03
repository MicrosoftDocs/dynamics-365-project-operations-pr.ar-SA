---
title: تقديرات الموارد
description: يقدم هذا الموضوع معلومات حول كيفية حساب تقديرات الموارد في Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070564"
---
# <a name="resource-estimates"></a>تقديرات الموارد

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

تأتي تقديرات الموارد من المجهود الموزع على الوقت الذي تم تحديده في هيكل تنظيم العمل بالإضافة إلى أبعاد التسعير القابلة للتطبيق. بشكل عام، يكون الحساب من خلال **المعدل/ساعة لكل دور x الساعات.** يتم تخزين المجهود الموزع على الوقت لكل مورد في سجل تعيين المورد. ويتم تخزين التسعير في قائمة أسعار محددة مسبقًا. يتم تطبيق تحويل الوحدات على أساس قائمة الأسعار القابلة للتطبيق.

![تقديرات الموارد](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a>سعر التكلفة الافتراضي وعملة التكلفة

يتم تعيين أسعار التكلفة افتراضيًا من الوحدة التنظيمية.

## <a name="default-bill-rate-and-sales-currency"></a>سعر الفاتورة الافتراضي وعملة المبيعات

يتم تطبيق أسعار المبيعات مرة واحدة لكل صفقة. التسلسل الهرمي لقائمة أسعار المبيعات الافتراضي هو كالتالي:

1. المنظمة
2. العميل
3. عرض الأسعار/العقد
