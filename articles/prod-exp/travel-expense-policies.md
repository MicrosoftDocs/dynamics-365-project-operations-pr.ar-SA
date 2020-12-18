---
title: إعداد سياسات المصروفات
description: يمكنك إعداد سياسات المصروفات التي يجب على العاملين اتباعها عند إدخال تقارير المصروفات وطلبات السفر وتقديمها في Microsoft Dynamics 365 Finance.
author: suvaidya
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6240a7be175800ce6f3b066de9e935ab370629ef
ms.sourcegitcommit: 13a4e58eddbb0f81aca07c1ff452c420dbd8a68f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/30/2020
ms.locfileid: "4650078"
---
# <a name="set-up-expense-policies"></a><span data-ttu-id="f6b1d-103">إعداد سياسات المصروفات</span><span class="sxs-lookup"><span data-stu-id="f6b1d-103">Set up expense policies</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="f6b1d-104">يمكنك تحديد النُهج التي يجب على العاملين اتباعها عند إدخال تقارير المصروفات وطلبات السفر وتقديمها.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="f6b1d-105">يمكن أن يساعدك تنفيذ نُهج المصروفات في إدارة المصروفات بشكل فعال.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="f6b1d-106">على سبيل المثال، يمكنك تعيين نهج لمصروفات الفندق في مدينة نيويورك والتي تنص على انه لا يمكن أن تتجاوز مصروفات الليلية 250 دولارًا.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="f6b1d-107">في حالة قيام أحد العاملين بإرسال تقرير مصروفات أو طلب سفر حيث يتجاوز سعر الغرفة هذا المبلغ، سيقوم النظام بإعلام</span><span class="sxs-lookup"><span data-stu-id="f6b1d-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="f6b1d-108">العامل بأنه قد تم تجاوز مبلغ نهج المصروفات.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="f6b1d-109">يمكنك تكوين الرسالة التي سيتلقاها العامل عند</span><span class="sxs-lookup"><span data-stu-id="f6b1d-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="f6b1d-110">تحديد النهج.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-110">define the policy.</span></span>      
        
<span data-ttu-id="f6b1d-111">يمكنك تحديد ثلاثة أنواع من النُهج:</span><span class="sxs-lookup"><span data-stu-id="f6b1d-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="f6b1d-112">تحذير – يتيح للعامل إرسال تقرير مصروفات أو طلب سفر ولكن سيتم تمييز المصروفات لكل الموافقين</span><span class="sxs-lookup"><span data-stu-id="f6b1d-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="f6b1d-113">ولإعداد التقارير في وقت لاحق.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-113">for later reporting.</span></span>        

- <span data-ttu-id="f6b1d-114">خطأ – يتطلب من العامل مراجعة المصروفات للتوافق مع السياسة قبل إرسال تقرير المصروفات أو طلب السفر.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="f6b1d-115">التبرير – يتطلب من العامل أو المدير إدخال تبرير لتجاوز مبلغ السياسة قبل إرسال تقرير المصروفات أو طلب السفر.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="f6b1d-116">تلميحات النهج</span><span class="sxs-lookup"><span data-stu-id="f6b1d-116">Policy tips</span></span>
<span data-ttu-id="f6b1d-117">فيما يلي بعض الاقتراحات التي يمكن أن تساعدك عند إنشاء سياسات جديدة لإدارة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-117">Here are a few suggestions that can assist you when creating new policies for expense management.</span></span> 
* <span data-ttu-id="f6b1d-118">تكون السياسات سارية المفعول مما يعني أن السياسة لن تكون نافذة المفعول إذا تم إنشاؤهها بتاريخ يلي التاريخ الذي حدثت فيه المصروفات.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="f6b1d-119">على سبيل المثال، إذا كنت تقوم بإنشاء سياسة جديدة اليوم لفرض الحد الأقصى لمصروفات الوجبات إلى 50 دولارًا، فلن يتم فحص أ مصروفات موجودة تم إدخالها اعتبارًا من الأمس في مقابل هذه السياسة.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="f6b1d-120">عند إنشاء نهج لفئة مصروفات يمكن تفصيلها، ضع في اعتبارك إضافة شرط لنوع سطر المصروفات.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="f6b1d-121">قد لا تكون بعض السياسات ذات معنىً، مثل طلب إيصال الاستلام، فيما يتعلق بالبنود المفصلة ويجب تطبيقها فقط على بند الرأس أو بند غير مفصل.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 
* <span data-ttu-id="f6b1d-122">يتم تقييم سياسات إدارة المصروفات مقابل كيان المصدر بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-122">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="f6b1d-123">بالنسبة للسيناريوهات الشقيقة، يمكنك تعيين النهج الذي سيتم تقييمه مقابل الكيان الوجهة (الكيان المقترض) بدلا من ذلك.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-123">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="f6b1d-124">لتشغيل السياسات في مقابل الكيان الوجهة، قم بتشغيل ميزة تقييم سياسة المصروفات مقابل الكيان القانوني المقترض في مساحة عمل **إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-124">To run the policies against the destination entity, turn on the "Evaluate Expense policy against borrowing legal entity" feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="f6b1d-125">متى يتم تقييم النهج</span><span class="sxs-lookup"><span data-stu-id="f6b1d-125">When to evaluate policies</span></span>

<span data-ttu-id="f6b1d-126">في معلمات إدارة المصروفات، يوجد خيار يسمح لك بتقييم سياسات إدارة المصروفات عند حفظ بند أو عند إرسال تقرير مصروفات.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-126">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="f6b1d-127">إذا اخترت التقييم عند حفظ بند، فهذا سيضمن حصول المستخدمين على رؤية مسبقة لما يحتاجونه لإكمال تقرير مصروفاتهم بهم مرة واحدة.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-127">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="f6b1d-128">أو، يمكنك تأخير تقييم السياسة وتوفير الوقت إذا حدثت عملية التحقق من الصحة في النهاية، أثناء الإرسال إلى سير العمل.</span><span class="sxs-lookup"><span data-stu-id="f6b1d-128">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>
