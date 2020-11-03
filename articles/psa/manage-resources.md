---
title: إدارة الموارد
description: يوفر هذا الموضوع معلومات حول كيف يمكنك إدارة الموارد.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/13/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 5b34ad66750dba9459d551a2527c13111196511e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070845"
---
# <a name="manage-resources"></a><span data-ttu-id="cfa14-103">إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="cfa14-103">Manage resources</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="cfa14-104">يشتمل Dynamics 365 Project Service Automation على لوحة معلومات مدير موارد توفر نظرة عامة مرئية على طلب المورد واستخدامه عبر المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-104">Dynamics 365 Project Service Automation includes a resource manager dashboard that provides a visual overview of resource demand and utilization throughout the organization.</span></span> <span data-ttu-id="cfa14-105">يمكنك استخدام المخططات الموجودة في لوحة المعلومات هذه لتمثيل البيانات التالية:</span><span class="sxs-lookup"><span data-stu-id="cfa14-105">You can use the charts on this dashboard to visualize the following information:</span></span>

- <span data-ttu-id="cfa14-106">**طلب المورد** – يعرض مخطط **طلب المورد النشط** الموارد التي تم إرسالها.</span><span class="sxs-lookup"><span data-stu-id="cfa14-106">**Resource demand** – The **Active Resource Request** chart shows resources that have been submitted.</span></span> <span data-ttu-id="cfa14-107">يتم تجميع الموارد حسب إما الدور أو المشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-107">The resources are aggregated by either role or project.</span></span>
- <span data-ttu-id="cfa14-108">**طلب مورد غير مرسل** – يعرض مخطط **‏‫طلب موارد غير معيّنة‬** كافة متطلبات الموارد التي لم يتم إرسالها.</span><span class="sxs-lookup"><span data-stu-id="cfa14-108">**Unsubmitted resource demand** – The **Unassigned Resource Demand** chart shows all the resource requirements that haven't been submitted.</span></span> <span data-ttu-id="cfa14-109">ويساعد مديري الموارد في عرض طلب لم يتم تأكيده وقد يتم إرساله من خلال طلب مورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-109">It helps resource managers view demand that isn't firm and might be submitted through a resource request.</span></span>
- <span data-ttu-id="cfa14-110">**الاستخدام القابل للفوترة للأسبوع الماضي** - يعرض مخطط **الاستخدام حسب الدور** نسبة الاستخدام القابل للفوترة للقيمة الفعلية للمؤسسة حسب الدور مقابل الاستخدام القابل للفوترة المستهدف حسب الدور.</span><span class="sxs-lookup"><span data-stu-id="cfa14-110">**Billable utilization for the past week** – The **Utilization by Role** chart shows the percentage of the organization's actual billable utilization by role against its target billable utilization by role.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cfa14-111">لجعل مخطط **الاستخدام حسب الدور** متوفرًا، قم بإنشاء وظيفة تقوم بتشغيل سير العمل UpdateRoleUtilization.</span><span class="sxs-lookup"><span data-stu-id="cfa14-111">To make the **Utilization by Role** chart available, create a job that runs the UpdateRoleUtilization workflow.</span></span> <span data-ttu-id="cfa14-112">تعمل هذه الوظيفة المتكررة كل سبعة أيام لحساب الاستخدام القابل للفوترة للأيام السبعة السابقة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-112">This recurring job runs every seven days to calculate billable utilization for the previous seven days.</span></span> <span data-ttu-id="cfa14-113">يتم تجميع النتائج حسب الدور.</span><span class="sxs-lookup"><span data-stu-id="cfa14-113">The results are aggregated by role.</span></span>

## <a name="manage-project-team-members"></a><span data-ttu-id="cfa14-114">إدارة أعضاء فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="cfa14-114">Manage project team members</span></span>

<span data-ttu-id="cfa14-115">يمكن لمديري المشاريع استخدام لوحة معلومات إدارة الموارد لإدارة الموارد في المشاريع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-115">Project managers can use the resource manager dashboard to manage the resources on projects.</span></span> <span data-ttu-id="cfa14-116">على سبيل المثال، يمكنهم إضافة عضو فريق مباشرة إلى مشروع وحجز عضو فريق لتلبية متطلبات المورد التي تم التقاطها بواسطة مورد عام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-116">For example, they can add a team member directly to a project and book a team member to fulfill the resource requirements that were captured by a generic resource.</span></span>

### <a name="add-a-team-member-directly-to-a-project"></a><span data-ttu-id="cfa14-117">إضافة عضو فريق مباشرة إلى مشروع</span><span class="sxs-lookup"><span data-stu-id="cfa14-117">Add a team member directly to a project</span></span>

<span data-ttu-id="cfa14-118">لإضافة عضو فريق مباشرة إلى مشروع، من الصفحة **المشاريع** ، في علامة التبويب **فريق** ، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-118">To add a team member directly to a project, on the **Projects** page, on the **Team** tab, select **New**.</span></span> <span data-ttu-id="cfa14-119">يظهر مربع حوار **الإنشاء السريع: عضو فريق المشروع**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-119">The **Quick Create:Project Team Member** dialog box appears.</span></span> <span data-ttu-id="cfa14-120">في مربع الحوار هذا، يمكنك تنفيذ هذه المهام:</span><span class="sxs-lookup"><span data-stu-id="cfa14-120">In this dialog box, you can perform these tasks:</span></span>

- <span data-ttu-id="cfa14-121">**حجز مورد مسمى** - في حقل **مورد قابل للحجز** ، حدد اسم المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-121">**Book a named resource** – In the **Bookable Resource** field, select the name of the resource.</span></span> <span data-ttu-id="cfa14-122">ثم حدد الدور، وقم بتعيين الفترة، وحدد طريقة توزيع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-122">Then select the role, set the period, and select an allocation method.</span></span> <span data-ttu-id="cfa14-123">يتم إضافة المورد المسمى الذي قمت بتحديده إلى المشروع باستخدام طريقة التوزيع المحددة وتقويم الموارد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-123">The named resource that you selected is added to the project by using the selected allocation method and the resources calendar.</span></span>
- <span data-ttu-id="cfa14-124">**إضافة مورد عام** - اترك حقل **مورد قابل للحجز** فارغا، ثم حدد الدور وقم بتعيين الفترة، وحدد طريقة التوزيع المفضلة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-124">**Add a generic resource** – Leave the **Bookable resource** field blank, and then select the role, set the period, and select the preferred allocation method.</span></span> <span data-ttu-id="cfa14-125">تتم إضافة مورد عام إلى الفريق كعنصر نائب للاحتفاظ بنمط الطلب الذي يتم استخدامه لحجز الموارد المسماة في الفريق.</span><span class="sxs-lookup"><span data-stu-id="cfa14-125">A generic resource is added to the team as a placeholder to hold the demand pattern that is used to book named resources on the team.</span></span> <span data-ttu-id="cfa14-126">يتم تنفيذ المتطلبات طبقا لتقويم المشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-126">The requirement is made according to the project calendar.</span></span>
- <span data-ttu-id="cfa14-127">**إضافة مورد مسمى إلى الفريق دون استهلاك سعة الموارد** - في الحقل **مورد قابل للحجز** ، حدد موردا.</span><span class="sxs-lookup"><span data-stu-id="cfa14-127">**Add a named resource to the team without consuming resource capacity** – In the **Bookable Resource** field, select a resource.</span></span> <span data-ttu-id="cfa14-128">ثم حدد الفترة، وحدد **بلا** باعتبارها طريقة التوزيع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-128">Then select the period, and select **None** as the allocation method.</span></span> <span data-ttu-id="cfa14-129">تتم إضافة المورد إلى الفريق، ولكن لا يمكن استهلاك سعة المورد من خلال حجز.</span><span class="sxs-lookup"><span data-stu-id="cfa14-129">The resource is added to the team, but the resource's capacity isn't consumed through a booking.</span></span>

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a><span data-ttu-id="cfa14-130">حجز عضو فريق لتلبية متطلبات الموارد لمورد عام</span><span class="sxs-lookup"><span data-stu-id="cfa14-130">Book a team member to fulfill resource requirements for a generic resource</span></span>

