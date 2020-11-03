---
title: توفير تقديرات العمل لمشروع أثناء عملية المبيعات
description: كيفية توفير تقديرات العمل لمشروع أثناء عملية المبيعات (Project Service)
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: ddb7f8c0ff8c7fd7e51edb42f9d227f2b91a811b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070694"
---
# <a name="provide-work-estimates-for-a-project-during-the-sales-process-project-service"></a><span data-ttu-id="045eb-103">توفير تقديرات العمل لمشروع أثناء عملية المبيعات (Project Service)</span><span class="sxs-lookup"><span data-stu-id="045eb-103">Provide work estimates for a project during the sales process (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="045eb-104">أثناء عملية المبيعات، يمكنك حل تقديرات المبيعات من الأساس بواسطة بنود عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="045eb-104">During the sales process, you can work out sales estimates from the ground up with quote lines.</span></span> <span data-ttu-id="045eb-105">توفر قدرات [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] في [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] طريقة علمية وحتمية للتوصل إلى وضع تقديرات المبيعات عبر تنظيم عناصر العمل وربط السمات ذات الصلة التي تساهم في وضع تقديرات المشروع في هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="045eb-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] provide a more scientific and deterministic way of coming up with sales estimates by breaking down work items and associating relevant attributes that contribute toward the estimates for the project in the work breakdown structure.</span></span>  
  
 <span data-ttu-id="045eb-106">بمجرد الفوز بالبيع، يمكنك استخدام هيكل تنظيم العمل المقترن في خطة المشروع، وتحسينه كما تقتضي الحاجة لإنجاز المشروع بشكل ناجح.</span><span class="sxs-lookup"><span data-stu-id="045eb-106">Once you win the sale, you can use the associated work breakdown structure in your project plan, refining it as necessary for successful completion of your project.</span></span>  
  
## <a name="link-a-project-to-a-quote-line"></a><span data-ttu-id="045eb-107">ربط مشروع ببند عرض أسعار</span><span class="sxs-lookup"><span data-stu-id="045eb-107">Link a project to a quote line</span></span>  
 <span data-ttu-id="045eb-108">عند إنشاء بند عرض أسعار يستند إلى المشروع، يمكنك إنشاء مشروع جديد من بند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="045eb-108">When creating a project-based quote line, you can create a new project from the quote line.</span></span> <span data-ttu-id="045eb-109">بعد ذلك، يمكنك استخدام قوالب المشروع، وهي إما خطط مشروع قياسية وتقديرات مالية مشتركة في مؤسستك تم تكوينها بشكل مسبق، أو نسخة من خطة مشروع وتقديراته من مشروع سابق.</span><span class="sxs-lookup"><span data-stu-id="045eb-109">You can then use project templates, which are either pre-configured standard project plans and financial estimates common to your organization, or a copy of a project plan and estimates from a past project.</span></span> <span data-ttu-id="045eb-110">عند إنشاء مشروع، يوفر اختيار قالب مشروع أساسًا لتحسين خطة المشروع والتقديرات ومتطلبات الدور.</span><span class="sxs-lookup"><span data-stu-id="045eb-110">When you create a project, choosing a project template provides a basis to refine the project plan, estimates, and role requirements.</span></span> <span data-ttu-id="045eb-111">من خلال إنشاء المشروع من عرض الأسعار، يتم ربط المشروع تلقائيًا ببند عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="045eb-111">By creating your project from the quote, the project is automatically associated with the quote line.</span></span>  
  
## <a name="project-estimate-components"></a><span data-ttu-id="045eb-112">مكونات تقديرات المشروع</span><span class="sxs-lookup"><span data-stu-id="045eb-112">Project estimate components</span></span>  
 <span data-ttu-id="045eb-113">يوفر هيكل تنظيم العمل في المشروع طريقة لتنظيم العمل في مهام والحفاظ على التدرج الهرمي للمهام بالإضافة إلى تعيين تقدير للجهد المطلوب لإكمال كل مهمة.</span><span class="sxs-lookup"><span data-stu-id="045eb-113">The work breakdown structure in a project provides a way to break down work into tasks, maintain a hierarchy of tasks, and assign an estimate of effort required to complete each task.</span></span> <span data-ttu-id="045eb-114">يمكنك أيضًا ربط الأدوار بمهمة للإشارة إلى تقدير لنوع المورد المطلوب لإكمال مهمة وجدول زمني.</span><span class="sxs-lookup"><span data-stu-id="045eb-114">You can also associate roles to a task to indicate an estimate of the type of resource required to complete a task and a schedule.</span></span>  
  
 <span data-ttu-id="045eb-115">يساعدك هيكل تنظيم العمل في تحديد تقديرات جهد العمل والجدول الزمني.</span><span class="sxs-lookup"><span data-stu-id="045eb-115">The work breakdown structure helps you determine work effort and schedule estimates.</span></span> <span data-ttu-id="045eb-116">بشكل افتراضي، يستخدم المشروع قوائم الأسعار الافتراضية التي قمت بتحديدها سابقًا.</span><span class="sxs-lookup"><span data-stu-id="045eb-116">By default, the project uses default price lists that you defined earlier.</span></span> <span data-ttu-id="045eb-117">تحدد أسعار التكلفة والمبيعات المحددة في قوائم الأسعار التقديرات المالية لتنظيم عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="045eb-117">The cost and sales prices defined in the price lists help determine financial estimates for the project’s work breakdown.</span></span>  
  
 <span data-ttu-id="045eb-118">إذا كان المشروع مقترنًا بعرض أسعار، وعرض الأسعار له قائمة أسعار مختلفة عن تلك الافتراضية، فسيتم استخدام قائمة أسعار عرض الأسعار للتقديرات المالية.</span><span class="sxs-lookup"><span data-stu-id="045eb-118">If your project is associated with a quote, and the quote has a different price list from the default, the quote’s price list is used for financial estimates.</span></span>  
  
## <a name="import-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="045eb-119">استيراد التقديرات من مشروع إلى عرض أسعار</span><span class="sxs-lookup"><span data-stu-id="045eb-119">Import estimates from a project into a quote</span></span>  
 <span data-ttu-id="045eb-120">عندما تتوفر لديك تقديرات المشروع في المشروع، يمكنك استيراد هذه التقديرات إلى بند عرض الأسعار:</span><span class="sxs-lookup"><span data-stu-id="045eb-120">Once you have project estimates in the project, you can import these estimates into the quote line:</span></span>  
  
-   <span data-ttu-id="045eb-121">في **تفاصيل بند عرض الأسعار‬‬** ، انقر فوق **استيراد من التقديرات**.</span><span class="sxs-lookup"><span data-stu-id="045eb-121">In **Quote Line Details** , click **Import from estimates**.</span></span> 

-   <span data-ttu-id="045eb-122">حدد ما إذا كانت تريد استيراد تقديرات المشروع الملخصة حسب نوع المعاملة أو الدور أو مستوى عقده هيكل تنظيم العمل.</span><span class="sxs-lookup"><span data-stu-id="045eb-122">Select whether to import project estimates summarized by transaction type, role, or work breakdown structure node level.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="045eb-123">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="045eb-123">See Also</span></span>  
 [<span data-ttu-id="045eb-124">دليل مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="045eb-124">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
