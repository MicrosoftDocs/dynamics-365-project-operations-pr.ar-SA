---
title: تأكيد فاتورة مورد المشروع
description: يشرح هذا المقال كيفية تأكيد فاتورة مورّد المشروع في Microsoft Dynamics 365 Project Operations والتأثير المالي لتأكيد فاتورة مورّد المشروع.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 4dafbe64e0727957068d68f510202a12871b62aa
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261495"
---
# <a name="confirm-a-project-vendor-invoice"></a>تأكيد فاتورة مورد المشروع

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_

بعد التحقق من جميع الشروط في فاتورة البائع في Microsoft Dynamics 365 Project Operations، يمكنك استخدام إجراء "التأكيد" لتأكيد فاتورة المورد.

عند تحديد **تأكيد** على فاتورة مورد، يحدث السلوك التالي:

1. يتم تحديث حالة فاتورة البائع إلى **مؤكدة**.
2. تصبح فاتورة المورد المؤكدة والسجلات المرتبطة بها للقراءة فقط، ولا يمكن تحريرها أو حذفها.
3. إذا أشارت أي قيم فعلية للتكلفة إلى سطر فاتورة المورد كجزء من عملية المطابقة، فسيتم عكس جميع القيم الفعلية للتكلفة المرتبطة بسطر فاتورة المورد المشار إليه.
4. يتم إنشاء القيم الفعلية الجديدة للتكلفة باستخدام المعلومات الموجودة في سطر فاتورة البائع.
5. بعد تأكيد فاتورة المورد، لم يعد بإمكانك إنشاء دفاتر يومية للتصحيح، أو معالجة حالات استدعاء إدخال وقت المعالجة، أو إلغاء الموافقة على الوقت الأصلي، أو المصروفات، أو القيم الفعلية المادية التي تم عكسها.

> [!NOTE]
> إذا كان أي سطر في فاتورة المورد به حالة تحقق بخلاف **مكتملة**، فلا يمكن تأكيد فاتورة المورد.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]