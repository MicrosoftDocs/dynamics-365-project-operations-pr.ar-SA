---
title: مجموعات الموافقة
description: يوفر موضوع هذا الموضوع معلومات حول مجموعة الموافقات والطلبات والمجموعة الفرعية لهذه العمليات.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116855"
---
# <a name="approval-sets"></a><span data-ttu-id="52272-103">مجموعات الموافقة</span><span class="sxs-lookup"><span data-stu-id="52272-103">Approval sets</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="52272-104">تعمل الموافقة على تعيين طلبات الموافقة على المجموعات في مجموعات فرعية أصغر من العمليات.</span><span class="sxs-lookup"><span data-stu-id="52272-104">Approval sets group approval requests together into smaller subsets of operations.</span></span> <span data-ttu-id="52272-105">يتيح هذا التجميع معالجة الموافقات بالترتيب حسب المشروع كما يتيح إعادة المحاولة والتسلسل.</span><span class="sxs-lookup"><span data-stu-id="52272-105">This grouping allows approvals to be processed in order by Project and allows for retrying and sequencing.</span></span> <span data-ttu-id="52272-106">يحسن التجميع وثوقية معالجة الموافقات وتعقبها لعدد كبيرة من الموافقات.</span><span class="sxs-lookup"><span data-stu-id="52272-106">Grouping improves the reliability and traceability of approval processing for large volumes of approvals.</span></span>

<span data-ttu-id="52272-107">وتشير مجموعات الموافقة إلى حالة المعالجة الإجمالية للسجلات المرتبطة بها.</span><span class="sxs-lookup"><span data-stu-id="52272-107">Approval sets indicate the overall processing state of their related records.</span></span> <span data-ttu-id="52272-108">عند معالجة سجل قبول باستخدام مجموعة الموافقة، يتم نقل السجل من **مرسل** إلى **تمت الموافقة** ، وإنه غير مرتبط بمجموعة الموافقة.</span><span class="sxs-lookup"><span data-stu-id="52272-108">When an approval record is processed using an approval set, the record moves from **Submitted** to **Approved**, and is unlinked from the approval set.</span></span> <span data-ttu-id="52272-109">إذا فشل سجل عند إرساله للموافقة عليه، يظل السجل في حالة **مرسل** ويتم وضع علامة على مجموعة الموافقة كفاشلة.</span><span class="sxs-lookup"><span data-stu-id="52272-109">If a record fails when it is submitted for approval, the record remains in a status of **Submitted** and the approval set is marked as failed.</span></span> <span data-ttu-id="52272-110">تقوم مجموعة الموافقة بتسجيل رسالة الخطأ الخاصة بالفشل.</span><span class="sxs-lookup"><span data-stu-id="52272-110">The approval set logs the error message of the failure.</span></span>

## <a name="processing-approvals-and-approval-sets"></a><span data-ttu-id="52272-111">الموافقات قيد المعالجة ومجموعات الموافقة</span><span class="sxs-lookup"><span data-stu-id="52272-111">Processing approvals and approval sets</span></span>
<span data-ttu-id="52272-112">تظهر الموافقات التي تم وضعها في قائمة انتظار للمعالجة في طريقة عرض **موافقات قيد الانتظار**.</span><span class="sxs-lookup"><span data-stu-id="52272-112">Approvals that are queued for processing are visible in the **Processing Approvals** view.</span></span> <span data-ttu-id="52272-113">ويحاول النظام معالجة جميع الإدخالات عدة مرات بشكل غير متزامن، بما في ذلك إعادة محاولة الموافقة في حالة فشل المحاولات السابقة.</span><span class="sxs-lookup"><span data-stu-id="52272-113">The system tries to process all the entries multiple times asynchronously, including retrying an approval if previous attempts failed.</span></span>

<span data-ttu-id="52272-114">يسجل الحقل **مجموعة الموافقة مدى الحياة** عدد المحاولات المتبقية لمعالجة المجموعة قبل أن يتم وضع علامة عليها كفاشلة.</span><span class="sxs-lookup"><span data-stu-id="52272-114">The **Approval Set Lifetime** field records the number of attempts left to process the set before it's marked as failed.</span></span>

