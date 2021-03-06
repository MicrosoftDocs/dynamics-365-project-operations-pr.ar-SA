---
title: نظرة عامة على أبعاد التسعير
description: يوفر هذا الموضوع معلومات حول أبعاد التسعير في Dynamics 365 Project operations.
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
ms.openlocfilehash: fe2ab3a1b12c00e346e27709d66b5a0cb81a3b56
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898200"
---
# <a name="pricing-dimensions-overview"></a>نظرة عامة على أبعاد التسعير

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

الأبعاد المستخدمة في الموارد البشرية لإعداد التسعير والتكاليف تنقسم إلى فئتين:

- أشخاص
- العمل المخطط

ولهذا السبب، هناك نوعان من قيم أبعاد التسعير المتوفرة:

- **مجموعات الخيارات**: الأبعاد التي تمثل تعدادًا ثابتًا لمجموعة من القيم.
- **القيم المستندة إلى الكيانات**: الأبعاد التي يمكن أن تكون مجموعة متنوعة من القيم.

## <a name="pricing-dimensions"></a>أبعاد التسعير

يُشحن Dynamics 365 Project Operations مع مجموعة افتراضية من أبعاد التسعير. يمكنك عرض أبعاد التسعير هذه عن طريق الانتقال إلى **عمليات المشروع** > **المعلمات**. في سجل المعلمات، في علامة التبويب **أبعاد التسعير المستندة إلى المبلغ**، تحقق من أن الدور، **msdyn_resourcecategory** والوحدة التنظيمية للموارد، **msdyn_organizationalunit** يشتملان على الحقلين **قابل للتطبيق على المبيعات** **قابل للتطبيق على التكلفة** معينين إلى **نعم**. مع تمكين هذه الحقول، سيتيح لك إمكانية إعداد السعر والتكلفة لكل مجموعة دور ووحدة تنظيمية.

إذا كنت بحاجة إلى أسعار أو تكلفه للموارد الخاصة بك باستخدام سمات إضافية، فيمكنك إنشاء حقول وكيانات وأبعاد مخصصة.

## <a name="pricing-human-resource-time"></a>وقت المورد البشري للتسعير
غالبًا ما تكون كيفية قيام المؤسسة بتسعير وقت الموارد البشرية اعتبارًا استراتيجيًا مهمًا يؤثر بشكل مباشر على ربحية المؤسسة. اعمل مع الفرق المالية ورؤساء التدريب عندما تكون مؤسستك جاهزة لتحديد كيف تريد إعداد فاتورة ومعدلات تكلفة لوقت الموارد البشرية.

تشمل الاعتبارات الأخرى للتسعير ما إذا كان يجب إعادة استخدام الحقول أو الكيانات التي لا تمثل أبعادًا للتسعير حاليًا ولكن يتم تطبيقها كبعد تسعير لمؤسستك. تعتبر الحقول مثل **فئة المعاملات** (**msdyn_transactioncategory**) و**المورد القابل للحجز** (**bookableresource**) أمثلة على أبعاد المرشحين. 

ضع في اعتبارك ما إذا كان يجب أن يكون بُعد التسعير الخاص بك عبارة عن جدول أو مجموعة خيارات. إذا كنت تتوقع تغييرات في قيم البعد الذي يتجاوز 10 أو 12 وتحتاج إلى سمات إضافية على هذه القيم ، فيمكنك إنشاء كيان بدلاً من مجموعة خيارات. تتطلب المحافظة على مجموعة خيارات ، مثل إضافة القيم أو إزالتها ، مسؤولًا أو مطورًا ، بينما يمكن لمعظم المستخدمين إضافة صفوف جديدة إلى جدول.

يوضح المثال التالي معدلات الفاتورة التي تم إعدادها بناءً على الدور ووحدة توفير الموارد التي ينتمي إليها المورد. تعتمد معدلات التكلفة عادة على نطاق مرتب الموظف ووحدة المؤسسة التي ينتمي إليها. في هذا المثال ، ستبدو جداول معدل الفاتورة ومعدل التكلفة كما يلي.

**نموذج أسعار الفاتورة**

| الدور        | الوحدة التنظيمية    |الوحدة      |السعر      |العملات  |
| ------------|-------------|----------|----------:|----------|
| المطور   | Contoso US  |Hour‬ | 200|دولار أمريكي     |
| المطور   | شركة حسني بالهند |Hour‬|   112|دولار أمريكي     |


**نموذج أسعار التكاليف**

| نطاق الراتب     | الوحدة التنظيمية    |الوحدة      |السعر      |العملات  |
| ----------------|-------------|----------|----------:|----------|
| My company_Band1 | Contoso US  |Hour‬ | 145|دولار أمريكي     |
| My company_Band2 | شركة حسني بالهند |Hour‬|   67|دولار أمريكي     |
