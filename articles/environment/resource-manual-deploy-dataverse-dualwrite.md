---
title: نشر تطبيق Project Operations Dataverse يدويًا مع دعم الكتابة المزدوجة
description: يوضح هذا الموضوع كيفية نشر تطبيق Project Operations Dataverse يدويًا بحيث يدعم الكتابة المزدوجة.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 06325a9a9f9084d1f506f2493c32565fe7b7c52ae6fe22c81339b9c1d632e688
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986430"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a>نشر تطبيق Project Operations Dataverse يدويًا مع دعم الكتابة المزدوجة

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يوضح هذا الموضوع كيفية نشر Microsoft Dynamics 365 Project Operations يدويًا في Microsoft Dataverse بحيث يدعم الكتابة المزدوجة. تكتشف Project Operations تكوين البيئة وتضيف دعمًا إضافيًا للكتابة المزدوجة إذا تم استيفاء المتطلبات الأساسية.

أثناء النشر من خلال Microsoft Dynamics Lifecycle Services (LCS)، إذا اتبعت الإرشادات الواردة في هذا الموضوع، فيمكنك تخطي نشر تكامل Microsoft Power Platform (المعروف سابقًا باسم بيئة Common Data Service).

عملية نشر Project Operations في Dataverse بحيث تدعم الكتابة المزدوجة‬ ويكون لها أربع خطوات رئيسية:

1. [إنشاء بيئة جديدة في Dataverse تدعم الكتابة المزدوجة](#create).
2. [إضافة المتطلبات المسبقة للكتابة المزدوجة إلى البيئة](#prerequisites).
3. [أضف تطبيق Project Operations Dataverse ](#dataverse).
4. [ربط بيئتك](#link).

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a>إنشاء بيئة جديدة في Dataverse تدعم الكتابة المزدوجة

لإكمال هذا الإجراء، يتعين عليك تسجيل الدخول كمسؤول.

1. افتح مركز الإدارة [Power Platform ](https://admin.powerplatform.com)، ثم قم بتسجيل الدخول كمسؤول.
2. إنشاء بيئة جديدة، وتسميتها.
3. حدد نوع البيئة. إذا قمت بالاشتراك في العرض التجريبي، فحدد **"تجريبي" (مستند إلى الاشتراك)**.
4. تأكيد منطقة النشر.
5. تمكين خيار **إنشاء قاعدة بيانات لهذه البيئة**. 
6. تأكد من اللغة، ثم تأكد من تطابق العملة مع العملة الخاصة بتطبيقات Finance and Operations الخاصة بك.
7. تمكين الخيار **تطبيقات Dynamics 365** وتأكد من تعيين الحقل **النشر التلقائي لهذه التطبيقات** على **بلا**.
8. قم بإضافة مجموعة أمان، إذا كانت مجموعة الأمان مطلوبة.
9. حدد **حفظ** لإنشاء البيئة.
10. انتظر حتى تكتمل عملية النشر حتى تصل البيئة إلى حالة **الجاهزية**.

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a>إضافة المتطلبات المسبقة للكتابة المزدوجة إلى البيئة

يتضمن دعم الكتابة المزدوجة الحقول الإضافية التي تمت إضافتها إلى الكيانات الرئيسية، مثل كيان **الشركة**. إذا كنت تقوم بإضافة دعم الكتابة المزدوجة إلى بيئة موجودة، فقد تضطر إلى تحديث البيانات لتمكين الدعم. لمزيد من المعلومات حول كيفية تمهيد البيانات، راجع [تمهيد بيانات شركة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data) لمزيد من المعلومات حول الكتابة المزدوجة، راجع [متطلبات نظام الكتابة المزدوجة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req)

أكمل هذا الإجراء لإضافة متطلبات الكتابة المزدوجة إلى بيئتك.

1. افتح البيئة التي أنشأتها للتو، ثم انتقل إلى **مورد** \> **تطبيقات Dynamics 365**.
2. حدد **الحل الأساسي للكتابة المزدوجة** في قائمة التطبيق، ثم قم بتثبيته.
3. انتظر حتى تكتمل عملية التثبيت. ثم حدد **حل تزامن تطبيق الكتابة المزدوجة** في قائمة التطبيقات، وقم بتثبيته.

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a>إضافة تطبيق Project Operations Dataverse.

لا يمكنك إكمال هذا الإجراء إلا إذا أكملت الإجراءات السابقة قبل تثبيت Project Operations. أثناء التثبيت، يقوم النظام بتحليل تكوين البيئة وإضافة دعم للكتابة المزدوجة في حالة الحاجة إلى ذلك.

1. افتح البيئة التي أنشأتها سابقًا، ثم انتقل إلى **مورد** \> **تطبيقات Dynamics 365**.
2. حدد **Microsoft Dynamics 365 Project Operations** في قائمة التطبيق، ثم قم بتثبيتها.

## <a name="link-your-environments"></a><a name="link"></a>ربط بيئاتك

بعد نشر بيئة Dataverse، يمكنك إعداد الارتباط في تطبيقات Finance and Operations الخاصة بك. اتبع الخطوات المتبعة في [استخدام معالج الكتابة المزدوجة لربط بيئاتك](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).
