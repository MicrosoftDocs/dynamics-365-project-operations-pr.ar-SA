---
title: إضافة نماذج كيانات مخصصة جديدة (Project Service Automation 2.x)
description: يقدم هذا الموضوع معلومات حول كيفية إضافة نماذج كيانات مخصصة للفرص أو عروض الأسعار أو أوامر الشراء أو الفواتير في Dynamics 365 Project Service Automation 2.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 9eb9fc5e-4c7d-466c-9362-fdb0faa30506
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
ms.openlocfilehash: 2bd955ad3eb26d31676ac4ad387baccaee913cd2
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748566"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a><span data-ttu-id="d0b1b-103">إضافة نماذج كيانات مخصصة جديدة (Project Service Automation 2.x)</span><span class="sxs-lookup"><span data-stu-id="d0b1b-103">Add new custom entity forms (Project Service Automation 2.x)</span></span>

## <a name="type-field"></a><span data-ttu-id="d0b1b-104">حقل النوع</span><span class="sxs-lookup"><span data-stu-id="d0b1b-104">Type field</span></span> 

<span data-ttu-id="d0b1b-105">يعتمد Dynamics 365 Project Service Automation على حقل **النوع** (**msdyn\_ordertype**) لكيانات الفرصة وعرض الأسعار والطلب والفاتورة لتمييز الإصدارات **المستندة إلى العمل** لهذه الكيانات عن الإصدارات **المستندة إلى الصنف** و**المستندة إلى الخدمة**.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-105">Dynamics 365 Project Service Automation relies on the **Type** (**msdyn\_ordertype**) field of the Opportunity, Quote, Order, and Invoice entities to distinguish **work-based** versions of these entities from **item-based** and **service-based** versions.</span></span> <span data-ttu-id="d0b1b-106">تتم معالجة الإصدارات المستندة إلى العمل من هذه الكيانات بواسطة PSA.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-106">Work-based versions of these entities are handled by PSA.</span></span> <span data-ttu-id="d0b1b-107">ويعتمد الكثير من منطق العمل على جانب العميل وعلى جانب خادم في الحل على حقل  **النوع**.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-107">Lots of business logic on the client side and server side of the solution depends on the **Type** field.</span></span> <span data-ttu-id="d0b1b-108">بالتالي، من المهم أن تتم تهيئة الحقل بقيمة صحيحة عند إنشاء الكيانات.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-108">Therefore, it's important that the field be initialized with a correct value when the entities are created.</span></span> <span data-ttu-id="d0b1b-109">وقد تتسبب القيمة غير الصحيحة في حدوث سلوكيات غير صحيحة، وقد لا تعمل بعض أنواع منطق الأعمال بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-109">An incorrect value can cause incorrect behaviors, and some business logic might not run correctly.</span></span>

## <a name="automatic-form-switching"></a><span data-ttu-id="d0b1b-110">التبديل التلقائي للنماذج</span><span class="sxs-lookup"><span data-stu-id="d0b1b-110">Automatic form switching</span></span>

<span data-ttu-id="d0b1b-111">لتجنب حدوث تلف محتمل في البيانات والسلوكيات غير المتوقعة الناتجة عن التهيئة غير الصحيحة وتحرير سجلات كيان المبيعات، يشتمل PSA الآن على منطق للتبديل التلقائي للنموذج في النماذج الجاهزة.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-111">To avoid potential data corruption and unexpected behaviors that are caused by incorrect initialization and editing of the sales entity records, PSA now includes logic for automatic form switching in out-of-box forms.</span></span> <span data-ttu-id="d0b1b-112">ويأخذ هذا المنطق المستخدمين إلى النموذج الصحيح للعمل مع الإصدار المستند إلى العمل أو أي نوع آخر من كيان الفرصة أو عرض الأسعار أو الأمر أو الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-112">This logic takes users to the correct form for working with the work-based version or any other type of Opportunity, Quote, Order, or Invoice entity.</span></span> <span data-ttu-id="d0b1b-113">عندما يقوم أحد المستخدمين بفتح الإصدار المستند إلى العمل الخاص بكيان فرصة أو عرض أسعار أو أمر شراء أو فاتورة ، يتم تبديل النموذج إلى **معلومات المشروع**.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-113">When a user opens the work-based version of an Opportunity, Quote, Order, or Invoice entity, the form is switched to **Project Information**.</span></span>

<span data-ttu-id="d0b1b-114">يعتمد منطق الانتقال التلقائي للنموذج علة التعيين بين قيمة **formId** والحقل **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-114">The automatic form switching logic relies on the mapping between the **formId** value and the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="d0b1b-115">تمت إضافة كافة النماذج الجاهزة إلى هذا التعيين.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-115">All out-of-box forms have been added to that mapping.</span></span> <span data-ttu-id="d0b1b-116">ومع ذلك، يجب إضافة النماذج المخصصة يدويا للاشارة إلى أي إصدار للكيان تم تخصيصه للمعالجة.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-116">However, custom forms must be manually added to indicate which version of the entity they are intended to handle.</span></span> <span data-ttu-id="d0b1b-117">هذا يعتمد على حقل **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-117">This is based on the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="d0b1b-118">إذا كان تبديل النموذج مفقودا من التعيين، سيقوم المنطق بالتبديل إلى النموذج الجاهز، وذلك استنادا إلى القيمة التي يتم حفظها في الحقل **msdyn\_ordertype** للكيان.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-118">If the form switching is missing from the mapping, logic will switch to the out-of-box form, based on the value that is saved in the **msdyn\_ordertype** field of the entity.</span></span>

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a><span data-ttu-id="d0b1b-119">إضافة نماذج مخصصة وتشغيل منطق تبديل النموذج</span><span class="sxs-lookup"><span data-stu-id="d0b1b-119">Add custom forms and turn on the form switching logic</span></span>

