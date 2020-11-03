---
title: تقدير مبيعات المشروع وتكلفته عندما يقوم مورد قابل للحجز بأداء أدوار متعددة على مشروع
description: يقدم هذا الموضوع معلومات حول كيفية استخدام أبعاد التسعير لدعم التسعير وتحديد التكاليف لمورد يقوم بأداء أدوار متعددة على أحد المشاريع.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 8ddc827a4170c5576c0a4350b51e6a119094ac50
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070696"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-mulitple-roles-on-a-project"></a><span data-ttu-id="322e6-103">تقدير مبيعات المشروع وتكلفته عندما يقوم مورد قابل للحجز بأداء أدوار متعددة على مشروع</span><span class="sxs-lookup"><span data-stu-id="322e6-103">Estimate project sales and costs when a bookable resource fills mulitple roles on a project</span></span> 

<span data-ttu-id="322e6-104">تحتاج الشركات القائمة على المشاريع في أغلب الأحيان إلى مورد واحد لتنفيذ ادوار متعددة على مشروع ما.</span><span class="sxs-lookup"><span data-stu-id="322e6-104">Project-based companies often have the need for one resource to perform mulitple roles on a project.</span></span> <span data-ttu-id="322e6-105">ويمكن تسعير كل واحد من هذه الأدوار وتحديد تكلفته بشكل مختلف مما يعني أن وقت المورد نفسه على المشروع قد يحصل على تقدير مالي مختلف بحسب أسعار الفاتورة وأسعار التكلفة لكل دور.</span><span class="sxs-lookup"><span data-stu-id="322e6-105">Each of these roles could be priced and costed differently which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="322e6-106">يسمح Project Service Automation بإعداد القيم في سجل عضو الفريق للمورد المسمى، ويسمح بتجاوزات مختلفة على كل مهمة من المهام التي تم تعيينها لعضو الفريق.</span><span class="sxs-lookup"><span data-stu-id="322e6-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="322e6-107">يوضح المثال التالي كيف أن التجاوز البسيط لهذه القيمة يسمح للمورد بتأدية أدوار متعددة على مشروع مع أسعار تكلفة وفاتورة مختلفة.</span><span class="sxs-lookup"><span data-stu-id="322e6-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="322e6-108">إنشاء مهام</span><span class="sxs-lookup"><span data-stu-id="322e6-108">Create tasks</span></span>
<span data-ttu-id="322e6-109">قم بإنشاء مهمتي مشروع لمدة 40 ساعة لكل واحدة منهما، المهمة A والمهمة B. حدد المهمة A كمهمة سابقة للمهمة B.</span><span class="sxs-lookup"><span data-stu-id="322e6-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="322e6-110">إعداد الدور والوحدة التنظيمية لعضو فريق عام في المشروع</span><span class="sxs-lookup"><span data-stu-id="322e6-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="322e6-111">في صفحة **الجدول** ، حدد صف **المهمة** للمهمة A.</span><span class="sxs-lookup"><span data-stu-id="322e6-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="322e6-112">في حقل **الموارد** ، حدد **إنشاء** في القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="322e6-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="322e6-113">في صفحة **الإنشاء السريع لعضو الفريق** ، حدد سمات عضو الفريق العام الذي يمكنه تنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="322e6-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="322e6-114">حدد الدور المناسب والوحدة التنظيمية المناسبة، ثم حدد **حفظ وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="322e6-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="322e6-115">يتم إنشاء عضو فريق عام ويتم تعيينه إلى هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="322e6-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="322e6-116">كرر هذه الخطوات للمهمة B وتأكد من أن الدور والوحدة التنظيمية على عضو الفريق العام الذي تم إنشاؤه للمهمة B يختلفان عن المهمة A.</span><span class="sxs-lookup"><span data-stu-id="322e6-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="322e6-117">إعداد الدور والوحدة التنظيمية لمهمة مشروع</span><span class="sxs-lookup"><span data-stu-id="322e6-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="322e6-118">بعد إنشاء المهمة A، حدد المهم، ثم حدد **تحرير المهمة**.</span><span class="sxs-lookup"><span data-stu-id="322e6-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="322e6-119">في صفحة **تفاصيل المهمة** ، ابحث عن حقلي **الدور** و **الوحدة التنظيمية** ، وأضف الحقول المطلوبة للمورد الذي سيقوم بتنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="322e6-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="322e6-120">إذا كنت تقوم بإكمال هذه السيناريوهات باستخدام بيانات العرض التوضيحي في Project Service Automation، فحدد **المستشار الرئيسي** للدور، و **Fabrikam US** كوحدة تنظيمية.</span><span class="sxs-lookup"><span data-stu-id="322e6-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="322e6-121">حدد المهمة B، ثم حدد **تحرير المهمة**.</span><span class="sxs-lookup"><span data-stu-id="322e6-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="322e6-122">في صفحة **تفاصيل المهمة** ، ابحث عن حقلي **الدور** و **الوحدة التنظيمية** ، وأضف الحقول المطلوبة للمورد الذي سيقوم بتنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="322e6-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="322e6-123">تأكد من أن القيم الموجودة في حقلي **الدور** و **الوحدة التنظيمية** تختلف للمهمة B عن قيم المهمة A.</span><span class="sxs-lookup"><span data-stu-id="322e6-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from those for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="322e6-124">إذا كنت تقوم بإكمال هذه السيناريوهات باستخدام بيانات العرض التوضيحي في Project Service Automation، فحدد **فني الشبكة** للدور، و **Fabrikam US** كوحدة تنظيمية.</span><span class="sxs-lookup"><span data-stu-id="322e6-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="322e6-125">احفظ صفحة **تفاصيل المهمة** ، ثم أغلقها.</span><span class="sxs-lookup"><span data-stu-id="322e6-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behaviour"></a><span data-ttu-id="322e6-126">سلوك عضو الفريق وتقديراته</span><span class="sxs-lookup"><span data-stu-id="322e6-126">Team member and estimates behaviour</span></span> 