<span data-ttu-id="cfa14-131">في PSA، يمكنك حجز مورد عام في فريق المشروع، ويمكنك تحديد الدور، والسعه المطلوبة، وكيف يتم توزيع هذه السعة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-131">In PSA, you can book a generic resource on a project team, and can specify the role, the required capacity, and how that capacity is distributed.</span></span> <span data-ttu-id="cfa14-132">في متطلب المورد، يمكنك تحديد سمات يتم إقرانها بالمورد العام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-132">On the resource requirement, you can specify attributes that are associated with the generic resource.</span></span> <span data-ttu-id="cfa14-133">تتضمن هذه السمات المهارات المطلوبة والوحدة التنظيمية المفضلة والموارد المفضلة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-133">These attributes include required skills, the preferred organizational unit, and preferred resources.</span></span>

<span data-ttu-id="cfa14-134">اتبع هذه الخطوات لتحديد المهارات المطلوبة في مورد عام لأحد المطورين.</span><span class="sxs-lookup"><span data-stu-id="cfa14-134">Follow these steps to specify required skills on a generic resource for a developer.</span></span>

1. <span data-ttu-id="cfa14-135">من صفحة **المشاريع** ، في علامة التبويب **الفريق** ، حدد **جديد** لحجز مورد عام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-135">On the **Projects** page, on the **Team** tab, select **New** to book a generic resource.</span></span>

    ![تم حجز المورد العام في الفريق](media/Resource-Management-image9.png)

2. <span data-ttu-id="cfa14-137">في طريقة عرض **كافة أعضاء الفريق** ، في العمود **متطلبات المورد** ، حدد الارتباط لإضافة المهارات المطلوبة للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-137">In the **All Team Members** view, in the **Resource Requirement** column, select the link to add required skills for the generic resource.</span></span>

    ![ارتباط المتطلب](media/Resource-Management-image10.png)

3. <span data-ttu-id="cfa14-139">في صفحة **متطلبات المورد** التي تظهر، في شبكة **المهارات** ، حدد علامة الحذف ( **...** ) ثم حدد **إضافة خاصية متطلب جديد** لإضافة المهارات المطلوبة للمطور.</span><span class="sxs-lookup"><span data-stu-id="cfa14-139">On the **Resource Requirement** page that appears, in the **Skills** grid, select the ellipsis ( **...** ) and then select **Add New Requirement Characteristic** to add the required skills for your developer.</span></span>

    ![أمر إضافة خاصية متطلب جديدة](media/Resource-Management-image11.png)

4. <span data-ttu-id="cfa14-141">في مربع حوار **الإنشاء السريع: خاصية المتطلب** التي تظهر، في حقل **الخصائص** ، حدد المهارة المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-141">In the **Quick Create: Requirement Characteristic** dialog box that appears, in the **Characteristic** field, select the required skill.</span></span> <span data-ttu-id="cfa14-142">ثم في الحقل **قيمة التصنيف** ، حدد مستوى الكفاءة لهذه المهارة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-142">Then, in the **Rating value** field, select the proficiency level for that skill.</span></span> <span data-ttu-id="cfa14-143">وأخيرا ، في حقل **متطلبات المورد** ، قم بتعيين المتطلب إلى الموارد المصدر من الوحدات التنظيمية أو حتى الموارد المسماة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-143">Finally, in the **Resource Requirement** field, set the requirement to source resources from organizational units or even named resources.</span></span> <span data-ttu-id="cfa14-144">عند الانتهاء، حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-144">When you've finished, select **Save**.</span></span>

    ![الإنشاء السريع: مربع حوار خصائص المتطلبات](media/Resource-Management-image12.png)

5. <span data-ttu-id="cfa14-146">في صفحة **متطلبات المورد** ، حدد **حجز** لاستيفاء متطلبات المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-146">On the **Resource Requirement** page, select **Book** to fulfill the resource requirement.</span></span>

    ![زر حجز في صفحة متطلبات المورد](media/Resource-Management-image13.png)

    <span data-ttu-id="cfa14-148">يمكنك أيضا تحديد مورد عام في شبكة **كافة أعضاء الفريق** ثم تحديد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-148">You can also select the generic resource in the **All Team Members** grid and then select **Book**.</span></span>

    ![زر حجز أعلى شبكة كافة أعضاء الفريق](media/Resource-Management-image14.png)

    > [!NOTE]
    > <span data-ttu-id="cfa14-150">في هذا المثال، مطلوب 40 ساعة ولكن لا يوجد ساعات محجوزة فعلية، لأن الموارد العامة ليس لها حجوزات.</span><span class="sxs-lookup"><span data-stu-id="cfa14-150">In this example, there are 40 required hours but no actual booked hours, because generic resources don't have bookings.</span></span> <span data-ttu-id="cfa14-151">بالإضافة إلى ذلك، لا توجد ساعات معينة، لأنه تمت إضافة المورد العام مباشرة إلى الفريق.</span><span class="sxs-lookup"><span data-stu-id="cfa14-151">Additionally, there are no assigned hours, because the generic resource was added directly to the team.</span></span> <span data-ttu-id="cfa14-152">ولم تتم إضافتها باستخدام تعيين المهمة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-152">It wasn't added by using task assignment.</span></span>

    <span data-ttu-id="cfa14-153">في صفحة **مساعد الجدولة** ، يمكنك تصفية الموارد المتوفرة بواسطة المتطلبات المحددة في متطلب المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-153">On the **Scheduling Assistant** page, you can filter available resources by the requirements that are specified on the resource requirement.</span></span> <span data-ttu-id="cfa14-154">يتم فرز الموارد وفقا لمعلمات الفرز المحددة في لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-154">Resources are sorted according to the sorting parameters that are specified on the Schedule Board.</span></span>

    ![صفحة مساعد الجدولة](media/Resource-Management-image15.png)

    <span data-ttu-id="cfa14-156">فيما يلي بعض عوامل التصفية التي غالبا ما يتم استخدامها:</span><span class="sxs-lookup"><span data-stu-id="cfa14-156">Here are some filters that are often used:</span></span>

    - <span data-ttu-id="cfa14-157">**الخصائص إلى جانب تصنيف** - تصفية حسب المهارات والشهادات وخواص الموارد الأخرى ، بالإضافة إلى تصنيفات الكفاءة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-157">**Characteristics along with a rating** – Filter by skills, certifications, and other resource qualities, in addition to ratings of proficiency.</span></span>
    - <span data-ttu-id="cfa14-158">**الأدوار** – تصفية حسب الأدوار الافتراضية التي تم تعيينها إلى الموارد القابلة للحجز.</span><span class="sxs-lookup"><span data-stu-id="cfa14-158">**Roles** – Filter by the default roles that are assigned to bookable resources.</span></span>
    - <span data-ttu-id="cfa14-159">**الوحدات التنظيمية** - تصفية الموارد القابلة للحجز حسب الوحدات التنظيمية التي تم تعيينها إليها.</span><span class="sxs-lookup"><span data-stu-id="cfa14-159">**Organizational units** – Filter bookable resources by the organizational units that they are assigned to.</span></span>

