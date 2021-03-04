---
title: كيف يمكنني تخصيص سير إجراءات العمل في مراحل المشروع؟
description: نظرة عامة على كيف يمكن تخصيص سير إجراءات العمل في مراحل المشروع
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
ms.topic: article
author: JohnPBurrows
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d0168f187e6b0880713aac04bd87dbc2209197d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148987"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a><span data-ttu-id="722c8-103">كيف يمكنني تخصيص سير إجراءات العمل في مراحل المشروع؟</span><span class="sxs-lookup"><span data-stu-id="722c8-103">How do I customize the Project Stages business process flow?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

<span data-ttu-id="722c8-104">هناك قيود معروفة في الإصدارات السابقة من تطبيق Project Service يقضي بأن تتطابق أسماء المراحل في سير إجراءات العمل في مراحل المشروع مع الأسماء الإنجليزية المتوقعة (**Quote** و **Plan** و **Close**).</span><span class="sxs-lookup"><span data-stu-id="722c8-104">There's a known limitation in earlier versions of the Project Service application that the names of the stages in the Project Stages business process flow must exactly match the expected English names (**Quote**, **Plan**, **Close**).</span></span> <span data-ttu-id="722c8-105">وبخلاف ذلك، لن يعمل منطق الأعمال الذي يعتمد على أسماء المراحل باللغة الإنجليزية، كما هو متوقع.</span><span class="sxs-lookup"><span data-stu-id="722c8-105">Otherwise, the business logic, which relies on the English stage names, doesn't work as expected.</span></span> <span data-ttu-id="722c8-106">ولهذا السبب، لا يمكنك العثور على إجراءات مألوفة مثل **تبديل العملية** أو **تحرير العملية‬** المتوفرة في نموذج المشروع، ومن غير المستحسن تخصيص سير إجراءات العمل.</span><span class="sxs-lookup"><span data-stu-id="722c8-106">That's why you don't see familiar actions such as **Switch Process** or **Edit Process** available on the project form, and customizing the business process flow isn't encouraged.</span></span> 

<span data-ttu-id="722c8-107">تمت معالجة هذا القيد في الإصدار 2.4.5.48 والإصدارات الأحدث.</span><span class="sxs-lookup"><span data-stu-id="722c8-107">This limitation has been addressed in version 2.4.5.48 and later.</span></span> <span data-ttu-id="722c8-108">توفر هذه المقالة حلولاً بديلة مقترحة للإصدارات السابقة إذا لم تكن بحاجة إلى تخصيص سير إجراءات العمل الافتراضي للإصدارات الأحدث.</span><span class="sxs-lookup"><span data-stu-id="722c8-108">This article provides suggested workarounds if you need to customize the default business process flow for earlier versions.</span></span>  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a><span data-ttu-id="722c8-109">يتطلب منطق الأعمال مطابقة تامة مع أسماء المراحل باللغة الإنجليزية</span><span class="sxs-lookup"><span data-stu-id="722c8-109">Business logic requires an exact match with English stage names</span></span>

<span data-ttu-id="722c8-110">يتضمن سير إجراءات العمل في مراحل المشروع منطق الأعمال الذي يعزز السلوكيات التالية في التطبيق:</span><span class="sxs-lookup"><span data-stu-id="722c8-110">The Project Stages business process flow includes business logic that drives the following behaviors in the app:</span></span>
- <span data-ttu-id="722c8-111">عندما يقترن المشروع بعرض أسعار، يعيّن الكود سير إجراءات العمل إلى مرحلة **Quote**.</span><span class="sxs-lookup"><span data-stu-id="722c8-111">When the project is associated with a quote, the code sets the business process flow to the **Quote** stage.</span></span>
- <span data-ttu-id="722c8-112">عندما يقترن المشروع بعقد، يعيّن الكود سير إجراءات العمل إلى مرحلة **Plan‎**.</span><span class="sxs-lookup"><span data-stu-id="722c8-112">When the project is associated with a contract, the code sets the business process flow to the **Plan** stage.</span></span>
- <span data-ttu-id="722c8-113">عندما يتقدم سير إجراءات العمل نحو المرحلة **Close**، يُلغى تنشيط سجل المشروع.</span><span class="sxs-lookup"><span data-stu-id="722c8-113">When the business process flow is advanced to the **Close** stage, the project record is deactivated.</span></span> <span data-ttu-id="722c8-114">عند إلغاء تنشيط المشروع، يتم تعيين نموذج المشروع وهيكل تنظيم العمل (WBS) إلى وضع القراءة فقط، ويتم إصدار حجوزات الموارد المسماة ويتم إلغاء تنشيط أية قوائم أسعار مقترنة.</span><span class="sxs-lookup"><span data-stu-id="722c8-114">When the project is deactivated, the project form and work breakdown structure (WBS) are set to read-only, the named resource bookings are released, and any associated price lists are deactivated.</span></span>