1. <span data-ttu-id="322e6-127">في صفحة **تفاصيل المهمة** ، في **عضو الفريق** ، حدد عضوين في الفريق العام، ثم حدد **إنشاء متطلبات**.</span><span class="sxs-lookup"><span data-stu-id="322e6-127">On the **Task Details** page, on the **Team Member** , select the two generic team Members and then select **Generate Requirements**.</span></span> <span data-ttu-id="322e6-128">سيؤدي ذلك إلى إنشاء متطلبات الموارد.</span><span class="sxs-lookup"><span data-stu-id="322e6-128">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="322e6-129">حدد صف عضو الفريق لدور **المستشار الرئيسي‬‏‫** ، ثم حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="322e6-129">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="322e6-130">تفتح لوحة الجدولة وتحجز موردًا لهذا المتطلب.</span><span class="sxs-lookup"><span data-stu-id="322e6-130">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="322e6-131">حدد صف عضو الفريق لدور **فني الشبكة‬‏‫** ، ثم حدد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="322e6-131">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="322e6-132">تفتح لوحة الجدولة وتحجز المورد نفسه لهذا المتطلب.</span><span class="sxs-lookup"><span data-stu-id="322e6-132">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="322e6-133">شبكة أعضاء الفريق</span><span class="sxs-lookup"><span data-stu-id="322e6-133">Team Member grid</span></span> 
<span data-ttu-id="322e6-134">في شبكة **عضو الفريق** ، لاحظ أنه تم حذف سجلين لعضوين في الفريق العام وتم استبدالهما بمورد واحد.</span><span class="sxs-lookup"><span data-stu-id="322e6-134">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="322e6-135">هناك مجموعة واحدة من القيم الخاصة بذلك المورد تعرض مجموعة افتراضية من القيم لكل من **الدور** و **الوحدة التنظيمية**.</span><span class="sxs-lookup"><span data-stu-id="322e6-135">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="322e6-136">عند توسيع صف سجل عضو الفريق هذا، يمكنك الاطلاع على تعيينات مميزة في سجل عضو الفريق لكل واحدة من هاتين المهمتين.</span><span class="sxs-lookup"><span data-stu-id="322e6-136">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="322e6-137">يتضمن كل صف تعيينات قيمًا خاصة بالمهمة لكل من **الدور** و **الوحدة التنظيمية**.</span><span class="sxs-lookup"><span data-stu-id="322e6-137">Each assignment row has task specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="322e6-138">شبكة التقديرات</span><span class="sxs-lookup"><span data-stu-id="322e6-138">Estimates grid</span></span> 
<span data-ttu-id="322e6-139">عند الانتقال إلى شبكة **التقديرات** ، ستلاحظ وجود تسعير مختلف لكلي التعيينين للمورد نفسه.</span><span class="sxs-lookup"><span data-stu-id="322e6-139">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="322e6-140">يتم تسعير تعيين المورد على المهمة A باستخدام قيمة سمة **دور** **المستشار الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="322e6-140">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="322e6-141">يتم تسعير تعيين المورد نفسه على المهمة B باستخدام قيمة سمة **دور** **فني الشبكة**.</span><span class="sxs-lookup"><span data-stu-id="322e6-141">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>