6. <span data-ttu-id="cfa14-160">إذا لم تكن راضيا عن نتائج البحث عن الطلبات الأولية، يمكنك تغيير معايير التصفية.</span><span class="sxs-lookup"><span data-stu-id="cfa14-160">If you aren't satisfied with the results of the initial requirement search, you can change the filter criteria.</span></span> <span data-ttu-id="cfa14-161">قم بتوسيع جزء **عرض التصفية** على اليمين، ثم حدد **بحث** للعثور على موارد إضافية.</span><span class="sxs-lookup"><span data-stu-id="cfa14-161">Expand the **Filter View** pane on the left, and then select **Search** to find additional resources.</span></span>

    ![جزء عرض التصفية](media/Resource-Management-image16.png)

7. <span data-ttu-id="cfa14-163">لتغيير طريقة فرز النتائج، حدد **"فرز** ".</span><span class="sxs-lookup"><span data-stu-id="cfa14-163">To change how the results are sorted, select **Sort**.</span></span>

    ![أمر الفرز](media/Resource-Management-image17.png)

8. <span data-ttu-id="cfa14-165">حدد الموارد وفقا للطلب المحدد فى المتطلب، كما هو موضح في الجزء العلوي من الشبكة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-165">Select resources according to the demand that is specified on the requirement, as indicated at the top of the grid.</span></span> <span data-ttu-id="cfa14-166">يمكنك مسح تحديد الخلايا في الشبكة وترك السعة المفتوحة لهذا المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-166">You can clear the selection of cells in the grid and leave that resource capacity open.</span></span> <span data-ttu-id="cfa14-167">يمكن تحديد مورد واحد فقط في كل مرة على أنه محجوز.</span><span class="sxs-lookup"><span data-stu-id="cfa14-167">Only one resource at a time can be selected as booked.</span></span>

9. <span data-ttu-id="cfa14-168">حدد **حجز** لحجز المورد المحدد واترك لوحة الجدولة مفتوحة، ومن ثم يمكنك تحديد موارد إضافية.</span><span class="sxs-lookup"><span data-stu-id="cfa14-168">Select **Book** to book the selected resource and leave the Schedule Board open, so that you can select additional resources.</span></span> <span data-ttu-id="cfa14-169">بدلا من ذلك حدد **حجز وإغلاق** لحجز المورد المحدد وإغلاق لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-169">Alternatively, select **Book & Exit** to book the selected resource and close the Schedule Board.</span></span>

    ![المورد المراد حجزه](media/Resource-Management-image19.png)

    <span data-ttu-id="cfa14-171">تتلقى إعلامًا بشأن الساعات المحجوزة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-171">You receive a notification about booked hours.</span></span> <span data-ttu-id="cfa14-172">تظهر مؤشرات الطلب مقدار الوفاء بمتطلب الحجز ومقدار الفترة المتبقية.</span><span class="sxs-lookup"><span data-stu-id="cfa14-172">The demand indicators show how much the booking requirement is satisfied and how much remains.</span></span> <span data-ttu-id="cfa14-173">يمكنك أيضا الاطلاع على مقدار استهلاك سعة المورد المحدد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-173">You can also see how much of the selected resource's capacity is consumed.</span></span> <span data-ttu-id="cfa14-174">حدد **توسيع** لعرض المزيد من التفاصيل حول حجوزات الموارد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-174">Select **Expand** to view more details about resource bookings.</span></span>

9. <span data-ttu-id="cfa14-175">ارجع إلى طريقة عرض **كافة أعضاء الفريق**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-175">Return to the **All Team Members** view.</span></span> <span data-ttu-id="cfa14-176">في الشبكة، لاحظ أنه قد تم استبدال المورد العام بالمورد المسمى، وتم سرد 40 ساعة كمحجوزة لذلك المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-176">In the grid, notice that the generic resource has been replaced by the named resource, and 40 hours are listed as booked for that resource.</span></span>

    ![شبكة كافة أعضاء الفريق المحدثة](media/Resource-Management-image20.png)

    > [!NOTE]
    > <span data-ttu-id="cfa14-178">لا يتم عرض أي ساعات معينة، لأنه قد تم حجزها مباشرة للفريق.</span><span class="sxs-lookup"><span data-stu-id="cfa14-178">No assigned hours are shown, because they were booked directly on the team.</span></span> <span data-ttu-id="cfa14-179">ولم يتم حجزها باستخدام تعيين المهمة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-179">They weren't booked by using task assignment.</span></span>

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a><span data-ttu-id="cfa14-180">تعيين موارد عامة إلى مهام وإنشاء متطلبات مورد</span><span class="sxs-lookup"><span data-stu-id="cfa14-180">Assign generic resources to tasks and generate resource requirements</span></span>

<span data-ttu-id="cfa14-181">في PSA، يمكنك إنشاء مهام ثم تعيين موارد عامة لها.</span><span class="sxs-lookup"><span data-stu-id="cfa14-181">In PSA, you can create tasks and then assign generic resources to them.</span></span> <span data-ttu-id="cfa14-182">وبهذه الطريقة، يمكن تمثيل طلب المورد بعناصر نائبة أثناء تقدير الجدول والأرقام المالية الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="cfa14-182">In this way, resource demand can be represented by placeholders while you estimate your schedule and financial numbers.</span></span> <span data-ttu-id="cfa14-183">يمكنك بعد ذلك إنشاء متطلبات المورد للموارد العامة وتنفيذها.</span><span class="sxs-lookup"><span data-stu-id="cfa14-183">You can then generate resource requirements for the generic resources and fulfill them.</span></span>

1. <span data-ttu-id="cfa14-184">في صفحة **المشاريع** في علامة التبويب **جدولة** ، حدد **إضافة** لإنشاء مهمة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-184">On the **Projects** page, on the **Schedule** tab, select **Add** to create a task.</span></span>

    ![يتم إنشاء مهمة جديدة](media/Resource-Management-image21.png)

2. <span data-ttu-id="cfa14-186">في حقل **الموارد** ، حدد رمز **منتقي المورد**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-186">In the **Resources** field, select the **Resource Picker** symbol.</span></span> <span data-ttu-id="cfa14-187">يظهر منتقي المورد ويظهر أعضاء الفريق الموجودين للمشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-187">The Resource Picker appears and shows existing team members for the project.</span></span>

    ![منتقي الموارد](media/Resource-Management-image22.png)

3. <span data-ttu-id="cfa14-189">أدخل اسم المورد العام الجديد، ثم حدد **إنشاء.**</span><span class="sxs-lookup"><span data-stu-id="cfa14-189">Enter the name of the new generic resource, and then select **Create**.</span></span>

    ![يتم إدخال اسم المورد العام الجديد](media/Resource-Management-image23.png)

4. <span data-ttu-id="cfa14-191">في مربع حوار **الإنشاء السريع: عضو فريق المشروع** التي تظهر، في حقل **الدور** ، حدد الدور للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-191">In the **Quick Create: Project Team Member** dialog box that appears, in the **Role** field, select the role for the generic resource.</span></span> <span data-ttu-id="cfa14-192">في الحقل **‏‫وحدة تعيين الموارد‬** ، حدد الوحدة التنظيمية للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-192">In the **Resourcing Unit** field, select the organizational unit for the generic resource.</span></span> <span data-ttu-id="cfa14-193">ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-193">Then select **Save**.</span></span>

    ![مربع حوار الإنشاء السريع: عضو فريق المشروع](media/Resource-Management-image24.png)

    <span data-ttu-id="cfa14-195">تم الآن تعيين عضو الفريق العام لتنفيذ المهمة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-195">The generic team member is now assigned to the task.</span></span>

    ![تعيين عضو الفريق العام لتنفيذ المهمة](media/Resource-Management-image25.png)

    <span data-ttu-id="cfa14-197">في علامة التبويب **فريق** ، سوف تري عضو الفريق العام الجديد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-197">On the **Team** tab, you will see the new generic team member.</span></span> <span data-ttu-id="cfa14-198">لاحظ أنه يحتوي فقط على ساعات معينة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-198">Notice that it has only assigned hours.</span></span> <span data-ttu-id="cfa14-199">تمثل هذه الساعات مجموع كافة المهام التي تم تعيينها لعضو الفريق العام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-199">These hours are the sum of all tasks that are assigned to the generic team member.</span></span> <span data-ttu-id="cfa14-200">وليس لدي عضو الفريق العام بعد الساعات المطلوبة أو متطلبات المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-200">The generic team member doesn't yet have required hours or a resource requirement.</span></span>

    ![عضو فريق عام في علامة تبويب الفريق](media/Resource-Management-image26.png)

