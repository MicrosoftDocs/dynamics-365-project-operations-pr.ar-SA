---
title: إغلاق عرض أسعار- خفيف
description: يوفر هذا الموضوع معلومات حول إقفال عروض الأسعار في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5ad206232d616cdbdc83e2a17b9177cfb98ffda9
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175695"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="ab609-103">إغلاق عرض أسعار- خفيف</span><span class="sxs-lookup"><span data-stu-id="ab609-103">Close a quote - lite</span></span>

<span data-ttu-id="ab609-104">_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_</span><span class="sxs-lookup"><span data-stu-id="ab609-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ab609-105">يمكن إقفال عرض أسعار مشروع على أنه تم الفوز به أو تمت خسارته.</span><span class="sxs-lookup"><span data-stu-id="ab609-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="ab609-106">لا يتم دعم عمليتي التنشيط والمراجعة في عروض الأسعار في Microsoft Dynamics 365 Project Operations، لذلك يمكن إغلاق عرض الأسعار المسودة.</span><span class="sxs-lookup"><span data-stu-id="ab609-106">The Activate and Revise operations on quotes is not supported in Microsoft Dynamics 365 Project Operations, so a draft quote can be closed.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="ab609-107">إقفال عرض أسعار على أنه تم الفوز به</span><span class="sxs-lookup"><span data-stu-id="ab609-107">Close a quote as Won</span></span>

<span data-ttu-id="ab609-108">يؤدي إغلاق عرض أسعار مشروع على أنه تم الفوز به إلى إغلاق عرض الأسعار مع تعيين الحالة إلى مغلق وتعيين السبب الحالة إلى تم الفوز به.</span><span class="sxs-lookup"><span data-stu-id="ab609-108">Closing a project quote as Won will close the quote with the status set to Closed and the status reason set to Won.</span></span> <span data-ttu-id="ab609-109">يؤدي إغلاق عرض الأسعار إلى جعل عرض أسعار المشروع للقراءة فقط ويتم إنشاء مسودة عقد مشروع تحتوي على معلومات عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="ab609-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="ab609-110">ونظرًا لأنه لا يمكن إعادة فتح عرض الأسعار، سيظهر هناك مربع حوار تأكيد قبل إجراء التغييرات حيث لا يمكن فتح عرض الأسعار الذي تم إغلاقه ولا يمكن التراجع عن التغييرات.</span><span class="sxs-lookup"><span data-stu-id="ab609-110">Because a closed quote can't be reopened, a confirmation dialog There is a confirmation dialog before the changes are done since a closed quote cannot be re-opened and the changes are irreversible.</span></span>

<span data-ttu-id="ab609-111">إذا تم إرفاق عرض الأسعار بفرصة، سيتم إغلاق أية عروض أسعار أخرى للمشروع في الفرصة تلقائيًا على أنه تمت خسارتها.</span><span class="sxs-lookup"><span data-stu-id="ab609-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="ab609-112">التأثير المالي لإغلاق عرض أسعار على أنه تم الفوز به</span><span class="sxs-lookup"><span data-stu-id="ab609-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="ab609-113">إذا كان هناك أي قيم فعلية للوقت المسجل في أحد المشروعات بينما لا تزال مرفقة بمسودة عرض الأسعار، فسيتم تسجيل تكلفة الوقت أو المصروفات فقط.</span><span class="sxs-lookup"><span data-stu-id="ab609-113">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="ab609-114">وبعد إغلاق عرض الأسعار بالفوز، يقوم التطبيق بإعادة بناء التكاليف من خلال عكس القيمة الفعلية للتكلفة القديمة وإعادة إنشاء التكلفة الفعلية الجديدة.</span><span class="sxs-lookup"><span data-stu-id="ab609-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="ab609-115">سيعالج التطبيق القيم الفعلية لهذه التكلفة استنادا إلى أسلوب الفوترة لبند عقد المشروع المقترن.</span><span class="sxs-lookup"><span data-stu-id="ab609-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="ab609-116">إذا كانت القيم الفعلية للتكلفة تشير إلى بند الوقت والمواد في العقد، سيقوم النظام تلقائيًا بإنشاء القيمة الفعلية للمبيعات غير المفوترة المقابلة عند إغلاق عرض الأسعار وإنشاء عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="ab609-116">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="ab609-117">إذا كانت القيم الفعلية للتكلفة مرجعا لبند عقد سعر ثابت، سيتوقف التطبيق إعادة معالجة التكلفة الفعلية استنادا إلى قواعد الفوترة المقسمة لعملاء عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="ab609-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="ab609-118">إغلاق عرض أسعار كخسارة:</span><span class="sxs-lookup"><span data-stu-id="ab609-118">Closing a quote as lost:</span></span>

<span data-ttu-id="ab609-119">سيؤدي إغلاق عرض أسعار مشروع على أنه تمت خسارته إلى تعيين الحالة إلى مغلق وسبب الحالة إلى تمت خسارته.</span><span class="sxs-lookup"><span data-stu-id="ab609-119">Closing a project quote as Lost will set the status to Closed and status reason to Lost.</span></span> <span data-ttu-id="ab609-120">يؤدي إغلاق عرض الأسعار إلى جعل عرض أسعار المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="ab609-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="ab609-121">ونظرًا لأنه لا يمكن إعادة فتح عرض أسعار مغلق، قبل إغلاق أي عرض أسعار، سيقوم مربع حوار التأكيد بتأكيد التغييرات.</span><span class="sxs-lookup"><span data-stu-id="ab609-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="ab609-122">إذا كان عرض أسعار المشروع الذي تم إغلاقه على أنه تمت خاسرته يتضمن مشروعًا يتم الرجوع إليه في أي من بنوده، سيتم تمييز هذا المشروع أيضا كمغلق ويتم إلغاء أي حجوزات موارد بدء من ذلك اليوم.</span><span class="sxs-lookup"><span data-stu-id="ab609-122">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="ab609-123">في Project Operations، لن يؤثر إغلاق عرض الأسعار على الفوز أو الخسارة في حالة الفرصة، والتي ستظل مفتوحة إلى أن يتم إغلاقها يدويًا.</span><span class="sxs-lookup"><span data-stu-id="ab609-123">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
