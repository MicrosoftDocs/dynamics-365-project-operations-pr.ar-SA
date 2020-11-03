---
title: استرجاع إدخالات الوقت أو المصروفات المعتمدة
description: يوفر هذا الموضوع معلومات حول كيفية استرجاع الوقت أو حركة المصروفات المعتمدة مسبقًا.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: ''
ms.author: rumant
ms.date: 03/08/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 7bacd70881a6c463cc449a365173da5338a3d3fc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070691"
---
# <a name="recall-approved-time-or-expense-entries"></a>استرجاع إدخالات الوقت أو المصروفات المعتمدة

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

يمكن لعضو فريق المشروع أو أي شخص آخر يقدم وقتًا أو إدخال نفقة أن يستدعي ذلك الوقت أو إدخال المصروفات بعد الموافقة عليه. تتضمن عملية استرجاع إدخال وقت أو مصروفات معتمدة خطوتين:

1. يطلب المرسل استرجاع.
2. يقوم أحد الموافقين باعتماد الاسترجاع.

## <a name="request-a-recall"></a>طلب استرجاع

اتبع هذه الخطوات لطلب استرجاع أحد إدخالات الوقت أو المصروفات المعتمدة.

1. بالنسبة لإدخالات الوقت، انتقل إلى **المشاريع**\> **عملي** \> **إدخال الوقت**.

    -أو-

    بالنسبة لإدخالات المصروفات، انتقل إلى **المشاريع**\> **عملي** \> **المصروفات**.

2. بالنسبة لإدخالات الوقت، حدد كافة الإدخالات الزمنيه الخاصة بمجموعه معينة من المشروع والمهمة. أو بدلا من ذلك، في الشبكة ، حدد الخلايا الفردية للوقت في تاريخ محدد لمشروع محدد.

    -أو-

    بالنسبة لإدخالات المصروفات ، حدد صف إدخال المصروفات المراد استدعاؤه.

3. حدد **استرجاع**. يظهر مربع حوار التأكيد. إذا كان قد تم اعتماد إدخالات الوقت والمصروفات المحددة بالفعل، ستتم مطالبتك بإدخال سبب لل استرجاع.
4. أدخل سببا لعمليه ال استرجاع، ثم حدد **موافق** لتاكيد العملية. يرسل النظام للشخص الذي قام بالموافقة على الإدخالات طلبًا الموافقة على ال استرجاع.

> [!NOTE]
> على الرغم من إمكانية  استرجاع إدخالات الوقت والمصروفات المعتمدة، وذلك في حاله فوتره الوقت أو المصروفات المعتمدة بالفعل إلى العميل، فلا يمكن إنشاء طلب  استرجاع. سيتلقى المستخدم الذي يحاول إنشاء طلب  استرجاع رسالة توضح أنه لا يمكن استرجاع الوقت أو المصروفات لأنه قد تمت فوترته بالفعل.

## <a name="approve-or-reject-a-recall-request"></a>الموافقة على طلب استرجاع أو رفضه

اتبع هذه الخطوات للموافقة علي طلب استرجاع أو رفضه.

1. انتقل إلى **المشاريع** \> **عملي** \> **الموافقات**.
2. في صفحة قائمة **الموافقات** ، قم بتغيير طريقة العرض إلى **‏‫طلبات الاسترجاع للموافقة**. يتم عرض قائمه بطلبات الاسترجاع المرسلة.
3. حدد واحدًا أو أكثر من الإدخالات، ثم حدد **موافقة** أو **رفض**.
4. إذا قمت بتحديد **موافقة** ، تتلقى رسالة تحذير توضح تأثير الموافقة. حدد **موافق** لتأكيد العملية. تمت الموافقة على طلب الاسترجاع.

    -أو-

    إذا حددت **رفض** ، سيتم رفض طلب الاسترجاع.

> [!NOTE]
> وعندما يتم طلب عمليه استرجاع، عندما تتم الموافقة علي عمليه استرجاع، يقوم النظام بالتحقق من أي نشاط فوترة في إدخالات الوقت أو المصروفات. إذا تمت فوترة إدخال بالفعل، أو إذا كان في فاتورة مسودة، سيتلقى القائم بالموافقة رسالة خطأ توضح انه لا يمكن اعتماد الوقت والمصروفات للاسترجاع، وذلك لأنه قد تمت فوترته بالفعل.

## <a name="impact-of-a-recall-request"></a>تأثير طلب الاسترجاع

عند استرجاع موافقة، يحدث هناك تأثير تشغيلي وتأثير مالي.

### <a name="operational-impact"></a>التأثير التشغيلي

إذا تمت الموافقة على طلب استرجاع، يتم تمييز سجل الموافقة على أنه **مرفوض**. يتم تغيير حالة الإدخال إلى **مسترجع** أو **مرفوض** ، وذلك استنادًا إلى ما إذا كان ذلك إدخال وقت أو إدخال مصروفات.

يستطيع عضو فريق المشروع عرض الإدخالات، وتحرير الإدخالات ثم إعادة إرسالها، أو حذف الإدخالات بالكامل.

إذا تم رفض طلب استرجاع، فستظل حالة الإدخال **تمت الموافقة عليه** ، ولا يمكن تحرير الإدخال بواسطة عضو فريق المشروع أو القائم بالموافقة للمشروع.

### <a name="financial-impact"></a>التأثير المالي

في حالة الموافقة على طلب استرجاع، يتم تحديث القيم الفعلية المتعلقة بالتكلفة والمبيعات بالطريقة التالية:

- تم تحديث حقل **حالة التسوية** إلى **تم التعديل**.
- تم تحديث حقل **حالة الفوترة** إلى **تم الإلغاء**.

بعد ذلك، يتم إنشاء إدخالات إلغاء في جدول القيم الفعلية. لإنشاء إدخالات إلغاء، ينسخ النظام قيم الحقول من القيم الفعلية الأصلية. والقيم الوحيدة التي لا يتم نسخها هي قيم الكمية. يتم إلغاء هذه القيم بدلا من ذلك. يتم إنشاء القيم الفعلية المعكوسة لكل من القيم الفعلية لـ **التكلفة** و **المبيعات غير المفوترة**. يتم تعيين حقل **حالة التسوية** للقيم الفعلية الملغاة إلى **غير قابل للتسوية** ، ويتم تعيين حقل **حالة الفوترة** إلى **تم الإلغاء**. بسبب إجراء هذه التغييرات، فإن المصروفات المسجلة وتراكم إيراد في المشروع لن يتم حسابه ضمن المبالغ التي تمثلها هذه القيم الفعلية.

إذا تم رفض طلب استرجاع، فلن يكون هناك تاثير مالي علي المشروع.

## <a name="changes-to-time-entry-records"></a>التغييرات على سجلات إدخال الوقت

يوضح الرسم التوضيحي التالي التغييرات التي تحدث لإدخالات الوقت التي تمت الموافقة عليها عند استرجاعها.

![انتقالات حالة إدخال الوقت](media/TimeEntryStateTransitions.png)

## <a name="changes-to-expense-entry-records"></a>التغييرات على سجلات إدخال المصروفات

يوضح الرسم التوضيحي التالي التغييرات التي تحدث لإدخالات المصروفات التي تمت الموافقة عليها عند استرجاعها.

![انتقالات حالة إدخال المصروفات](media/ExpenseEntryStateTransitions.png)