<span data-ttu-id="722c8-115">يعتمد منطق العمل هذا على أسماء مراحل المشروع باللغة الإنجليزية.</span><span class="sxs-lookup"><span data-stu-id="722c8-115">This business logic relies on the English names for the project stages.</span></span> <span data-ttu-id="722c8-116">هذا الاعتماد على أسماء المراحل باللغة الإنجليزية هو السبب الرئيسي الذي يحول دون التشجيع على تخصيص سير إجراءات العمل في مراحل المشروع، الإضافة إلى عدم رؤيتك الإجراءات الشائعة لسير إجراءات العمل مثل **تبديل العملية‬** أو **تحرير العملية** على كيان المشروع.</span><span class="sxs-lookup"><span data-stu-id="722c8-116">This dependency on the English stage names is the main reason why customization of the Project Stages business process flow isn't encouraged, as well as why you don’t see the common business process flow actions like **Switch Process** or **Edit Process** on the project entity.</span></span>

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a><span data-ttu-id="722c8-117">ماذا يحدث إذا لم تتطابق أسماء المراحل مع الأسماء الإنجليزية؟</span><span class="sxs-lookup"><span data-stu-id="722c8-117">What happens if the stage names don't match the English names?</span></span>

<span data-ttu-id="722c8-118">في الإصدار 1.x من تطبيق Project Service على النظام الأساسي 8.2، عندما لا تتطابق أسماء المراحل في سير إجراءات العمل مع أسماء المراحل باللغة الإنجليزية بشكل تام، يتم تخطي منطق الأعمال الذي يعيّن المرحلة المناسبة لعروض الأسعار أو العقود أو الذي يغلق المشروع.</span><span class="sxs-lookup"><span data-stu-id="722c8-118">In the Project Service app version 1.x on the 8.2 platform, when the stage names in the business process flow don’t match the English stage names exactly, the business logic that sets the right stage for quotes or contracts, or that closes the project, is skipped.</span></span> <span data-ttu-id="722c8-119">لا تظهر أي رسائل خطأ.</span><span class="sxs-lookup"><span data-stu-id="722c8-119">No error messages are displayed.</span></span> <span data-ttu-id="722c8-120">وبالتالي، يبدو وكأنه باستطاعتك تخصيص سير إجراءات العمل في مراحل المشروع.</span><span class="sxs-lookup"><span data-stu-id="722c8-120">Therefore it appears that you are able to customize the Project Stages business process flow.</span></span> <span data-ttu-id="722c8-121">ومع ذلك، لن تتمكن من رؤية أي من عمليات تلقائية تعمل بشكل صحيح لعروض الأسعار والعقود وإغلاق المشروع.</span><span class="sxs-lookup"><span data-stu-id="722c8-121">However, you won’t see any of the automatic processes working for quotes, contracts, and project close.</span></span>

