---
title: قوالب المشروع
description: يقدم هذا الموضوع معلومات حول كيفية استخدام قوالب المشروع لإعداد المشروع السريع.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: f0161bf9-af4c-4a21-b767-ac20a8e30688
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5a3112c2eef9525946314bdb587c44904557fa52
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748628"
---
# <a name="project-templates"></a><span data-ttu-id="4900c-103">قوالب المشروع</span><span class="sxs-lookup"><span data-stu-id="4900c-103">Project templates</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="4900c-104">قالب المشروع هو إطار عمل معرف مسبقا يساعدك على بدء تشغيل مشروع بسرعة وبسهولة.</span><span class="sxs-lookup"><span data-stu-id="4900c-104">A project template is a predefined framework that helps you quickly and easily start a project.</span></span> <span data-ttu-id="4900c-105">يمكنك استخدام قالب محدد مسبقًا لإنشاء مشروع جديد بنقرة واحدة.</span><span class="sxs-lookup"><span data-stu-id="4900c-105">You can use a predefined template to create a new project with a single click.</span></span> <span data-ttu-id="4900c-106">بالنسبة إلى المشروعات ، يجب عليك تحديد المتطلبات الأساسية لقوالب المشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-106">As for projects, you must define the prerequisites for project templates.</span></span> <span data-ttu-id="4900c-107">يجب عليك تحديد تقويم مشروع لكل قالب مشروع ، ويجب تحديد الأدوار وقوائم الأسعار مسبقًا في المؤسسة ، بحيث تحتوي مكونات القالب على بيانات مفيدة.</span><span class="sxs-lookup"><span data-stu-id="4900c-107">You must define a project calendar for each project template, and roles and price lists must be predefined in the organization, so that the components of the template have useful data.</span></span>

<span data-ttu-id="4900c-108">يتكون قالب المشروع من ثلاثة مكونات: الجدول الزمني ، وتقديرات المشروع ، وأعضاء فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-108">A project template consists of three components: a schedule, project estimates, and project team members.</span></span>

## <a name="schedule"></a><span data-ttu-id="4900c-109">جدول</span><span class="sxs-lookup"><span data-stu-id="4900c-109">Schedule</span></span>

<span data-ttu-id="4900c-110">يحتوي الجدول في قالب المشروع على نفس مجموعة العناصر مثل الجدول في المشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-110">A schedule in a project template has the same set of elements as a schedule in a project.</span></span> <span data-ttu-id="4900c-111">يمكنك إنشاء تدرج هرمي للمهام وربط الأدوار بالمهام وتحديد سمات الجدول وتعيين التبعيات.</span><span class="sxs-lookup"><span data-stu-id="4900c-111">You can create a task hierarchy, associate roles with tasks, define schedule attributes, and set dependencies.</span></span> <span data-ttu-id="4900c-112">يدعم الجدول في قالب المشروع أيضًا أوضاع المهام لكل مهمة.</span><span class="sxs-lookup"><span data-stu-id="4900c-112">A schedule in a project template also supports task modes for each task.</span></span> <span data-ttu-id="4900c-113">لذلك ، يدعم محرك الجدولة.</span><span class="sxs-lookup"><span data-stu-id="4900c-113">Therefore, it supports the scheduling engine.</span></span> <span data-ttu-id="4900c-114">يجب ربط تقويم المشروع بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-114">You must associate a project calendar with the project.</span></span> <span data-ttu-id="4900c-115">عند إنشاء جدول عمل ، لا يوجد فرق بين قالب المشروع ومشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-115">When you create a work schedule, there is no difference between a project template and a project.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="4900c-116">تقديرات المشروع</span><span class="sxs-lookup"><span data-stu-id="4900c-116">Project estimates</span></span>

<span data-ttu-id="4900c-117">تعمل تقديرات المشروع في قالب المشروع بنفس الطريقة التي تعمل بها تقديرات المشروع في المشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-117">Project estimates in a project template work the same way as project estimates in a project.</span></span> <span data-ttu-id="4900c-118">ومع ذلك ، يتم سحب أسعار التكلفة والمبيعات من قوائم التكلفة الافتراضية وسعر المبيعات المحددة في المعلمات.</span><span class="sxs-lookup"><span data-stu-id="4900c-118">However, the cost and sales prices are pulled from the default cost and sales price lists that are defined in the parameters.</span></span>

## <a name="creating-a-project-from-a-template"></a><span data-ttu-id="4900c-119">إنشاء مشروع من قالب</span><span class="sxs-lookup"><span data-stu-id="4900c-119">Creating a project from a template</span></span>
 
<span data-ttu-id="4900c-120">هناك عدة طرق لإنشاء مشروع من قالب مشروع:</span><span class="sxs-lookup"><span data-stu-id="4900c-120">There are several ways to create a project from a project template:</span></span>

- <span data-ttu-id="4900c-121">عند إنشاء مشروع من عرض أسعار، يمكنك تحديد قالب مشروع في مربع الحوار **إنشاء سريع: مشروع**.</span><span class="sxs-lookup"><span data-stu-id="4900c-121">When you create a project from a quote, you can select a project template in the **Quick Create: Project** dialog box.</span></span>

> ![مربع الحوار إنشاء سريع: مشروع](media/project-11.png)

