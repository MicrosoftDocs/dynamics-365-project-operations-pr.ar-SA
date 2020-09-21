---
title: حجز موارد مسماة من متطلبات الموارد
description: يوفر هذا الموضوع معلومات حول حجز الموارد المسماة لمتطلب مورد عام.
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 83ac2056-313e-4f90-8297-238fd4d25ef9
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: eab280cd1a670cc2a6ed0ae02cde7ba9bf7d601d
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748616"
---
# <a name="book-named-resources-from-resource-requirements"></a><span data-ttu-id="c4814-103">حجز موارد مسماة من متطلبات الموارد</span><span class="sxs-lookup"><span data-stu-id="c4814-103">Book named resources from resource requirements</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="c4814-104">يمكنك حجز مورد مسمى بحيث يحل محل مورد عام يتضمن متطلب مورد.</span><span class="sxs-lookup"><span data-stu-id="c4814-104">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="c4814-105">في Project Service Automation (PSA) في صفحة **المشاريع**، انقر فوق علامة تبويب **الفريق**.</span><span class="sxs-lookup"><span data-stu-id="c4814-105">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab.</span></span>
2. <span data-ttu-id="c4814-106">حدد المورد العام الذي يحتوي على متطلب مورد من القائمة ثم انقر فوق **حجز**.</span><span class="sxs-lookup"><span data-stu-id="c4814-106">Select the generic resource that has a resource requirement from the list and then click **Book**.</span></span> <span data-ttu-id="c4814-107">أو، افتح متطلب المورد ثم انقر فوق **حجز**.</span><span class="sxs-lookup"><span data-stu-id="c4814-107">Or, open the resource requirement and then click **Book**.</span></span>


![حجز عضو فريق عام](media/RM-how-to-14.png)


3. <span data-ttu-id="c4814-109">في صفحة **مساعد الجدولة**، حدد مورد مسمى لحجزه إلى فريق المشروع ثم انقر فوق **حجز**.</span><span class="sxs-lookup"><span data-stu-id="c4814-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then click **Book**.</span></span>

![حجز عضو فريق عام باستخدام مساعد الجدولة](media/RM-how-to-15.png)

<span data-ttu-id="c4814-111">عند اكتمال الحجز وإنجازه بواسطة مورد محدد، يتم استبدال المورد العام بالمورد المسمى.</span><span class="sxs-lookup"><span data-stu-id="c4814-111">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

![استبدال عضو فريق مسمى بعضو فريق عام](media/RM-how-to-16.png)

<span data-ttu-id="c4814-113">يتم تحديث التعيينات في الجدولة بالمورد المسمى أيضا.</span><span class="sxs-lookup"><span data-stu-id="c4814-113">The assignments on the schedule are updated with the named resource as well.</span></span>

![تعيين عضو الفريق المسمى لمهام المشروع](media/RM-how-to-17.png)

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="c4814-115">إنجاز مورد عام بالعديد من الموارد المسماة</span><span class="sxs-lookup"><span data-stu-id="c4814-115">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="c4814-116">يشبه إنجاز متطلب مورد عام بالعديد من الموارد المسماة تعيين مورد مسمى فردي.</span><span class="sxs-lookup"><span data-stu-id="c4814-116">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="c4814-117">على سبيل المثال، توجد مهمة مدتها خمسة أيام و120 ساعة من الجهد</span><span class="sxs-lookup"><span data-stu-id="c4814-117">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="c4814-118">لا يمكن إكمال هذه المهمة بواسطة مورد واحد يعمل بشكل عاد لثمان ساعات في اليوم خلال أسبوع من خمسة أيام.</span><span class="sxs-lookup"><span data-stu-id="c4814-118">This task can't be completed by one resource that works a typical eight-hour day over a five day week.</span></span> 

![مهمة تحتاج إلى 120 ساعة من المجهود خلال خمسة أيام](media/RM-how-to-21.png)

<span data-ttu-id="c4814-120">المتطلب لمدة 120 ساعة من هندسة الروبوت خلال خمسة أيام، وهو بمثابة 24 ساعة في اليوم.</span><span class="sxs-lookup"><span data-stu-id="c4814-120">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

![المتطلب لكل يوم](media/RM-how-to-22.png)

<span data-ttu-id="c4814-122">هذا مثال على الحالة التي يلزم فيها الاستعانة بعدة موارد مسماة لتلبية طلب مورد عام.</span><span class="sxs-lookup"><span data-stu-id="c4814-122">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="c4814-123">ستحتاج إلى حجز العديد من الموارد لتنفيذ المطلب.</span><span class="sxs-lookup"><span data-stu-id="c4814-123">You will need to book multiple resources to fulfill the requirement.</span></span>

![حجز العديد من الموارد لاستيفاء متطلب.](media/RM-how-to-23.png)

<span data-ttu-id="c4814-125">الفرق الرئيسي في هذا السيناريو هو أن يظل المورد العام في الفريق المعين للمهمة، ولا يتم تعيين أعضاء فريق المورد المسمى كجزء من الموضع.</span><span class="sxs-lookup"><span data-stu-id="c4814-125">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="c4814-126">يمكن لمدير المشروع تعيين العمل بالشكل المناسب للموارد المسماة.</span><span class="sxs-lookup"><span data-stu-id="c4814-126">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="c4814-127">يمكن أن يساعد عرض **التسوية** مدير المشروع في تقسيم الحجوزات عبر موارد متعددة إلى تعيينات مهام.</span><span class="sxs-lookup"><span data-stu-id="c4814-127">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="c4814-128">وهذا لا يتم تلقائيا لأنه في أي سيناريو أكثر تعقيدا من المثال البسيط أعلاه، حين يكون لديك مجموعة من المهام التي تشكل المتطلب، يكون الغرض من كيف يقوم مدير المشروع بالتعيين، هو ما يلزم أن يفترضه النظام.</span><span class="sxs-lookup"><span data-stu-id="c4814-128">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement, the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="c4814-129">ونظرا لأن النظام لا يمكنه فهم الهدف، فمن المحتمل أن تكون الافتراضات مختلفة عن تلك المقصودة وسوف تحدث نتيجة غير صحيحة أو غير متوقعة.</span><span class="sxs-lookup"><span data-stu-id="c4814-129">Because the system can't understand intent, chances are that the assumptions will be different than intended and an incorrect or unpredictable result will happen.</span></span> <span data-ttu-id="c4814-130">والناتج الذي يمكن التنبؤ به هو أن يبقي المورد العام معينا حتى يقوم مدير المشروع بإنشاء تعيينات عن قصد بمساعدة طريقة عرض **التسوية**.</span><span class="sxs-lookup"><span data-stu-id="c4814-130">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>


