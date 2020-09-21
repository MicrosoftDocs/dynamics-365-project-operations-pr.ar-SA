---
title: نظرة عامة على Project Service Automation
description: يقدم هذا الموضوع معلومات عن حل دمج Dynamics 365 Project Service Automation في Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 897e1a1c-d31c-42b8-bb59-6b67202d8d61
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 080a545d8713e52d9778367aec1969b815d683e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748677"
---
# <a name="project-service-automation-overview"></a>نظرة عامة على Project Service Automation

[!include[banner](../includes/banner.md)]

يستخدم حل تكامل Project Service Automation إلى Finance ميزة تكامل البيانات لمزامنة البيانات عبر مثيلات Dynamics 365 Finance وDynamics 365 Project Service Automation من خلال Common Data Service. تعمل قوالب التكامل المتوفرة مع ميزة تكامل البيانات على تمكين تدفق المشاريع وعقود المشروع وبنود عقود المشروع ومراحل بنود عقد المشروع ومهام المشروع وفئات حركات المصروفات وتقديرات الساعات وتقديرات المصروفات من Project Service Automation إلى Finance.

> [!NOTE]
> - إذا كنت تستخدم الإصدار 7.3.0 ، فيجب عليك تثبيت قاعدة المعارف 4074835. ستتمكن بعد ذلك من دمج مشاريع السعر الثابت.
> - إذا كنت تستخدم الإصدار 7.3.0 ، وقمت بإحضار معاملات الرسوم من Project Service Automation ، فيجب عليك تثبيت قاعدة معارف 4345320 لتضمين هذه الرسوم في فاتورة المشروع.
> - إذا كنت تستخدم الإصدار 8.0 ، فستتمكن من استخدام تكامل مهام المشروع وفئات حركات المصروفات وتقديرات الساعة وتقديرات المصروفات وتأمين الوظائف.
> - إذا كنت تستخدم الإصدار 8.0.1 أو أحدث ، فستتمكن من مزامنة القيم الفعلية.

قبل أن تتمكن من دمج Project Service Automation Finance ، يجب عليك تكوين معلمات تكامل Project Service Automation. لمزيد من المعلومات، راجع [معلمات تكامل Project Service Automation](PSA-parameters.md).

يتيح حل التكامل هذا المزامنة المباشرة في السيناريوهات التالية:

- احتفظ بعقود المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.
- قم بإنشاء مشاريع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.
- حافظ على بنود عقد المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.
- حافظ على معالم بنود عقد المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.
- حافظ على مهام المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.
- احتفظ بفئات حركات المصروفات في Finance ، وقم بمزامنتها مباشرة من Finance إلى Project Service Automation.
- قم بإنشاء تقديرات ساعات المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.
- قم بإنشاء تقديرات مصروفات المشروع في Project Service Automation ، وقم بمزامنتها مباشرة من Project Service Automation إلى Finance.
- قم بإنشاء وقت المشروع والمصروفات والرسوم الفعلية في Project Service Automation ، وأنشئ حركات المشروع في دفتر يومية تكامل Project Service Automation بحيث يمكن ترحيلها في Finance.

## <a name="data-synchronization"></a>مزامنة البيانات

يوضح الرسم التوضيحي التالي كيفية مزامنة البيانات كجزء من التكامل بين Project Service Automation وFinance.

> [!NOTE]
> ليست كل القوالب متوفرة حاليا. سيتم إصدار القوالب بمجرد اكتمالها.

[![تكامل Project Service Automation مع Finance](./media/PSA-integration.png)](./media/PSA-integration.png)

## <a name="system-requirements-for-finance"></a>متطلبات النظام لـ Finance

لاستخدام حل تمامل Project Service Automation مع Finance ، يجب عليك تثبيت إصدار Enterprise 7.3 مع تحديث النظام الأساسي 12 أو إصدار لاحق.

## <a name="system-requirements-for-project-service-automation"></a>متطلبات النظام لـ Project Service Automation

لاستخدام حل تكامل Project Service Automation مع Finance ، يجب عليك تثبيت المكونات التالية:

- Dynamics 365 Project Service Automation الإصدار 9.0.0.0 أو إصدار أحدث
- العميل المتوقع إلى الحل النقدي لـ Dynamics 365 Sales، الإصدار 1.14.0.0 (v14) أو إصدار لاحق
- حل تكامل Project Service Automation مع Finance لـ Dynamics 365 Project Service Automation لإصدار 1.0.0.0 أو إصدار لاحق.

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a>قم بتثبيت حل تكامل Project Service Automation مع Finance في مثيل Project Service Automation الخاص بك

قم بتنزيل حل تمامل Project Service Automation مع Finance من [مركز تنزيل Microsoft‬](https://www.microsoft.com/download/details.aspx?id=57016)، واتبع التعليمات المضمنة مع الحل.