- <span data-ttu-id="4900c-123">عندما تقوم بإنشاء مشروع عن طريق تحديد **مشروع جديد**، تظهر صفحة **المشروع** قبل أن يتم حفظ السجل.</span><span class="sxs-lookup"><span data-stu-id="4900c-123">When you create a project by selecting **New Project**, the **Project** page appears before the record is saved.</span></span> <span data-ttu-id="4900c-124">في الحقل **اختيار قالب**، حدد أحد قوالب المشروع المعرفة مسبقًا في المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="4900c-124">In the **Pick a Template** field, select one of the predefined project templates in the organization.</span></span>
- <span data-ttu-id="4900c-125">استخدم **إنشاء مشروع من قالب** في صفحة **كيان القالب**.</span><span class="sxs-lookup"><span data-stu-id="4900c-125">Use **Create Project from a Template** on the **Template Entity** page.</span></span>

## <a name="copying-components-of-template-to-project"></a><span data-ttu-id="4900c-126">نسخ مكونات قالب إلى مشروع</span><span class="sxs-lookup"><span data-stu-id="4900c-126">Copying components of template to project</span></span>

<span data-ttu-id="4900c-127">عندما تقوم بنسخ مكونات قالب المشروع إلى مشروع ، يمكن أن تحدث بعض التجاوزات، اعتمادًا على الإعدادات في المشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-127">When you copy the components of a project template to a project, a few overrides can occur, depending on the settings in the project.</span></span>

### <a name="copying-the-schedule"></a><span data-ttu-id="4900c-128">نسخ الجدول</span><span class="sxs-lookup"><span data-stu-id="4900c-128">Copying the schedule</span></span>

<span data-ttu-id="4900c-129">عند نسخ الجدول من قالب مشروع ، إذا كان للمشروع تقويم مشروع مختلف عن القالب ، يتم تطبيق ساعات العمل من تقويم المشروع على جدول المهام.</span><span class="sxs-lookup"><span data-stu-id="4900c-129">When you copy the schedule from a project template, if the project has a different project calendar than the template, work hours from the project's calendar are applied to the task schedule.</span></span> <span data-ttu-id="4900c-130">بهذه الطريقة ، يتم تعديل الجدول لمطابقة تقويم مشروع الدعم.</span><span class="sxs-lookup"><span data-stu-id="4900c-130">In this way, the schedule is adjusted to match the backing project calendar.</span></span> <span data-ttu-id="4900c-131">وبالمثل، تأخذ المهمة الأولى في الجدول تاريخ بدء المشروع ، ويتم تحديث الجدول الزمني لبقية التدرج الهرمي بناءً على المدة والتبعيات المحددة في القالب.</span><span class="sxs-lookup"><span data-stu-id="4900c-131">Similarly, the first task on the schedule takes the project's start date, and the schedule of the rest of the hierarchy is updated based on the duration and dependencies that are specified in the template.</span></span> 

### <a name="copying-project-estimates"></a><span data-ttu-id="4900c-132">نسخ تقديرات المشروع</span><span class="sxs-lookup"><span data-stu-id="4900c-132">Copying project estimates</span></span> 

<span data-ttu-id="4900c-133">عند النسخ عبر بنود تقدير المشروع ، يتم تحديث قوائم الأسعار.</span><span class="sxs-lookup"><span data-stu-id="4900c-133">When you copy across project estimate lines, the price lists are updated.</span></span> <span data-ttu-id="4900c-134">للحصول على قائمة أسعار التكلفة ، تستند هذه التحديثات إلى الوحدة المالكة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-134">For the cost price list, these updates are based on the owning unit of the project.</span></span> <span data-ttu-id="4900c-135">بالنسبة لقائمة أسعار المبيعات ، إنها تستند إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="4900c-135">For the sales price list, they are based on the customer.</span></span> <span data-ttu-id="4900c-136">بالنسبة للمشاريع المرتبطة بكيان مبيعات ، يتم تحديد تكلفة الوحدة وأسعار المبيعات بناءً على قوائم الأسعار هذه.</span><span class="sxs-lookup"><span data-stu-id="4900c-136">For projects that are associated with a sales entity, the unit cost and sales prices are determined based on these price lists.</span></span>

### <a name="copying-a-project-team"></a><span data-ttu-id="4900c-137">نسخ فريق مشروع</span><span class="sxs-lookup"><span data-stu-id="4900c-137">Copying a project team</span></span>

<span data-ttu-id="4900c-138">عندما يتم نسخ فريق مشروع من قالب مشروع إلى مشروع ، يتم نسخ الموارد العامة ، إلى جانب المهارات والكفاءات المحددة في القالب.</span><span class="sxs-lookup"><span data-stu-id="4900c-138">When a project team is copied from a project template to a project, the generic resources are copied, together with the skills and proficiencies that are defined in the template.</span></span> <span data-ttu-id="4900c-139">يتم أيضًا الاحتفاظ بتعيينات الموارد العامة كما كانت في قالب المشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-139">Generic resource assignments are also maintained as they were in the project template.</span></span> <span data-ttu-id="4900c-140">الموارد المسماة غير مدعومة في قوالب المشروع.</span><span class="sxs-lookup"><span data-stu-id="4900c-140">Named resources aren't supported in project templates.</span></span>