<span data-ttu-id="d0b1b-120">يوضح المثال التالي كيفية إضافة نموذج مخصص ، **معلومات مشروعي**، بحيث يعمل مع الفرص المستندة إلى العمل.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-120">The following example shows how to add a custom form, **My Project Information**, so that it works with work-based opportunities.</span></span> <span data-ttu-id="d0b1b-121">يتم استخدام نفس العملية لإضافة نماذج مخصصة بحيث تعمل مع عروض الأسعار وأوامر الشراء والفواتير.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-121">The same process is used to add custom forms so that they work with quotes, orders, and invoices.</span></span>

<span data-ttu-id="d0b1b-122">اتبع هذه الخطوات لإنشاء إصدار مخصص من نموذج **معلومات المشروع**.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-122">Follow these steps to create a custom version of the **Project Information** form.</span></span>

1. <span data-ttu-id="d0b1b-123">في كيان فرصة المبيعات، افتح نموذج **معلومات المشروع** واحفظ نسخة تحت مسمى **معلومات مشروعي**.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-123">In the Opportunity entity, open the **Project Information** form, and save a copy under the name **My Project Information**.</span></span>
2. <span data-ttu-id="d0b1b-124">افتح النموذج الجديد، ثم في الخصائص، تأكد من وجود البرامج النصية لتهيئه النموذج من نموذج **معلومات المشروع**.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-124">Open the new form, and then, in the properties, make sure that the form initialization scripts from the **Project Information** form are present.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="d0b1b-125">لا تقم بإزالة البرامج النصية.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-125">Don't remove the scripts.</span></span> <span data-ttu-id="d0b1b-126">خلاف ذلك، قد تتم تهيئة بعض البيانات بشكل غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-126">Otherwise, some data might be initialized incorrectly.</span></span>

3. <span data-ttu-id="d0b1b-127">تحقق من وجود حقل **النوع** (**msdyn\_ordertype**) في النموذج.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-127">Verify that the **Type** (**msdyn\_ordertype**) field is present in the form.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="d0b1b-128">لا تقم بإزالة هذا الحقل.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-128">Don't remove this field.</span></span> <span data-ttu-id="d0b1b-129">خلاف ذلك، ستفشل البرامج النصية للتهيئة.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-129">Otherwise, the initialization scripts will fail.</span></span>

4. <span data-ttu-id="d0b1b-130">ابحث عن القيمة **formId** للنموذج الجديد.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-130">Find the **formId** value of the new form.</span></span> <span data-ttu-id="d0b1b-131">يمكنك استكمال هذه الخطوة بطريقتين:</span><span class="sxs-lookup"><span data-stu-id="d0b1b-131">You can complete this step in two ways:</span></span>

    - <span data-ttu-id="d0b1b-132">قم بتصدير نموذج **معلومات المشروع** كجزء من حل غير مدار، ثم ابحث عن القيمة **formId** في الملف customization.xml الخاص بالحل الذي تم تصديره.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-132">Export the **My Project Information** form as part of an unmanaged solution, and then look up the **formId** value in the customization.xml file of the exported solution.</span></span>
    - <span data-ttu-id="d0b1b-133">افتح نموذج **معلومات المشروع** في محرر النماذج، ثم ابحث عن المعرف الفريد العمومي (GUID) بجوار المعلمة **fromId** في URL، كما هو موضح في الشكل التوضيحي التالي.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-133">Open the **My Project Information** form in the form editor, and then look for the globally unique identifier (GUID) next to the **fromId** parameter in the URL, as shown in the following illustration.</span></span>

    ![قيمة formId للنموذج الجديدفي URL](media/how-to-add-custom-forms-in-v2.0.png)

5. <span data-ttu-id="d0b1b-135">قم بإنشاء تعيين **msdyn\_ordertype** للقيمة **formId** من خلال تحرير مورد الويب msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-135">Create an **msdyn\_ordertype** mapping for the **formId** value by editing the msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web resource.</span></span> <span data-ttu-id="d0b1b-136">قم بإزالة التعليمات البرمجية من المورد واستبدله بالتعليمات البرمجية التالية.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-136">Remove the code from the resource, and replace it with the following code.</span></span>

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

6. <span data-ttu-id="d0b1b-137">احفظ التخصيصات وانشرها.</span><span class="sxs-lookup"><span data-stu-id="d0b1b-137">Save and then publish the customizations.</span></span>
