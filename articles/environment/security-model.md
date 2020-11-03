---
title: نموذج الأمان
description: يوفر هذا الموضوع معلومات حول نموذج الأمان في Dynamics 365 Project operations.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e875d1765b5038e60830d626abb5bcd61749ece1
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070529"
---
# <a name="security-model"></a>نموذج الأمان

_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_

يحتوي Microsoft Dynamics 365 Project Operations على نموذج أمان فريد يسمح لنموذج أمان الأعمال المعتمد على الدور والذي يتعاون مع مجموعات Microsoft Office. 


## <a name="security-roles"></a>أدوار الأمان
تشمل إمكانات الواجهة الأمامية في Project Operations الأدوار التالية:

| الدور                          | ‏‏الوصف                                                                                                                                                                 | Scope |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| مدير الممارسة              | يدعم رفع التقارير عبر المشاريع.                                                                                                            | وحدة العمل              |
| الموافق على المشروع              | يوافق على الوقت والمصروفات مقابل أحد المشاريع.                                                                                                                              | وحدة العمل |
| مسؤول فوترة المشروع | ينشئ مقترح الفاتورة.                                                                                                                                                 | وحدة العمل |
| مدير المشروع               | يقوم بإنشاء خطة المشروع ويطلب الموارد.                                                                                                                              | وحدة العمل |
| مورد المشروع              | أعضاء الفريق الذين يمكن حجزهم ووقت التقرير.                                                                                                          | وحدة العمل|
| مدير الموارد              | تكون كافة وظائف إدارة الموارد، مثل استيفاء طلبات الموارد والحجوزات، مفصولة لدعم تكوين مدير مشروع مختلط + مدير الموارد ودعم دور مدير موارد واحد ومركزي. | وحدة العمل |


يتضمن Microsoft Project للويب الأدوار التالية:

| الدور           | ‏‏الوصف                                                                                                        | Scope  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| مستخدم المشروع   | المستخدم التعاوني للمشروع الذي يمكنه إنشاء المشروعات الخاصة به وعرض أية مشاريع مشتركة معه. | المستخدم   |
| نظام المشروع | الدور المستخدم لسياق التطبيق. لا ينبغي أن يستخدم العملاء دور النظام هذا.                                    | عمومي |

## <a name="security-enforcement"></a>فرض الأمان
الإجراءات التي يتم تنفيذها على مستوي المشروع يتم تنفيذها في سياق المستخدم الذي قام بتسجيل الدخول. وهذا يعني أنه لإنشاء مشروع أو فتحه أو حذفه، سيكون المستخدم مطالبا بتوفر حق الوصول له إلى CDS. قد يتم منح الوصول إلى CDS من خلال أي من الأليات المحتملة المضمنة في النظام الأساسي. على سبيل المثال، قد يصل مستخدم ذو نطاق أكبر إلى المشروع أو تم تنفيذ إجراء مشاركة مشروع واضح والذي يمنح الوصول للمستخدم.

من المهم وضع ذلك في الاعتبار عند إنشاء المشروعات في Project Operations.

## <a name="modern-group-collaboration-with-project-operations"></a>تعاون المجموعة الحديثة باستخدام Project Operations
يدعم تطبيق Project for the Web و Project Operations المجموعات الحديثة للتعاون. يمكن للمستخدمين الذين تتم إضافتهم إلى المشروع من خلال مجموعة تحرير خطة المشروع.

يضيف Project for the Web المستخدمين إلى المجموعة تلقائيًا عند التعيين.

تسمح المجموعات لأذونات المشروع وتدعم العمل على البيانات الاصطناعية للتعاون بشكل تعاوني. يصف المخطط التالي الأحداث وتغييرات الحالة التي تحدث أثناء عملية تعيين المجموعة.

لا يقوم Project Operations بإنشاء مجموعة من خلال إجراء ضمني وإنما يقوم بذلك من خلال الإجراء الصريح للمجموعات الضاغطة.

يقتصر بحث أعضاء المجموعة في مربع الحوار **إدارة المجموعات** على هؤلاء الذين تم تعيينهم كجزء من مجموعة أمان البيئة. لمزيد من المعلومات، راجع [التحكم في وصول المستخدم إلى البيئات: مجموعات الأمان والتراخيص](https://docs.microsoft.com/power-platform/admin/control-user-access).

![وضع المجموعة](./media/groupsmode.png)

1. يتم إنشاء المشروع وامتلاكه بواسطة المستخدم الذي قام بالإنشاء.
2. يتم تحديث مالك المشروع إلى الفريق.
3. تم تعيين الفريق المالك إلى مجموعة Office المحددة أو التي تم إنشاؤها.
4. تتم إضافة المالك الأصلي للمشروع إلى مجموعة Office.

## <a name="deployment-recommendation"></a>توصيات التوزيع
مع تطوير نموذج تعاون مجموعة Office، ستتم إضافة الوظائف لتوفير مزيد من التحكم المفصل بمرور الوقت. سيتم تشجيع العملاء الذين يقومون بنشر Project Operations اليوم على التركيز على نموذج أمان Microsoft Dynamics 365 التقليدي.

لمزيد من المعلومات، انظر [الأمان في Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a>أمان Project Operations وMicrosoft Dynamics 365 Finance
يشمل Project Operations الأدوار التالية:

- مدير المشروع
- محاسب المشروع

للحصول على مزيد من المعلومات حول الأمان في Finance، راجع [الأمان المستند إلى الدور](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).