<span data-ttu-id="722c8-122">في الإصدار 2.4.4.30 أو إصدار سابق من تطبيق Project Service على النظام الأساسي 9.0، حدث تغيير هندسي ملحوظ في سير إجراءات العمل، تتطلب عملية إعادة كتابة لمنطق أعمال سير إجراءات العمل.</span><span class="sxs-lookup"><span data-stu-id="722c8-122">In the Project Service app version 2.4.4.30 or earlier on the 9.0 platform, there was a significant architectural change to business process flows, which required a re-write of the business process flow business logic.</span></span> <span data-ttu-id="722c8-123">ونتيجة لذلك، إذا لم تتطابق أسماء مراحل المشروع مع الأسماء الإنجليزية المتوقعة، فلن تتلق رسالة خطأ.</span><span class="sxs-lookup"><span data-stu-id="722c8-123">As a result, if the process stage names don’t match the expected English names, you do receive an error message.</span></span> 

<span data-ttu-id="722c8-124">وبالتالي، إذا أرت تخصيص سير إجراءات العمل في مراحل المشروع لكيان المشروع، يمكنك فقط إضافة مراحل جديدة بالكامل إلى سير إجراءات العمل الافتراضي الخاص بكيان المشروع، مع الاحتفاظ بمراحل **Quote** و **Plan** و **Close** كما هي.</span><span class="sxs-lookup"><span data-stu-id="722c8-124">Therefore, if you want to customize the Project Stages business process flow for the project entity, you can only add brand new stages to the default business process flow for the project entity, while keeping the **Quote**, **Plan**, and **Close** stages as-is.</span></span> <span data-ttu-id="722c8-125">من شأن هذا القيد أن يضمن عدم حصولك على رسائل خطأ من منطق الأعمال الذي يتوقع أسماء المراحل باللغة الإنجليزية في سير إجراءات العمل.</span><span class="sxs-lookup"><span data-stu-id="722c8-125">This restriction ensures that you don’t get errors from the business logic that expects the English stage names in the business process flow.</span></span>

<span data-ttu-id="722c8-126">في الإصدار رقم 2.4.5.48 أو الإصدارات الأحدث، تمت إزالة منطق الأعمال الموضح في هذه المقالة من سير إجراءات العمل الافتراضي لكيان المشروع.</span><span class="sxs-lookup"><span data-stu-id="722c8-126">In version 2.4.5.48 or later, the business logic described in this article has been removed from the default business process flow for the project entity.</span></span> <span data-ttu-id="722c8-127">وستسمح لك الترقية إلى هذا الإصدار أو الإصدار الأحدث بتخصيص أو استبدال سير إجراءات العمل الافتراضي بسير إجراءات عمل خاص بك.</span><span class="sxs-lookup"><span data-stu-id="722c8-127">Upgrading to that version or later will let you customize or replace the default business process flow with one of your own.</span></span> 

## <a name="workarounds-for-earlier-versions"></a><span data-ttu-id="722c8-128">الحلول البديلة للإصدارات السابقة</span><span class="sxs-lookup"><span data-stu-id="722c8-128">Workarounds for earlier versions</span></span>

<span data-ttu-id="722c8-129">إذا لم تختر الترقية، يمكنك تخصيص سير إجراءات العمل في مراحل المشروع لكيان المشروع باستخدام إحدى الطريقتين التاليتين:</span><span class="sxs-lookup"><span data-stu-id="722c8-129">If upgrading isn't an option, you can customize the Project Stages business process flow for the project entity in one of these two ways:</span></span>

1. <span data-ttu-id="722c8-130">إضافة مراحل إضافية إلى التكوين الافتراضي، مع الاحتفاظ بأسماء المراحل باللغة الإنجليزية لكل من **Quote** و **Plan** و **Close**.</span><span class="sxs-lookup"><span data-stu-id="722c8-130">Add additional stages to the default configuration, while retaining the English stage names for **Quote**, **Plan**, and **Close**.</span></span>


![لقطة شاشة لإضافة مراحل إلى التكوين الافتراضي](media/FAQ-Customize-BPF-1.png)
 
