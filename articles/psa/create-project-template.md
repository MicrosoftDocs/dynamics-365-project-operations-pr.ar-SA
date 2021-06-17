---
title: إنشاء قالب مشروع
description: كيفية إنشاء قالب مشروع في Project Service
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 148bf1d42b640ff7b58b13bb0c30c7e583d803c8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997225"
---
# <a name="create-a-project-template-project-service"></a><span data-ttu-id="42e94-103">إنشاء قالب مشروع (Project Service)</span><span class="sxs-lookup"><span data-stu-id="42e94-103">Create a project template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="42e94-104">تساعدك قوالب المشروع على توفير الوقت إذا كانت شركتك تقدم مناقصات على أنواع مشابهة من المشاريع بشكل منتظم.</span><span class="sxs-lookup"><span data-stu-id="42e94-104">Project templates save you time if your company regularly bids on similar types of projects.</span></span> <span data-ttu-id="42e94-105">وهي توفر مجموعة قياسية من الأدوار والساعات المقدّرة لنوع المشروع.</span><span class="sxs-lookup"><span data-stu-id="42e94-105">They provide a standard set of roles and estimated hours for a type of project.</span></span> <span data-ttu-id="42e94-106">باستطاعة مدراء الحسابات ومدراء المشاريع إنشاء مشاريع استنادًا إلى قالب مشروع، أو يمكنهم نسخ القالب وإنشاء قالب خاص بهم.</span><span class="sxs-lookup"><span data-stu-id="42e94-106">Account managers and project managers can create projects based on a project template, or they can copy the template and make one of their own.</span></span>  
  
## <a name="components-of-project-template"></a><span data-ttu-id="42e94-107">مكونات قالب المشروع</span><span class="sxs-lookup"><span data-stu-id="42e94-107">Components of project template</span></span>
 <span data-ttu-id="42e94-108">هناك ثلاثة مكونات في قالب المشروع:</span><span class="sxs-lookup"><span data-stu-id="42e94-108">A project template consists of three components:</span></span>  
  
- <span data-ttu-id="42e94-109">**هيكل تنظيم العمل**: يتضمن هيكل تنظيم العمل‏‎ في قالب المشروع مجموعة العناصر نفسها الموجودة في المشروع.</span><span class="sxs-lookup"><span data-stu-id="42e94-109">**Work breakdown structure**: A work breakdown structure in a project template has the same set of elements as in the project.</span></span> <span data-ttu-id="42e94-110">يمكنك إنشاء تدرج هرمي للمهام، وربط أدوار بمهمة وتحديد سمات الجدول وتعيين التبعيات وعرض كافة البيانات في مخطط جانت.</span><span class="sxs-lookup"><span data-stu-id="42e94-110">You can create a task hierarchy, associate roles to task, define schedule attributes, set dependencies and view all the data in the Gantt.</span></span> <span data-ttu-id="42e94-111">يدعم أيضًا هيكل تنظيم العمل في قوالب المشروع أوضاع المهام لكل مهمة.</span><span class="sxs-lookup"><span data-stu-id="42e94-111">The work breakdown structure in project templates also support task modes for each task.</span></span> <span data-ttu-id="42e94-112">لا يوجد فرق بين قالب المشروع والمشروع عند إنشاء جدول العمل.</span><span class="sxs-lookup"><span data-stu-id="42e94-112">There is no difference between a project template and a project when creating work schedule.</span></span>  
  
