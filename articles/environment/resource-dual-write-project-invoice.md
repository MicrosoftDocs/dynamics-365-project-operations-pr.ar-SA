---
title: تكامل فاتورة المشروع
description: يوفر هذا موضوع معلومات حول تكامل الكتابة المزدوجة في Project Operations لفوترة العملاء.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 37549080d76e3bffd7cb002aee8e3c46b9eeb18e3cec915cd971881b69747534
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2021
ms.locfileid: "6993225"
---
# <a name="project-invoice-integration"></a>تكامل فاتورة المشروع

يوفر هذا موضوع معلومات حول تكامل الكتابة المزدوجة في Project Operations لفوترة العملاء.

في Project Operations، يدير مدير المشروع تراكم الفاتورة وينشئ فاتورة أولية للعميل في Microsoft Dataverse. وبناء على هذه الفاتورة الأولية، يقوم موظف حسابات المقبوضات أو محاسب المشروع بإنشاء فاتورة مواجهة للعميل. يضمن تكامل الكتابة التلقائية مزامنة تفاصيل الفاتورة الأولية مع تطبيقات Finance and Operations. وبعد ترحيل الفاتورة المواجهة للعميل، يقوم النظام بتحديث القيم الفعلية للمشروع ذات الصلة في Dataverse بتفاصيل المحاسبة. يوفر الرسم التالي نظرة عامة تصورية رفيعة المستوى لهذا التكامل.

   ![تكامل فاتورة المشروع.](./media/DW5Invoicing.png)

بعد أن يؤكد مدير المشروع الفاتورة الأولية في Dataverse، يتم مزامنة معلومات رأس الفاتورة الأولية مع تطبيقات Finance and Operations باستخدام مخطط جدول الكتابة المزدوجة **اقتراح فاتورة المشروع V2 (الفواتير)**. وهذا تكامل من جانب واحد من Dataverse إلى تطبيقات Finance and Operations. لا يتم دعم إنشاء مقترحات فاتورة المشروع أو حذفها مباشرة في تطبيقات Finance and Operations.

كما يؤدي تأكيد الفاتورة في Dataverse أيضا إلى إطلاق منطق الأعمال لإنشاء سجلات متعلقة بالفوترة في كيان **القيم الفعلية**. تتم مزامنة هذه السجلات مع Finance and Operations باستخدام مخطط جدول الكتابة المزدوجة **القيم الفعلية لتكامل Project Operations (msdyn\_actuals)**. للحصول على مزيد من المعلومات، راجع [تقديرات المشروع والقيم الفعلية](resource-dual-write-estimates-actuals.md). 

يتم إنشاء بنود عرض فاتورة المشروع بواسطة العملية الدورية، **مراحل استيراد النموذج**. تعتمد هذه العملية على تفاصيل القيم الفعلية للمبيعات التي تمت فوترتها في جدول **مراحل القيمة الفعلية**. لمزيد من المعلومات، راجع [إدارة مقترحات فواتير المشروع](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
