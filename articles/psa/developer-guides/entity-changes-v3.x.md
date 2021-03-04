---
title: تغييرات الكيانات وعناصر التحكم وواجهة المستخدم (Project Service Automation 3.x)
description: يوضح هذا الموضوع التغييرات التي تم اجراؤها علي الحل لـ Microsoft Dynamics Project Service Automation 3.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/15/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 48062eda1f524dd3ca0d5feccf11fd5577521275
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148717"
---
# <a name="entity-control-and-user-interface-changes-project-service-automation-3x"></a>تغييرات الكيانات وعناصر التحكم وواجهة المستخدم (Project Service Automation 3.x)

[!include [banner](../../includes/psa-now-project-operations.md)]


مع الإصار الجديد من Microsoft Dynamics Project Service Automation (PSA) 3.x، تم إجراء من التغييرات على الكيانات، وعناصر التحكم، وطرق العرض، وواجهة المستخدم. يوفر هذا الموضوع معلومات حول هذه التغيرات المهمة:

## <a name="parent-child-relationships-for-sales-document-sales-document-line-sales-document-line-detail-entities"></a>علاقات الأصل-التابع لمستند المبيعات ،وسطر مستند المبيعات، والكيانات التفصيلية لسطر مستندات المبيعات
في إصدارات Dynamics 365 Project Service Automation (PSA) التي تم إصدارها قبل الإصدار 3.0، كان يتم تطبيق بعض العلاقات بين مستندات المبيعات وسطور مستندات المبيعات والكيانات التفصيلية لسطور مستندات المبيعات من خلال حقول السلسلة التي قد تحتفظ بتمثيل سلسلة للمعرف الفريد العمومي للكيان المرتبط. ويرجع السبب في ذلك إلى تقييدات النظام الأساسي التي تتطلب تعليمة برمجية مهمة على الخادم وعلى جوانب العميل بالحل لكي تعمل هذه العلاقات بشكل مماثل لكيان Dynamics CRM النموذجي ولجعل حقول السلسلة تعمل كحقول البحث.

تم تحديث PSA 3.0 للاستفادة من علاقات الكيانات الجديدة بين مستندات المبيعات وكيانات سطور مستندات المبيعات.

ولأنه يمكن استخدام حقول البحث الآن للإشارة إلى الكيانات، فإن الحقول التي تتضمن قيمة السلسلة الخاصة بالمعرف الفريد العمومي للكيان المرتبط في الإصدارات السابقة لم تعد مطلوبة والتالي أصبحت مهملة. كما تم الآن إهمال التعليمة البرمجية للعميل المخصص وبجانب الخادم التي تعالج العلاقات المحددة بواسطة حقول السلسلة القديمة.

### <a name="entity-schema-changes"></a>تغييرات مخطط الكيانات
يقدم الجدول التالي قائمة واحد إلى واحد لحقول السلسلة المهملة وحقول البحث الجديدة الخاصة بالكيانات. 

 الكيان |   الحقل المهمل (سلسلة) | الحقل الجديد (بحث)
--- | --- | ---
invoicedetail (سطر الفاتورة) |  msdyn_contractline |    msdyn_contractlineid
msdyn_actual (الفعلي) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_contractlineinvoiceschedule (جدول فاتورة شرط التعاقد لمشروع) |    msdyn_contractline |    msdyn_contractlineid
msdyn_contractlinescheduleofvalue (حدث رئيسي لشرط تعاقد المشروع) |   msdyn_contractline |    msdyn_contractlineid
msdyn_fact (الحقيقة) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_invoicelinetransaction (تفاصيل سطر الفاتورة) | msdyn_invoiceline <br> msdyn_salescontractline | msdyn_invoicelineid <br> msdyn_salescontractlineid
msdyn_journalline (سطر دفتر اليومية) |  msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlineresourcecategory (فئة مورد شرط التعاقد لمشروع) | msdyn_salescontractline |   msdyn_contractlineid
msdyn_orderlinetransaction (تفاصيل شرط التعاقد لمشروع) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlinetransactioncategory (فئة الحركة لشرط التعاقد لمشروع) |   msdyn_contractline |    msdyn_contractlineid
msdyn_orderlinetransactionclassification (تصنيف الحركة لشرط التعاقد لمشروع) |   msdyn_contractline |    msdyn_contractlineid
msdyn_quotelineinvoiceschedule (جدول فاتورة بند عرض الأسعار) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelineresourcecategory (فئة مورد بند عرض الأسعار) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinescheduleofvalue (حدث رئيسي لبند عرض الأسعار) | msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransaction (تفاصيل بند عرض الأسعار) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactioncategory (فئة حركة بند عرض الأسعار) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactionclassification (فئة حركة بند عرض الأسعار) |  msdyn_quoteline |   msdyn_quotelineid
SalesOrderDetail (سطر الأمر) | msdyn_quotelineid | msdyn_quoteline 

### <a name="deprecated-custom-views-and-controls"></a>طرق العرض وعناصر التحكم المخصصة المهملة
تم إهمال طرق العرض وعناصر التحكم المخصصة التالية والبيانات الاصطناعية ذات الصلة الخاصة بها.

- طريقة عرض الخضوع للرسوم
- عناصر تحكم الشبكة المخصصة لعرض تفاصيل بند عرض الأسعار في صفحة **معلومات المشروع** لبند عرض الأسعار.
- عناصر تحكم الشبكة المخصصة لعرض تفاصيل شرط التعاقد للمشروع في صفحة **معلومات المشروع** لبند أمر المبيعات.

> [!NOTE]
> للحصول على قائمة كاملة بالموارد المهمة، راجع [موارد الويب المهملة في Project Service Automation v3.x](../developer-guides/web-resources-deprecated-v3.x.md)

## <a name="unified-client-interface-app-module"></a>وحدة تطبيق واجهة العميل الموحدة
مع تقديم وحدات تطبيق واجهة العميل الموحدة (UCI) ، تكون إدخالات مخطط موقع PSA قد تمت ازالتها من النظام.  
تم إهمال الوظيفة المرتبطة بتبديل النموذج الخاص بالفرصة وعرض الأسعار والأمر والفاتورة نظرا لأنها لم تعد مطلوبة لأن وحدة تطبيق UCI تتضمن إصدارات PSA فقط من النماذج.  

تم إهمال موارد الويب التالية:

- msdyn_\SalesDocument\SalesDocumentFormLoader.js
- msdyn_\SalesDocument\PSSalesDocumentCustomFormIds.js

> [!NOTE]
> للحصول على قائمة كاملة بالموارد المهمة، راجع [موارد الويب المهملة في Project Service Automation v3.x](../developer-guides/web-resources-deprecated-v3.x.md).




[!INCLUDE[footer-include](../../includes/footer-banner.md)]