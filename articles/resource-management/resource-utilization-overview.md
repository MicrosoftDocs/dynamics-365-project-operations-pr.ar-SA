---
title: نظرة عامة على استخدام الموارد
description: يوفر هذا الموضوع معلومات حول استخدام الموارد في Project Operations.
author: ruhercul
ms.date: 11/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: c9464b1de87211f8317a39a1d749e619769309ae
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/07/2021
ms.locfileid: "6367920"
---
# <a name="resource-utilization-overview"></a><span data-ttu-id="ab1df-103">نظرة عامة على استخدام الموارد</span><span class="sxs-lookup"><span data-stu-id="ab1df-103">Resource utilization overview</span></span>

<span data-ttu-id="ab1df-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="ab1df-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ab1df-105">يمكن للموارد أن تشتمل على الاستخدام القابل للفوترة للهدف.</span><span class="sxs-lookup"><span data-stu-id="ab1df-105">Resources can have a target billable utilization.</span></span> <span data-ttu-id="ab1df-106">ويتم تحديد هذا الاستخدام الهدف كسمة في دور افتراضي لأحد الموارد أو يتم تعيينه في سجل فردي لمورد قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="ab1df-106">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="ab1df-107">وتعتمد العمليات الحسابية للاستخدام على الساعات الفعلية التي قامت الموارد بالإعلام عنها باستخدام قيود الوقت المعتمدة.</span><span class="sxs-lookup"><span data-stu-id="ab1df-107">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="ab1df-108">تُستخدم الصيغ التالية لحساب الاستخدام:</span><span class="sxs-lookup"><span data-stu-id="ab1df-108">The following formulas are used to calculate utilization:</span></span>

  - <span data-ttu-id="ab1df-109">الاستخدام القابل للفوترة = الساعات الفعلية الخاضعة للرسوم ÷ القدرة الإنتاجية للمورد.</span><span class="sxs-lookup"><span data-stu-id="ab1df-109">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
  - <span data-ttu-id="ab1df-110">الاستخدام غير القابل للفوترة = الوقت الفعلي مع معرف نوع الفوترة = غير خاضع للرسوم أو التكميلي أو غير المتوفر ÷ القدرة الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="ab1df-110">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
  - <span data-ttu-id="ab1df-111">داخلي = الوقت الفعلي بلا عقد مبيعات ÷ القدرة الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="ab1df-111">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
  - <span data-ttu-id="ab1df-112">القدرة الإنتاجية للمورد = ساعات عمل المورد - خارج المكتب - غير أيام العمل</span><span class="sxs-lookup"><span data-stu-id="ab1df-112">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="ab1df-113">يمكنك العثور على طريقة عرض **استخدام الموارد** في جزء **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="ab1df-113">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="ab1df-114">تمثل كل خلية في الشبكة النسبة المئوية للاستخدام القابل للفوترة من المورد في فترة، مثل اليوم أو الأسبوع أو الشهر.</span><span class="sxs-lookup"><span data-stu-id="ab1df-114">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="ab1df-115">تُستخدم الصيغ التالية لتلوين الخلايا:</span><span class="sxs-lookup"><span data-stu-id="ab1df-115">The following formulas are used to color the cells:</span></span>

  - <span data-ttu-id="ab1df-116">**أخضر**: استخدام قابل للفوترة >= استخدام مستهدف للمورد</span><span class="sxs-lookup"><span data-stu-id="ab1df-116">**Green**: Billable utilization >= Resource target utilization</span></span>
  - <span data-ttu-id="ab1df-117">**أصفر**: استخدام مستهدف – 20 <= استخدام قابل للفوترة < استخدام مستهدف</span><span class="sxs-lookup"><span data-stu-id="ab1df-117">**Yellow**: Target utilization – 20 <= Billable utilization < Target utilization</span></span>
  - <span data-ttu-id="ab1df-118">**أحمر**: استخدام قابل للفوترة < استخدام مستهدف – 20</span><span class="sxs-lookup"><span data-stu-id="ab1df-118">**Red**: Billable utilization < Target utilization – 20</span></span>

<span data-ttu-id="ab1df-119">ونظرًا لأن طريقة عرض **استخدام المورد** تستند إلى لوحة الجدولة، فيمكنك استخدام إمكانات تصفية لوحة الجدولة لتصفية النتائج.</span><span class="sxs-lookup"><span data-stu-id="ab1df-119">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="ab1df-120">تتطلب الشبكة أن تقوم بتعيين استخدام الهدف لكل من الدور أو المورد الفردي.</span><span class="sxs-lookup"><span data-stu-id="ab1df-120">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="ab1df-121">لإجراء هذا الإعداد، انتقل إلى **الموارد‏‎** > **أدوار الموارد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="ab1df-121">To do this setup, go to **Resources** > **Resource roles**.</span></span>

<span data-ttu-id="ab1df-122">بالإضافة إلى ذلك، يجب تعيين دور افتراضي لكل مورد قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="ab1df-122">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="ab1df-123">انتقل إلى **الموارد** > **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="ab1df-123">Go to **Resources** > **Resources**.</span></span> <span data-ttu-id="ab1df-124">في علامة التبويب **Project Service**، تحقق من تحديد دور مورد، ومن تعيين حقل **افتراضي** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="ab1df-124">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field is set to **Yes**.</span></span> <span data-ttu-id="ab1df-125">يمكنك إضافة أدوار إضافية حيث **افتراضي** = **لا**.</span><span class="sxs-lookup"><span data-stu-id="ab1df-125">You can add additional roles where **Is Default** = **No**.</span></span> <span data-ttu-id="ab1df-126">يتم استخدام الدور حيث **افتراضي** = **نعم‏‎** لتقييم استخدام المورد مقابل الهدف لذلك الدور.</span><span class="sxs-lookup"><span data-stu-id="ab1df-126">The role where the **Is Default** = **Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="ab1df-127">من علامة التبويب **Project Service**، يمكنك أيضًا تعيين استخدام هدف فردي للمورد.</span><span class="sxs-lookup"><span data-stu-id="ab1df-127">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="ab1df-128">ويقوم حساب الاستخدام بعد ذلك باستخدام هذه الطريقة لتقييم هدف المورد بدلاً من هدف الدور الافتراضي للمورد.</span><span class="sxs-lookup"><span data-stu-id="ab1df-128">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="ab1df-129">يتم عرض الاستخدام لمورد فقط إذا وافق ذلك المورد، ويتم عرض الوقت الخاضع للرسوم خلال الفترة في الشبكة.</span><span class="sxs-lookup"><span data-stu-id="ab1df-129">Utilization is only shown for a resource if that resource has approved, chargeable time during the period shown in the grid.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]