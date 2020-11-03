---
title: مزامنة عقود المشاريع والمشاريع مباشرة من Project Service Automation إلى Finance and Operations
description: يصف هذا الموضوع القالب والمهام الأساسية المستخدمة لمزامنة عقود المشاريع والمشاريع مباشرة من Microsoft Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.
author: Yowelle
manager: AnnBe
ms.date: 09/09/2019
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
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 9e4f11ec0bb88ed0971a3d082e7ca7823fcf8453
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070778"
---
# <a name="synchronize-project-contracts-and-projects-directly-from-project-service-automation-to-finance-and-operations"></a>مزامنة عقود المشاريع والمشاريع مباشرة من Project Service Automation إلى Finance and Operations

[!include[banner](../includes/banner.md)]

يصف هذا الموضوع القالب والمهام الأساسية المستخدمة لمزامنة عقود المشاريع والمشاريع مباشرة من Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.

> [!NOTE] 
> إذا كنت تستخدم الإصدار 7.3.0 من Enterprise ، فيجب عليك تثبيت قاعدة المعارف 4074835.

## <a name="data-flow-for-project-service-automation-to-finance"></a>تدفق البيانات لـ Project Service Automation إلى Finance

> [!NOTE]
> قبل أن تتمكن من استخدام حل تكامل Project Service Automation مع Finance، يجب أن تكون علي دراية بميزة تكامل بيانات Dynamics 365.

يستخدم حل تكامل Project Service إلى Finance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Project Service Automation وFinance. يتيح قالب التكامل المتوفر مع ميزة تكامل البيانات تدفق البيانات حول عقود المشروع والمشاريع وبنود عقود المشروع والأحداث الرئيسية لبنود عقد المشروع من Project Service Automation إلى Finance.

يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات بين Project Service Automation وFinance.

