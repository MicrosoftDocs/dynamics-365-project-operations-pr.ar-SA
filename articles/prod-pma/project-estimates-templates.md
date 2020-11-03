---
title: مزامنة تقديرات المشاريع مباشرة من Project Service Automation إلى Finance and Operations
description: يصف هذا الموضوع القوالب والمهام الأساسية المستخدمة لمزامنة تقديرات ساعات المشروع وتقديرات نفقات المشروع مباشرةً من Microsoft Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 336de474c859d30d1ec07ae34bf0c3d578faeef1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070772"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a>مزامنة تقديرات المشاريع مباشرة من Project Service Automation إلى Finance and Operations

[!include[banner](../includes/banner.md)]

يصف هذا الموضوع القوالب والمهام الأساسية المستخدمة لمزامنة تقديرات ساعات المشروع وتقديرات نفقات المشروع مباشرةً من Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.

> [!NOTE]
> - يتوفر تكامل مهام المشروع ، وفئات حركات المصروفات ، وتقديرات الساعة ، وتقديرات المصروفات ، وتأمين الوظائف في الإصدار 8.0.
> - القيم الفعلية المتكاملة متوفرة في الإصدار 8.0.1 أو أحدث.

## <a name="data-flow-for-project-service-automation-to-finance"></a>تدفق البيانات لـ Project Service Automation إلى Finance

يستخدم حل تكامل Project Service إلى Finance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Project Service Automation وFinance. تعمل قوالب التكامل المتوفرة مع ميزة تكامل البيانات على تمكين تدفق البيانات حول تقديرات ساعات المشروع وتقديرات نفقات المشروع من Project Service Automation إلى Finance.

يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات بين Project Service Automation وFinance.

