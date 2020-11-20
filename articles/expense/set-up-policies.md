---
title: تحديد نُهج المصروفات
description: يمكنك تحديد نُهج المصروفات التي يجب على العاملين اتباعها عند إدخال تقارير المصروفات وطلبات السفر وتقديمها.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: c55cec132649daf9ee08ea4d8db3668860247934
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128402"
---
# <a name="define-expense-policies"></a><span data-ttu-id="38495-103">تحديد نُهج المصروفات</span><span class="sxs-lookup"><span data-stu-id="38495-103">Define expense policies</span></span>

<span data-ttu-id="38495-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="38495-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="38495-105">يمكنك تحديد النُهج التي يجب على العاملين اتباعها عند إدخال تقارير المصروفات وطلبات السفر وتقديمها.</span><span class="sxs-lookup"><span data-stu-id="38495-105">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="38495-106">يمكن أن يساعدك تنفيذ نُهج المصروفات في إدارة المصروفات بشكل فعال.</span><span class="sxs-lookup"><span data-stu-id="38495-106">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="38495-107">على سبيل المثال، يمكنك تعيين نهج لمصروفات الفندق في مدينة نيويورك والتي تنص على انه لا يمكن أن تتجاوز مصروفات الليلية 250 دولارًا.</span><span class="sxs-lookup"><span data-stu-id="38495-107">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="38495-108">في حالة قيام أحد العاملين بإرسال تقرير مصروفات أو طلب سفر حيث يتجاوز سعر الغرفة هذا المبلغ، سيقوم النظام بإعلام</span><span class="sxs-lookup"><span data-stu-id="38495-108">If a worker submits an expense report or travel requisition where the room rate exceeds this amount, the system will notify the</span></span>         
<span data-ttu-id="38495-109">العامل بأنه قد تم تجاوز مبلغ نهج المصروفات.</span><span class="sxs-lookup"><span data-stu-id="38495-109">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="38495-110">يمكنك تكوين الرسالة التي سيتلقاها العامل عند</span><span class="sxs-lookup"><span data-stu-id="38495-110">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="38495-111">تحديد النهج.</span><span class="sxs-lookup"><span data-stu-id="38495-111">define the policy.</span></span>      
        
<span data-ttu-id="38495-112">يمكنك تحديد ثلاثة أنواع من النُهج:</span><span class="sxs-lookup"><span data-stu-id="38495-112">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="38495-113">**تحذير**: يتيح للعامل إرسال تقرير مصروفات أو طلب سفر ولكن سيتم تمييز المصروفات لكل الموافقين</span><span class="sxs-lookup"><span data-stu-id="38495-113">**Warning**: Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>         
  <span data-ttu-id="38495-114">لإعداد تقارير في وقت لاحق.</span><span class="sxs-lookup"><span data-stu-id="38495-114">for later reporting.</span></span>        

- <span data-ttu-id="38495-115">**خطأ**: للطلب من العامل مراجعة المصروفات للتوافق مع النهج قبل إرسال تقرير المصروفات أو طلب السفر.</span><span class="sxs-lookup"><span data-stu-id="38495-115">**Error**: Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>        
 
 - <span data-ttu-id="38495-116">**المبرر** للطلب من العامل أو المدير إدخال مبررات لتجاوز مبلغ النهج قبل إرسال تقرير المصروفات أو طلب السفر.</span><span class="sxs-lookup"><span data-stu-id="38495-116">**Justification**: Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="38495-117">تلميحات النهج</span><span class="sxs-lookup"><span data-stu-id="38495-117">Policy tips</span></span>
<span data-ttu-id="38495-118">فيما يلي بعض الاقتراحات التي يمكن ان تساعدك عند إنشاء نُهج جديدة لإدارة المصروفات:</span><span class="sxs-lookup"><span data-stu-id="38495-118">Here are a few suggestions that can assist you when creating new policies for expense management:</span></span> 

- <span data-ttu-id="38495-119">تكون النُهج سارية المفعول مما يعني أن النهج لن يكون نافذ المفعول إذا تم إنشاؤه بتاريخ بعد التاريخ الذي حدثت فيه المصروفات.</span><span class="sxs-lookup"><span data-stu-id="38495-119">Policies are date effective which means a policy won't take effect if it's created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="38495-120">على سبيل المثال، يمكنك إنشاء نهج جديد اليوم لفرض الحد الأقصى لمصروفات الوجبات لـ $50.</span><span class="sxs-lookup"><span data-stu-id="38495-120">For example, you create a new policy today to enforce a maximum meal expense of $50.</span></span> <span data-ttu-id="38495-121">لن يتم التحقق من إيه مصروفات تم إدخالها اعتبارًا من الأمس مقابل هذا النهج.</span><span class="sxs-lookup"><span data-stu-id="38495-121">Any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
- <span data-ttu-id="38495-122">عند إنشاء نهج لفئة مصروفات يمكن تفصيلها، ضع في اعتبارك إضافة شرط لنوع سطر المصروفات.</span><span class="sxs-lookup"><span data-stu-id="38495-122">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="38495-123">قد لا تكون بعض السياسات، مثل طلب استلام، ذات معني للبنود المفصلة.</span><span class="sxs-lookup"><span data-stu-id="38495-123">Some policies, such as requiring a receipt, may not make sense for itemized lines.</span></span> <span data-ttu-id="38495-124">في هذه الحالة، يتم تطبيق النهج فقط على سطر العنوان أو السطر غير المفصل.</span><span class="sxs-lookup"><span data-stu-id="38495-124">In this situation, the policy only is applied to the header line or a non-itemized line.</span></span> 
- <span data-ttu-id="38495-125">يتم تقييم سياسات إدارة المصروفات مقابل كيان المصدر بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="38495-125">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="38495-126">بالنسبة للسيناريوهات الشقيقة، يمكنك تعيين النهج الذي سيتم تقييمه مقابل الكيان الوجهة (الكيان المقترض) بدلا من ذلك.</span><span class="sxs-lookup"><span data-stu-id="38495-126">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="38495-127">لتشغيل النُهج في مقابل الكيان الوجهة، قم بتشغيل ميزة **تقييم نهج المصروفات مقابل كيان قانوني مقترض** في مساحة العمل **إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="38495-127">To run the policies against the destination entity, turn on the **Evaluate Expense policy against borrowing legal entity** feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="38495-128">متى يتم تقييم النهج</span><span class="sxs-lookup"><span data-stu-id="38495-128">When to evaluate policies</span></span>

<span data-ttu-id="38495-129">في محددات إدارة المصروفات، يمكنك تحديد تقييم سياسات إدارة المصروفات عند حفظ سطر أو عند إرسال تقرير مصروفات.</span><span class="sxs-lookup"><span data-stu-id="38495-129">In expense management parameters, you can select to evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="38495-130">إذا اخترت تقييم موعد حفظ سطر، سيكون المستخدمون قد قاموا بالمشاهدة المسبقة لما يحتاجونه لإكمال تقرير المصروفات الخاصة بهم في وقت واحد.</span><span class="sxs-lookup"><span data-stu-id="38495-130">If you choose to evaluate when a line is saved, users will have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="38495-131">أو يمكنك تأخير تقييم النهج وتوفير الوقت من خلال التحقق من الصحة في النهاية، أثناء الإرسال إلى سير العمل.</span><span class="sxs-lookup"><span data-stu-id="38495-131">Otherwise, you can delay policy evaluation and save time by validating at the end, during the submission to workflow.</span></span>