[![تدفق البيانات لتكامل Project Service Automation مع Finance](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)

## <a name="templates-and-tasks"></a>القوالب والمهام

للوصول إلى القوالب المتوفرة، في مركز إدارة Microsoft Power Apps، حدد **المشاريع** ، ثم في الركن الأيمن العلوي، حدد **مشروع جديد** لتحديد القوالب العامة.

تُستخدم القوالب والمهام الأساسية التالية لمزامنة عقود المشاريع والمشاريع من Project Service Automation إلى Finance:

### <a name="integrating-with-dynamics-365-project-service-automation-v2x"></a>التكامل مع Dynamics 365 Project Service Automation v2.x
- **اسم القالب في تكامل البيانات:** المشاريع والعقود (PSA إلى Fin and Ops)
- **اسم المهام في المشروع:**

    - عقود المشروع PSA إلى Fin and Ops
    - مشاريع PSA إلى Fin and Ops
    - خطوط عقد المشروع PSA إلى Fin and Ops
    - مراحل خط عقد المشروع PSA إلى Fin and Ops
  
### <a name="integrating-with-dynamics-365-project-service-automation-v3x"></a>التكامل مع Dynamics 365 Project Service Automation v3.x
هناك تغيير في المخطط في Project Service Automation يؤثر على قالب الحدث الرئيسي لبنود عقد المشروع ، ويلزم استخدام الإصدار 2 من القالب لتكامل Project Service Automation v3.x مع Dynamics 365.

- **اسم القالب في تكامل البيانات:** المشاريع والعقود (PSA 3.x إلى Fin and Ops) - الإصدار 2.0
- **اسم المهام في المشروع:**

    - عقود المشروع PSA إلى Fin and Ops
    - مشاريع PSA إلى Fin and Ops
    - خطوط عقد المشروع PSA إلى Fin and Ops
    - مراحل خط عقد المشروع PSA إلى Fin and Ops

قبل أن تتم مزامنة عقود المشاريع والمشاريع ، يجب عليك مزامنة الحسابات.

## <a name="entity-set"></a>مجموعة الكيانات

| Project Service Automation       | التمويل                                                |
|----------------------------------|--------------------------------------------------------|
| الأوامر                           | كيان التكامل لعقد المشروع                |
| المشروعات                         | كيان التكامل للمشروع                         |
| بنود الأمر                      | كيان التكامل لبند عقد المشروع           |
| المراحل الرئيسية لبنود عقود المشاريع | كيان التكامل للمرحلة الرئيسية لبند عقد المشروع |

## <a name="entity-flow"></a>تدفق الكيانات

تتم إدارة عقود المشروع في Project Service Automation ، وتتم مزامنتها مع Finance كعقود مشروع. كجزء من قالب التكامل ، يمكنك تعيين مصدر التكامل في Finance لعقد المشروع.

تتم إدارة مشروع الوقت والمواد ومشاريع الأسعار الثابتة في Project Service Automation ، وتتم مزامنتها مع Finance كمشاريع. كجزء من تكامل القالب ، يمكنك تعيين مصدر التكامل في Finance للمشروع.

تتم إدارة بنود عقد المشروع في Project Service Automation ، وتتم مزامنتها مع Finance كقواعد فوترة عقد المشروع. إذا كانت طريقة الفوترة تختلف عن نوع المشروع الافتراضي ، تقوم المزامنة بتحديث نوع المشروع لمشروع بند العقد ومجموعة المشروع.

تتم إدارة المعالم الرئيسية لبنود عقد المشروع في Project Service Automation ، وتتم مزامنتها مع Finance باعتبارها المراحل الرئيسية لقاعدة فوترة عقد المشروع.

## <a name="project-service-automation-to-finance-integration-solution"></a>حل تكامل Project Service Automation مع Finance

يتوفر حقل **معرف عقد المشروع** في صفحة **عقود المشاريع**. تم جعل هذا الحقل مفتاحا طبيعيا وفريدا لدعم التكامل.

عند إنشاء عقد مشروع جديد، إذا لم تكن **قيمة معرف عقد مشروع** موجودة بالفعل، سيتم إنشاؤها تلقائيا باستخدام تسلسل رقمي. تتكون القيمة من **ORD** متبوعة بتسلسل الأرقام المتزايد ثم لاحقه من ستة أحرف. إليك مثال: **ORD-01022-Z4M9Q0**.

يتوفر حقل **رقم المشروع** في صفحة **المشاريع**. تم جعل هذا الحقل مفتاحا طبيعيا وفريدا لدعم التكامل.

عند إنشاء مشروع جديد، إذا لم يكن **رقم المشروع** موجودًا بالفعل، سيتم إنشاؤه تلقائيا باستخدام تسلسل رقمي. تتكون القيمة من **PRJ** متبوعة بتسلسل الأرقام المتزايد ثم لاحقه من ستة أحرف. إليك مثال: **PRJ-01049-CCNID0**.

عند تطبيق حل تكامل Project Service Automation مع Finance، يقوم برنامج نصي للترقية بتعيين حقل **معرف عقد المشروع** لعقود المشاريع القائمة وحقل **رقم المشروع** للمشاريع القائمة في Project Service Automation.

## <a name="prerequisites-and-mapping-setup"></a>إعداد المتطلبات المسبقة والتعيين

- قبل أن تتم مزامنة عقود المشاريع والمشاريع ، يجب عليك مزامنة الحسابات.
- في مجموعة الاتصال الخاصة بك ، أضف تعيين حقل مفتاح تكامل لـ **msdyn\_organizationalunits** إلى **msdyn\_name \[Name\]**. قد تحتاج أولا إلى أضافه مشروع إلى مجموعه الاتصال. لمزيد من المعلومات، راجع [دمج البيانات في Common Data Service للتطبيقات](https://docs.microsoft.com/powerapps/administrator/data-integrator).
- في مجموعة الاتصال الخاصة بك ، أضف تعيين حقل مفتاح تكامل لـ **msdyn\_المشاريع** إلى **msdynce\_projectnumber \[رقم المشروع\]**. قد تحتاج أولا إلى أضافه مشروع إلى مجموعه الاتصال. لمزيد من المعلومات، راجع [دمج البيانات في Common Data Service للتطبيقات](https://docs.microsoft.com/powerapps/administrator/data-integrator).
- **SourceDataID** لعقود المشروع والمشاريع يمكن تحديثها بقيمة مختلفة أو إزالتها من التعيين. قيمة القالب الافتراضية هي **Project Service Automation**.
- يجب تحديث تعيين **PaymentTerms** بحيث يعكس شروط الدفع الصالحة في التمويل. يمكنك أيضا أزاله التعيين من مهمة المشروع. تعيين القيمة الافتراضية له القيم الافتراضية لبيانات العرض التوضيحي. يوضح الجدول التالي القيم الموجودة في التنفيذ التلقائي لخدمه المشروع.

    | قيمة | ‏‏الوصف   |
    |-------|---------------|
    | 1     | صافي 30        |
    | 2     | 2% 10، صافي 30 |
    | 3     | صافي 45        |
    | 4     | صافي 60        |

## <a name="power-query"></a>Power Query

يجب استخدام Microsoft Power Query لـ Excel لتصفية البيانات إذا تم استيفاء الشروط التالية:

- يكون لديك أوامر مبيعات في Dynamics 365 Sales.
- لديك وحدات تنظيمية متعددة في Project Service Automation ، وسيتم تعيين هذه الوحدات التنظيمية إلى كيانات قانونية متعددة في Finance.

إذا كان يجب عليك استخدام Power Query ، فاتبع الإرشادات التالية:

- يحتوي قالب المشاريع والعقود (PSA إلى Fin and Ops) على عامل تصفية افتراضي يتضمن أوامر مبيعات فقط من نوع **صنف العمل (msdyn\_ordertype = 192350001)**. يساعد عامل التصفية هذا على ضمان عدم إنشاء عقود المشروع لأوامر المبيعات في Finance. إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة عامل التصفية هذا.
- يجب عليك إنشاء عامل تصفية Power Query يتضمن فقط المؤسسات التعاقدية التي يجب مزامنتها مع الكيان القانوني لمجموعة اتصال التكامل. على سبيل المثال ، يجب مزامنة عقود المشروع التي أبرمتها مع الوحدة التنظيمية للعقد لشركة Contoso US مع الكيان القانوني USSI ، ولكن يجب مزامنة عقود المشروع التي أبرمتها مع الوحدة التنظيمية للعقد في شركة Contoso Global مع الكيان القانوني USMF. إذا لم تقم بإضافة عامل التصفية هذا إلى تعيين المهام الخاص بك ، فستتم مزامنة جميع عقود المشروع مع الكيان القانوني المحدد لمجموعة الاتصال ، بغض النظر عن الوحدة التنظيمية للعقد.

## <a name="template-mapping-in-data-integration"></a>تعيين القالب في تكامل البيانات

> [!NOTE] 
> لم يتم تضمين حقول **CustomerReference** ، و **AddressCity** ، و **AddressCountryRegionID** ، و **AddressDescription** , **AddressLine1** ، و **AddressLine2** ، و **AddressState** ، و **AddressZipCode** في التعيين الافتراضي لعقود المشروع. يمكنك أضافه التعيينات إذا كنت تطلب ان تتم مزامنة هذه البيانات لعقود المشروعات.
>
> لا يتم تضمين حقول **الوصف** ، و **المعرف الأصلي** ، و **مجموعة المشاريع** ، و **ProjectManagerPersonnelNumber** ، و **نوع المشروع** في التعيين الافتراضي للمشاريع. يمكنك أضافه التعيينات إذا كنت تطلب ان تتم مزامنة هذه البيانات للمشاريع.

توضح الرسوم التوضيحية التالية أمثلة لتعيينات مهام القالب في تكامل البيانات. يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.

[![تعيين قالب عقد المشروع](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)

[![تعيين قالب المشروع](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)

[![تعيين قالب شروط تعاقد المشروع](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)

[![تعيين قالب المرحلة الرئيسية لشروط تعاقد المشروع](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)

#### <a name="project-contract-line-milestone-mapping-in-the-projects-and-contracts-psa-3x-to-dynamics---v2-template"></a>تعيين المراحل الرئيسية لعقود المشاريع في المشاريع والعقود (PSA 3.x إلى Dynamics) - قالب v2:

[![تعيين المرحلة الرئيسية لشروط تعاقد المشروع مع قالب من الإصدار الثاني](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)