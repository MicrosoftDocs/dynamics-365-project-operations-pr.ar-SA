---
title: منح المشروع
description: توضح هذه الموضوع كيفية إنشاء منحة أو تعديلها.
author: RadhikaRS
manager: AnnBe
ms.date: 04/22/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 89801696d6a2924d78c85f6e9b4281409222dbb0
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070825"
---
# <a name="project-grants"></a>منح المشروع

[!include [banner](../includes/banner.md)]

المنحة هي هدية مالية لغرض أو مشروع معين. توجد عادةً قيود علة كيفية إنفاق المنحة. في إدارة المشاريع والمحاسبة، يمكنك إدخال المنح وتتبعها، وتحديد علاقاتها بالمشاريع وعقود المشاريع. على سبيل المثال، يمكنك تنفيذ المهام التالية:

- ربط المنح بالمشاريع ومصادر التمويل من خلال ارتباطات بصفحات **المشروع** و **تفاصيل عقد المشروع**.
- إدخال تغييرات على المنحة وتعقبها بينما تنتقل من حالة إلى أخرى.
- إدخال التكاليف والمبالغ المطلوبة والمبالغ الممنوحة وتعقبها.
- إنشاء منح رئيسية وربط منح فرعية بها.

يمكنك إنشاء منحة من خلال إدخال كافة التفاصيل في سجل جديد، أو يمكنك نسخ التفاصيل من منحة موجودة ثم تحديثها.

## <a name="create-a-new-grant"></a>إنشاء منحة جديدة

1. انتقل إلى **إدارة المشاريع والمحاسبة** \> **المنح** \> **المنح‏‎**.
2. حدد **جديد** \> **منحة**.
3. في صفحة تفاصيل المنحة، على علامة التبويب السريعة **عام** ، في حقل **معرف المنحة** ، أدخل معرفًا أبجديًا رقميًا للمنحة.
4. في حقل **اسم المنحة** ، أدخل اسمًا للمنحة.
5. في حقل **الوصف** ، أضف تفاصيل حول المنحة الجديدة.

    معظم الحقول الأخرى الموجودة على الصفحة اختيارية، ويمكنك إدخال القدر الذي تريده من المعلومات، قيلاً كان أم كبيرًا.

    تصف القائمة التالية المعلومات المحددة على كل علامة تبويب سريعة لصفحة تفاصيل المنحة:

    - **عام** – أدخل تفاصيل حول المنحة، مثل الاسم والحالة والوصف والغرض والمبلغ.
    - **معلومات الاتصال** – أدخل التفاصيل المتعلقة بأعضاء الفريق والقسم الذي يدير المنحة ومصدر العميل أو المؤسسة التي تقدم المنحة. يمكنك أيضًا الإشارة إلى ما إذا كانت المؤسسة عبارة عن كيان يتلقى المنحة ثم يقوم بتمريرها إلى مستلم آخر. حدد **إضافة** لإضافة معلومات الاتصال مثل أرقام الهواتف وعناوين البريد الإلكتروني الخاصة بالمؤسسة التي توفر المنحة.
    - **التواريخ والمواعيد النهائية** – أدخل التواريخ المتعلقة بالمنحة وتطبيق المنحة. تتضمن الأمثلة تاريخ استحقاق التطبيق وتاريخ الإرسال وتاريخ الموافقة على المنحة أو رفضها.
    - **المشاريع وعقود المشاريع المقترنة** – يمكنك إدخال معلومات على علامة التبويب السريعة هذا فقط إذا تم إعداد حقل **حالة المنحة** على علامة التبويب السريعة **عام** إلى **نشطة** أو **ممنوحة**. حدد من بين الخيارات التالية لإكمال المهمة ذات الصلة:

        - **إضافة مصدر تمويل** – إضافة مصدر تمويل جديد للمنحة. يمكنك إدخال كافة التفاصيل الآن، أو يمكنك استخدام المعلومات الافتراضية ثم تحديثها لاحقًا.
        - **إضافة عقد مشروع** – إضافة معلومات عقد المشروع أو تحديثها.
        - **إضافة مشروع** – إضافة تفاصيل المشروع أو تحديثها.

    - **الإعداد** – إدخال التفاصيل المتعلقة بالأموال المطابقة، إذا كانت هذه المعلومات مطلوبة. يطلب عدد كبير من المؤسسات التي تقدم المنح قيام المستلمين بإنفاق مبلغ معين من أموالهم أو مواردهم الخاصة، لمطابقة المبلغ المقدم في المنحة. في حقل **المشروع المحلي أو معرف التعقب** ، يمكنك إدخال معرف يختلف عن معرف المشروع.

        > [!NOTE]
        > إذا كان جزء من المنحة سيُمنح إلى مؤسسه أخرى، فعليك تعيين الخيار **مانح فرعي** إلى **نعم**. بالنسبة إلى المنح الممنوحة في الولايات المتحدة، يمكنك تحديد ما إذا كان سيتم تقديم المنحة ضمن سلطة الولاية أو سلطة فدرالية.

    - **تفاصيل السحب** – إضافة أو تحديث معلومات حول مدى تكرار سحب الأموال الممنوحة أو الفوترة لها أو إنفاقها.

## <a name="create-a-new-grant-from-a-copy"></a>إنشاء منحة جديدة من نسخة

1. انتقل إلى **إدارة المشاريع والمحاسبة** \> **المنح** \> **المنح‏‎**.
2. حدد **جديد** \> **نسخ من منحة**.
3. ادخل معرفًا أبجديًا رقميًا واسمًا للمنحة الجديدة، ثم حدد **موافق**.
4. في صفحة تفاصيل المنحة، راجع تفاصيل المنحة المنسوخة، وأدخل التغييرات المطلوبة. معظم الحقول الموجودة على الصفحة اختيارية.

## <a name="view-or-modify-grant-details"></a>عرض تفاصيل المنحة أو تعديلها

1. انتقل إلى **إدارة المشاريع والمحاسبة** \> **المنح** \> **المنح‏‎**.
2. حدد المنحة لتعديلها.
3. في جزء الإجراءات، ضمن علامة التبويب **المنحة** ، في مجموعة **المحافظة** ، حدد **تحرير**.
4. راجع تفاصيل المنحة، وأدخل التغييرات المطلوبة.