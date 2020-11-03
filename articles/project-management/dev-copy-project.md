---
title: تطوير قوالب المشروع مع نسخ المشروع‬
description: يوفر هذا الموضوع معلومات حول كيفية إنشاء قوالب مشروع باستخدام إجراء "نسخ المشروع" المخصص.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb49109e8c199bc4569702ae844a19985534294d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070584"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="01d13-103">تطوير قوالب المشروع مع نسخ المشروع‬</span><span class="sxs-lookup"><span data-stu-id="01d13-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="01d13-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="01d13-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="01d13-105">يدعم Dynamics 365 Project Operations القدرة على نسخ مشروع وإرجاع أي تعيينات إلى الموارد العامة التي تمثل الدور.</span><span class="sxs-lookup"><span data-stu-id="01d13-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="01d13-106">يمكن للعملاء استخدام هذه الوظيفة لبناء قوالب المشروع الأساسية.</span><span class="sxs-lookup"><span data-stu-id="01d13-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="01d13-107">عند تحديد **نسخ المشروع** ، يتم تحديث حالة المشروع الهدف.</span><span class="sxs-lookup"><span data-stu-id="01d13-107">When you select **Copy Project** , the status of the target project is updated.</span></span> <span data-ttu-id="01d13-108">استخدم **سبب الحالة** لتحديد وقت اكتمال إجراء النسخ.</span><span class="sxs-lookup"><span data-stu-id="01d13-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="01d13-109">يؤدي أيضًا تحديد **نسخ المشروع** إلى تحديث تاريخ بدء المشروع إلى تاريخ البدء الحالي في حال عدم اكتشاف تاريخ مستهدف في كيان المشروع الهدف.</span><span class="sxs-lookup"><span data-stu-id="01d13-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="01d13-110">الإجراء المخصص "نسخ المشروع"</span><span class="sxs-lookup"><span data-stu-id="01d13-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="01d13-111">اسم</span><span class="sxs-lookup"><span data-stu-id="01d13-111">Name</span></span> 

<span data-ttu-id="01d13-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="01d13-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="01d13-113">معلمات الإدخال</span><span class="sxs-lookup"><span data-stu-id="01d13-113">Input parameters</span></span>
<span data-ttu-id="01d13-114">توجد ثلاث معلمات إدخال:</span><span class="sxs-lookup"><span data-stu-id="01d13-114">There are three input parameters:</span></span>

| <span data-ttu-id="01d13-115">المعلمة‬</span><span class="sxs-lookup"><span data-stu-id="01d13-115">Parameter</span></span>          | <span data-ttu-id="01d13-116">النوع</span><span class="sxs-lookup"><span data-stu-id="01d13-116">Type</span></span>   | <span data-ttu-id="01d13-117">القيم</span><span class="sxs-lookup"><span data-stu-id="01d13-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="01d13-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="01d13-118">ProjectCopyOption</span></span>  | <span data-ttu-id="01d13-119">String</span><span class="sxs-lookup"><span data-stu-id="01d13-119">String</span></span> | <span data-ttu-id="01d13-120">**{"removeNamedResources":true}** أو **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="01d13-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="01d13-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="01d13-121">SourceProject</span></span>      | <span data-ttu-id="01d13-122">مرجع الكيان</span><span class="sxs-lookup"><span data-stu-id="01d13-122">Entity Reference</span></span> | <span data-ttu-id="01d13-123">Source Project</span><span class="sxs-lookup"><span data-stu-id="01d13-123">Source Project</span></span> |
| <span data-ttu-id="01d13-124">هدف</span><span class="sxs-lookup"><span data-stu-id="01d13-124">Target</span></span>             | <span data-ttu-id="01d13-125">مرجع الكيان</span><span class="sxs-lookup"><span data-stu-id="01d13-125">Entity Reference</span></span> | <span data-ttu-id="01d13-126">المشروع الهدف</span><span class="sxs-lookup"><span data-stu-id="01d13-126">Target Project</span></span> |


- <span data-ttu-id="01d13-127">**{"clearTeamsAndAssignments":true}** : السلوك الافتراضي لمشروع الويب، وستتم إزالة جميع التعيينات وأعضاء الفريق.</span><span class="sxs-lookup"><span data-stu-id="01d13-127">**{"clearTeamsAndAssignments":true}** : Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="01d13-128">**{"removeNamedResources":true}** السلوك الافتراضي لـ Project Operations، وستُعاد التعيينات إلى الموارد العامة.</span><span class="sxs-lookup"><span data-stu-id="01d13-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="01d13-129">لمزيد من الإعدادات الافتراضية حول الإجراءات، راجع [استخدام إجراءات API الويب](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="01d13-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="01d13-130">تحديد الحقول المراد نسخها</span><span class="sxs-lookup"><span data-stu-id="01d13-130">Specify fields to copy</span></span> 
<span data-ttu-id="01d13-131">عند استدعاء الإجراء، يبحث **نسخ المشروع** في طريقة عرض المشروع **نسخ أعمدة المشروع** لتحديد الحقول التي يجب نسخها عند نسخ المشروع.</span><span class="sxs-lookup"><span data-stu-id="01d13-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>
