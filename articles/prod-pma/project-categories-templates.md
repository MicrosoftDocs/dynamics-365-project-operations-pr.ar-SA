---
title: مزامنة فئات مصروفات المشاريع بين Finance and Operations وProject Service Automation
description: يصف هذا الموضوع القوالب والمهام الأساسية المستخدمة لمزامنة فئات مصروفات المشروع بين Microsoft Dynamics 365 Finance وDynamics 365 Project Service Automation.
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
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 4abb7fe6554825b97df4cc04ee1b02d731cb4af9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289623"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a>مزامنة فئات مصروفات المشاريع بين Finance and Operations وProject Service Automation

[!include[banner](../includes/banner.md)]

يصف هذا الموضوع القوالب والمهام الأساسية المستخدمة لمزامنة فئات مصروفات المشروع بين Dynamics 365 Finance وDynamics 365 Project Service Automation.

> [!NOTE]
> - يتوفر تكامل مهام المشروع ، وفئات حركات المصروفات ، وتقديرات الساعة ، وتقديرات المصروفات ، وتأمين الوظائف في الإصدار 8.0.
> - القيم الفعلية المتكاملة متوفرة في الإصدار 8.0.1 أو أحدث.
> - إذا كنت تستخدم إصدار Enterprise 7.3.0، بعد تثبيت قاعدة المعارف 4132657 وقاعدة المعارف 4132660، ستتمكن من استخدام القوالب لدمج مهام المشروع وفئات حركات المصروفات وتقديرات الساعات وتقديرات المصروفات والقيم الفعلية ولتكوين الوظائف قفل. إذا كان يجب عليك إعادة تعيين التوزيعات المحاسبية ، فننصحك أيضًا بتثبيت قاعدة المعارف 4131710.

## <a name="data-flow-for-project-service-automation-and-finance"></a>تدفق البيانات لـ Project Service Automation وFinance

يستخدم حل تكامل Project Service وFinance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Project Service Automation وFinance. تعمل قوالب التكامل المتوفرة مع ميزة تكامل البيانات على تمكين تدفق البيانات حول فئات حركات مصروفات المشروع بين Finance وProject Service Automation.

إذا تم إتقان فئات مصروفات المشروع في Finance ، فسيكون تدفق التكامل أولاً من Finance إلى Project Service Automation. يتم بعد ذلك تحديث معرّفات التكامل لفئات مصروفات المشروع من خلال المزامنة من Project Service Automation إلى Finance.

إذا تم إتقان فئات مصروفات المشروع في Project Service Automation ، فسيكون تدفق التكامل أولاً من Project Service Automation إلى Finance. يجب تكوين فئات المشروع بالفعل في Finance قبل المزامنة من Project Service Automation. ثم قم بالمزامنة من Finance مرة أخرى إلى Project Service Automation ، ثم من Project Service Automation إلى Finance مرة أخرى. بهذه الطريقة ، فإنك تضمن أن الفئات مرتبطة ، وأنه لا يتم إنشاء أي تكرارات.

> [!NOTE]
> عادةً ما يتم إتقان فئات مصروفات المشروع في Finance. ومع ذلك ، إذا لم تكن كذلك ، أو إذا تم بالفعل إنشاء فئات المصروفات في Project Service Automation ، فيجب عليك أولاً إجراء المزامنة باستخدام قالب فئات حركة مصروفات المشروع (PSA إلى Fin and Ops). ثم قم بالمزامنة باستخدام قالب فئات معاملات مصروفات المشروع (Fin and Ops إلى PSA). يجب عليك بعد ذلك تشغيل المزامنة من Project Service Automation إلى Finance مرة أخرى.
>
> إذا أجريت المزامنة أولاً من Project Service Automation ، فيجب استيفاء المتطلبات التالية في Finance قبل تشغيل المزامنة:
>
> - يجب أن تكون الفئة المشتركة التي تطابق فئة المشروع التي تم إعدادها في Project Service Automation موجودة ، ويجب تمكينها لكل من **المشروع** و **المصروفات**.
> - لكل كيان مالي قانوني يجب أن يتكامل معه ، يجب أن توجد فئات المشروع التالية:
>
>     - **فئة المشروع** موجودة. 
>     - تم تمكين **الاستخدام في المصروفات**.
>     - تم تمكين **نشط في دفتر اليومية**.
>     - تم تعيين **نوع الحركة** إلى **المصروفات**.

يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات بين Project Service Automation وFinance.

[![تدفق البيانات لتكامل Project Service Automation مع Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a>مزامنة فئة مصروفات المشروع من Finance إلى Project Service Automation

### <a name="template-and-task"></a>القالب والمهمة

للوصول إلى القالب، في مركز إدارة Microsoft Power Apps، حدد **المشاريع**، ثم في الركن الأيمن العلوي، حدد **مشروع جديد** لتحديد القوالب العامة.

يتم استخدام القالب والمهمة الأساسية التالية لمزامنة فئات مصروفات المشروع من Finance إلى Project Service Automation:

- **اسم القالب في تكامل البيانات:** فئات معاملات مصروفات المشروع (Fin and Ops إلى PSA)
- **اسم المهمة في المشروع:** مزامنة الفئات إلى PSA

### <a name="entity-set"></a>مجموعة الكيانات

| التمويل                           | Project Service Automation |
|-----------------------------------|----------------------------|
| كيان التكامل للفئات | فئات المعاملات     |

### <a name="entity-flow"></a>تدفق الكيانات

تتم إدارة فئات مصروفات المشروع في Finance ، وتتم مزامنتها مع Project Service Automation كفئات حركات.

### <a name="power-query"></a>Power Query

عندما تقوم بالمزامنة مع Project Service Automation ، يجب عليك استخدام Microsoft Power Query لـ Excel لتعيين نوع الفوترة في فئة الحركة. يوفر قالب فئات حركات مصروفات المشروع (Fin and Ops إلى PSA) عمودًا افتراضيًا وتعيينًا. إذا قمت بإنشاء القالب الخاص بك ، فيجب إضافة عمود شرطي في Power Query. اتبع الخطوات التالية.

1. انقر فوق السهم لفتح تعيين مهمة فئات مصروفات المشروع في قالب فئات حركات مصروفات المشروع (Fin and Ops إلى PSA).
2. انقر فوق ارتباط **الاستعلام المتقدم والتصفية** لفتح Power Query.
2. حدد **إضافة العمود الشرطي**.
3. أدخل اسمًا للعمود الجديد، مثل **نوع الفوترة**.
4. أدخل الشرط التالي: **إذا كانت CATEGORYID لا تساوي قيمة خالية ، فسيكون 19235001 ، وإلا فسيكون فارغًا**.
5. انقر فوق **موافق** في العمود.
6. تاكد من تعيين هذا العمود الجديد في صفحه التعيين.

يُظهر الرسم التوضيحي التالي مثالاً لتعيينات مهام القالب في تكامل البيانات. يُظهر التعيين معلومات الحقل التي ستتم مزامنتها من Finance إلى Project Service Automation.

[![تعيين فئة مصروفات المشروع إلى قالب Project Service Automation](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a>مزامنة فئة مصروفات المشروع من Project Service Automation إلى Finance

### <a name="template-and-task"></a>القالب والمهمة

يتم استخدام القالب والمهمة الأساسية التالية لمزامنة فئات مصروفات المشروع من Project Service Automation إلى Finance:

- **اسم القالب في تكامل البيانات:** فئات معاملات مصروفات المشروع (PSA إلى Fin and Ops)
- **اسم المهمة في المشروع:** مزامنة الفئات إلى Fin Ops

### <a name="entity-set"></a>مجموعة الكيانات

| Project Service Automation | التمويل                           |
|----------------------------|-----------------------------------|
| فئات المعاملات     | كيان التكامل للفئات |

### <a name="entity-flow"></a>تدفق الكيانات

تتم إدارة فئات مصروفات المشروع في Finance ، وتتم مزامنتها مع Project Service Automation كفئات حركات. تعمل المزامنة مرة أخرى إلى Finance على تحديث فئة المشروع في Finance بمعرف التكامل من Project Service Automation.

### <a name="template-mapping-in-data-integration"></a>تعيين القالب في تكامل البيانات

يُظهر الرسم التوضيحي التالي مثالاً لتعيينات مهام القالب في تكامل البيانات.

> [!NOTE]
> يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.

[![تعيين Project Service Automation إلى قالب Finance](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]