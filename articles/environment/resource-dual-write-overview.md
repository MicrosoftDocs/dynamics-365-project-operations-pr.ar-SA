---
title: تكامل ‏‫الكتابة المزدوجة في Project Operations
description: يوفر هذا موضوع نظرة عامة على تكامل الكتابة المزدوجة في Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: overview
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 9b57b8bab9a6821e71a16b191804af21ae5d0b5a
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582740"
---
# <a name="project-operations-dual-write-integration-overview"></a>نظرة عامة حول تكامل ‏‫الكتابة المزدوجة في Project Operations

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يستخدم Project Operations [إمكانات الكتابة المزدوجة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) لمزامنة البيانات عبر Microsoft Dataverse وDynamics 365 Finance.

يوضح الشكل التوضيحي التالي كيفية مزامنة البيانات كجزء من هذا التكامل بين Dataverse وFinance.

![نظرة عامة حول تدفقات بيانات Project Operations.](./media/ProjectOperationsFlows.jpg)

توفر Project Operations في Dataverse واجهة مستخدم حديثة وقابلة للتوسع بسهولة بدون تعليمات برمجية/بتعمليات برمجية طفيفة باستخدام إمكانات Power Platform. ويمكن لمديري المشروع ومديري الموارد وأعضاء فريق المشروع وموظفي المكتب الأمامي الآخرين، تنفيذ أنشطتهم في Project Operations على Dataverse.

يوفر Project Operations في Finance دعم محاسبة المشروع وتقدير الإيرادات. يتم ربط Project Operations بإطار العمل المالي في Finance لحساب ضريبة المبيعات وأسعار صرف العملات ورفع تقارير بالأبعاد المالية وغير ذلك. تعتمد تجارب محاسب المشروع في الغالب على Finance.

يتكون تكامل Project Operations من تكامل المكون التالي:


- [تكامل بيانات التكوين والإعداد في Project Operations](resource-dual-write-setup-integration.md) 
- [تقديرات المشروع والقيم الفعلية](resource-dual-write-estimates-actuals.md)
- [فواتير المشروع](resource-dual-write-project-invoice.md)
- [إدارة المصروفات](resource-dual-write-expense.md)
- [فاتورة المورّد](resource-dual-write-vendor-invoice.md)
