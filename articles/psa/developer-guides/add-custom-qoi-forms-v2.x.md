---
title: إضافة نماذج كيانات مخصصة جديدة (Project Service Automation 2.x)
description: يقدم هذا الموضوع معلومات حول كيفية إضافة نماذج كيانات مخصصة للفرص أو عروض الأسعار أو أوامر الشراء أو الفواتير في Dynamics 365 Project Service Automation 2.x.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: ffc702bbe9cedb2a0cc8da8d8f58e48005950127
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2022
ms.locfileid: "8584304"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a>إضافة نماذج كيانات مخصصة جديدة (Project Service Automation 2.x)

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a>حقل النوع 

يعتمد Dynamics 365 Project Service Automation على حقل **النوع** (**msdyn\_ordertype**) لكيانات الفرصة وعرض الأسعار والطلب والفاتورة لتمييز الإصدارات **المستندة إلى العمل** لهذه الكيانات عن الإصدارات **المستندة إلى الصنف** و **المستندة إلى الخدمة**. تتم معالجة الإصدارات المستندة إلى العمل من هذه الكيانات بواسطة PSA. ويعتمد الكثير من منطق العمل على جانب العميل وعلى جانب خادم في الحل على حقل  **النوع**. بالتالي، من المهم أن تتم تهيئة الحقل بقيمة صحيحة عند إنشاء الكيانات. وقد تتسبب القيمة غير الصحيحة في حدوث سلوكيات غير صحيحة، وقد لا تعمل بعض أنواع منطق الأعمال بشكل صحيح.

## <a name="automatic-form-switching"></a>التبديل التلقائي للنماذج

لتجنب حدوث تلف محتمل في البيانات والسلوكيات غير المتوقعة الناتجة عن التهيئة غير الصحيحة وتحرير سجلات كيان المبيعات، يشتمل PSA الآن على منطق للتبديل التلقائي للنموذج في النماذج الجاهزة. ويأخذ هذا المنطق المستخدمين إلى النموذج الصحيح للعمل مع الإصدار المستند إلى العمل أو أي نوع آخر من كيان الفرصة أو عرض الأسعار أو الأمر أو الفاتورة. عندما يقوم أحد المستخدمين بفتح الإصدار المستند إلى العمل الخاص بكيان فرصة أو عرض أسعار أو أمر شراء أو فاتورة ، يتم تبديل النموذج إلى **معلومات المشروع**.

يعتمد منطق الانتقال التلقائي للنموذج علة التعيين بين قيمة **formId** والحقل **msdyn\_ordertype**. تمت إضافة كافة النماذج الجاهزة إلى هذا التعيين. ومع ذلك، يجب إضافة النماذج المخصصة يدويا للاشارة إلى أي إصدار للكيان تم تخصيصه للمعالجة. هذا يعتمد على حقل **msdyn\_ordertype**. إذا كان تبديل النموذج مفقودا من التعيين، سيقوم المنطق بالتبديل إلى النموذج الجاهز، وذلك استنادا إلى القيمة التي يتم حفظها في الحقل **msdyn\_ordertype** للكيان.

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a>إضافة نماذج مخصصة وتشغيل منطق تبديل النموذج

يوضح المثال التالي كيفية إضافة نموذج مخصص ، **معلومات مشروعي**، بحيث يعمل مع الفرص المستندة إلى العمل. يتم استخدام نفس العملية لإضافة نماذج مخصصة بحيث تعمل مع عروض الأسعار وأوامر الشراء والفواتير.

اتبع هذه الخطوات لإنشاء إصدار مخصص من نموذج **معلومات المشروع**.

1. في كيان فرصة المبيعات، افتح نموذج **معلومات المشروع** واحفظ نسخة تحت مسمى **معلومات مشروعي**.
2. افتح النموذج الجديد، ثم في الخصائص، تأكد من وجود البرامج النصية لتهيئه النموذج من نموذج **معلومات المشروع**. 

    > [!IMPORTANT]
    > لا تقم بإزالة البرامج النصية. خلاف ذلك، قد تتم تهيئة بعض البيانات بشكل غير صحيح.

3. تحقق من وجود حقل **النوع** (**msdyn\_ordertype**) في النموذج. 

    > [!IMPORTANT]
    > لا تقم بإزالة هذا الحقل. خلاف ذلك، ستفشل البرامج النصية للتهيئة.

4. ابحث عن القيمة **formId** للنموذج الجديد. يمكنك استكمال هذه الخطوة بطريقتين:

    - قم بتصدير نموذج **معلومات المشروع** كجزء من حل غير مدار، ثم ابحث عن القيمة **formId** في الملف customization.xml الخاص بالحل الذي تم تصديره.
    - افتح نموذج **معلومات المشروع** في محرر النماذج، ثم ابحث عن المعرف الفريد العمومي (GUID) بجوار المعلمة **fromId** في URL، كما هو موضح في الشكل التوضيحي التالي.

    ![قيمة formId للنموذج الجديدفي URL.](media/how-to-add-custom-forms-in-v2.0.png)

5. قم بإنشاء تعيين **msdyn\_ordertype** للقيمة **formId** من خلال تحرير مورد الويب msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js. قم بإزالة التعليمات البرمجية من المورد واستبدله بالتعليمات البرمجية التالية.

    ```javascript
    define(["require", "exports"], function (require, exports) {
        "use strict";
        var SalesDocumentCustomFormIds = (function () {
            function SalesDocumentCustomFormIds() {
            }
            SalesDocumentCustomFormIds.overwriteFormIds = function (mappedFormIds) {
                /*
                ---- Notes ----
                mappedFormIds[SalesEntity][OrderType] => The array of forms IDs that support particular entity and order type
                Add or overwrite customized formId for the particular entity and order type by calling:
                    mappedFormIds[<EntityType>][<msdyn_ordertype>].push("<formId>");
                Allowed msdyn_ordertype values for reference:
                    ServiceBased: 690970002 (Field Service version of the entity)
                    WorkBased: 192350001 (PSA version of the entity)
                    ItemBased: 192350000 (Regular out of the box entity)
                Uncomment and update one of the following lines to register custom PSA form for required entity:
                */      
                //mappedFormIds[1][192350001].push("<formId>"); //Quote
                //mappedFormIds[5][192350001].push("<formId>"); //Quote Line
                //mappedFormIds[2][192350001].push("<formId>"); //Sales Order
                //mappedFormIds[6][192350001].push("<formId>"); //Sales Order Line
                // In this example we have added new form for Opportunity
                mappedFormIds[0][192350001].push("192EE537-DCC4-45D3-B7AF-EA694B9113D2"); //Opportunity
                //mappedFormIds[4][192350001].push("<formId>"); //Opportunity Line
            };
            return SalesDocumentCustomFormIds;
        }());
        exports.default = SalesDocumentCustomFormIds;
    });
    ```

6. احفظ التخصيصات وانشرها.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