## <a name="failed-approvals-and-approval-sets"></a><span data-ttu-id="52272-115">الموافقات الفاشلة ومجموعات الموافقة</span><span class="sxs-lookup"><span data-stu-id="52272-115">Failed approvals and approval sets</span></span>
<span data-ttu-id="52272-116">تسرد طريقة عرض **الموافقات الفاشلة** كافة الموافقات التي تتطلب تدخل المستخدم.</span><span class="sxs-lookup"><span data-stu-id="52272-116">The **Failed Approvals** view lists all approvals that require user intervention.</span></span> <span data-ttu-id="52272-117">افتح سجلات مجموعة الموافقة المقترنة لتحديد سبب الفشل.</span><span class="sxs-lookup"><span data-stu-id="52272-117">Open the associated approval set logs to identify the cause of the failure.</span></span>
<span data-ttu-id="52272-118">يضيف تحديد **إعادة المحاولة** إلى فترة مدة بقاء مجموعة الموافقة، وتنقل الموافقة التي تتم إعادة تعيينها إلى حالة **المعالجة**، ومحاولة معالجة السجلات المتبقية.</span><span class="sxs-lookup"><span data-stu-id="52272-118">Selecting **Retry** adds to the approval set lifetime count, moves the approval set back to a status of **Processing**, and attempts to process the remaining records.</span></span>

## <a name="configure-approval-sets"></a><span data-ttu-id="52272-119">تكوين مجموعات الموافقة</span><span class="sxs-lookup"><span data-stu-id="52272-119">Configure approval sets</span></span>

###  <a name="enable-the-approval-sets-feature"></a><span data-ttu-id="52272-120">تمكين ميزة مجموعات الموافقة</span><span class="sxs-lookup"><span data-stu-id="52272-120">Enable the Approval sets feature</span></span>
<span data-ttu-id="52272-121">قبل تمكين ميزة مجموعات الموافقة، تحقق من عدم وجود موافقات تتم معالجتها حاليًا.</span><span class="sxs-lookup"><span data-stu-id="52272-121">Before you enable the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="52272-122">انتقل إلى الصفحة **معلمات المشروع** وحدد **التحكم في الميزات** > **تمكين الموافقات الحديثة**.</span><span class="sxs-lookup"><span data-stu-id="52272-122">Go to the **Project parameters** page and select **Feature Control** > **Enable Modern Approvals**.</span></span>

### <a name="turn-off-the-approval-sets-feature"></a><span data-ttu-id="52272-123">إيقاف تشغيل ميزة مجموعات الموافقة</span><span class="sxs-lookup"><span data-stu-id="52272-123">Turn off the Approval sets feature</span></span>
<span data-ttu-id="52272-124">قبل إيقاف تشغيل ميزة مجموعات الموافقة، تحقق من عدم وجود موافقات تتم معالجتها حاليًا.</span><span class="sxs-lookup"><span data-stu-id="52272-124">Before you turn off the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="52272-125">انتقل إلى الصفحة **معلمات المشروع** وحدد **التحكم في الميزات** > **تعطيل الموافقات الحديثة**.</span><span class="sxs-lookup"><span data-stu-id="52272-125">Go to the **Project Parameters** page and select **Feature Control** > **Disable Modern Approvals**.</span></span>

### <a name="configuring-the-asynchronous-threshold"></a><span data-ttu-id="52272-126">تكوين الحد غير المتزامن</span><span class="sxs-lookup"><span data-stu-id="52272-126">Configuring the asynchronous threshold</span></span> 
<span data-ttu-id="52272-127">عند إنشاء مجموعات الموافقة، يتم نقل المعالجة إلى الخلفية عندما يتجاوز العدد المحدد من السجلات للموافقة الحد المُشار إليه.</span><span class="sxs-lookup"><span data-stu-id="52272-127">When approval sets are created, processing moves to the background when the selected number of records for approval exceeds the indicated threshold.</span></span> <span data-ttu-id="52272-128">استخدم الحقل **الحد غير المتزامن** لتكوين الوقت الذي يجب فيه تشغيل معالجة الموافقة بشكل متزامن أو غير متزامن.</span><span class="sxs-lookup"><span data-stu-id="52272-128">Use the **Asynchronous Threshold** field to configure when approval processing should be run synchronously or asynchronously.</span></span>
<span data-ttu-id="52272-129">القيم الصالحة هي:</span><span class="sxs-lookup"><span data-stu-id="52272-129">Valid values are:</span></span>

  - <span data-ttu-id="52272-130">صفر: ينبغي معالجة كافة الطلبات بشكل غير متزامن.</span><span class="sxs-lookup"><span data-stu-id="52272-130">Zero: All requests should be processed asynchronously.</span></span> 
  - <span data-ttu-id="52272-131">الأرقام أكبر من صفر: تتم معالجة الموافقات بشكل غير متزامن فقط عندما يتجاوز عدد الموافقات الذي تم إرساله هذه القيمة.</span><span class="sxs-lookup"><span data-stu-id="52272-131">Numbers greater than zero: Approvals are processed asynchronously only when the submitted number of approvals exceeds this value.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