5. <span data-ttu-id="cfa14-202">يمكنك الآن تعيين عضو الفريق العام إلى المهام الأخرى عن طريق استخدام منتقي المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-202">You can now assign the generic team member to other tasks by using the Resource Picker.</span></span>

    ![عضو فريق عام في منتقي المورد](media/Resource-Management-image27.png)

    <span data-ttu-id="cfa14-204">عند الانتهاء من تعيين المورد العام إلى المهام، يمكنك إنشاء متطلب مورد للمورد العام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-204">When you've finished assigning the generic resource to tasks, you can generate a resource requirement for the generic resource.</span></span>

5. <span data-ttu-id="cfa14-205">في علامة التبويب **الفريق** ، حدد المورد العام ، ثم حدد **إنشاء متطلب**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-205">On the **Team** tab, select the generic resource, and then select **Generate Requirement**.</span></span>

    ![أمر إنشاء متطلب](media/Resource-Management-image28.png)

    <span data-ttu-id="cfa14-207">عند إنشاء المتطلب، سيكون لعضو الفريق العام الساعات المطلوبة وارتباط لمتطلب المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-207">When the requirement is generated, the generic team member will have required hours and a link for the resource requirement.</span></span>

    ![ارتباط متطلب الموارد](media/Resource-Management-image29.png)

    <span data-ttu-id="cfa14-209">بعد حجز مورد مسمى، تتم إزالة المورد العام من الفريق واستبداله بالمورد المسمى.</span><span class="sxs-lookup"><span data-stu-id="cfa14-209">After you book a named resource, the generic resource is removed from the team and replaced by the named resource.</span></span>

    ![تم استبدال المورد العام بالمورد المسمى](media/Resource-Management-image30.png)

    <span data-ttu-id="cfa14-211">في علامة التبويب **جدولة** ، تتم إزالة تعيينات الموارد العامة واستبدالها بالمورد المسمى.</span><span class="sxs-lookup"><span data-stu-id="cfa14-211">On the **Schedule** tab, the generic resource assignments are removed and replaced by the named resource.</span></span>

    ![يتم استبدال تعيينات الموارد العامة بالمورد المسمى في علامة التبويب جدولة.](media/Resource-Management-image31.png)

    > [!NOTE]
    > <span data-ttu-id="cfa14-213">يحدث هذا السلوك فقط عندما يكون المورد المسمى محجوزًا بالكامل لمتطلبات المورد العام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-213">This behavior occurs only when a named resource is fully booked for the generic resource requirement.</span></span> <span data-ttu-id="cfa14-214">عندما يستبدل مورد مسمى متطلب مورد عام جزئيًا أو عندما يستبدل عدة موارد مسماء متطلب مورد عام، يبقي المورد العام معينا للمهمة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-214">When either a named resource partially replaces the generic resource requirement or multiple named resources replace the generic resource requirement, the generic resource remains assigned to the task.</span></span>

    <span data-ttu-id="cfa14-215">في التوضيح التالي، تم تخطيط مهمة 80 ساعة لمدة خمسة أيام (16 ساعة في اليوم خلال خمسة أيام) ومعينه إلى المورد العام الذي يحمل اسم **وظيفي**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-215">In the following illustration, an 80-hour task has been planned for a five-day duration (16 hours per day over five days) and assigned to the generic resource that is named **Functional**.</span></span>

    ![تم تعيين مهمة ثماني ساعات، لمدة خمسة أيام المورد العام الوظيفي](media/Resource-Management-image32.png)

    <span data-ttu-id="cfa14-217">عندما تقوم بإنشاء المتطلب، فانه يكون لمدة 80 ساعة خلال خمسة أيام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-217">When you generate the requirement, it's for 80 hours over five days.</span></span>

    ![تم إنشاء المتطلب لمدة 80 ساعة خلال خمسة أيام](media/Resource-Management-image33.png)

    <span data-ttu-id="cfa14-219">ونظرا لأن الموارد المتوفرة تعمل فقط لمدة ثمان ساعات في اليوم، يلزم وجود موردين لتنفيذ المتطلب.</span><span class="sxs-lookup"><span data-stu-id="cfa14-219">Because available resources work only eight hours per day, two resources are needed to fulfill the requirement.</span></span>

    ![المورد الثاني](media/Resource-Management-image35.png)

    <span data-ttu-id="cfa14-221">في علامة التبويب **الفريق** ، يمكنك الآن رؤية أن المورد العام ليس له ساعات مطلوبة، ولكن الساعات المعينة لا تزال تظهر معا مع موردين مسميين اللذين يشكلان الاستيفاء.</span><span class="sxs-lookup"><span data-stu-id="cfa14-221">On the **Team** tab, you can now see that the generic resource has no required hours, but the assigned hours still appear together with the two named resources that make up the fulfillment.</span></span>

    ![موردان مسميان في علامة تبويب الفريق](media/Resource-Management-image36.png)

    <span data-ttu-id="cfa14-223">في علامة التبويب **جدولة** ، يبقي المورد العام معينا للمهمة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-223">On the **Schedule** tab, the generic resource remains assigned to the task.</span></span>

    ![الموارد العامة في علامة التبويب جدولة](media/Resource-Management-image37.png)

<span data-ttu-id="cfa14-225">لا يعين PSA كلا الموردين للمهمة، وذلك لأن ذلك السلوك قد ينتج عنه جدولة أقل توقعا.</span><span class="sxs-lookup"><span data-stu-id="cfa14-225">PSA doesn't assign both resources to the task, because that behavior would produce a less predictable schedule.</span></span> <span data-ttu-id="cfa14-226">في هذا المثال البسيط، من السهل تقسيم الساعات بالتساوي بين موردين.</span><span class="sxs-lookup"><span data-stu-id="cfa14-226">In this simple example, it's easy to divide the hours equally between two resources.</span></span> <span data-ttu-id="cfa14-227">ومع ذلك، في السيناريوهات الأكثر تعقيدا التي تتضمن العديد من المهام والموارد المتعددة، فإنه يتعين على PSA اتخاذ افتراضات حول كيفية تخصيص الحجوزات التي يتم تلقيها لموارد متعددة عبر العديد من المهام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-227">However, in more complex scenarios that involve multiple tasks and multiple resources, PSA would have to make assumptions about how it should allocate the bookings that are received for multiple resources across multiple tasks.</span></span>

<span data-ttu-id="cfa14-228">بالتالي، في هذه السيناريوهات، يتولى مدير المشروع مسؤولية تحليل الحجوزات المتعددة وتعيينها حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-228">Therefore, in these scenarios, the project manager is responsible for parsing the multiple bookings and assigning them as needed.</span></span> <span data-ttu-id="cfa14-229">لتوزيع الحجوزات، يقوم مدير المشروع بتعيين المهام من الموارد العامة إلى الموارد المسماة ثم يستخدم طريقه عرض **التسوية** للتأكد من أن التوزيع يتماشى مع الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="cfa14-229">To allocate the bookings, the project manager assigns the tasks from the generic resources to the named resources and then uses the **Reconciliation** view to make sure that the allocation works with the bookings.</span></span>

### <a name="edit-a-resource-requirement"></a><span data-ttu-id="cfa14-230">تحرير متطلبات مورد</span><span class="sxs-lookup"><span data-stu-id="cfa14-230">Edit a resource requirement</span></span>

