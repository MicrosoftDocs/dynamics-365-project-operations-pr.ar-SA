---
title: مزامنة القيم الفعلية لمشروع مباشرةً من Project Service Automation إلى دفتر يومية تكامل المشروع للترحيل في Finance and Operations
description: يصف هذا المقال القوالب والمهام الأساسية التي يتم استخدامها لمزامنة قيم المشروع الفعلية مباشرة من Microsoft Dynamics 365 Project Service Automation إلى Finance and Operations.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 7d912a11d9c7bc66ed43911ee32f25092d551cd6
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2022
ms.locfileid: "8929474"
---
# <a name="synchronize-project-actuals-directly-from-project-service-automation-to-the-project-integration-journal-for-posting-in-finance-and-operations"></a>مزامنة القيم الفعلية لمشروع مباشرةً من Project Service Automation إلى دفتر يومية تكامل المشروع للترحيل في Finance and Operations

[!include[banner](../includes/banner.md)]

يصف هذا المقال القوالب والمهام الأساسية التي يتم استخدامها لمزامنة مهام المشاريع مباشرة من Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.

يقوم القالب بمزامنة الحركات من Project Service Automation إلى جدول مرحلي في Finance. بعد اكتمال المزامنة، **يجب** عليك استيراد البيانات من جدول التجهيز المرحلي إلى دفتر يومية التكامل.

> [!NOTE]
> - يتوفر تكامل القيم الفعلية للمشروع بدءًا من الإصدار 8.0.1.
> - إذا كنت تستخدم إصدار Enterprise 7.3.0، بعد تثبيت قاعدة المعارف 4132657 وقاعدة المعارف 4132660، ستتمكن من استخدام القوالب لدمج مهام المشروع وفئات حركات المصروفات وتقديرات الساعات وتقديرات المصروفات والقيم الفعلية ولتكوين الوظائف قفل. إذا كان يجب عليك إعادة تعيين التوزيعات المحاسبية ، فننصحك أيضًا بتثبيت قاعدة المعارف 4131710.
> - إذا كنت تستخدم الإصدار 7.3.0 ، وقمت بإحضار معاملات الرسوم من Project Service Automation ، فيجب عليك تثبيت قاعدة معارف 4345320 لتضمين هذه الرسوم في فاتورة المشروع.
> - إذا كنت تقوم بإدخال مبالغ ضريبة المبيعات في الوقت المحدد أو حركات النفقات في Project Service Automation ، فيجب عليك تثبيت Project Service Automation Update 7. وبخلاف ذلك ، لن يتم ربط القيم الفعلية للضرائب بالوقت أو القيم الفعلية للمصروفات ، ولن تتم مزامنتها مع Finance. لمزيد من المعلومات ، اتصل بالدعم.

## <a name="data-flow-for-project-service-automation-to-finance"></a>تدفق البيانات لـ Project Service Automation إلى Finance

يستخدم حل تكامل Project Service إلى Finance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Project Service Automation وFinance. تعمل قوالب التكامل المتوفرة مع ميزة تكامل البيانات على تمكين تدفق البيانات حول القيم الفعلية للمشروع من Project Service Automation إلى Finance.

يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات بين Project Service Automation وFinance.

