---
title: إغلاق عرض أسعار- خفيف
description: يوفر هذا الموضوع معلومات حول إقفال عروض الأسعار في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8d387816f51f63ecd95df6534c7c012b323e6ddc
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764848"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="3fa0f-103">إغلاق عرض أسعار- خفيف</span><span class="sxs-lookup"><span data-stu-id="3fa0f-103">Close a quote - lite</span></span>

<span data-ttu-id="3fa0f-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="3fa0f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3fa0f-105">يمكن إقفال عرض أسعار مشروع على أنه تم الفوز به أو تمت خسارته.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="3fa0f-106">ويمكن إغلاق مسودة عروض الأسعار نظرا لأن عمليات التنشيط ومراجعة عروض الأسعار غير مدعومة في Dynamics 365 Project OperationsMicrosoft.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-106">A draft quote can be closed because the Activate and Revise operations on quotes isn't supported in Microsoft Dynamics 365 Project Operations.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="3fa0f-107">إقفال عرض أسعار على أنه تم الفوز به</span><span class="sxs-lookup"><span data-stu-id="3fa0f-107">Close a quote as Won</span></span>

<span data-ttu-id="3fa0f-108">عند إغلاق عرض أسعار مشروع باعتباره بالحالة "فوز"، يتم تعيين الحالة إلى "مغلق" وسبب الحالة هو الفوز.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-108">When you close a project quote as Won, the status is set to Closed and the status reason is Won.</span></span> <span data-ttu-id="3fa0f-109">يؤدي إغلاق عرض الأسعار إلى جعل عرض أسعار المشروع للقراءة فقط ويتم إنشاء مسودة عقد مشروع تحتوي على معلومات عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="3fa0f-110">ونظرا لأنه لا يمكن إعادة فتح عرض أسعار مغلق، فإن حوار التأكيد سيؤكد التغييرات التي تريدها.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-110">Because a closed quote can't be reopened, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="3fa0f-111">إذا تم إرفاق عرض الأسعار بفرصة، سيتم إغلاق أية عروض أسعار أخرى للمشروع في الفرصة تلقائيًا على أنه تمت خسارتها.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="3fa0f-112">التأثير المالي لإغلاق عرض أسعار على أنه تم الفوز به</span><span class="sxs-lookup"><span data-stu-id="3fa0f-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="3fa0f-113">في حالة وجود أي قيم الفعلية للوقت في المشروع بينما لا يزال مرفقًا بمسودة عرض الأسعار، يتم تسجيل تكلفة الوقت أو نفقات المشروع فقط.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-113">If there are any actuals for time on a project while is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="3fa0f-114">وبعد إغلاق عرض الأسعار بالفوز، يقوم التطبيق بإعادة بناء التكاليف من خلال عكس القيمة الفعلية للتكلفة القديمة وإعادة إنشاء التكلفة الفعلية الجديدة.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="3fa0f-115">سيعالج التطبيق القيم الفعلية لهذه التكلفة استنادا إلى أسلوب الفوترة لبند عقد المشروع المقترن.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="3fa0f-116">وإذا كانت القيم الفعلية للتكلفة تشير إلى شرط تعاقد يتعلق بالوقت والمواد، يتم إنشاء القيم الفعلية المقابلة للمبيعات غير المفقودة عندما يتم إغلاق عرض الأسعار وإنشاء عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-116">If the cost actuals reference a time and material contract line, corresponding unbilled sales actuals are created for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="3fa0f-117">إذا كانت القيم الفعلية للتكلفة تشير إلى شرط تعاقد لسعر ثابت، سيتوقف التطبيق عن إعادة معالجة القيم الفعلية للتكلفة المستندة إلى قواعد الفوترة المنقسمة لعملاء عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals that are based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="3fa0f-118">إغلاق عرض أسعار كخسارة:</span><span class="sxs-lookup"><span data-stu-id="3fa0f-118">Closing a quote as lost:</span></span>

<span data-ttu-id="3fa0f-119">عند إغلاق عرض أسعار مشروع باعتباره بالحالة "تمت خسارته"، يتم تعيين الحالة إلى "مغلق" وسبب الحالة هو تمت الخسارة.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-119">When you close a project quote as Lost, the status is set to Closed and status reason is Lost.</span></span> <span data-ttu-id="3fa0f-120">يؤدي إغلاق عرض الأسعار إلى جعل عرض أسعار المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="3fa0f-121">ونظرًا لأنه لا يمكن إعادة فتح عرض أسعار مغلق، قبل إغلاق أي عرض أسعار، سيقوم مربع حوار التأكيد بتأكيد التغييرات.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="3fa0f-122">إذا كان عرض أسعار المشروع الذي تم إغلاقه يشير إلى مشروع في أي من أسطره، يتم تعليم ذلك المشروع أيضا كـ "مغلق".</span><span class="sxs-lookup"><span data-stu-id="3fa0f-122">If the project quote that is closed as Lost references a project on any of its lines, that project is also marked as Closed.</span></span> <span data-ttu-id="3fa0f-123">يتم إلغاء حجوزات الموارد من هذا اليوم.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-123">Any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="3fa0f-124">في Project Operations، لن يؤثر إغلاق عرض الأسعار على الفوز أو الخسارة في حالة الفرصة، والتي ستظل مفتوحة إلى أن يتم إغلاقها يدويًا.</span><span class="sxs-lookup"><span data-stu-id="3fa0f-124">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
