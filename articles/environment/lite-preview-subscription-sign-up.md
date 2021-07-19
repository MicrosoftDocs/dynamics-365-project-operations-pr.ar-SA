---
title: التسجيل في اشتراك معاينة - خفيف
description: يقدم هذا الموضوع معلومات حول كيفية الاشتراك في Project Operations Lite – التعامل مع الفواتير الأولية‬ ونشره.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2b5a65f5e29915c349d40400ebbf3e4923b36a67
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334766"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a>التسجيل في اشتراك معاينة - خفيف 

يوضح هذا الموضوع كيفية الاشتراك في العرض التجريبي ونشر إصدار النشر الخفيف لـ Dynamics 365 Project Operations- التعامل مع الفواتير الأولية‬.

> [!NOTE]
> ستتغير هذه العملية في الإصدارات القادمة من Project Operations.

## <a name="prerequisites"></a>المتطلبات الأساسية
- يجب أن يكون لدي المستخدم الذي ينشر المعاينة حقوق المسؤول العمومي لمستأجر Azure. يمكنك إنشاء مستأجر أثناء عملية استرداد العرض الأول.

> [!IMPORTANT]
> شخص واحد فقط، مسؤول المستأجر، في مؤسسة تحتاج إلى تنفيذ هذه المهمة. إذا لم تكن أنت المشترك في هذا الإصدار، فانتظر حتى يتم تسجيل مؤسستك وتستلم بيانات اعتماد المستخدم الخاصة بك.
> 
> تستخدم الإصدارات التجريبية مرة واحدة في المستأجر. يمكنك تشغيل النسخة التجريبية مرة واحدة فقط. من المستحسن إنشاء مستأجر جديد لغرض الإصدار التجريبي.

### <a name="dynamics-365-project-operations-trial"></a>الإصدار التجريبي من Dynamics 365 Project Operations 

قبل البدء، تأكد من تسجيل الدخول إلى مستعرض باستخدام حساب عمل المستخدم في المستأجر حيث تريد معاينة Project Operations.

1. انتقل إلى [الإصدار التجريبي لـ Project Operations](https://aka.ms/try-po)من أجل استرداد رمز العرض الأول، **Dynamics 365 Project Operations**.
2. أكد طلبك.

  وسترى أنه تم استرداد عرض التأكيد بنجاح.

## <a name="assign-licenses"></a>تعيين التراخيص

> [!IMPORTANT]
> ستحتاج إلى حق وصول إداري إلى مدخل Microsoft 365 الخاص بمؤسستك لإكمال الخطوات التالية.


1. انتقل إلى [مركز إدارة](https://portal.office.com/) لتعيين التراخيص إلى المستخدمين.
2. في صفحة **المستخدمين النشطين**، حدد المستخدمين الذين ترغب في تعيين ترخيص لهم.
3. تحقق من تحديد ترخيص **Dynamics 365 Project Operations**. 
4. حدد **حفظ التغييرات**.

## <a name="create-a-new-dataverse-environment"></a>إنشاء بيئة Dataverse جديدة

1. يمكنك توفير بيئة نشر Project Operations Dataverse جديدة باتباع الإرشادات في الموضوع،  [ نموذج نشر Dataverse ](lite-deployment.md). عند تحديد نوع البيئة، تأكد من استخدام **الإصدار التجريبي (مستند إلى اشتراك)**.

  ![بيئة جديدة](./media/19CreateEnvironment.png)

2. حدد الإعداد **تمكين تطبيقات Dynamics 365**، واترك الخيار **نشر هذه التطبيقات تلقائيًا** فارغًا.  
3. حدد **حفظ** لإنشاء البيئة.

  ![إضافة قاعدة بيانات](./media/20CreateEnvironment1.png)

4. بعد إنشاء البيئة، ثبّت حل **Microsoft Dynamics 365 Project Operations**. 

![تثبيت الحل](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>تثبيت تكوين CDS وإعداد بيانات العرض التوضيحي

قم بتثبيت تكوين CDS وإعداد بيانات العرض التوضيحية باتباع الإرشادات الواردة في الموضوع، [تطبيق إعداد بيانات العرض التوضيحي وبيانات التكوين‬](lite-apply-demo-setup-config-data.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
