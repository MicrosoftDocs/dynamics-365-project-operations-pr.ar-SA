---
title: نسخ مشروع
description: يقدم هذا الموضوع معلومات حول نسخ المشاريع في Dynamics 365 Project Operations.
author: ruhercul
ms.date: 03/07/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: e9b637d2d282d123dfacb8a295292ea06549aa1e
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8574414"
---
# <a name="copy-a-project"></a>نسخ مشروع

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

باستخدام Dynamics 365 Project Operations، يمكنك إنشاء مشاريع جديدة بسرعة من خلال تحديد **نسخ المشروع** على نموذج **المشاريع**. لنسخ مشروع، افتح المشروع الذي تريد نسخه، ثم حدد **نسخ المشروع**. سينسخ الإجراء ما يلي:

- خصائص المشروع 
- هيكل تنظيم العمل
- أعضاء فريق المشروع
- تقديرات المشروع
- تقديرات مصروفات المشاريع
- تقديرات مواد المشروع
- قوائم اختيار المشروع
- مستودعات المشروع

## <a name="project-properties"></a>خصائص المشروع

عند نسخ المشروع، يتم نسخ القيم الموجودة في الحقول التالية.

| الحقل | مواد Project Operations غير المخزنة | Project Operations Lite | Project for the Web |
|-------|------------------------------------------|-------------------------|---------------------|
| Name | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| الوصف  | :heavy_check_mark: | :heavy_check_mark: | |
| العميل  | :heavy_check_mark: | :heavy_check_mark: | |
| قالب التقويم | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| ‏‏العملة | :heavy_check_mark: | :heavy_check_mark: | |
| الوحدة المتعاقدة | :heavy_check_mark: | :heavy_check_mark: | |
| الشركة المالكة | :heavy_check_mark: | | |
| مدير المشروع | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| الحالة  | :heavy_check_mark: | :heavy_check_mark: | |
| الحالة الإجمالية للمشروع | :heavy_check_mark: | :heavy_check_mark: | |
| تعليقات | :heavy_check_mark: | :heavy_check_mark: | |
| التقديرات | :heavy_check_mark: | :heavy_check_mark: | |
| <p>تاريخ البدء المقدر</p><p><strong>ملاحظة:</strong> يحدد هذا الحقل تاريخ إنشاء المشروع من النسخة. | :heavy_check_mark: | :heavy_check_mark: | |
| <p>تاريخ الانتهاء المقدر</p><p><strong>ملاحظة:</strong> يتم تعديل التاريخ في هذا الحقل بناءً على تاريخ بدء المشروع الجديد الذي تم إنشاؤه من النسخة.</p> | :heavy_check_mark: | :heavy_check_mark: | |
| الجهد (بالساعات) | :heavy_check_mark: | :heavy_check_mark: | |
| تكلفة العمالة المقدّرة | :heavy_check_mark: | :heavy_check_mark: | |
| تكلفة المصروفات المقدّرة | :heavy_check_mark: | :heavy_check_mark: | |
| تكلفة المواد المقدّرة | | :heavy_check_mark: | |

> [!NOTE]
> تُعد عملية نسخ المشروع عملية تشغيل طويلة. يتم أيضًا نسخ سجلات المشروع وسماته ذات الصلة والعديد من الكيانات المرتبطة. نظرًا لطبيعة التشغيل الطويلة للعملية، بعد بدء النسخ، يتم تأمين صفحة المشروع الهدف للتحرير حتى تكتمل عملية النسخ.

## <a name="work-breakdown-structure"></a>هيكل تنظيم العمل

عند نسخ المشروع، يتم نسخ هيكل تنظيم العمل المحمّل بالكامل للمورد. تم استبدال الموارد المسماة بالموارد العامة. إذا كانت الموارد المسماة لا تحتوي على نفس ساعات العمل مثل المورد العام، فستتم إعادة حساب الجدول، وقد تتغير مدد المهام.

## <a name="project-team-members"></a>أعضاء فريق المشروع

عندما يتم نسخ فريق مشروع من المشروع المصدر، يتم نسخ الموارد العامة. يتم أيضًا الاحتفاظ بتعيينات الموارد العامة كما كانت في المشروع المصدر. سيتم تحويل الموارد المسامة إلى أعضاء فريق عام.

> [!NOTE]
> لا يتم نسخ أعضاء الفريق والتعيينات في Project for the Web.

## <a name="estimates"></a>التقديرات

وعند نسخ المشروع، يتم نسخ بنود الموارد والمصروفات وتقديرات المواد من المشروع المصدر. 

للحصول على معلومات حول كيفية الوصول إلى "نسخ المشروع" برمجيًا، راجع [تطوير قوالب المشروع مع نسخ المشروع‬‬](dev-copy-project.md).

## <a name="quotes-and-contracts"></a>عروض الأسعار والعقود

عروض الأسعار والعقود غير مرتبطة بالمشروع الوجهة.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
