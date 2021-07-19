---
title: تكامل ‏‫الكتابة المزدوجة في Project Operations
description: يوفر هذا موضوع نظرة عامة على تكامل الكتابة المزدوجة في Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: 540b6f74d8e79116e5fdb2ceffaa4bbb487ff08f
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368415"
---
# <a name="project-operations-dual-write-integration-overview"></a>نظرة عامة حول تكامل ‏‫الكتابة المزدوجة في Project Operations

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يستخدم Project Operations [إمكانات الكتابة المزدوجة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) لمزامنة البيانات عبر Microsoft Dataverse وDynamics 365 Finance.

يوضح الشكل التوضيحي التالي كيفية مزامنة البيانات كجزء من هذا التكامل بين Dataverse وFinance.

![نظرة عامة حول تدفقات بيانات Project Operations](./media/ProjectOperationsFlows.jpg)

توفر Project Operations في Dataverse واجهة مستخدم حديثة وقابلة للتوسع بسهولة بدون تعليمات برمجية/بتعمليات برمجية طفيفة باستخدام إمكانات Power Platform. ويمكن لمديري المشروع ومديري الموارد وأعضاء فريق المشروع وموظفي المكتب الأمامي الآخرين، تنفيذ أنشطتهم في Project Operations على Dataverse.

يوفر Project Operations في Finance دعم محاسبة المشروع وتقدير الإيرادات. يتم ربط Project Operations بإطار العمل المالي في Finance لحساب ضريبة المبيعات وأسعار صرف العملات ورفع تقارير بالأبعاد المالية وغير ذلك. تعتمد تجارب محاسب المشروع في الغالب على Finance.

يتكون تكامل Project Operations من تكامل المكون التالي:


- [تكامل بيانات التكوين والإعداد في Project Operations](resource-dual-write-setup-integration.md) 
- [تقديرات المشروع والقيم الفعلية](resource-dual-write-estimates-actuals.md)
- [فواتير المشروع](resource-dual-write-project-invoice.md)
- [إدارة المصروفات](resource-dual-write-expense.md)
- [فاتورة المورّد](resource-dual-write-vendor-invoice.md)