<span data-ttu-id="cfa14-231">بعد إنشاء متطلبات مورد، قد يرغب مدير المشروع أو مدير الموارد في تحرير التفاصيل لتنقيح معايير البحث عند استخدام لوحة الجدولة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-231">After a resource requirement has been created, a project manager or resource manager might want to edit the details to refine the search criteria when the Schedule Board is used.</span></span> <span data-ttu-id="cfa14-232">لتحرير متطلبات المورد، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="cfa14-232">To edit the resource requirement, follow these steps.</span></span>

1. <span data-ttu-id="cfa14-233">من صفحة **المشاريع** ، في علامة التبويب **الفريق** ، حدد الارتباط لأي متطلب في مورد عام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-233">On the **Projects** page, on the **Team** tab, select the link to any requirement on a generic resource.</span></span>
2. <span data-ttu-id="cfa14-234">في صفحة **متطلبات المورد** التي تظهر، يمكنك تحديث سمات متعددة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-234">On the **Resource Requirement** page that appears, you can update several attributes.</span></span> <span data-ttu-id="cfa14-235">وإليك بعض الأمثلة:</span><span class="sxs-lookup"><span data-stu-id="cfa14-235">Here are some examples:</span></span>

    - <span data-ttu-id="cfa14-236">الاسم</span><span class="sxs-lookup"><span data-stu-id="cfa14-236">Name</span></span>
    - <span data-ttu-id="cfa14-237">من تاريخ</span><span class="sxs-lookup"><span data-stu-id="cfa14-237">From Date</span></span>
    - <span data-ttu-id="cfa14-238">إلى التاريخ</span><span class="sxs-lookup"><span data-stu-id="cfa14-238">To Date</span></span>
    - <span data-ttu-id="cfa14-239">المدة</span><span class="sxs-lookup"><span data-stu-id="cfa14-239">Duration</span></span>
    - <span data-ttu-id="cfa14-240">نوع المورد</span><span class="sxs-lookup"><span data-stu-id="cfa14-240">Resource Type</span></span>

<span data-ttu-id="cfa14-241">في صفحة **"متطلبات المورد** ، يمكن لمدير المشروع أو مدير الموارد تعريف المعلومات التالية أيضا:</span><span class="sxs-lookup"><span data-stu-id="cfa14-241">On the **Resource Requirement** page, the project manager or resource manager can also define the following information:</span></span>

- <span data-ttu-id="cfa14-242">المهارات</span><span class="sxs-lookup"><span data-stu-id="cfa14-242">Skills</span></span>
- <span data-ttu-id="cfa14-243">الأدوار</span><span class="sxs-lookup"><span data-stu-id="cfa14-243">Roles</span></span>
- <span data-ttu-id="cfa14-244">تفضيلات الموارد</span><span class="sxs-lookup"><span data-stu-id="cfa14-244">Resource preferences</span></span>
- <span data-ttu-id="cfa14-245">الوحدات التنظيمية المفضلة</span><span class="sxs-lookup"><span data-stu-id="cfa14-245">Preferred organizational unit</span></span>

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a><span data-ttu-id="cfa14-246">تحديث حجوزات الموارد بعد حجزها في مشروع</span><span class="sxs-lookup"><span data-stu-id="cfa14-246">Update resource bookings after they are booked on a project</span></span>

<span data-ttu-id="cfa14-247">بعد إضافة مورد عام أو مسمى إلى فريق مشروع، يمكنك تغيير حجوزات المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-247">After you've added a generic or named resource to a project team, you can change the resource's bookings.</span></span>

1. <span data-ttu-id="cfa14-248">في صفحة **المشاريع** ، في علامة تبويب **الفريق** ، حدد عضو الفريق، ثم حدد **المحافظة على الحجوزات**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-248">On the **Projects** page, on the **Team** tab, select a team member, and then select **Maintain Bookings**.</span></span>

    ![يتم فتح لوحة الجدولة لعضو الفريق المحدد](media/Resource-Management-image40.png)

    <span data-ttu-id="cfa14-250">تظهر لوحة الجدولة وتظهر حجوزات عضو فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-250">The Schedule Board appears and shows the project team member's bookings.</span></span> <span data-ttu-id="cfa14-251">قم بتوسيع سجل عضو الفريق لعرض الساعات التي تم حجزها مقابل هذا المشروع والمشاريع الأخرى التي تستهلك سعة عضو الفريق.</span><span class="sxs-lookup"><span data-stu-id="cfa14-251">Expand the team member's record to view the hours that have been booked against this project and other projects that are consuming the team member's capacity.</span></span>

2. <span data-ttu-id="cfa14-252">حدد الحجز واسحبه لإطالته أو تقصيره.</span><span class="sxs-lookup"><span data-stu-id="cfa14-252">Select and drag the booking to extend or shorten it.</span></span> <span data-ttu-id="cfa14-253">يظهر مربع الحوار **إنشاء حجز مورد** الذي يتيح لك إمكانية تعديل الحجز.</span><span class="sxs-lookup"><span data-stu-id="cfa14-253">A **Create Resource Booking** dialog box appears that lets you adjust the booking.</span></span>

    ![مربع حوار إنشاء حجز مورد](media/Resource-Management-image41.png)

3. <span data-ttu-id="cfa14-255">انقر بزر الماوس الأيمن فوق الحجز.</span><span class="sxs-lookup"><span data-stu-id="cfa14-255">Right-click the booking.</span></span> <span data-ttu-id="cfa14-256">يمكنك بعد ذلك استخدام القائمة المختصرة لإكمال الإجراءات التالية:</span><span class="sxs-lookup"><span data-stu-id="cfa14-256">You can then use the shortcut menu to complete the following actions:</span></span>

    - <span data-ttu-id="cfa14-257">قم بتغيير حالة الحجز.</span><span class="sxs-lookup"><span data-stu-id="cfa14-257">Change the booking status.</span></span>
    - <span data-ttu-id="cfa14-258">حرر الحجز.</span><span class="sxs-lookup"><span data-stu-id="cfa14-258">Edit the booking.</span></span>
    - <span data-ttu-id="cfa14-259">استبدال مورد بفريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-259">Substitute a resource on the project team.</span></span>

### <a name="change-the-booking-status"></a><span data-ttu-id="cfa14-260">قم بتغيير حالة الحجز</span><span class="sxs-lookup"><span data-stu-id="cfa14-260">Change the booking status</span></span>

<span data-ttu-id="cfa14-261">يمكنك تغيير أي حالة حجز افتراضية أو مخصصة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-261">You can change any default or custom booking status.</span></span>

![أمر تغيير الحالة](media/Resource-Management-image42.png)

<span data-ttu-id="cfa14-263">يتم تضمين الحالات التالية في PSA:</span><span class="sxs-lookup"><span data-stu-id="cfa14-263">The following statuses are included in PSA:</span></span>