- <span data-ttu-id="42e94-113">**تقديرات المشروع**: تعمل تقديرات المشروع في القوالب تمامًا كما تعمل في المشاريع، فيما عدا قوائم الأسعار لأن أسعار التكلفة والمبيعات الافتراضية هي دائمًا قوائم أسعار المبيعات والتكلفة الافتراضية المحددة في معلمات [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="42e94-113">**Project estimates**: Project estimates in templates work the same way as they do in projects, except the price lists for defaulting the cost and sales prices are always the default cost and sales price lists defined in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parameters.</span></span> <span data-ttu-id="42e94-114">أما الوظائف المتبقية فهي نفسها كما في مشروع.</span><span class="sxs-lookup"><span data-stu-id="42e94-114">The rest of the functionality is the same as in a project.</span></span>  
  
- <span data-ttu-id="42e94-115">**تشكيل فريق المشروع**: عند تشكيل فريق مشروع لقالب مشروع، يتعذر حجز مورد مسمى في قالب.</span><span class="sxs-lookup"><span data-stu-id="42e94-115">**Project team formation**: When forming a project team for a project template, you can’t book a named resource in a template.</span></span> <span data-ttu-id="42e94-116">يمكنك استخدام **إنشاء فريق المشروع** في هيكل تنظيم العمل لإنشاء مجموعة من الموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="42e94-116">You can use **Generate Project Team** in the work breakdown structure to generate a set of generic resources.</span></span> <span data-ttu-id="42e94-117">يمكنك أيضًا تحديد المهارات والكفاءات المطلوبة للموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="42e94-117">You can also specify required skills and proficiencies for generic resources.</span></span> <span data-ttu-id="42e94-118">ولا يمكنك استبدال مورد عام بمورد الحجز في قوالب المشروع.</span><span class="sxs-lookup"><span data-stu-id="42e94-118">You can’t substitute a generic resource with a bookable resource in project templates.</span></span>  
  
## <a name="create-a-project-from-a-template"></a><span data-ttu-id="42e94-119">إنشاء مشروع من قالب</span><span class="sxs-lookup"><span data-stu-id="42e94-119">Create a project from a template</span></span>  
 <span data-ttu-id="42e94-120">يمكنك إنشاء مشروع من قالب باستخدام الطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="42e94-120">You can create a project from a template in these following ways:</span></span>  
  
-   <span data-ttu-id="42e94-121">عند إنشاء مشروع من عرض الأسعار، يمكنك اختيار قالب مشروع في نموذج إنشاء سريع للمشروع‬.</span><span class="sxs-lookup"><span data-stu-id="42e94-121">When creating a project from the quote, you can choose a project template in the project quick create form.</span></span>  
  
-   <span data-ttu-id="42e94-122">عند إنشاء مشروع بالنقر فوق **مشروع جديد**، يظهر نموذج المشروع قبل حفظ السجل.</span><span class="sxs-lookup"><span data-stu-id="42e94-122">When creating a project by clicking **New Project**, the project form displays before you save the record.</span></span> <span data-ttu-id="42e94-123">ومن هنا، يمكنك النقر فوق الحقل **اختيار قالب** للاختيار من قائمة قوالب المشروع المعرفة مسبقًا في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="42e94-123">From here, you can click **Pick a template** field to choose from the list of pre-defined project templates in your organization.</span></span>  
  
-   <span data-ttu-id="42e94-124">انقر فوق **إنشاء مشروع من قالب** في صفحة **قالب المشروع** لإنشاء مشروع من القالب.</span><span class="sxs-lookup"><span data-stu-id="42e94-124">Click **Create project from a template** on the **Project Template** page to create a project from the template.</span></span>  
  
## <a name="copying-components-of-a-template-to-a-project"></a><span data-ttu-id="42e94-125">نسخ مكونات قالب إلى مشروع</span><span class="sxs-lookup"><span data-stu-id="42e94-125">Copying components of a template to a project</span></span>  
 <span data-ttu-id="42e94-126">عندما تنسخ مكونات قالب إلى مشروع، هناك بعض الأمور التي يجب عليك معرفتها حول هذا الأمر.</span><span class="sxs-lookup"><span data-stu-id="42e94-126">When you copy components of a template into a project, there are a few things you should know about.</span></span>  
  
 <span data-ttu-id="42e94-127">**نسخ هيكل تنظيم العمل**: عند نسخ هيكل تنظيم العمل من قالب مشروع، إذا تضمن المشروع تقويم مشروع مختلفًا عن القالب، فسيتم تطبيق ساعات العمل من تقويم المشروع على جدول المهام.</span><span class="sxs-lookup"><span data-stu-id="42e94-127">**Copying a work breakdown structure**: When you copy the work breakdown structure from a project template, if the project has a different project calendar than the template, the work hours from the project’s calendar will be applied to the schedule of tasks.</span></span> <span data-ttu-id="42e94-128">يؤدي ذلك إلى ضبط الجدول وفقًا لتقويم المشروع المساعد.</span><span class="sxs-lookup"><span data-stu-id="42e94-128">This adjusts the schedule to the backing project calendar.</span></span> <span data-ttu-id="42e94-129">وبالمثل، تأخذ المهمة الأولى في هيكل تنظيم العمل تاريخ بدء المشروع، بحيث يتم تحديث باقي جدول التدرج الهرمي للمهام استنادًا إلى المدة والتبعيات المحددة في هيكل تنظيم العمل الخاص بالقالب.</span><span class="sxs-lookup"><span data-stu-id="42e94-129">Similarly, the first task on the work breakdown structure takes the project’s start date, so the rest of the task hierarchy schedule is updated based on the duration and dependencies specified in the template’s work breakdown structure.</span></span>  
  
 <span data-ttu-id="42e94-130">**نسخ تقديرات المشروع**: عندما تجري النسخ عبر بنود تقديرات المشروع، يتم تحديث قوائم الأسعار استنادًا إلى الوحدة المالكة للمشروع لقائمة أسعار التكلفة والعميل لقائمة أسعار المبيعات.</span><span class="sxs-lookup"><span data-stu-id="42e94-130">**Copying project estimates**: When you copy across project estimate lines, price lists are updated based on the owning unit of the project for the cost price list and customer for the sales price list.</span></span> <span data-ttu-id="42e94-131">يتم تحديد أسعار تكلفة الوحدات وأسعار المبيعات من قوائم الأسعار هذه في المشاريع المرتبطة بوحدة مبيعات.</span><span class="sxs-lookup"><span data-stu-id="42e94-131">The unit cost and sales prices are determined from these price lists on projects that are associated to a sales entity.</span></span>  
  
 <span data-ttu-id="42e94-132">**نسخ فريق مشروع**: عند نسخ فريق المشروع من القالب إلى مشروع، يتم نسخ الموارد العامة عبره، إلى جانب المهارات والكفاءات التي تم تعريفها في القالب.</span><span class="sxs-lookup"><span data-stu-id="42e94-132">**Copying a project team**: When you copy the project team from the template to a project, the generic resources are copied across, along with the skills and proficiencies defined in the template.</span></span> <span data-ttu-id="42e94-133">يتم أيضًا الاحتفاظ بتعيينات الموارد العامة كما في قالب المشروع.</span><span class="sxs-lookup"><span data-stu-id="42e94-133">Generic resource assignments are also maintained as in the project template.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="42e94-134">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="42e94-134">See Also</span></span>  
 [<span data-ttu-id="42e94-135">دليل مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="42e94-135">Project Manager Guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]