[![تدفق البيانات الخاصة بـ Project Service Automation مع Finance and Operations.](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)

## <a name="project-actuals-from-project-service-automation"></a>القيم الفعلية للمشروع من Project Service Automation

### <a name="template-and-tasks"></a>القوالب والمهام

للوصول إلى القوالب المتوفرة، في مركز إدارة Microsoft Power Apps، حدد **المشاريع**، ثم في الركن الأيمن العلوي، حدد **مشروع جديد** لتحديد القوالب العامة.

يتم استخدام القالب والمهام الأساسية التالية لمزامنة القيم الفعلية للمشروع من Project Service Automation إلى Finance:

- **اسم القالب في تكامل البيانات:** القيم الفعلية للمشاريع (PSA إلى Fin and Ops)
- **اسم المهام في المشروع:**

    - الفعلي
    - TransactionConnections

### <a name="entity-set"></a>مجموعة الكيانات

| Project Service Automation | التمويل                                   |
|----------------------------|----------------------------------------------------------|
| الفعلي                    | كيان التكامل للقيم الفعلية للمشاريع                   |
| اتصالات المعاملات    | كيان التكامل لعلاقات معاملات المشروع |

### <a name="entity-flow"></a>تدفق الكيانات

تتم إدارة القيم الفعلية للمشروع في Project Service Automation ، وتتم مزامنتها مع دفتر يومية تكامل المشروع في Finance. سيتم تطبيق المحاسبة استنادًا إلى الأبعاد المالية الافتراضية وإعداد الترحيل.

### <a name="prerequisites"></a>المتطلبات الأساسية

قبل أن تحدث مزامنة القيم الفعلية ، يجب عليك تكوين معلمات تكامل Project Service Automation ومزامنة المشاريع ومهام المشروع وفئات حركات مصروفات المشروع.

### <a name="power-query"></a>Power Query

في قالب القيم الفعلية للمشروع، يجب عليك استخدام Microsoft Power Query لـ Excel لإكمال هذه المهام:

- قم بتحويل نوع الحركة في Project Service Automation إلى نوع الحركة الصحيح في Finance. تم تحديد هذا التحويل بالفعل في قالب القيم الفعلية للمشروع (PSA إلى Fin and Ops).
- قم بتحويل نوع الفوترة في Project Service Automation إلى نوع الفوترة الصحيح في Finance. تم تحديد هذا التحويل بالفعل في قالب القيم الفعلية للمشروع (PSA إلى Fin and Ops). يتم بعد ذلك تعيين نوع الفوترة إلى خاصية الخط ، بناءً على التكوين الموجود في صفحة **معلمات تكامل Project Service Automation**.
- التصفية إلى وحدات تنظيمية موارد معينة يجب مزامنتها مع هذا القالب.
- إذا تمت مزامنة الوقت بين الشركات الشقيقة أو القيم الفعلية للمصروفات بين الشركات الشقيقة إلى Finance ، فيجب عليك تحويل الوحدة التنظيمية للعقد إلى الكيان القانوني الصحيح في Finance. في قالب القيم الفعلية للمشروع (PSA إلى Fin and Ops) ، يتم تحديد عمود شرطي استنادًا إلى بيانات العرض التوضيحي. يجب عليك تحديث آخر عمود شرطي مدرج إلى الكيانات القانونية الصحيحة. وإلا ، فقد يحدث خطأ في التكامل ، أو قد يتم استيراد حركات فعلية غير صحيحة إلى Finance.
- إذا لم تتم مزامنة الوقت بين الشركات الشقيقة أو القيم الفعلية للمصروفات بين الشركات الشقيقة إلى Finance ، يجب عليك حذف آخر عمود شرطي تم إدراجه من القالب الخاص بك. وإلا ، فقد يحدث خطأ في التكامل ، أو قد يتم استيراد حركات فعلية غير صحيحة إلى Finance.

#### <a name="contract-organizational-unit"></a>الوحدة التنظيمية للعقد
لتحديث العمود الشرطي المدرج في القالب، انقر فوق السهم **تعيين** لفتح التعيين. حدد رابط **الاستعلام والتصفية المتقدمة** لفتح Power Query.

- إذا كنت تستخدم قالب القيم الفعلية للمشروع الافتراضي (PSA إلى Fin and Ops)، في Power Query، حدد **الشرط المُدرج** من قسم **الخطوات المُطبقة**. في إدخال **الوظيفة**، استبدل **USSI** باسم الكيان القانوني الذي يجب استخدامه مع التكامل. أضف الشروط الإضافية إلى إدخال **الوظيفة** عند اللزوم، وقم بتحديث شرط **آخر** من **USMF** إلى الكيان القانوني الصحيح.
- إذا كنت تقوم بإنشاء قالب جديد ، فيجب عليك إضافة العمود لدعم الوقت والنفقات بين الشركات الشقيقة. حدد **إضافه عمود شرطي**، وأدخل اسما للعمود، مثل **الكيان القانوني**. أدخل الشرط للعمود، حيث، إذا كان **msdyn\_contractorganizationalunitid.msdyn\_name** \<organizational unit\>، عندئذٍ \<enter the legal entity\>؛ وإلا فقيمة فارغة.

### <a name="template-mapping-in-data-integration"></a>تعيين القالب في تكامل البيانات

يُظهر الرسم التوضيحي التالي مثالاً لتعيينات مهام القالب في تكامل البيانات. يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.

[![تعيين القالب - القيم الفعلية.](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)

[![تعيين القالب - اتصالات الحركات.](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)

## <a name="import-from-staging-table-after-integration-from-project-service-automation"></a>الاستيراد من الجدول المرحلي بعد التكامل من Project Service Automation

يجب تشغيل عملية الاستيراد من الجدول المرحلي الدورية بعد مزامنة القيم الفعلية من Project Service Automation إلى Finance. ستقوم هذه العملية باستيراد حركات المشروع من الجدول المرحلي إلى دفتر يومية تكامل Project Service Automation ، حيث يتم تطبيق المحاسبة ويمكن ترحيل الحركات المستوردة. نوصي بتشغيل هذه العملية في وضع الدُفعات ؛ يمكن إعداده اختياريًا للتشغيل كدفعة متكررة.

## <a name="update-actuals-from-finance"></a>تحديث القيم الفعلية من Finance

### <a name="template-and-tasks"></a>القوالب والمهام

يتم استخدام القالب والمهام الأساسية التالية لمزامنة رقم الإيصال وضرائب المبيعات لحركات المشروع المُرحلة من Finance إلى Project Service Automation:

- **اسم القالب في تكامل البيانات:** تحديث القيم الفعلية للمشاريع (Fin Ops إلى PSA)
- **اسم المهام في المشروع:**

    - الفعلي 
    - TransactionConnections

### <a name="entity-set"></a>مجموعة الكيانات

| التمويل                                                  | Project Service Automation |
|----------------------------------------------------------|----------------------------|
| كيان التكامل للقيم الفعلية للمشاريع                   | الفعلي                    |
| كيان التكامل لعلاقات معاملات المشروع | اتصالات المعاملات    |

### <a name="entity-flow"></a>تدفق الكيانات

تتم إدارة القيم الفعلية للمشروع في Project Service Automation ، وتتم مزامنتها مع دفتر يومية تكامل المشروع في Finance. بعد ترحيل القيم الفعلية في Finance ، يتم تحديثها في Project Service Automation برقم الإيصال من Finance. إذا تمت إضافة ضرائب المبيعات في Finance ، فسيتم إنشاء قيم ضريبية فعلية جديدة في Project Service Automation.

### <a name="power-query"></a>Power Query

في قالب تحديث القيم الفعلية للمشروع، يجب عليك استخدام Power Query لإكمال هذه المهام:

- قم بتحويل نوع الحركة في Finance إلى نوع الحركة الصحيح في Project Service Automation. تم تحديد هذا التحويل بالفعل في قالب تحديث القيم الفعلية للمشروع (Fin Ops إلى PSA).
- قم بتحويل نوع الفوترة في Finance إلى نوع الفوترة الصحيح في Project Service Automation. تم تحديد هذا التحويل بالفعل في قالب تحديث القيم الفعلية للمشروع (Fin Ops إلى PSA).

### <a name="template-mapping-in-data-integration"></a>تعيين القالب في تكامل البيانات

توضح الرسوم التوضيحية التالية أمثلة لتعيينات مهام القالب في تكامل البيانات. يُظهر التعيين معلومات الحقل التي ستتم مزامنتها من Finance إلى Project Service Automation.

[![تعيين القالب - تحديث القيم الفعلية.](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)

[![تعيين القالب - تحديث الحركة.](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]