---
title: إنشاء تعيينات الموارد
description: يوفر هذا الموضوع معلومات حول إنشاء تعيينات الموارد العامة والمسماة.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 20eb3880b17fb1f765ad79bd720520b0c8004c0a
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906045"
---
# <a name="create-resource-assignments"></a><span data-ttu-id="03670-103">إنشاء تعيينات الموارد</span><span class="sxs-lookup"><span data-stu-id="03670-103">Create resource assignments</span></span>

<span data-ttu-id="03670-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="03670-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="03670-105">يشكّل تعيين المورد الاقتران المباشر لعضو فريق المشروع بمهمة عقدة طرفية.</span><span class="sxs-lookup"><span data-stu-id="03670-105">A resource assignment is the direct association of a project team member to a leaf node task.</span></span> <span data-ttu-id="03670-106">يوفر هذا الموضوع معلومات حول الطرق المختلفة لتعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="03670-106">This topic provides information about the different ways to assign resources.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="03670-107">إنشاء عضو فريق عام من خلال تعيين المهام</span><span class="sxs-lookup"><span data-stu-id="03670-107">Create a generic team member through task assignment</span></span>


<span data-ttu-id="03670-108">عند إنشاء عضو فريق عام من خلال تعيين المهمة، فأنت تنشئ عنصرًا نائبًا أو موردًا عامًا.</span><span class="sxs-lookup"><span data-stu-id="03670-108">When you create a generic team member through task assignment, you create a placeholder or generic resource.</span></span> <span data-ttu-id="03670-109">يصف هذا المورد العام خصائص المورد المسمى الذي تريده في النهاية أن يعمل على المهام.</span><span class="sxs-lookup"><span data-stu-id="03670-109">This generic resource describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="03670-110">وعليك بعد ذلك إنشاء متطلب، أو ترسل طلبًا باستخدام المتطلب، يُستخدم للبحث عن المورد المسمى وحجزه.</span><span class="sxs-lookup"><span data-stu-id="03670-110">You then generate a requirement, or submit a request using the requirement, that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="03670-111">على شبكة الجدولة لمهمة ما، حدد أيقونة المورد في خلية **المورد**.</span><span class="sxs-lookup"><span data-stu-id="03670-111">On the Schedule grid for a task, select the Resource icon in the **Resource** cell.</span></span>
2. <span data-ttu-id="03670-112">اكتب اسمًا يُستخدم كاسم مورد نائب.</span><span class="sxs-lookup"><span data-stu-id="03670-112">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="03670-113">على سبيل المثال، مدير مشروع.</span><span class="sxs-lookup"><span data-stu-id="03670-113">For example, Program Manager.</span></span>
3. <span data-ttu-id="03670-114">حدد **إنشاء**، وفي حقل **إنشاء سريع لعضو فريق المشروع**، قم بتعيين دور للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="03670-114">Select **Create**, and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>
4. <span data-ttu-id="03670-115">يمكنك تعيين المهام إلى هذا المورد النائب عن طريق تحديد المورد على **محدد المورد** للمهمة.</span><span class="sxs-lookup"><span data-stu-id="03670-115">Assign tasks as needed to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="03670-116">الموارد المدرجة ضمن **أعضاء الفريق**.</span><span class="sxs-lookup"><span data-stu-id="03670-116">The resources listed under **Team Members**.</span></span>
5. <span data-ttu-id="03670-117">عند الانتهاء من تعيين المورد العام، حدد المورد العام على علامة تبويب **الفريق**، ثم حدد **إنشاء المتطلب** لإنشاء متطلبات الموارد للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="03670-117">When you’re finished assigning the generic resource, on the **Team** tab, select the generic resource, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>
6. <span data-ttu-id="03670-118">حدد **حجز** للمورد العام، ثم استخدم لوحة الجدولة للبحث عن مورد حقيقي وحجزه.</span><span class="sxs-lookup"><span data-stu-id="03670-118">Select **Book** for the generic resource and then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="03670-119">يمكنك أيضًا إرسال متطلبات التنفيذ بواسطة مدير الموارد.</span><span class="sxs-lookup"><span data-stu-id="03670-119">You can also submit the requirement for fulfillment by a resource manager.</span></span>
7. <span data-ttu-id="03670-120">عندما يتم استيفاء المورد العام بالكامل (لن يؤدي استيفاء متطلبات الموارد الجزئية إلى تعيين مورد) مع مورد مسمى، تتم إزالة المورد العام من الفريق.</span><span class="sxs-lookup"><span data-stu-id="03670-120">When the generic resource is fully fulfilled (partial resource requirement fulfillment will not result in a resource assignment) with a named resource, the generic resource is removed from the team.</span></span> <span data-ttu-id="03670-121">يتم تعيين تعيينات المهام الخاصة بالمورد العام إلى المورد المسمى الذي استوفى متطلبات الموارد للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="03670-121">The task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="03670-122">تعيين مورد مسمى من قائمة جميع الموارد القابلة للحجز</span><span class="sxs-lookup"><span data-stu-id="03670-122">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="03670-123">يمكنك استخدام مربع البحث في **منتقي المورد** للبحث عن جميع الموارد النشطة القابلة للحجز وتعيينها لأي مهمة عقدة طرفية.</span><span class="sxs-lookup"><span data-stu-id="03670-123">You can use the search box in the **Resource Picker** to search all active bookable resources and assign them to any leaf node task.</span></span> <span data-ttu-id="03670-124">تُضاف الموارد التي تم تعيينها بهذه الطريقة إلى الفريق دون أية حجوزات.</span><span class="sxs-lookup"><span data-stu-id="03670-124">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="03670-125">وهذا يشبه إضافة عضو فريق وتحديد **بلا** كأسلوب توزيع.</span><span class="sxs-lookup"><span data-stu-id="03670-125">This is similar to adding a team member and selecting **None** as the allocation method.</span></span> <span data-ttu-id="03670-126">تظهر المورد في علامات التبويب **الفريق** و**تعيين الموارد** و**التسوية** كموارد ذات تعيينات فقط ونقص في الحجز.</span><span class="sxs-lookup"><span data-stu-id="03670-126">The resource is displayed on the **Team**, **Resource Assignment**, and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="03670-127">يمكنك حجز هذه الموارد إذا أردت استخدام توافرها.</span><span class="sxs-lookup"><span data-stu-id="03670-127">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="03670-128">من شبكة المهام أو اللوحة أو المخطط الزمني، انتقل إلى الخلية **معين إلى**.</span><span class="sxs-lookup"><span data-stu-id="03670-128">From the task grid, board, or timeline, navigate to the **Assigned To** cell.</span></span>
2. <span data-ttu-id="03670-129">في مربع البحث، ابدأ بكتابة اسم.</span><span class="sxs-lookup"><span data-stu-id="03670-129">In the search box, start typing a name.</span></span> <span data-ttu-id="03670-130">يتم عرض نتائج البحث عن الاسم في **محدد المورد** ضمن **الموارد الأخرى**.</span><span class="sxs-lookup"><span data-stu-id="03670-130">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>
3. <span data-ttu-id="03670-131">حدد المورد الذي ترغب في تعيينه للمهمة أو حدد اسم المورد ضمن **موارد الفريق الأخرى**.</span><span class="sxs-lookup"><span data-stu-id="03670-131">Select the resource that you want to assign to the task or select the name of the resource under **Other Team Resources**.</span></span>
