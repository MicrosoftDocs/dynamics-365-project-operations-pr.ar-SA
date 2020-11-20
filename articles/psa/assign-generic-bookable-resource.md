---
title: تعيين موارد عامة قابل للحجز إلى مهمة وفريق مشروع
description: يوفر هذا الموضوع معلومات حول حجز الموارد العامة للمهام وفرق المشروع.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: 19761b3e570ad664522e832069a8ac50fffead64
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127052"
---
# <a name="assign-generic-bookable-resources-to-a-task-and-generate-resource-requirements"></a><span data-ttu-id="42aac-103">تعيين موارد عامة قابل للحجز إلى مهمة وإنشاء متطلبات مورد</span><span class="sxs-lookup"><span data-stu-id="42aac-103">Assign generic bookable resources to a task and generate resource requirements</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="42aac-104">بالاضافه إلى حجز وتعيين الموارد الفعلية أو المسماة إلى المشروع، يمكنك تعيين موارد عامة لمهام المشروع.</span><span class="sxs-lookup"><span data-stu-id="42aac-104">In addition to booking and assigning named or real resources to your project, you can assign generic resources to project tasks.</span></span> <span data-ttu-id="42aac-105">يمكن أن تعمل هذه الموارد كعناصر نائبه للموارد المسماة حتى تصبح مستعدا لعمل فريق للمشروع بموارد مسماة.</span><span class="sxs-lookup"><span data-stu-id="42aac-105">These resources can serve as placeholders for named resources until you are ready to staff your project with named resources.</span></span> 

1. <span data-ttu-id="42aac-106">في Project Service Automation (PSA)، افتح صفحة **المشروع** وفي علامة تبويب **الجدول**، أدخل اسم موضع للمورد العام في خلية **المورد** بالجدول.</span><span class="sxs-lookup"><span data-stu-id="42aac-106">In Project Service Automation (PSA), open the **Project** page and on the **Schedule** tab, enter the position name of the generic resource in the **Resource** cell of the schedule.</span></span> <span data-ttu-id="42aac-107">أو ، انقر فوق رمز **المورد** في الخلية لفتح منتقي المورد ثم قم بإدخال اسم للمورد العام الذي تريد إنشاؤه.</span><span class="sxs-lookup"><span data-stu-id="42aac-107">Or, click the **Resource** icon in the cell to open the resource picker and then enter the name of the generic resource that you want to create.</span></span>

![إنشاء وتعيين عضو فريق عام](media/RM-how-to-9.png)

<span data-ttu-id="42aac-109">سيؤدي هذا إلى فتح لوحة **الإنشاء السريع: أعضاء فريق المشروع**.</span><span class="sxs-lookup"><span data-stu-id="42aac-109">This will open the **Quick Create: Project Team Member** panel.</span></span> 

2. <span data-ttu-id="42aac-110">ادخل الدور والوحدة التنظيمية الخاصة بعضو فريق المورد العام ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="42aac-110">Enter the role and organization unit of the generic resource team member and then click **Save**.</span></span>

![الإنشاء السريع لعضو الفريق العام](media/RM-how-to-10.png)

3. <span data-ttu-id="42aac-112">بعد أن تقوم بإنشاء عضو فريق المورد العام الجديد، يتم تعيينه للمهمة.</span><span class="sxs-lookup"><span data-stu-id="42aac-112">After you have created the new generic resource team member, it is assigned to the task.</span></span> <span data-ttu-id="42aac-113">يمكنك الاستمرار في تعيين هذا المورد العام للمهام الأخرى في جدول المهمة.</span><span class="sxs-lookup"><span data-stu-id="42aac-113">You can continue to assign that generic resource to other tasks in the task schedule.</span></span>

![تعيين عضو فريق عام موجود إلى المهام](media/RM-how-to-11.png)

4. <span data-ttu-id="42aac-115">بعد تعيين المورد العام، يمكنك إنشاء متطلب مورد وتنفيذه من خلال حجز طلب مورد أو إرساله مباشرة إلى مدير مورد.</span><span class="sxs-lookup"><span data-stu-id="42aac-115">After you have assigned the generic resource, you can generate a resource requirement and fulfill it by directly booking or submitting a resource request to a resource manager.</span></span>

![إنشاء متطلب لعضو فريق عام](media/RM-how-to-12.png)

<span data-ttu-id="42aac-117">في شبكة أعضاء الفريق، بالإضافة إلى إمكانية استخدام منتقي الموارد كما هو موضح أعلاه، يمكنك إضافة موارد عامة مباشرة.</span><span class="sxs-lookup"><span data-stu-id="42aac-117">On the team member grid, in addition to being able to use the resource picker as mentioned above, you can add generic resources directly.</span></span> <span data-ttu-id="42aac-118">تتم إضافة الموارد مع متطلب المورد الذي يستند إلى تاريخي البدء/الانتهاء وأسلوب التخصيص المحدد في لوحة **الإنشاء السريع: أعضاء فريق المشروع**.</span><span class="sxs-lookup"><span data-stu-id="42aac-118">The resources are added with a resource requirement that is based on the start/end dates and allocation method specified in the **Quick Create: Project Team Member** panel.</span></span>

<span data-ttu-id="42aac-119">يمكنك رؤية الفرق إذا قمت بإضافة عضو الفريق العام مباشرة ثم قمت بتعيين مزيد من المهام إلى المورد العام تزيد عن قدرته على تغطية الساعات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="42aac-119">You can see a difference if you add the generic team member directly and then assign more tasks to the generic resource than they have required hours to cover.</span></span> <span data-ttu-id="42aac-120">انقر فوق **إنشاء متطلب** لإعادة إنشاء المتطلب لموازنة الساعات المطلوبة مقابل التعيينات.</span><span class="sxs-lookup"><span data-stu-id="42aac-120">Click **Generate Requirement** to regenerate the requirement to balance the required hours against assignments.</span></span>

<span data-ttu-id="42aac-121">يمكنك أيضا النقر فوق ارتباط **متطلب الموارد** في شبكة الفريق لفتح المتطلبات وإضافة مهارات والموارد المفضلة وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="42aac-121">You can also click the **Resource requirement** link in the team grid to open the requirement and add skills, preferred resources, etc.</span></span>

![متطلبات الموارد](media/RM-how-to-13.png)

