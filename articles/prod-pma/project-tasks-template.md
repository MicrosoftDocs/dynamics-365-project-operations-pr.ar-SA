---
title: مزامنة مهام المشروع مباشرةً من Project Service Automation إلى Finance and Operations
description: يصف هذا الموضوع القالب والمهام الأساسية التي يتم استخدامها لمزامنة مهام المشاريع مباشرة من Microsoft Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.
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
ms.openlocfilehash: 666e0d757969b32f16e08128d9f78a2ffe1e8357
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/04/2022
ms.locfileid: "8683134"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>مزامنة مهام المشروع مباشرةً من Project Service Automation إلى Finance and Operations

[!include[banner](../includes/banner.md)]

يصف هذا الموضوع القالب والمهام الأساسية التي يتم استخدامها لمزامنة مهام المشاريع مباشرة من Dynamics 365 Project Service Automation إلى Dynamics 365 Finance.

> [!NOTE]
> - يتوفر تكامل مهام المشروع ، وفئات حركات المصروفات ، وتقديرات الساعة ، وتقديرات المصروفات ، وتأمين الوظائف في الإصدار 8.0.
> - إذا كنت تستخدم إصدار Enterprise 7.3.0، بعد تثبيت قاعدة المعارف 4132657 وقاعدة المعارف 4132660، ستتمكن من استخدام القوالب لدمج مهام المشروع وفئات حركات المصروفات وتقديرات الساعات وتقديرات المصروفات والقيم الفعلية ولتكوين الوظائف قفل. إذا كان يجب عليك إعادة تعيين التوزيعات المحاسبية ، فننصحك أيضًا بتثبيت قاعدة المعارف 4131710.
> - القيم الفعلية المتكاملة متوفرة في الإصدار 8.0.1 أو أحدث.

## <a name="data-flow-for-project-service-automation-to-finance"></a>تدفق البيانات لـ Project Service Automation إلى Finance

يستخدم حل تكامل Project Service إلى Finance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Project Service Automation وFinance. يتيح قالب التكامل المتوفر مع ميزة تكامل البيانات تدفق البيانات حول مهام المشروع من Project Service Automation إلى Finance.

يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات بين Project Service Automation وFinance.

[![تدفق البيانات لتكامل Project Service Automation مع Finance.](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>القالب والمهمة

للوصول إلى القالب، في مركز إدارة Microsoft Power Apps، حدد **المشاريع**، ثم في الركن الأيمن العلوي، حدد **مشروع جديد** لتحديد القوالب العامة.

يتم استخدام القالب والمهمة الأساسية التالية لمزامنة مهام المشروع من Project Service Automation إلى Finance:

- **اسم القالب في تكامل البيانات:** مهام المشروع (PSA إلى Fin and Ops)
- **اسم المهمة في المشروع:** مهام المشروع

قبل أن تتم مزامنة مهام المشروع ، يجب عليك مزامنة عقود المشروع والمشاريع.

## <a name="entity-set"></a>مجموعة الكيانات

| Project Service Automation | التمويل                             |
|----------------------------|-------------------------------------|
| مهام المشروع              | كيان التكامل لمهمة المشروع |

## <a name="entity-flow"></a>تدفق الكيانات

تتم إدارة مهام المشروع في Project Service Automation ، وتتم مزامنتها مع Finance باعتبارها أنشطة مشروع.

## <a name="prerequisites-and-mapping-setup"></a>إعداد المتطلبات المسبقة والتعيين

قبل أن تتم مزامنة مهام المشروع ، يجب عليك مزامنة عقود المشروع والمشاريع.

## <a name="power-query"></a>Power Query

يجب عليك استخدام Microsoft Power Query لـ Excel لتصفية البيانات في حالة تحقق الشرط التالي:

- لديك سجلات خاصة بالمورد في مهمة مشروع.

إذا كنت مضطرًا إلى استخدام Power Query، فاتبع هذه الإرشادات:

- يحتوي قالب مهام المشروع (PSA إلى Fin and Ops) على عامل تصفية افتراضي يستبعد السجلات الخاصة بالموارد من مهمة المشروع عن طريق تعيين عامل التصفية على **IsLineTask** إلى **False**. إذا قمت بإنشاء القالب الخاص بك ، يجب عليك إضافة عامل التصفية هذا.

## <a name="template-mapping-in-data-integration"></a>تعيين القالب في تكامل البيانات

يُظهر الرسم التوضيحي التالي مثالاً لتعيينات مهام القالب في تكامل البيانات. يعرض التعيين معلومات الحقل التي ستتم مزامنتها من Project Service Automation إلى Finance.

[![تعيين القالب.](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]