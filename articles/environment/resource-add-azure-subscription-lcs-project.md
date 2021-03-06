---
title: إضافة اشتراك Azure إلى مشروع LCS
description: يوفر هذا الموضوع معلومات حول كيفية توصيل اشتراك Azure الخاص بك بمشروع LCS.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0b5703542ac58adcc710890d9676dd0090a82f25
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948721"
---
# <a name="add-an-azure-subscription-to-lcs-project"></a>إضافة اشتراك Azure إلى مشروع LCS

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

يجب نشر البيئات المستضافة على السحابة باستخدام اشتراك Azure موجود. يشرح هذا الموضوع كيفية توصيل اشتراك Azure الخاص بك بمشروع LCS. 

## <a name="grant-admin-consent"></a>منح موافقة المسؤول

1. في مشروع LCS الخاص بك، في قسم **البيئات**، حدد **إعدادات Microsoft Azure**.

![إعدادات تطبيق Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. في صفحة **إعدادات المشروع**، في علامة التبويب **موصلات Azure**، حدد **تخويل**. هذا يسمح بنشر البيئات في هذا المشروع.

![موصلات Azure](./media/2AzureConnectors.png)

3. حدد **تخويل** مرة أخرى لتوفير موافقة المسؤول.

![منح موافقة المسؤول](./media/3GrantAdminConsent.png)

4. اقبل طلب الأذونات.

![قبول طلب الأذونات](./media/4AcceptPermissionRequest.png)

اكتمل التخويل الآن. 

![نجح التخويل](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a>يوفر Dynamics Deployment Services الوصول إلى اشتراك Azure

1. اذهب إلى [Microsoft Azure الفوترة](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) وحدد الاشتراك الخاص بك. تحتاج Dynamics Deployment Services إلى الوصول إلى هذا الاشتراك لكي تتمكن من نشر البيئات.

![تفاصيل اشتراك Azure](./media/6AzureSubscription.png)

2. حدد **الوصول للتحكم (IAM)** في جزء التنقل، ثم حدد **إضافة تعيين دور**.
3. في شريط التمرير الموجود على الجانب الأيسر، حدد **دور المساهم**، وفي القائمة المتوفرة، ابحث عن وحدد**Dynamics Deployment Services**. 
4. حدد **حفظ**.

![الوصول إلى الاشتراك](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a>إضافة اشتراك موصل إلى مشروع LCS

1. في مشروع LCS الخاص بك، في صفحة **إعدادات Microsoft Azure**، حدد **إضافة** لإضافة موصل جديد.
2. أدخل معرف اشتراك Azure الخاص بك. يمكنك العثور على معرف اشتراك Azure في [مدخل Azure](https://ms.portal.azure.com/)، أسفل **الإعدادات** في الجزء السفلي الأيمن من الشاشة.
3. في حقل **التكوين لاستخدام Azure Resource Manager**، حدد **نعم**.
4. تأكد من أن مجال مستأحر AAD الخاص باشتراك Azure يطابق المجال الذي يمتلك اشتراك Azure الذي تستخدمه، وحدد **التالي**.
5. في شاشة **إعداد Microsoft Azure**، حدد **التالي** للتأكيد. إذا تلقيت خطأ في هذه الشاشة، فقم بالرجوع إلى القسم [توفير وصول Dynamics Deployment Services إلى اشتراك Azure](#provide) في هذه الموضوع وتأكد من إتمام كافة الخطوات.
6. قم بتنزيل شهادة إدارة Azure إلى مجلد محلي على جهاز الكمبيوتر الخاص بك ثم قم بتحميلها إلى مدخل إدارة Azure بالانتقال إلى **الإعدادات** > **إدارة الشهادات**. ستعمل هذه الشهادة على تمكين LCS من الاتصال مع Azure نيابة عنك. يمكنك تخطي هذه الخطوة إذا كان المستخدم لديه حق الوصول إلى الاشتراك.
7. حدد **التالي**.
8. حدد منطقه Azure التي سيتم النشر فيها وحدد مركز بيانات قريب من المكان الذي تخطط لاستخدام هذا النظام فيه.
9.  حدد **اتصال**.

لقد قمت بالاتصال بنجاح باشتراك Azure. يمكنك الآن نشر بيئات Dynamics 365 Finance المستضافة على السحابة.