- <span data-ttu-id="cfa14-264">**تم الإلغاء** – تلغي هذه الحالة حجز مورد وتحرر سعة المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-264">**Canceled** – This status cancels a resource's booking and frees up the resource's capacity.</span></span>
- <span data-ttu-id="cfa14-265">**حجز محدد** – تستهلك هذه الحالة سعة المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-265">**Hard Book** – This status consumes a resource's capacity.</span></span> <span data-ttu-id="cfa14-266">وعادة ما يكون الحجز بهذه الحالة عند فتح **المحافظة على الحجوزات** من شبكة **كافة أعضاء الفريق** في صفحة **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-266">A booking typically has this status when you open **Maintain Bookings** from the **All Team Members** grid on the **Projects** page.</span></span>
- <span data-ttu-id="cfa14-267">**حجز مبدئي** – تقوم هذه الحالة بإضافة مورد إلى فريق ولكنه لا يستهلك سعة المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-267">**Soft Book** – This status adds a resource to a team but doesn't consume the resource's capacity.</span></span> <span data-ttu-id="cfa14-268">ويشير إلى أن المورد قد تم حجزه للعمل المحتمل ولكنه لا يزال يحتوي على سعة إذا كانت مطلوبة في الوظائف الأخرى.</span><span class="sxs-lookup"><span data-stu-id="cfa14-268">It indicates that the resource has been reserved for potential work but still has capacity if it's needed on other jobs.</span></span> <span data-ttu-id="cfa14-269">في طريقة عرض إتاحة الموارد الكلية، تكون عمليات الحجز المبدئية بحالة مختلفة عن الحجوزات المحددة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-269">In the view of overall resource availability, soft bookings have a different status than hard bookings.</span></span>
- <span data-ttu-id="cfa14-270">**مقترح** -هذه الحالة تمثل اقتراحًا من مدير المورد أو مدير المشروع لأحد الموارد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-270">**Proposed** – This status represents a resource manager's or project manager's proposal for a resource.</span></span> <span data-ttu-id="cfa14-271">لا تستهلك الاقتراحات سعة المورد، ولا تتم إضافة المورد إلى فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-271">Proposals don't consume the capacity of a resource, and the resource isn't added to the project team.</span></span> <span data-ttu-id="cfa14-272">لحجز مورد بشكل محدد في فريق، يجب أن يقبل مدير المشروع الاقتراح.</span><span class="sxs-lookup"><span data-stu-id="cfa14-272">To hard-book the resource on the team, the project manager must accept the proposal.</span></span>

### <a name="submit-resource-requests"></a><span data-ttu-id="cfa14-273">إرسال طلبات الموارد</span><span class="sxs-lookup"><span data-stu-id="cfa14-273">Submit resource requests</span></span>

<span data-ttu-id="cfa14-274">تُستخدم طلبات المورد لتنفيذ الطلب (متطلب المورد) الذي يجب تحقيقه بواسطة مدير الموارد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-274">Resource requests are used to carry the demand (resource requirement) that must be fulfilled by a resource manager.</span></span> <span data-ttu-id="cfa14-275">في حالة وجود مورد عام بالفعل في الفريق، يمكنك إرسال طلب مورد مباشرة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-275">For a generic resource that is already on the team, you can submit a resource request directly.</span></span> <span data-ttu-id="cfa14-276">يمكن استيفاء طلب مورد بطريقتين:</span><span class="sxs-lookup"><span data-stu-id="cfa14-276">A resource request can be fulfilled in two ways:</span></span>

- <span data-ttu-id="cfa14-277">يستوفي مدير الموارد الطلب مباشرة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-277">The resource manager directly fulfills the request.</span></span> <span data-ttu-id="cfa14-278">في هذه الحالة، يتم استبدال المورد العام بحجز محدد له مورد مسمى.</span><span class="sxs-lookup"><span data-stu-id="cfa14-278">In this case, the generic resource is replaced by a hard booking that has a named resource.</span></span>
- <span data-ttu-id="cfa14-279">يقترح مدير الموارد موردًا لمدير المشروع، ويوافق مدير المشروع أو يرفض المورد المقترح.</span><span class="sxs-lookup"><span data-stu-id="cfa14-279">The resource manager proposes a resource to the project manager, and the project manager approves or rejects the proposed resource.</span></span>

#### <a name="direct-fulfillment-of-resource-requests"></a><span data-ttu-id="cfa14-280">الاستيفاء المباشر لطلبات الموارد</span><span class="sxs-lookup"><span data-stu-id="cfa14-280">Direct fulfillment of resource requests</span></span>

<span data-ttu-id="cfa14-281">عندما يتم إنشاء متطلب مورد، يمكن لمدير المشروع إرسال طلب مورد لمورد عام من خلال تحديد المورد ثم تحديد **إرسال طلب**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-281">When a resource requirement is generated, a project manager can submit a resource request for a generic resource by selecting the resource and then selecting **Submit Request**.</span></span>

![زر إرسال الطلب](media/Resource-Management-image45.png)

<span data-ttu-id="cfa14-283">ويمكن توفير تعليقات حول المورد لمدير الموارد الذي يستوفي الطلب.</span><span class="sxs-lookup"><span data-stu-id="cfa14-283">Comments about the resource can be provided to the resource manager who is fulfilling the request.</span></span> <span data-ttu-id="cfa14-284">بعد إرسال الطلب، يتغير حقل **الحالة** لعضو الفريق إلى **تم الإرسال**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-284">After the request is submitted, the **Status** field for the team member is changed to **Submitted**.</span></span>

![إدخال تعليقات اختيارية](media/Resource-Management-image46.png)

<span data-ttu-id="cfa14-286">عندما يقوم مدير الموارد باستيفاء الطلب، يتم استبدال عضو الفريق العام بالمورد المسمى في شبكة **كافة أعضاء الفريق**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-286">When the resource manager fulfills the request, the generic team member is replaced by the named resource in the **All Team Members** grid.</span></span>

![تم استبدال عضو الفريق العام بالمورد المسمى في شبكة كافة أعضاء الفريق](media/Resource-Management-image47.png)

#### <a name="use-a-resource-proposal-for-resource-requests"></a><span data-ttu-id="cfa14-288">استخدام مقترح مورد لطلبات الموارد</span><span class="sxs-lookup"><span data-stu-id="cfa14-288">Use a resource proposal for resource requests</span></span>

<span data-ttu-id="cfa14-289">بدلا من حجز مورد في طلب مورد مباشرة، يمكن لمدير الموارد اقتراح مورد إلى مدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-289">Instead of directly booking a resource on a resource request, a resource manager can propose a resource to the project manager.</span></span> <span data-ttu-id="cfa14-290">قد يستخدم مدير الموارد هذا الخيار عندما يكون التطابق التام للمتطلبات غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="cfa14-290">A resource manager might use this option when an exact match for the requirements isn't available.</span></span> <span data-ttu-id="cfa14-291">عندما يقترح مدير الموارد موردًا ما، فإن مدير المشروع يري أن حقل **الحالة** لعضو الفريق العام قد تغير إلى **يحتاج إلى المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-291">When a resource manager proposes a resource, the project manager sees that the **Status** field for the generic team member is changed to **Needs Review**.</span></span>

![تم تغيير حالة عضو الفريق العام إلى يحتاج إلى المراجعة](media/Resource-Management-image48.png)

<span data-ttu-id="cfa14-293">لعرض المورد المقترح مع مرئيات تأثير حجز المقترح، انقر نقرا مزدوجا فوق عضو الفريق الذي بالحالة **يحتاج إلى مراجعة**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-293">To view the proposed resource together with a visualization of the effect of the proposal's booking, double-click the team member that has a status of **Needs Review**.</span></span> <span data-ttu-id="cfa14-294">ثم حدد علامة التبويب **الموارد المقترحة**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-294">Then select the **Proposed Resources** tab.</span></span>

![علامة تبويب الموارد المقترحة](media/Resource-Management-image49.png)

<span data-ttu-id="cfa14-296">حدد **قبول كافة المقترحات** لقبول كافة الموارد المقترحة أو **رفض كافة المقترحات** لرفضها.</span><span class="sxs-lookup"><span data-stu-id="cfa14-296">Select **Accept All Proposals** to accept all proposed resources or **Reject All Proposals** to reject them.</span></span> <span data-ttu-id="cfa14-297">إذا قمت بقبول الموارد المقترحة، سيتم حجزها بشكل محدد في المشروع كأعضاء فريق واستبدال الموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-297">If you accept the proposed resources, they are hard-booked on the project as team members and replace the generic resources.</span></span>

