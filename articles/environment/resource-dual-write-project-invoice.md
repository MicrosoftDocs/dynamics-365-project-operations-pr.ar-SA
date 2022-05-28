---
title: تكامل فاتورة المشروع
description: يوفر هذا موضوع معلومات حول تكامل الكتابة المزدوجة في Project Operations لفوترة العملاء.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 1e7294360f041b030efca225c6754fe3bbc0eadf
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581222"
---
# <a name="project-invoice-integration"></a>تكامل فاتورة المشروع

يوفر هذا موضوع معلومات حول تكامل الكتابة المزدوجة في Project Operations لفوترة العملاء.

في Project Operations، يدير مدير المشروع تراكم الفاتورة وينشئ فاتورة أولية للعميل في Microsoft Dataverse. وبناء على هذه الفاتورة الأولية، يقوم موظف حسابات المقبوضات أو محاسب المشروع بإنشاء فاتورة مواجهة للعميل. يضمن تكامل الكتابة المزدوجة مزامنة تفاصيل الفاتورة الأولية مع تطبيقات Finance and Operations. وبعد ترحيل الفاتورة المواجهة للعميل، يقوم النظام بتحديث القيم الفعلية للمشروع ذات الصلة في Dataverse بتفاصيل المحاسبة. يوفر الرسم التالي نظرة عامة تصورية رفيعة المستوى لهذا التكامل.

   ![تكامل فاتورة المشروع.](./media/DW5Invoicing.png)

بعد أن يؤكد مدير المشروع الفاتورة الأولية في Dataverse، يتم مزامنة معلومات رأس الفاتورة الأولية لتطبيقات Finance and Operations باستخدام مخطط جدول الكتابة المزدوجة، **اقتراح فاتورة المشروع V2 (الفواتير)**. وهذا هو تكامل من جانب واحد من Dataverse إلى تطبيقات Finance and Operations. لا يتم دعم إنشاء مقترحات فاتورة المشروع أو حذفها مباشرةً في تطبيقات Finance and Operations.

كما يؤدي تأكيد الفاتورة في Dataverse أيضا إلى إطلاق منطق الأعمال لإنشاء سجلات متعلقة بالفوترة في كيان **القيم الفعلية**. تتم مزامنة هذه السجلات مع Finance and Operations باستخدام خريطة جدول الكتابة المزدوجة، **القيم الفعلية لتكامل Project Operations ‏(msdynactuals\_).** للحصول على مزيد من المعلومات، راجع [تقديرات المشروع والقيم الفعلية](resource-dual-write-estimates-actuals.md). 

يتم إنشاء بنود عرض فاتورة المشروع بواسطة العملية الدورية، **مراحل استيراد النموذج**. تعتمد هذه العملية على تفاصيل القيم الفعلية للمبيعات التي تمت فوترتها في جدول **مراحل القيمة الفعلية**. لمزيد من المعلومات، راجع [إدارة مقترحات فواتير المشروع](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
