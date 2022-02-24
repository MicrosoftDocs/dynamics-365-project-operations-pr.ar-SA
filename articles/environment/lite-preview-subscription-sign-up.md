---
title: التسجيل في اشتراك معاينة - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية الاشتراك في Project Operations Lite – التعامل مع الفواتير الأولية‬ ونشره.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6f4360b7febab57b97df0776ef9148d2a38f16a7
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175875"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a>التسجيل في اشتراك معاينة - خفيف 

يشرح هذا الموضوع كيفية الاشتراك في عرض شريك المعاينة ونشر Dynamics 365 Project Operations Lite – التعامل مع الفواتير الأولية‬.

> [!NOTE]
> ستتغير هذه العملية في الإصدارات القادمة من Project Operations.

## <a name="prerequisites"></a>المتطلبات الأساسية

- ستتلقى رسالة بريد إلكتروني لدعوتك للمشاركة في المعاينة. يمكنك طلب معاينة من [موقع الويب الخاص بـ Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- يجب أن يكون لدي المستخدم الذي ينشر المعاينة حقوق المسؤول العمومي لمستأجر Azure.
- راجع كل البنود والشروط.

## <a name="subscribe"></a>الاشتراك

عندما تتلقى الموافقة على [طلب معاينة](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u)، ستتلقى عرضين من Microsoft بواسطة البريد الإلكتروني. تسمح لك هذه العروض بنشر معاينة Project Operations:

- Dynamics 365 Project Operations (CRM) - إصدار تجريبي للمعاينة
- Office 365 Project Operations - إصدار تجريبي للمعاينة

> [!IMPORTANT]
> شخص واحد فقط، مسؤول المستأجر، في مؤسسة تحتاج إلى تنفيذ هذه المهمة. إذا لم تكن أنت المشترك في هذا الإصدار، فانتظر حتى يتم تسجيل مؤسستك وتستلم بيانات اعتماد المستخدم الخاصة بك.

### <a name="dynamics-365-project-operations-crm---preview-trial"></a>Dynamics 365 Project Operations (CRM) - إصدار تجريبي للمعاينة 

قبل البدء، تأكد من تسجيل الدخول إلى مستعرض باستخدام حساب عمل المستخدم في المستأجر حيث تريد معاينة Project Operations.

1. استرجع كود العرض الأول، **Dynamics 365 Project Operations (CRM) - الإصدار التجريبي للمعاينة** عن طريق لصقه في عنوان URL للمستعرض.

![استرداد العرض](./media/16RedeemFirstOfferNew.png)

2. أكد طلبك.
![تأكيد الأمر](./media/17ConfirmOrderNew.png)

سترى أنه تم استرجاع عرض التأكيد بنجاح.

![تأكيد](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a>Office 365 Project Operations - إصدار تجريبي للمعاينة

كرر الخطوات نفسها التي تم تنفيذها لكود العرض الأول. تأكد من إضافة كود العرض الثاني باستخدام حساب المستخدم نفسه الذي تم استخدامه مع كود العرض الأول.

## <a name="assign-licenses"></a>تعيين التراخيص

> [!IMPORTANT]
> ستحتاج إلى حق وصول إداري إلى مدخل Microsoft 365 الخاص بمؤسستك لإكمال الخطوات التالية.


1. انتقل إلى [مركز إدارة](https://portal.office.com/) لتعيين التراخيص إلى المستخدمين.

![الصفحة الرئيسية لمركز الإدارة](./media/14AdminPortal.png)

2. في صفحة **المستخدمين النشطين**، حدد المستخدمين الذين ترغب في تعيين ترخيص لهم.

![تعيين التراخيص](./media/15AssignLicenses.png)

3. تأكد من تحديد تراخيص **معاينة Dynamics 365 Project Operations (CRM)** و **Office 365 Project Operations - معاينة**. 
4. حدد **حفظ التغييرات**.

## <a name="create-a-new-cds-environment"></a>إنشاء بيئة CDS جديدة

1. يمكنك تزويد بيئة نشر Project Operations CDS جديدة باتباع الإرشادات في الموضوع، [نموذج نشر CDS](lite-deployment.md). عند تحديد نوع البيئة، تأكد من استخدام **الإصدار التجريبي (مستند إلى اشتراك)**.
![بيئة جديدة](./media/19CreateEnvironment.png)

2. حدد الإعداد **تمكين تطبيقات Dynamics 365**، واترك الخيار **نشر هذه التطبيقات تلقائيًا** فارغًا.  
3. حدد **حفظ** لإنشاء البيئة.

![إضافة قاعدة بيانات](./media/20CreateEnvironment1.png)

4. بعد إنشاء البيئة، قم بتثبيت الحل **Microsoft Dynamics 365 Project Operations**. 

![تثبيت الحل](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>تثبيت تكوين CDS وإعداد بيانات العرض التوضيحي

قم بتثبيت تكوين CDS وإعداد بيانات العرض التوضيحية باتباع الإرشادات الواردة في الموضوع، [تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين‬](lite-apply-demo-setup-config-data.md).
