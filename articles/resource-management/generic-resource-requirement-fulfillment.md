---
title: استيفاء متطلبات الموارد العامة
description: يوفر هذا الموضوع معلومات حول كيفية حجز الموارد المسماة لمتطلبات مورد عام.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 6bb7c185656ff87bb3ca24209594c07d25862d70
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070589"
---
# <a name="generic-resource-requirement-fulfillment"></a><span data-ttu-id="43e13-103">استيفاء متطلبات الموارد العامة</span><span class="sxs-lookup"><span data-stu-id="43e13-103">Generic resource requirement fulfillment</span></span>

<span data-ttu-id="43e13-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="43e13-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="43e13-105">يمكنك حجز مورد مسمى بحيث يحل محل مورد عام يتضمن متطلب مورد.</span><span class="sxs-lookup"><span data-stu-id="43e13-105">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="43e13-106">في صفحة **المشاريع** ، حدد علامة التبويب **‏‫الفريق‬**.</span><span class="sxs-lookup"><span data-stu-id="43e13-106">On the **Projects** page, select the **Team** tab.</span></span>
2. <span data-ttu-id="43e13-107">حدد المورد العام الذي يحتوي على متطلب مورد من القائمة، ثم حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="43e13-107">Select the generic resource that has a resource requirement from the list, and then select **Book**.</span></span> <span data-ttu-id="43e13-108">أو، افتح متطلب المورد ثم حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="43e13-108">Or, open the resource requirement and then select **Book**.</span></span>
3. <span data-ttu-id="43e13-109">في صفحة **مساعد الجدولة** ، حدد مورد مسمى لحجزه إلى فريق المشروع ثم حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="43e13-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then select **Book**.</span></span>

<span data-ttu-id="43e13-110">عند اكتمال الحجز وإنجازه بواسطة مورد محدد، يتم استبدال المورد العام بالمورد المسمى.</span><span class="sxs-lookup"><span data-stu-id="43e13-110">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

<span data-ttu-id="43e13-111">يتم تحديث التعيينات في الجدولة بالمورد المسمى أيضا.</span><span class="sxs-lookup"><span data-stu-id="43e13-111">The assignments on the schedule are updated with the named resource as well.</span></span>

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="43e13-112">إنجاز مورد عام بالعديد من الموارد المسماة</span><span class="sxs-lookup"><span data-stu-id="43e13-112">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="43e13-113">يشبه إنجاز متطلب مورد عام بالعديد من الموارد المسماة تعيين مورد مسمى فردي.</span><span class="sxs-lookup"><span data-stu-id="43e13-113">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="43e13-114">على سبيل المثال، توجد مهمة مدتها خمسة أيام و120 ساعة من الجهد</span><span class="sxs-lookup"><span data-stu-id="43e13-114">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="43e13-115">لا يمكن إكمال هذه المهمة بواسطة مورد واحد يعمل بشكل عاد لثمان ساعات في اليوم على مدار خمسة أيام في الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="43e13-115">This task can't be completed by one resource that works a typical eight-hour day over a five-day week.</span></span> 

<span data-ttu-id="43e13-116">المتطلب لمدة 120 ساعة من هندسة الروبوت خلال خمسة أيام، وهو بمثابة 24 ساعة في اليوم.</span><span class="sxs-lookup"><span data-stu-id="43e13-116">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

<span data-ttu-id="43e13-117">هذا مثال على الحالة التي يلزم فيها الاستعانة بعدة موارد مسماة لتلبية طلب مورد عام.</span><span class="sxs-lookup"><span data-stu-id="43e13-117">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="43e13-118">ستحتاج إلى حجز العديد من الموارد لتنفيذ المطلب.</span><span class="sxs-lookup"><span data-stu-id="43e13-118">You will need to book multiple resources to fulfill the requirement.</span></span>

<span data-ttu-id="43e13-119">الفرق الرئيسي في هذا السيناريو هو أن يظل المورد العام في الفريق المعين للمهمة، ولا يتم تعيين أعضاء فريق المورد المسمى كجزء من الموضع.</span><span class="sxs-lookup"><span data-stu-id="43e13-119">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="43e13-120">يمكن لمدير المشروع تعيين العمل بالشكل المناسب للموارد المسماة.</span><span class="sxs-lookup"><span data-stu-id="43e13-120">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="43e13-121">يمكن أن يساعد عرض **التسوية** مدير المشروع في تقسيم الحجوزات عبر موارد متعددة إلى تعيينات مهام.</span><span class="sxs-lookup"><span data-stu-id="43e13-121">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="43e13-122">لا يتم ذلك تلقائيًا لأنه في أي سيناريو أكثر تعقيدًا من المثال البسيط أعلاه، مثل عندما يكون لديك مجموعة من المهام التي تشكل المطلب أو القصد من كيفية تعيين مدير المشروع، يجب أن يفترضه النظام.</span><span class="sxs-lookup"><span data-stu-id="43e13-122">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement or the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="43e13-123">نظرًا لأن النظام لا يستطيع فهم القصد، فمن المحتمل أن تكون الافتراضات مختلفة عما هو مقصود وستحدث نتيجة غير صحيحة أو غير متوقعة.</span><span class="sxs-lookup"><span data-stu-id="43e13-123">Because the system can't understand intent, it's likely that the assumptions will be different than intended and an incorrect or unpredictable result will occur.</span></span> <span data-ttu-id="43e13-124">والناتج الذي يمكن التنبؤ به هو أن يبقي المورد العام معينا حتى يقوم مدير المشروع بإنشاء تعيينات عن قصد بمساعدة طريقة عرض **التسوية**.</span><span class="sxs-lookup"><span data-stu-id="43e13-124">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>


