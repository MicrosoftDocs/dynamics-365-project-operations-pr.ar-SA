---
title: إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة
description: يوفر هذا الموضوع معلومات حول كيفية الاشتراك في Project Operations ونشرها للسيناريوهات المستندة إلى المورد/المنتجات غير المخزنة.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 75ee31e67018fe2a7655d8a8f11e40b433a9a5db6f8f2addac27844f18fffe8d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007850"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

يوضح هذا الموضوع كيفية الاشتراك في العرض التجريبي ونشر بيئة Project Operations للسيناريوهات المستندة إلى الموارد/المنتجات غير المخزنة.

## <a name="prerequisites"></a>المتطلبات الأساسية
- يجب أن يكون لدي المستخدم الذي ينشر المعاينة حقوق المسؤول العمومي لمستأجر Azure. يمكنك إنشاء مستأجر أثناء عملية استرداد العرض الأول. 
- يتطلب نشر بيئة Finance وجود اشتراك Azure صالح والذي ستتم فوترته لكل بيئة. يمكنك استخدام الاشتراك الموجود في المؤسسات أو استخدام [الإصدار التجريبي من Azure](https://azure.microsoft.com/en-us/free/) لبدء العمل. سيتم توفير بيئة CDS مجانًا لفترة زمنية محددة بمدة 30 يومًا.

> [!IMPORTANT]
> شخص واحد فقط، مسؤول المستأجر، في مؤسسة تحتاج إلى تنفيذ هذه المهمة. إذا لم تكن أنت المشترك في هذا الإصدار، فانتظر حتى يتم تسجيل مؤسستك وتستلم بيانات اعتماد المستخدم الخاصة بك.
> 
> تستخدم الإصدارات التجريبية مرة واحدة في المستأجر. يمكنك تشغيل النسخة التجريبية مرة واحدة فقط. من المستحسن إنشاء مستأجر جديد لغرض الإصدار التجريبي.


### <a name="dynamics-365-project-operations-ce---preview-trial"></a>Dynamics 365 Project Operations(CE) - معاينة الإصدار التجريبي 

قبل البدء، تأكد من تسجيل الدخول إلى مستعرض باستخدام حساب عمل المستخدم في المستأجر حيث تريد معاينة Project Operations.

1. استرداد رمز العرض الأول، **Dynamics 365 Project Operations**، هنا [الإصدار التجريبي لـ Project Operations](https://aka.ms/try-po).
2. أكد طلبك.

  سترى أنه تم استرجاع عرض التأكيد بنجاح.

### <a name="dynamics-365-finance-preview-trial"></a>إصدار تجريبي لمعاينة Dynamics 365 Finance

انتقل إلى [الإصدار التجريبي من Dynamics 365 for Finance Preview](https://aka.ms/trypoche) وكرر الخطوات من القسم السابق مع العرض، قم بالتسجيل في البيئة المستضافة على السحابة.  

## <a name="assign-licenses"></a>تعيين التراخيص

> [!IMPORTANT]
> ستحتاج إلى حق وصول إداري إلى مدخل Microsoft 365 الخاص بمؤسستك لإكمال الخطوات التالية.

1. انتقل إلى [مركز إدارة](https://portal.office.com/) لتعيين التراخيص إلى المستخدمين.

2. في صفحة **المستخدمين النشطين**، حدد المستخدمين الذين ترغب في تعيين ترخيص لهم.

3. تحقق من أنه تم تحديد ترخيص **Dynamics 365 Project Operations** وحدد **حفظ التغييرات**.

> [!NOTE]
> لا يلزم تعيين مستخدم إلى عرض الإصدار التجريبي من Finance.

## <a name="start-a-new-project-in-lcs"></a>بدء مشروع جديد في LCS

قم بإنشاء مشروع LCS جديد كما هو موضح في موضوع، [بدء مشروع جديد في LCS](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>إضافة اشتراك Azure إلى مشروع LCS

لإكمال هذه المهمة، اتبع الخطوات الواردة في الموضوع، [إضافة اشتراك Azure إلى مشروع LCS](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>نشر بيئة عرض توضيحي من Finance مع Project Operations لسيناريوهات المورد/المنتجات غير المخزنة

اتبع الإرشادات الموضحة في موضوع، [توفير بيئة جديدة](resource-provision-new-environment.md) لإكمال النشر. استخدم نوع نشر [بيئة العرض التوضيحي](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) للمعاينة. 

## <a name="install-cds-setup-and-configuration-data"></a>تثبيت إعداد CDS وبيانات التكوين

قم بتثبيت إعداد CDS وبيانات التكوين كما هو موضح في الموضوع، [إعداد بيانات التكوين وتطبيقها في Common Data Service](resource-apply-pro-setup-config-data.md).
أكمل هذه الخطوة فقط بعد نشر بيئة العرض التوضيحي لـ Finance وسوف تكون بيانات العرض التوضيحي جاهزة.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