> [!NOTE]
> <span data-ttu-id="cfa14-298">يجب عليك إما قبول كافة الموارد المقترحة أو رفضها.</span><span class="sxs-lookup"><span data-stu-id="cfa14-298">You must either accept or reject all proposed resources.</span></span> <span data-ttu-id="cfa14-299">لا يمكنك قبولها أو رفضها جزئيا.</span><span class="sxs-lookup"><span data-stu-id="cfa14-299">You can't partially accept or reject them.</span></span>

### <a name="substitute-a-resource-on-the-project-team"></a><span data-ttu-id="cfa14-300">استبدال مورد في فريق المشروع</span><span class="sxs-lookup"><span data-stu-id="cfa14-300">Substitute a resource on the project team</span></span>

<span data-ttu-id="cfa14-301">في بعض الأحيان، يجب أن يقوم مدير المشروع باستبدال عضو فريق محجوز في أحد المشاريع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-301">Sometimes, a project manager must substitute a booked team member on a project.</span></span>

1. <span data-ttu-id="cfa14-302">في صفحة **المشاريع** ، في علامة تبويب **الفريق** ، حدد المورد الذي يحتاج إلى استبدال، ثم حدد **المحافظة على الحجوزات**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-302">On the **Projects** page, on the **Team** tab, select the resource that needs a substitute, and then select **Maintain Bookings**.</span></span>
2. <span data-ttu-id="cfa14-303">قم بتوسيع المورد لعرض المشروعات التي تم تعيينها إليه.</span><span class="sxs-lookup"><span data-stu-id="cfa14-303">Expand the resource to view the projects that it's assigned to.</span></span>

    ![تم توسيع المورد لإظهار المشروعات المعينة](media/Resource-Management-image50.png)

3. <span data-ttu-id="cfa14-305">انقر بزر الماوس الأيمن فوق المشروع، ثم حدد **استبدال المورد**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-305">Right-click the project, and then select **Substitute Resource**.</span></span>
4. <span data-ttu-id="cfa14-306">إذا كنت تعرف المورد الذي تريد استبداله بالمورد الحالي، فحدد أو اكتب الاسم، ثم حدد **إعادة تعيين**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-306">If you know the resource that you want to substitute for the current resource, select or type the name, and then select **Re-assign**.</span></span>

    ![تحديد مورد بديل](media/Resource-Management-image51.png)

    <span data-ttu-id="cfa14-308">بدلا من ذلك، اتبع هذه الخطوات للبحث عن مورد:</span><span class="sxs-lookup"><span data-stu-id="cfa14-308">Alternatively, follow these steps to search for a resource:</span></span>

    1. <span data-ttu-id="cfa14-309">حدد **‏‏بحث عن بديل**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-309">Select **Find Substitution**.</span></span>

        ![البحث عن مورد بديل](media/Resource-Management-image52.png)

        <span data-ttu-id="cfa14-311">يقوم مساعد الجدولة بإرجاع قائمة بالبدائل المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-311">The Schedule Assistant returns a list of available substitutes.</span></span> <span data-ttu-id="cfa14-312">في مساعد الجدولة، يمكنك أيضا تصفية الموارد المتوفرة للعثور على بديل مناسب.</span><span class="sxs-lookup"><span data-stu-id="cfa14-312">In the Schedule Assistant, you can further filter the available resources to find a suitable substitute.</span></span>

        ![قائمة بالبدائل المتوفرة.](media/Resource-Management-image53.png)

    2. <span data-ttu-id="cfa14-314">لاستبدال المورد، حدد المورد الذي تريده، ثم حدد **استبدال**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-314">To substitute the resource, select the resource that you want, and then select **Substitute**.</span></span>

        ![استبدال المورد المحدد](media/Resource-Management-image54.png)

    <span data-ttu-id="cfa14-316">ويتم استبدال الحجوزات والتعيينات بالمورد الجديد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-316">The bookings and assignments are substituted with the new resource.</span></span>

    ![الحجوزات والتعيينات المستبدلة بالمورد الجديد](media/Resource-Management-image55.png)

## <a name="reconcile-team-member-bookings-and-assignments"></a><span data-ttu-id="cfa14-318">تسوية حجوزات وتعيينات عضو الفريق</span><span class="sxs-lookup"><span data-stu-id="cfa14-318">Reconcile team member bookings and assignments</span></span>

<span data-ttu-id="cfa14-319">بالنسبة لأعضاء الفريق، تكون لا الحجوزات والتعيينات مقترنة بدقة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-319">For team members, bookings and assignments are loosely coupled.</span></span> <span data-ttu-id="cfa14-320">بمعنى آخر، يمكن أن يكون للموارد تعيينات وليس ليها حجوزات، أو يمكن أن يكون لها حجوزات وليس تعيينات.</span><span class="sxs-lookup"><span data-stu-id="cfa14-320">In other words, resources can have assignments but no bookings, or they can have bookings but no assignments.</span></span> <span data-ttu-id="cfa14-321">وبشكل مثالي، يجب انسجام الحجوزات والتعيينات، بحيث تكون الموارد ذات سعة مخصصة لأداء تعيينات المهام الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="cfa14-321">Ideally, bookings and assignments should be aligned, so that resources have committed capacity to perform the task assignments.</span></span> <span data-ttu-id="cfa14-322">ومع ذلك، فان الحجوزات قد تكون مستندة إلى التوفر ، وقد تتغير توقيتات المهام نظرًا لاستمرار المشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-322">However, the bookings might be based on availability, and task timings might change as the project continues.</span></span> <span data-ttu-id="cfa14-323">لذا، فان الإقران غير الدقيق للحجوزات والتعيينات يوفر المرونة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-323">Therefore, the loose coupling of bookings and assignments provides flexibility.</span></span>

<span data-ttu-id="cfa14-324">يتضمن PSA علامة تبويب **التسوية** التي تتيح مديري المشاريع تسوية حجوزات أعضاء الفريق وتعييناتهم لفريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-324">PSA has a **Reconciliation** tab that lets project managers reconcile team members' bookings and their assignments for project teams.</span></span>

![علامة تبويب التسوية](media/Resource-Management-image56.png)

<span data-ttu-id="cfa14-326">تعرض علامة التبويب **التسوية** الحجوزات والتعيينات وصولاً إلى تعيين المهمة الفردية لكل عضو فريق.</span><span class="sxs-lookup"><span data-stu-id="cfa14-326">The **Reconciliation** tab shows bookings and assignments down to the level of the individual task assignment for each team member.</span></span> <span data-ttu-id="cfa14-327">وتعرض الساعات الموجودة في الخلايا والتي تمثل فترات زمنية من الشهور إلى الأيام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-327">It shows hours in cells that represent time periods from months down to days.</span></span>

<span data-ttu-id="cfa14-328">كما تُظهر علامة التبويب أيضا الإجمالي الصافي الكلي للمشروع، مع عمود الإجمالي.</span><span class="sxs-lookup"><span data-stu-id="cfa14-328">The tab also shows an overall net total for the project, together with a total column.</span></span>

<span data-ttu-id="cfa14-329">بالنسبة لكل مورد، تحسب علامة التبويب الفرق بين حجوزات عضو الفريق والقيمة المحتسبة لتعيينات مهمة عضو الفريق.</span><span class="sxs-lookup"><span data-stu-id="cfa14-329">For each resource, the tab calculates the difference between the team member's bookings and a rollup of the team member's task assignments.</span></span> <span data-ttu-id="cfa14-330">وبشكل مثالي، يجب أن يكون هذا الفرق 0 (صفر).</span><span class="sxs-lookup"><span data-stu-id="cfa14-330">Ideally, this difference should be 0 (zero).</span></span> <span data-ttu-id="cfa14-331">وبمعنى آخر، لا ينبغي أن يكون هناك اختلاف بين الحجوزات والتعيينات.</span><span class="sxs-lookup"><span data-stu-id="cfa14-331">In other words, there should be no difference between bookings and assignments.</span></span> <span data-ttu-id="cfa14-332">يتم تلوين الاختلافات وتظليلها للفت الانتباه إلى حالتين:</span><span class="sxs-lookup"><span data-stu-id="cfa14-332">Differences are colored and shaded to draw attention to two conditions:</span></span>

