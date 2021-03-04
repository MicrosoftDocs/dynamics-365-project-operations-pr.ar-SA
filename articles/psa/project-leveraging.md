---
title: تقديرات المبيعات والمشاريع
description: يوفر هذا الموضوع معلومات حول كيفية الاستفادة من الجدولة والتقديرات في عملية المبيعات.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: 76e21f80e51e6f3092880dc629ba90b400805486
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148357"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="988ff-103">تقديرات المبيعات والمشاريع</span><span class="sxs-lookup"><span data-stu-id="988ff-103">Sales estimates and projects</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="988ff-104">أثناء عملية المبيعات ، يمكنك إنشاء تقديرات للمبيعات عن طريق ربط المشروع بعرض أسعار للمبيعات.</span><span class="sxs-lookup"><span data-stu-id="988ff-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="988ff-105">وبهذه الطريقة ، يمكن أن يحدث التقدير الحتمي أثناء عملية المبيعات ، للاستفادة من إمكانات جدولة المشروع وتقديره.</span><span class="sxs-lookup"><span data-stu-id="988ff-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="988ff-106">إذا تمت عملية البيع ، فيمكن استخدام الجدول الذي تم استخدامه لأغراض تقدير المبيعات كأساس لمزيد من التنقيح لخطة المشروع.</span><span class="sxs-lookup"><span data-stu-id="988ff-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="988ff-107">ربط مشروع ببند عرض أسعار</span><span class="sxs-lookup"><span data-stu-id="988ff-107">Linking a project to a quote line</span></span>

<span data-ttu-id="988ff-108">عندما تقوم بإنشاء بند عرض أسعار قائم على المشروع، يمكنك إنشاء مشروع جديد أو إقران مشروع موجود في صفحة **بند عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="988ff-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![نموذج بند عرض الأسعار](media/project-8.png)
 
<span data-ttu-id="988ff-110">عندما تنشئ مشروعًا جديدًا من تفاصيل سطر عرض الأسعار ، يمكنك الاستفادة من قوالب المشروع.</span><span class="sxs-lookup"><span data-stu-id="988ff-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="988ff-111">قوالب المشروع هي مشاريع نموذجية تمثل خطط مشروع قياسية وتقديرات مالية نموذجية في المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="988ff-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="988ff-112">يمكنهم أيضًا تمثيل نسخ من خطط المشروع وتقديرات المشاريع السابقة.</span><span class="sxs-lookup"><span data-stu-id="988ff-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![تفاصيل بند عرض الأسعار‬](media/project-9.png)
  
<span data-ttu-id="988ff-114">عند إنشاء المشروع من عرض الأسعار، يتم ربط المشروع تلقائيًا ببند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="988ff-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="988ff-115">مكونات التقديرات في مشروع</span><span class="sxs-lookup"><span data-stu-id="988ff-115">Components of estimates in a project</span></span>

<span data-ttu-id="988ff-116">تتيح لك الجدولة تقسيم العمل إلى مهام ، والمحافظة على تدرج هرمي للمهام ، وتحديد الموارد اللازمة لإكمال المهمة ، وتعيين تقدير للجهد المطلوب لإكمال المهمة.</span><span class="sxs-lookup"><span data-stu-id="988ff-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="988ff-117">يمكنك تحديد مجهود العمل وجدوله التقديرات باستخدام الحقول الموجودة في علامة التبويب **جدولة** في صفحة **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="988ff-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="988ff-118">نظرًا لأن قائمة الأسعار مرتبطة بالمشروع ، يتم حساب التقديرات المالية باستخدام التكلفة ومبيعات الأسعار المحددة في قائمة الأسعار.</span><span class="sxs-lookup"><span data-stu-id="988ff-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="988ff-119">استيراد التقديرات من مشروع إلى عرض أسعار</span><span class="sxs-lookup"><span data-stu-id="988ff-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="988ff-120">بعد تحديد تقديرات المشروع ، يمكنك استيرادها في بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="988ff-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="988ff-121">في صفحة **تفاصيل بند عرض الأسعار**، حدد **استيراد من التقديرات** على الشريط لتلخيص تقديرات المشروع حسب نوع الحركة أو الدور أو مستوى المهمة.</span><span class="sxs-lookup"><span data-stu-id="988ff-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>