2. <span data-ttu-id="722c8-132">إنشاء سير إجراءات عمل خاص بك وجعله سير إجراءات العمل الأساسي لكيان المشروع، مما يسمح لك باختيار أسماء المراحل التي تريدها.</span><span class="sxs-lookup"><span data-stu-id="722c8-132">Create your own business process flow and make it the primary business process flow for the project entity, which lets you have any stage names you want.</span></span> <span data-ttu-id="722c8-133">ومع ذلك، إذا أردت استخدام مراحل المشروع القياسية نفسها **Quote** و **Plan** و **Close**، فيجب القيام ببعض التخصيصات التي قد تفرضها أسماء المراحل المخصصة.</span><span class="sxs-lookup"><span data-stu-id="722c8-133">However, if you want to use the same standard project stages **Quote**, **Plan**, and **Close**, you need to do some customizations that are driven off your custom stage names.</span></span> <span data-ttu-id="722c8-134">يكمن المنطق الأكثر تعقيدًا في إغلاق المشروع، والذي يبقى باستطاعتك تشغيله عن طريق إلغاء تنشيط سجل المشروع.</span><span class="sxs-lookup"><span data-stu-id="722c8-134">The more complex logic is in the closing of the project, which you can still trigger by just deactivating the project record.</span></span>

![تخصيص BPF](media/FAQ-Customize-BPF-2.png)

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a><span data-ttu-id="722c8-136">اعتبارات إضافية للإصدار 2.4.4.30 أو إصدار سابق من تطبيق Project Service على النظام الأساسي 9.0</span><span class="sxs-lookup"><span data-stu-id="722c8-136">Additional considerations for Project Service app version 2.4.4.30 or earlier on platform 9.0</span></span>

<span data-ttu-id="722c8-137">في الإصدار 2.4.4.30 أو إصدار سابق من تطبيق Project Service على النظام الأساسي 9.0، ومع سير إجراءات عمل مخصص، لن يتم تحديث حقل **اسم المرحلة** على كيان المشروع المستخدم في مخطط **المشروع حسب المرحلة‬** وطرق عرض القائمة، لأنه مرتبط بسير إجراءات العمل الافتراضي في مراحل المشروع.</span><span class="sxs-lookup"><span data-stu-id="722c8-137">In Project Service 2.4.4.30 or earlier on platform 9.0, with a custom business process flow the **Stage Name** field on the project entity used in the **Project By Stage** chart and project list views won’t update, because it’s coupled to the default Project Stages business process flow.</span></span> <span data-ttu-id="722c8-138">يمكنك معالجة هذه المشكلة بتنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="722c8-138">You can address this issue with the following steps:</span></span>

- <span data-ttu-id="722c8-139">إضافة حقل مخصص لالتقاط المرحلة الحالية لسير إجراءات العمل يتم تحديثه كلما تقدم المستخدم من خلال سير إجراءات العمل المخصص.</span><span class="sxs-lookup"><span data-stu-id="722c8-139">Add a custom field to capture the current business process flow stage that is updated as the user advances through the custom business process flow.</span></span>

- <span data-ttu-id="722c8-140">تعديل مخطط **المشروع حسب المرحلة‬** بحيث يعمل مع الحقل المخصص بدلاً من التكوين الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="722c8-140">Modify the **Project By Stage** chart to work with your custom field instead of the default configuration.</span></span>

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a><span data-ttu-id="722c8-141">الخطوات اللازمة لإنشاء سير إجراءات العمل لكيان المشروع</span><span class="sxs-lookup"><span data-stu-id="722c8-141">Steps to create your own business process flow for the project entity</span></span>

<span data-ttu-id="722c8-142">لإنشاء سير إجراءات العمل المخصص، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="722c8-142">To create your own business process flow for the project entity do the following:</span></span>

1. <span data-ttu-id="722c8-143">انتقل إلى **الإعدادات** > **مركز العمليات‬**.</span><span class="sxs-lookup"><span data-stu-id="722c8-143">Go to **Settings** > **Process Center**.</span></span> <span data-ttu-id="722c8-144">لا تنسخ سير إجراءات العمل في مراحل المشروع لأن ذلك يؤدي أيضًا إلى نسخ منطق أعمال Project Service.</span><span class="sxs-lookup"><span data-stu-id="722c8-144">Don’t copy the Project Stages business process flow because that also copies the Project Service business logic.</span></span>

  ![إنشاء عملية](media/FAQ-Customize-BPF-3.png)

