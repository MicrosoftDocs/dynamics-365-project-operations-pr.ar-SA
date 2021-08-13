---
title: نظرة عامة على عملية الفوترة
description: يوفر هذا الموضوع نظرة عامة على عملية الفوترة في Project Operations للسيناريوهات المستندة إلى الموارد/غير المخزنة.
author: sigitac
ms.date: 01/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: 804d42f7e8bfd103b9143dc0f5c7ddecdee9e66e6072c3e7bf76b2a8c549cf55
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "7003755"
---
# <a name="invoicing-process-overview"></a>نظرة عامة على عملية الفوترة

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يوفر Project Operations للسيناريوهات المستندة إلى الموارد/غير المخزنة إمكانيات شاملة مصممة بما يلائم احتياجات كل من مدير المشروع وموظف حسابات المقبوضات/محاسب المشروع. بالنسبة لعملية الفوترة، يدير مدير المشروع تراكم فوترة للمشروع، بينما يقوم موظف حسابات المقبوضات/محاسب المشروع بإنشاء مستند فاتورة متوافق ودقيق موجهًا للعميل.

![مخطط سير عمل الفوترة.](./media/invoicing-flow.png)

تحدد شروط تعاقد المشروع طريقة الفوترة لحركات المشروع ذات الصلة. عندما يوافق مدير المشروع على معاملات الوقت والمصروفات، فإن النظام يسجل المعاملات في كيان **القيم الفعلية للمشروع** ويرسل المعلومات إلى وحدة **إدارة المشاريع والمحاسبة** في Dynamics 365 Finance. يراجع محاسب المشروع بعد ذلك ويقوم بترحيل السجلات باستخدام [دفتر يومية تكامل Project Operations](../project-accounting/project-operations-integration-journal.md). يتضمن دفتر اليومية تفاصيل المحاسبة المهمة للقيم الفعلية للمشروع، مثل الفوترة، ومجموعة ضريبة المبيعات، ومجموعة ضريبة مبيعات عناصر الفوترة، والأبعاد المالية.

يمكن لمدير المشروع مراجعة معاملات المبيعات غير المفوترة باستخدام أسلوب فوترة الوقت والمواد في [تراكم فوترة الوقت والمواد](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) وفوترة السعر الثابت في [الأحداث الرئيسية للأسعار الثابتة](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones). وتتيح طرق العرض هذه إمكانية تصفية الحركات التي يجب تضمينها في دوره الفوترة التالية وتحديدها ثم وضع علامة عليها كحركات **جاهزة للفوترة**.

يمكنك [إنشاء فاتورة أولية يدويا](../proforma-invoicing/create-manual-proforma-invoice.md) أو استخدام [عملية دورية](../proforma-invoicing/configure-automated-invoice-creation.md). يمكن لمدير المشروع [تعديل مسودة فاتورة أولية](../proforma-invoicing/manage-proforma-invoice.md) حسب الحاجة ثم تأكيدها.

يتم إرسال الفاتورة الأولية التي تم تأكيدها إلى وحدة **إدارة المشاريع والمحاسبة** في Finance. حيث يقوم محاسب المشروع بتنسيق وتحديث اقتراح فاتورة المشروع، ثم يقوم بنشر المستند وطباعته. يتم تسجيل الفواتير المنشورة للمشروع في دفتر الأستاذ العام بالإضافة إلى الدفاتر الفرعية للعملاء والمشروع.


[!INCLUDE[footer-include](../includes/footer-banner.md)]