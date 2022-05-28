---
title: نشر Project Operations - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية تثبيت نشر Project Operations Lite – التعامل مع الفواتير الأولية‬.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: e33506504665f2e7ef7ad48469082f9f64a2a44b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580716"
---
# <a name="deploy-project-operations---lite"></a>نشر Project Operations - خفيف

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_



يدعم Project Operations نماذج نشر متعددة. لتحديد نموذج النشر الأفضل، راجع [أنواع النشر](determine-deployment-type.md).


> [!IMPORTANT]
> ينتج عن هذا النشر، النشر الخفيف – التعامل مع الفواتير الأولية، **Dataverse-نشر Project Operations فقط**.

- [تثبيت Project Operations في بيئة Dataverse جديدة](#new)
- [تثبيت في بيئة Dataverse الحالية](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a>تثبيت Project Operations في بيئة Dataverse جديدة

1. بصفتك المسؤول [العمومي أو مسؤول Power Platform ](/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص Project Operations، قم بإنشاء بيئة Dataverse جديدة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com). تأكد من تمكين **إنشاء قاعدة بيانات لهذه البيئة** و **تطبيقات Dynamics 365**. للحصول على مزيد من المعلومات، راجع [إنشاء البيئات وإدارتها في مركز إدارة Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. حدد **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a>تثبيت Project Operations في بيئة Dataverse موجودة
1. تأكد من عدم تكوين البيئة باستخدام [الكتابة المزدوجة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) حيث سيؤدي التثبيت إلى تثبيت إمكانات [Project Operations للسيناريوهات المستندة إلى الموارد/المنتجات غير المخزنة](project-operations-integrated-deployment-overview.md).
2. بصفتك [المسؤول العمومي أو مسؤول Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص Project Operations، حدد موقع البيئة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com) حيث تريد تثبيت Project Operations.
3. قم بتثبيت **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365. لمزيد من المعلومات، راجع [إدارة تطبيقات Dynamics 365](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