- <span data-ttu-id="cfa14-333">**نقص الحجز** – يحدث نقص الحجز عندما يحتوي مورد على تعيينات أكثر من الحجوزات.</span><span class="sxs-lookup"><span data-stu-id="cfa14-333">**Booking shortage** – A booking shortage occurs when a resource has more assignments than bookings.</span></span> <span data-ttu-id="cfa14-334">ونظرًا لأنه لم يتم حجز هذه السعة، فقد يحتاج مدير المشروع إلى تصحيح هذا الشرط من خلال توسيع حجوزات المورد لتغطيه العجز.</span><span class="sxs-lookup"><span data-stu-id="cfa14-334">Because this capacity hasn't been reserved, a project manager might want to correct this condition by extending the resource's bookings to cover the deficit.</span></span>
- <span data-ttu-id="cfa14-335">**الحجوزات الزائدة** - تحدث الحجوزات الزائدة عندما يتم حجز مورد للمشروع ولكن لم يتم تعيينه إلى المهام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-335">**Excess bookings** – Excess bookings occur when a resource has been booked to the project but hasn't been assigned to tasks.</span></span> <span data-ttu-id="cfa14-336">قد يكون هذا الشرط مقبولا في الحالات التي تم فيها حجز المورد إلى المشروع قبل حدوث تعيين المهمة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-336">This condition might be acceptable in the cases where the resource was booked to the project before task assignment occurred.</span></span> <span data-ttu-id="cfa14-337">ومع ذلك، في حالات أخرى، لا يتم تخطيط المورد ليتم تعيينه إلى المهام.</span><span class="sxs-lookup"><span data-stu-id="cfa14-337">However, in other cases, the resource isn't planned to be assigned to tasks.</span></span> <span data-ttu-id="cfa14-338">وفي هذه الحالات، يتعين على مدير المشروع الأخذ في الاعتبار إلغاء حجوزات المورد، وبذلك يمكن استخدام السعة لمشروع آخر.</span><span class="sxs-lookup"><span data-stu-id="cfa14-338">In these cases, the project manager should consider canceling the resource's bookings, so that the capacity can be used for another project.</span></span>

<span data-ttu-id="cfa14-339">في بعض الحالات، عندما تعرض الوقت على مستوى أعلى من مستوى اليوم (على سبيل المثال، مستوى الشهر)، ربما تشاهد صافي فرق الصفر لأحد الموارد (بمعنى آخر، الحجوزات = التعيينات).</span><span class="sxs-lookup"><span data-stu-id="cfa14-339">In some cases, when you view time at a higher level than the day level (for example, the month level), you might see a net difference of zero for a resource (in other words, bookings = assignments).</span></span> <span data-ttu-id="cfa14-340">ومع ذلك، إذا استعرضت الوقت بمستوى الأسبوع، فقد ترى أن هناك تعيينات من 0 (صفر) وحجوزات تصل إلى 40 ساعة في الأسبوع الأول، ولكن التعيينات لمدة 40 ساعة وحجوزات من 0 (صفر) في الأسبوع الثاني.</span><span class="sxs-lookup"><span data-stu-id="cfa14-340">However, if you view time at the week level, you might see that there are assignments of zero hours and bookings of 40 hours in the first week, but assignments of 40 hours and bookings of zero hours in the second week.</span></span> <span data-ttu-id="cfa14-341">وبشكل عام، يتم تسوية الحجوزات والتعيينات، ولكنها تختلف من أسبوع للأسبوع التالي.</span><span class="sxs-lookup"><span data-stu-id="cfa14-341">Overall, the bookings and assignments are reconciled, but they differ from one week to the next.</span></span>

<span data-ttu-id="cfa14-342">عند عرض الوقت بمستويات أعلى، فإن الخلايا في علامة التبويب **التسوية** تتضمن مؤشرًا لإعلامك بوجود اختلافات على المستويات الأقل.</span><span class="sxs-lookup"><span data-stu-id="cfa14-342">When you view time at higher levels, cells in the **Reconciliation** tab have an indicator to inform you that there are differences at lower levels.</span></span> <span data-ttu-id="cfa14-343">ومن خلال النقر المزدوج فوق الخلية، يمكنك التكبير لعرض الفرق.</span><span class="sxs-lookup"><span data-stu-id="cfa14-343">By double-clicking in a cell, you can zoom in to view the difference.</span></span> <span data-ttu-id="cfa14-344">يمكنك بعد ذلك النقر بزر الماوس الأيمن للتصغير. ومن خلال تحديد مورد ثم استخدام عنصر التحكم **الفرق التالي** على شريط أدوات الشبكة، يمكنك الانتقال إلى الفرق التالي بين الحجوزات والتعيينات لذلك المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-344">You can then right-click to zoom out. By selecting a resource and then using the **Next difference** control on the grid toolbar, you can go to the next difference between bookings and assignments for that resource.</span></span> <span data-ttu-id="cfa14-345">يمكنك بعد ذلك استخدام عنصر تحكم **الفرق السابق** للرجوع.</span><span class="sxs-lookup"><span data-stu-id="cfa14-345">You can then use the **Previous difference** control to go back.</span></span> <span data-ttu-id="cfa14-346">كما يمكنك إيقاف تشغيل مؤشر الفرق وسلوك التنقل تحت **الإعدادات**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-346">You can also turn off the difference indicator and navigation behavior under **Settings**.</span></span>

![مؤشر الفرق](media/Resource-Management-image57.png)

<span data-ttu-id="cfa14-348">إذا كان لديك تعيينات مهمة لمورد ولكن بدون حجوزات، ففي صفحة **المشاريع** ، في علامة تبويب **التسوية** ، حدد عجز الحجز، ثم حدد **توسيع الحجز**.</span><span class="sxs-lookup"><span data-stu-id="cfa14-348">If you have task assignments for a resource but no bookings, on the **Projects** page, on the **Reconciliation** tab, select the booking shortage, and then select **Extend Booking**.</span></span> <span data-ttu-id="cfa14-349">يُظهر مربع الحوار **توسيع الحجز** ويعض الحجز المطلوب لمعالجة نقص المورد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-349">The **Extend Booking** dialog box appears and shows the booking that is needed to address the resource's shortage.</span></span> <span data-ttu-id="cfa14-350">كما يوضح أيضا الحجوزات الموجودة للمورد عبر كافة المشروعات أو الكيانات الأخرى القابلة للجدولة.</span><span class="sxs-lookup"><span data-stu-id="cfa14-350">It also shows the resource's existing bookings across all projects or other schedulable entities.</span></span> <span data-ttu-id="cfa14-351">إذا قمت بتحديد **موافق** لإنشاء الحجز للمورد، بغض النظر عن مدى توافر ذلك المورد، فقد تتسبب في الحجز الزائد.</span><span class="sxs-lookup"><span data-stu-id="cfa14-351">If you select **OK** to create the booking for the resource, regardless of that resource's availability, you might cause overbooking.</span></span>

![مربع الحوار توسيع الحجز](media/Resource-Management-image58.png)

<span data-ttu-id="cfa14-353">يستطيع مدير المشروع أو مدير المورد استخدام لوحة الجدولة بعد ذلك لإدارة أي حالات يكون فيها المورد محجوزًا بشكل زائد بحيث يتجاوز السعة الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="cfa14-353">The project manager or resource manager can then use the Schedule Board to manage any situations where a resource is overbooked beyond its capacity.</span></span>
