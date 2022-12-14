---
title: نشر Project Operations Lite
description: يوفر هذا المقال معلومات حول كيفية تثبيت النشر الخفيف لـ Project Operations – التعامل مع الفواتير الأولية‬
author: stsporen
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 2c508f56b3018b6a86fea78bcf9ee4136e90f385
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/30/2022
ms.locfileid: "9810962"
---
# <a name="deploy-project-operations-lite"></a>نشر Project Operations Lite

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_



يدعم Project Operations نماذج نشر متعددة. لتحديد نموذج النشر الأفضل، راجع [أنواع النشر](determine-deployment-type.md).


> [!IMPORTANT]
> ينتج عن هذا النشر، النشر الخفيف – التعامل مع الفواتير الأولية، **Dataverse-نشر Project Operations فقط**.

- [تثبيت Project Operations في بيئة Dataverse جديدة](#new)
- [تثبيت في بيئة Dataverse الحالية](#existing)
- [التثبيت في بيئة Dataverse موجودة تتضمن مكونات الكتابة المزدوجة](#existingdw)



## <a name="install-project-operations-lite-to-a-new-dataverse-environment"></a><a name="new"></a>تثبيت Project Operations Lite في بيئة Dataverse جديدة

1. بصفتك المسؤول [العمومي أو مسؤول Power Platform ](/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص Project Operations، قم بإنشاء بيئة Dataverse جديدة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com). تأكد من تمكين **إنشاء قاعدة بيانات لهذه البيئة** و **تطبيقات Dynamics 365**. للحصول على مزيد من المعلومات، راجع [إنشاء البيئات وإدارتها في مركز إدارة Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
1. حدد **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365.


## <a name="install-project-operations-lite-to-an-existing-dataverse-environment"></a><a name="existing"></a>تثبيت Project Operations Lite في بيئة Dataverse موجودة 
1. بصفتك [المسؤول العمومي أو مسؤول Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص Project Operations، حدد موقع البيئة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com) حيث تريد تثبيت Project Operations.
1. قم بتثبيت **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365. لمزيد من المعلومات، راجع [إدارة تطبيقات Dynamics 365](/power-platform/admin/manage-apps).

## <a name="install-project-operations-lite-to-an-existing-dataverse-environment-where-dual-write-solutions-are-already-present"></a><a name="existingdw"></a>تثبيت Project Operations Lite في بيئة Dataverse موجودة توجد بها حلول الكتابة المزدوجة

إذا كنت تريد متابعة تشغيل Project Operations في وضع النشر الخفيف، يجب اتباع هذه الخطوات:

1. بصفتك [المسؤول العمومي أو مسؤول Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) ولديك ترخيص Project Operations، حدد موقع البيئة في [مركز إدارة PowerPlatform](https://admin.powerplatform.com) حيث تريد تثبيت Project Operations.
1. قم بتثبيت **Microsoft Dynamics 365 Project Operations** من قائمة نشر تطبيقات Dynamics 365. لمزيد من المعلومات، راجع [إدارة تطبيقات Dynamics 365](/power-platform/admin/manage-apps).
1. لأن بيئتك تتضمن مكونات الكتابة المزدوجة التي تساعد في التكامل مع تطبيقات التمويل والعمليات المثبتة، فإن تثبيت Project Operations سيؤدي أيضًا إلى بتثبيت الإمكانيات والملحقات المطلوبة لتكامل البيانات المتعلقة بـ Project في تطبيقات التمويل والعمليات. بما أنك تريد تشغيل Project Operations في وضع النشر الخفيف، يجب إزالة مكونات التكامل هذه لأنها ستنشئ قيودا وتكاليف لسيناريوهات النشر الخفيف. قم بإزالة تثبيت حلول **الكتابة المزدوجة في Dynamics 365 Project Operations** و **خرائط كيانات الكتابة المزدوجة في Dynamics 365 Project Operations** يدويًا لإزالة هذه المكونات.
1. انتقل إلى **Project Operations -> الإعدادات -> المعلمات**. افتح صفحة تفاصيل **معلمة المشروع** وعيّن الحقل **سلوك ترقية الحل** إلى **Lite فقط**. ويضمن ذلك أن أي ترقيات Project Operations تتم في وقت لاحق لن تعيد مكونات التكامل إلى Project Operations.  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
