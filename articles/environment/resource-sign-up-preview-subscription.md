---
title: إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة
description: يوفر هذا الموضوع معلومات حول كيفية الاشتراك في Project Operations ونشرها للسيناريوهات المستندة إلى المورد/المنتجات غير المخزنة.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4d35a8bf9e8a841b45808b26ae2587c5b7d99d72
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948722"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>إعداد اشتراكات معاينة Project Operations لسيناريوهات المورد/المنتجات غير المخزنة

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يشرح هذا الموضوع كيفية الاشتراك في المعاينة/عرض الشريك ونشر بيئة Project Operations للسيناريوهات المستندة إلى مورد/منتجات غير مخزنة.

## <a name="prerequisites"></a>المتطلبات الأساسية

- ستتلقى رسالة بريد إلكتروني لدعوتك للمشاركة في المعاينة. يمكنك طلب معاينة من [موقع الويب الخاص بـ Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- يجب أن يكون لدي المستخدم الذي ينشر المعاينة حقوق المسؤول العمومي لمستأجر Azure.
- يتطلب نشر بيئة Finance وجود اشتراك Azure صالح والذي ستتم فوترته لكل بيئة. يمكنك استخدام الاشتراك الموجود في المؤسسات أو استخدام [الإصدار التجريبي من Azure](https://azure.microsoft.com/en-us/free/) لبدء العمل. سيتم توفير بيئة CDS مجانًا لفترة زمنية محددة بمدة 30 يومًا.

## <a name="subscribe"></a>الاشتراك

عند اعتماد [طلب المعاينة](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) الخاص بك، ستتلقى عرضين من Microsoft بواسطة البريد الإلكتروني. تسمح لك هذه العروض بنشر معاينة Project Operations:

- Dynamics 365 Project Operations – إصدار تجريبي للمعاينة
- إصدار تجريبي لمعاينة Dynamics 365 for Finance and Operations.

> [!IMPORTANT]
> شخص واحد فقط، مسؤول المستأجر، في مؤسسة تحتاج إلى تنفيذ هذه المهمة. إذا لم تكن أنت المشترك في هذا الإصدار، فانتظر حتى يتم تسجيل مؤسستك وتستلم بيانات اعتماد المستخدم الخاصة بك.

### <a name="dynamics-365-project-operations--preview-trial"></a>Dynamics 365 Project Operations – إصدار تجريبي للمعاينة

1. استرد العرض الأول، **الإصدار التجريبي من Dynamics 365 Project Operations** باستخدام عنوان URL المضمن في البريد الإلكتروني الترحيبي.

![العرض الأول](./media/1FirstOffer.png)

2. تحقق من أنك قمت بتسجيل الدخول باسم المستخدم الذي ينتمي إلى المؤسسة التي ستقوم بالاشتراك في الخدمة.
3. تابع عملية استرداد العرض. 
4. حدد **نعم، أضفه إلى حسابي**.

![استرداد العرض](./media/2RedeemFirstOffer.png)

![تأكيد العرض](./media/3ConfirmFirstOffer.png)

![تم استرداد العرض](./media/4OfferSuccessfulyRedeemed.png)

### <a name="dynamics-365-finance-preview-trial"></a>إصدار تجريبي لمعاينة Dynamics 365 Finance

كرر نفس الخطوات مع العرض الثاني من البريد الإلكتروني الترحيبي.

## <a name="assign-licenses"></a>تعيين التراخيص

> [!IMPORTANT]
> ستحتاج إلى حق وصول إداري إلى مدخل Office 365 الخاص بمؤسستك لإكمال الخطوات التالية.

1. انتقل إلى [مركز إدارة Microsoft 365](https://portal.office.com/) لتعيين التراخيص إلى المستخدمين.

![مدخل مسؤول Office](./media/5OfficeAdminPortal.png)

2. في صفحة **المستخدمين النشطين**، حدد المستخدمين الذين ترغب في تعيين ترخيص لهم.

![تعيين التراخيص](./media/6AssignLicenses.png)

3. تحقق من تحديد ترخيص Project Operations وحدد **حفظ التغييرات**. 

> [!NOTE]
> لا يلزم تعيين مستخدم إلى عرض الإصدار التجريبي من Finance.

## <a name="start-a-new-project-in-lcs"></a>بدء مشروع جديد في LCS

قم بإنشاء مشروع LCS جديد كما هو موضح في موضوع، [بدء مشروع جديد في LCS](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>إضافة اشتراك Azure إلى مشروع LCS

لإكمال هذه المهمة، اتبع الخطوات الواردة في الموضوع، [إضافة اشتراك Azure إلى مشروع LCS](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>نشر بيئة عرض توضيحي من Finance مع Project Operations لسيناريوهات المورد/المنتجات غير المخزنة

اتبع الإرشادات الموضحة في موضوع، [توفير بيئة جديدة](resource-provision-new-environment.md) لإكمال النشر. استخدم نوع نشر [بيئة العرض التوضيحي](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) للمعاينة.

## <a name="install-cds-setup-and-configuration-data"></a>تثبيت إعداد CDS وبيانات التكوين

قم بتثبيت إعداد CDS وبيانات التكوين كما هو موضح في الموضوع، [إعداد بيانات التكوين وتطبيقها في Common Data Service](resource-apply-pro-setup-config-data.md).

