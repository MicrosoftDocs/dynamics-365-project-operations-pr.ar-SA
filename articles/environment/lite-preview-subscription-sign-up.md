---
title: التسجيل في اشتراك معاينة - خفيف
description: يوفر هذا المقال معلومات حول كيفية الاشتراك في النشر الخفيف لـ Project Operations ونشره – التعامل مع الفواتير الأولية‬
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 29bf31cd1bc9c1c5ac757de989154b4c7acc53fe
ms.sourcegitcommit: 16c9eded66d60d4c654872ff5a0267cccae9ef0e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/07/2022
ms.locfileid: "9409970"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a>التسجيل في اشتراك معاينة - خفيف 

يشرح هذا المقال حول كيفية الاشتراك في العرض التجريبي ونشر النشر الخفيف لـ Dynamics 365 Project Operations – التعامل مع الفواتير الأولية‬

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


1. انتقل إلى مركز مسؤول [Microsoft 365 ](https://portal.office.com/) لتعيين التراخيص إلى مستخدميك.
2. في صفحة **المستخدمين النشطين**، حدد المستخدمين الذين ترغب في تعيين ترخيص لهم.
3. تحقق من تحديد ترخيص **Dynamics 365 Project Operations**. 
4. حدد **حفظ التغييرات**.

## <a name="create-a-new-dataverse-environment"></a>إنشاء بيئة Dataverse جديدة

1. قم بتزويد بيئة نشر جديدة Project Operations Dataverse باتباع الإرشادات في المقال، [ نموذج نشر Dataverse](lite-deployment.md). عند تحديد نوع البيئة، تأكد من استخدام **الإصدار التجريبي (مستند إلى اشتراك)**.

  ![بيئة جديدة.](./media/19CreateEnvironment.png)

2. حدد الإعداد **تمكين تطبيقات Dynamics 365**، واترك الخيار **نشر هذه التطبيقات تلقائيًا** فارغًا.  
3. حدد **حفظ** لإنشاء البيئة.

  ![إضافة قاعدة بيانات.](./media/20CreateEnvironment1.png)

4. بعد إنشاء البيئة، ثبّت حل **Microsoft Dynamics 365 Project Operations**. 

![تثبيت الحل.](./media/21InstallSolution.png)

## <a name="set-up-demo-data"></a>إعداد بيانات عرض توضيحي

قم بإعداد بيانات تجريبية من خلال اتباع الإرشادات الواردة في المقالة [، تطبيق اعداد العرض التوضيحي وبيانات التكوين‬](lite-apply-demo-setup-config-data.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