2. <span data-ttu-id="722c8-146">استخدم مصمم العمليات لإنشاء أسماء المراحل التي تريدها.</span><span class="sxs-lookup"><span data-stu-id="722c8-146">Use the Process Designer to create the stage names you want.</span></span> <span data-ttu-id="722c8-147">إذا أردت الحصول على الوظائف نفسها كما في المراحل الافتراضية لكل من **Quote** و **Plan** و **Close**، يجب عليك إنشاء ذلك استنادًا إلى أسماء مراحل سير إجراءات العمل المخصص.</span><span class="sxs-lookup"><span data-stu-id="722c8-147">If you want the same functionality as the default stages for **Quote**, **Plan**, and **Close**, you’ll have to create that based on your custom business process flow’s stage names.</span></span>

   ![لقطة شاشة لمصمم العمليات المستخدم لتخصيص سير إجراءات العمل](media/FAQ-Customize-BPF-4.png) 

3. <span data-ttu-id="722c8-149">في مصمم العمليات، انقر فوق **ترتيب سير الإجراءات‬** لتحويل سير إجراءات العمل المخصص إلى سير إجراءات العمل الرئيسي لكيان المشروع من خلال نقله فوق سير إجراءات العمل في مراحل المشروع إلى أعلى القائمة.</span><span class="sxs-lookup"><span data-stu-id="722c8-149">In the Process Designer, click **Order Process Flow** to make the custom business process flow the primary business process flow for the project entity by moving it above the Project Stages business process flow to the top of the list.</span></span>


   [<span data-ttu-id="722c8-150">لقطة شاشة لاستخدام ترتيب سير الإجراءات</span><span class="sxs-lookup"><span data-stu-id="722c8-150">Screenshot of using Order Process Flow</span></span>](media/FAQ-Customize-BPF-5-720.png)

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a><span data-ttu-id="722c8-151">تنطبق الخطوات التالية على الإصدار 2.4.4.30 أو إصدار سابق من تطبيق Project Service على النظام الأساسي 9.0</span><span class="sxs-lookup"><span data-stu-id="722c8-151">The following steps apply to Project Service app 2.4.4.30 or earlier on the 9.0 platform</span></span>

4. <span data-ttu-id="722c8-152">أضف حقلاً مخصصًا جديدًا لكيان المشروع لالتقاط المراحل المخصصة في سير إجراءات العمل المخصص.</span><span class="sxs-lookup"><span data-stu-id="722c8-152">Add a new custom field to the project entity to capture the custom stages in your custom business process flow.</span></span> <span data-ttu-id="722c8-153">ستحتاج إلى إضافة منطق الأعمال (المكون الإضافي/سير العمل) لتحديث هذا الحقل عند تحديث المرحلة على سير إجراءات العمل المخصصة.</span><span class="sxs-lookup"><span data-stu-id="722c8-153">You’ll need to add business logic (plugin/workflow) to update this field when the stage on the custom business process flow is updated.</span></span>

   ![لقطة شاشة لتخصيص كيان المشروع](media/FAQ-Customize-BPF-6-720.png)

5. <span data-ttu-id="722c8-155">قم بتعديل مخطط **المشروع حسب المرحلة** لاستخدام الحقل المخصص الجديد للمراحل.</span><span class="sxs-lookup"><span data-stu-id="722c8-155">Modify the **Project By Stage** chart to use your new custom field for stages.</span></span>

   ![لقطة شاشة لاستخدام مخطط المشروع حسب المرحلة](media/FAQ-Customize-BPF-7-720.png)

6. <span data-ttu-id="722c8-157">قم بتعديل طرق عرض كيان المشروع بحيث تتضمن الحقل المخصص الجديد للمراحل.</span><span class="sxs-lookup"><span data-stu-id="722c8-157">Modify any views for the project entity to include your new custom field for stages.</span></span>

   ![لقطة شاشة لتعديل طرق العرض على كيان المشروع](media/FAQ-Customize-BPF-8-720.png)