[![تدفق البيانات لتكامل Project Service Automation مع Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)

## <a name="project-hour-estimates"></a>تقديرات ساعات المشاريع

### <a name="template-and-tasks"></a>القوالب والمهام

للوصول إلى القوالب المتوفرة، في مركز إدارة Microsoft Power Apps، حدد **المشاريع** ، ثم في الركن الأيمن العلوي، حدد **مشروع جديد** لتحديد القوالب العامة.

يتم استخدام القالب والمهام الأساسية التالية لمزامنة تقديرات ساعات المشروع من Project Service Automation إلى Finance:

- **اسم القالب في تكامل البيانات:** تقديرات ساعات المشاريع (PSA إلى Fin and Ops)
- **اسم المهام في المشروع:**

    - علاقات الحركة
    - تقديرات المصروفات

### <a name="entity-set"></a>مجموعة الكيانات

| Project Service Automation | التمويل                                       |
|----------------------------|-----------------------------------------------|
| مهام المشروع              | كيان التكامل لتقديرات ساعة المشروع |

### <a name="entity-flow"></a>تدفق الكيانات

تتم إدارة تقديرات ساعات المشروع في Project Service Automation ، وتتم مزامنتها مع Finance كتوقعات ساعة المشروع.

### <a name="prerequisites"></a>المتطلبات الأساسية

قبل ان تتم مزامنة تقديرات ساعات المشروع ، يتعين عليك مزامنة المشروعات ومهام المشروع وفئات حركات مصروفات المشروع.

### <a name="power-query"></a>Power Query

في قالب تقديرات الساعات للمشروع ، يجب استخدام Microsoft Power Query ل Excel لإكمال هذه المهام:

- قم بتعيين معرف نموذج التنبؤ الافتراضي الذي سيتم استخدامه عندما يقوم التكامل بإنشاء تنبؤات جديده بالساعات.
- يقوم بتصفية إيه سجلات خاصه بالموارد في المهمة التي ستؤدي إلى التكامل في التنبؤ بالساعات.
- تصفيه إيه صفوف فئات حركات فارغه. قد ينتج عن الفشل في إكمال هذه المهمة تنبؤات بالساعة غير صحيحه.

#### <a name="set-the-default-forecast-model-id"></a>تعيين معرف نموذج التنبؤ الافتراضي

لتحديث معرف نموذج التنبؤ الافتراضي في القالب ، انقر فوق سهم **التعيين** لفتح التعيين. ثم حدد ارتباط **الاستعلام المتقدم والتصفية**.

- إذا كنت تستخدم قالب تقديرات ساعات المشروع الافتراضية (PSA إلى Fin and Ops)، فحدد **الشرط المدرج** في قائمة **الخطوات المطبقة**. في إدخال **الوظيفة** ، استبدل **O\_التنبؤ** باسم معرف نموذج التنبؤ الذي يجب استخدامه مع التكامل. يحتوي القالب الافتراضي علي معرف نموذج تنبؤ من بيانات العرض التوضيحي.
- إذا كنت تقوم بإنشاء قالب جديد ، فيجب عليك أضافه هذا العمود. في Power Query، حدد **إضافه عمود شرطي** ، وادخل اسما للعمود الجديد، مثل **معرف النموذج**. أدخل الشرط للعمود، حيث، إذا لم تكن مهمة المشروع فارغة، عندئذٍ \<enter the forecast model ID\>؛ وإلا فقيمة فارغة.

#### <a name="filter-out-resource-specific-records"></a>تصفيه السجلات الخاصة بالمورد

يحتوي نموذج تقديرات ساعات المشروع (PSA إلى Fin and Ops) على عامل تصفية افتراضي يزيل أي سجلات خاصة بالموارد. إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة عامل التصفية هذا. حدد ارتباط **الاستعلام المتقدم والتصفية** للتصفية في عمود **msdyn\_islinetask** بحيث يتم تضمين السجلات **الزائفة** فقط.

#### <a name="filter-out-empty-transaction-category-rows"></a>تصفيه صفوف فئات حركات فارغه

يجب أضافه عامل تصفيه لأزاله إيه صفوف تشتمل علي فئات حركات فارغه. هذه المهمة مطلوبه ، بغض النظر عما إذا كنت تستخدم القالب الافتراضي أو إنشاء قالب خاص بك. يقوم عامل التصفية هذا بازاله أي صفوف ملخص من Project Service Automation والذي قد يتسبب في عدم صحة تنبؤات الساعات في Finance. حدد ارتباط **الاستعلام المتقدم والتصفية** لتصفية السجلات الفارغة في عمود **msdyn\_transactioncategory\_القيمة**.

### <a name="template-mapping-in-data-integration"></a>تعيين القالب في تكامل البيانات

يُظهر الرسم التوضيحي التالي مثالاً لتعيينات مهام القالب في تكامل البيانات. يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.

[![تعيين مهمة القالب في تكامل البيانات](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)

## <a name="project-expense-estimates"></a>تقديرات مصروفات المشاريع

### <a name="template-and-tasks"></a>القوالب والمهام

يتم استخدام القالب والمهام الأساسية التالية لمزامنة تقديرات مصروفات المشروع من Project Service Automation إلى Finance:

- **اسم القالب في تكامل البيانات:** تقديرات مصروفات المشاريع (PSA إلى Fin and Ops)
- **اسم المهام في المشروع:**

    - علاقات الحركة 
    - تقديرات المصروفات

### <a name="entity-set"></a>مجموعة الكيانات

| Project Service Automation | التمويل                                                  |
|----------------------------|----------------------------------------------------------|
| اتصالات المعاملات    | كيان التكامل لعلاقات معاملات المشروع |
| بنود التقدير             | كيان التكامل لتقديرات مصروفات المشاريع         |

### <a name="entity-flow"></a>تدفق الكيانات

تتم إدارة تقديرات مصروفات المشاريع في Project Service Automation ، وتتم مزامنتها مع Finance كتوقعات مصروفات المشاريع.

### <a name="prerequisites"></a>المتطلبات الأساسية

قبل ان تتم مزامنة تقديرات مصروفات المشروع ، يتعين عليك مزامنة المشروعات ومهام المشروع وفئات حركات مصروفات المشروع.

### <a name="power-query"></a>Power Query

في قالب تقديرات مصروفات المشروع ، يجب عليك استخدام Power Query لإكمال المهام التالية:

- تصفيه لتضمين سجلات سطور التقدير للمصروفات فقط.
- قم بتعيين معرف نموذج التنبؤ الافتراضي الذي سيتم استخدامه عندما يقوم التكامل بإنشاء تنبؤات جديده بالساعات.
- تحويل أنواع الفواتير.
- تحويل أنواع الحركات.

#### <a name="filter-to-include-only-expense-estimate-lines"></a>تصفيه لتضمين سطور التقدير للمصروفات فقط.

يحتوي قالب تقديرات مصروفات المشروع (PSA إلى Fin and Ops) على عامل تصفية افتراضي يتضمن فقط بنود المصروفات في التكامل. إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة عامل التصفية هذا. حدد مهمة **علاقات الحركات** ، ثم انقر فوق سهم **التعيين** لفتح التعيين. حدد ارتباط **الاستعلام المتقدم والتصفية**. قم بتصفية عمود **msdyn\_transactiontype1** بحيث يتضمن **msdyn\_estimateline** فقط.

#### <a name="set-the-default-forecast-model-id"></a>تعيين معرف نموذج التنبؤ الافتراضي

لتحديث معرف نموذج التنبؤ الافتراضي في القالب، فحدد **تقديرات المصروفات** ، ثم انقر فوق سهم **التعيين** لفتح التعيين. حدد ارتباط **الاستعلام المتقدم والتصفية**.

- إذا كنت تستخدم القالب الافتراضي لتقديرات مصروفات المشروع (PSA إلى Fin and Ops) ، في Power Query ، حدد **الشرط المدرج** الأول من قسم **الخطوات المطبقة**. في إدخال **الوظيفة** ، استبدل **O\_التنبؤ** باسم معرف نموذج التنبؤ الذي يجب استخدامه مع التكامل. يحتوي القالب الافتراضي علي معرف نموذج تنبؤ من بيانات العرض التوضيحي.
- إذا كنت تقوم بإنشاء قالب جديد ، فيجب عليك أضافه هذا العمود. في Power Query، حدد **إضافه عمود شرطي** ، وادخل اسما للعمود الجديد، مثل **معرف النموذج**. أدخل الشرط للعمود، حيث، إذا لم يكن معرف بند التقدير فارغًا، عندئذٍ \<enter the forecast model ID\>؛ وإلا فقيمة فارغة.

#### <a name="transform-the-billing-types"></a>تحويل أنواع الفواتير

يتضمن قالب تقديرات مصروفات المشروع (PSA إلى Fin and Ops) عمودًا شرطيًا يتم استخدامه لتحويل أنواع الفواتير التي يتم استلامها من Project Service Automation أثناء التكامل. إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة هذا العمود الشرطي. حدد ارتباط **الاستعلام المتقدم والتصفية** ثم حدد **إضافة عمود شرطي**. أدخل اسمًا للعمود الجديد، مثل **نوع الفوترة**. ثم أدخل الشرط التالي:

في حالة **msdyn\_billingtype** = 192350000، إذن **NonChargeable**  
وإلا إذا **msdyn\_billingtype** = 192350001، إذن **Chargeable**  
وإلا إذا **msdyn\_billingtype** = 192350002، إذن **Chargeable**  
وإلا **NotAvailable**

#### <a name="transform-the-transaction-types"></a>تحويل أنواع الحركات

يتضمن قالب تقديرات مصروفات المشروع (PSA إلى Fin and Ops) عمودًا شرطيًا يتم استخدامه لتحويل أنواع الحركات التي يتم استلامها من Project Service Automation أثناء التكامل. إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة هذا العمود الشرطي. حدد ارتباط **الاستعلام المتقدم والتصفية** ثم حدد **إضافة عمود شرطي**. أدخل اسمًا للعمود الجديد، مثل **نوع الحركة**. ثم أدخل الشرط التالي:

في حالة **msdyn\_transactiontypecode** = 192350000، إذن **التكلفة**  
وإلا إذا **msdyn\_transactiontypecode** = 192350005، إذن **المبيعات**  
وإلا **فارغ**

### <a name="template-mapping-in-data-integration"></a>تعيين القالب في تكامل البيانات

توضح الرسوم التوضيحية التالية أمثلة لتعيينات مهام القالب في تكامل البيانات. يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.

[![تعيين القالب لحركات تقدير المصروفات](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)

[![تعيين القالب لتقديرات المصروفات](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)