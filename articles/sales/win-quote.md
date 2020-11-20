---
title: إنشاء عرض أسعار
description: يوفر هذا الموضوع معلومات حول إقفال عروض الأسعار في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 47804db0144c2b0f9dee2c60518e8aba6fb27473
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124667"
---
# <a name="close-a-quote"></a><span data-ttu-id="0ff9b-103">إنشاء عرض أسعار</span><span class="sxs-lookup"><span data-stu-id="0ff9b-103">Close a quote</span></span>

<span data-ttu-id="0ff9b-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="0ff9b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="0ff9b-105">يمكن إقفال عرض أسعار مشروع على أنه تم الفوز به أو تمت خسارته.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="0ff9b-106">نظرًا لأنه يتم دعم عمليتي التنشيط والمراجعة في عروض الأسعار في Microsoft Dynamics 365 Project Operations، يمكنك إغلاق مسودة عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-106">Because the functions Activate and Revise are not supported on quotes in Microsoft Dynamics 365 Project Operations, you can close a draft quote.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="0ff9b-107">إقفال عرض أسعار على أنه تم الفوز به</span><span class="sxs-lookup"><span data-stu-id="0ff9b-107">Close a quote as Won</span></span>

<span data-ttu-id="0ff9b-108">يؤدي إغلاق عرض أسعار مشروع على أنه تم الفوز به إلى تعيين حالة عرض الأسعار إلى **مغلق** وتعيين سبب الحالة إلى **تم الفوز به**.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-108">Closing a project quote as Won will set the status of the quote to **Closed** and status reason to **Won**.</span></span> <span data-ttu-id="0ff9b-109">يؤدي إغلاق عروض الأسعار إلى جعلها للقراءة فقط ويتم إنشاء مسودة عقد مشروع تتضمن جميع معلومات عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-109">Closing the quotes makes it read-only and creates a draft project contract with all the quote information.</span></span> <span data-ttu-id="0ff9b-110">ونظرًا لأنه لا يمكن إعادة فتح عرض أسعار مغلق، قبل إغلاق أي عرض أسعار، سيقوم مربع حوار التأكيد بتأكيد التغييرات.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-110">Because a closed quote can't be reopened, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="0ff9b-111">كما يتم توفير عقد المشروع الذي تم إنشاؤه من خلال عرض أسعار المشروع في الوحدة النمطية لإدارة المشاريع والمحاسبة في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-111">The project contract created from a project quote is also made available in the Project management and accounting module of Project Operations.</span></span> <span data-ttu-id="0ff9b-112">إذا لم يتم تعيين عقد مشروع إلى مشروع في أي من بنوده، سيتم توفير عقد المشروع هذا كعقد مشروع غير نشط ويصبح نشطًا بمجرد تعيين مشروع إلى بند واحد على الأقل من بنود العقد الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-112">If a project contract is not mapped to a project on any of its lines, this project contract is made available as an inactive project contract and becomes active as soon as a project is mapped to at least one of its contract lines.</span></span>

<span data-ttu-id="0ff9b-113">إذا تم إرفاق عرض الأسعار بفرصة، سيتم إغلاق أية عروض أسعار أخرى للمشروع في الفرصة تلقائيًا على أنه تمت خسارتها.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-113">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="0ff9b-114">التأثير المالي لإغلاق عرض أسعار على أنه تم الفوز به</span><span class="sxs-lookup"><span data-stu-id="0ff9b-114">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="0ff9b-115">إذا كان هناك أي قيم فعلية للوقت المسجل في أحد المشروعات بينما لا تزال مرفقة بمسودة عرض الأسعار، فسيتم تسجيل تكلفة الوقت أو المصروفات فقط.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-115">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="0ff9b-116">وبعد إغلاق عرض الأسعار بالفوز، يقوم التطبيق بإعادة بناء التكاليف من خلال عكس القيمة الفعلية للتكلفة القديمة وإعادة إنشاء التكلفة الفعلية الجديدة.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-116">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="0ff9b-117">سيعالج التطبيق القيم الفعلية لهذه التكلفة استنادا إلى أسلوب الفوترة لبند عقد المشروع المقترن.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-117">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="0ff9b-118">إذا كانت القيم الفعلية للتكلفة تشير إلى بند الوقت والمواد في العقد، سيقوم النظام تلقائيًا بإنشاء القيمة الفعلية للمبيعات غير المفوترة المقابلة عند إغلاق عرض الأسعار وإنشاء عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-118">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="0ff9b-119">إذا كانت القيم الفعلية للتكلفة مرجعا لبند عقد سعر ثابت، سيتوقف التطبيق إعادة معالجة التكلفة الفعلية استنادا إلى قواعد الفوترة المقسمة لعملاء عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-119">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

<span data-ttu-id="0ff9b-120">تتوفر جميع القيم الفعلية المعاد معالجتها في الوحدة النمطية لإدارة المشروعات والمحاسبة لمحاسب المشروع لأجل مراجعة دفتر الأستاذ العام وتحديثه وترحيله.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-120">All reprocessed actuals are available in the Project management and accounting module for the Project accountant to review, update, and post to the General ledger.</span></span> 

## <a name="close-a-quote-as-lost"></a><span data-ttu-id="0ff9b-121">إقفال عرض أسعار على أنه تمت خسارته</span><span class="sxs-lookup"><span data-stu-id="0ff9b-121">Close a quote as Lost</span></span>

<span data-ttu-id="0ff9b-122">سيؤدي إغلاق عرض أسعار مشروع على أنه تمت خسارته إلى تعيين الحالة إلى **مغلق** وسبب الحالة إلى **تمت خسارته**.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-122">Closing a project quote as Lost will set the status to **Closed** and status reason to **Lost**.</span></span> <span data-ttu-id="0ff9b-123">ويؤدي إغلاق عرض الأسعار إلى جعله للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-123">Closing the quote makes it read-only.</span></span> <span data-ttu-id="0ff9b-124">ونظرًا لأنه لا يمكن إعادة فتح عرض أسعار مغلق، قبل إغلاق أي عرض أسعار، سيقوم مربع حوار التأكيد بتأكيد التغييرات.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-124">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="0ff9b-125">إذا كان عرض أسعار المشروع الذي تم إغلاقه على أنه تمت خاسرته يتضمن مشروعًا يتم الرجوع إليه في أي من بنوده، سيتم تمييز هذا المشروع أيضا كمغلق ويتم إلغاء أي حجوزات موارد بدء من ذلك اليوم.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-125">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="0ff9b-126">في Project Operations، لن يؤثر إغلاق عرض الأسعار على الفوز أو الخسارة في حالة الفرصة، والتي ستظل مفتوحة إلى أن يتم إغلاقها يدويًا.</span><span class="sxs-lookup"><span data-stu-id="0ff9b-126">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
