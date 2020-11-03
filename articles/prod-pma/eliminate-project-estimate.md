---
title: إزالة تقدير مشروع
description: يقدم هذا الموضوع معلومات حول إزالة تقدير المشروع بعد اكتماله.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 8bda8a7357e883b948449b2a19bea476996dde3c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070697"
---
# <a name="eliminate-a-project-estimate"></a><span data-ttu-id="fde89-103">إزالة تقدير مشروع</span><span class="sxs-lookup"><span data-stu-id="fde89-103">Eliminate a project estimate</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="fde89-104">توفر تقديرات المشروع طريقة عرض الشؤون المالية للعمل المقدر والمجدول لمشروع.</span><span class="sxs-lookup"><span data-stu-id="fde89-104">Project estimates provide the financial view for work that is estimated and scheduled for a project.</span></span> <span data-ttu-id="fde89-105">للعمل مع التقديرات الخاصة بمشروع، يجب إرفاق المشروع بمشروع تقديري.</span><span class="sxs-lookup"><span data-stu-id="fde89-105">To work with estimates for a project, you must attach the project to an estimate project.</span></span> <span data-ttu-id="fde89-106">يستند المشروع التقديري دائمًا إلى مشروع موجود، ومع ذلك بإمكان مشاريع متعددة أن تشير إلى مشروع تقديري واحد.</span><span class="sxs-lookup"><span data-stu-id="fde89-106">An estimate project is always based on an existing project, however multiple projects can refer to a single estimate project.</span></span> <span data-ttu-id="fde89-107">يمكن إرفاق مشروعات الأسعار الثابتة والاستثمارية فقط بالمشروعات التقديرية، ويجب أن تنتمي هذه المشاريع إلى مجموعة المشاريع نفسها التي ينتمي إليها المشروع التقديري.</span><span class="sxs-lookup"><span data-stu-id="fde89-107">Only fixed-price and investment projects can be attached to estimate projects, and those projects must belong to the same project group as the estimate project.</span></span>

<span data-ttu-id="fde89-108">لإزالة مشروع تقديري، يجب أن يكون مكتملاً.</span><span class="sxs-lookup"><span data-stu-id="fde89-108">To eliminate an estimate project, it must be complete.</span></span> <span data-ttu-id="fde89-109">توضح الخطوات التالية كيفية إزالة تقدير.</span><span class="sxs-lookup"><span data-stu-id="fde89-109">The following steps explain how to eliminate an estimate.</span></span>

1. <span data-ttu-id="fde89-110">انتقل إلى **إدارة المشاريع والمحاسبة** > **جميع المشاريع** وافتح المشروع.</span><span class="sxs-lookup"><span data-stu-id="fde89-110">Go to **Project management and accounting** > **All Projects** and open the project.</span></span> 
2. <span data-ttu-id="fde89-111">على علامة التبويب **إدارة** ، حدد **التقديرات** ، وفي الصفحة **تقدير** ، حدد **إزالة**.</span><span class="sxs-lookup"><span data-stu-id="fde89-111">On the **Manage** tab, select **Estimates** , and on the **Estimate** page select **Eliminate**.</span></span>
3. <span data-ttu-id="fde89-112">في الصفحة **إزالة التقدير** على علامة التبويب **عام** ، قم بتعيين الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="fde89-112">On the **Eliminate estimate** page on the **General** tab, set the following options:</span></span>

   - <span data-ttu-id="fde89-113">**كود الفترة** : حدد كود الفترة لاختيار المشروعات التقديرية المناسبة.</span><span class="sxs-lookup"><span data-stu-id="fde89-113">**Period code** : Select the period code to choose the appropriate estimate projects.</span></span> 
   - <span data-ttu-id="fde89-114">**تاريخ التقدير** : حدد تاريخ التقدير المناسب للإزالة.</span><span class="sxs-lookup"><span data-stu-id="fde89-114">**Estimate date** : Select the appropriate estimate date for elimination.</span></span>
   - <span data-ttu-id="fde89-115">**إزالة مع تحذيرات العمل قيد التنفيذ** : قم بتمكين هذا الخيار لتقديم إعلام عندما ستتم إزالة تقدير يرتبط بعمل قيد التنفيذ (WIP).</span><span class="sxs-lookup"><span data-stu-id="fde89-115">**Eliminate with WIP warnings** : Enable this option to provide notification when an estimate that is associated with a work in progress (WIP) will be eliminated.</span></span> <span data-ttu-id="fde89-116">عند عدم تمكين هذا الخيار، لا يمكن متابعة الإزالة في حال وجود حركات غير تقديرية.</span><span class="sxs-lookup"><span data-stu-id="fde89-116">When this option is not enabled, elimination can’t continue if any non-estimated transactions exist.</span></span> 
   > [!NOTE]
   > <span data-ttu-id="fde89-117">لا يتوفر هذا الخيار الا عندما يتم تطبيق الإزالة على مشروع تقديري.</span><span class="sxs-lookup"><span data-stu-id="fde89-117">This option is available only when elimination is applied to an estimate project.</span></span> <span data-ttu-id="fde89-118">ولا يكون متوفرًا إذا كنت تستخدم عمليات الترحيل الدورية.</span><span class="sxs-lookup"><span data-stu-id="fde89-118">It is not available if you are using periodic postings.</span></span> <span data-ttu-id="fde89-119">يعمل هذا الإعداد مع الإعدادات الموجودة على علامة التبويب **تقدير** في صفحة **معلمات المشروع** في مجموعة حقول **السماح بالإزالة عند وجود حركات غير مقدرة**.</span><span class="sxs-lookup"><span data-stu-id="fde89-119">This setting works with the settings on the **Estimate** tab on the **Project parameters** page, in the **Allow elimination when non-estimated transactions exist** field group.</span></span>
   - <span data-ttu-id="fde89-120">**تعيين المرحلة إلى منتهية** : يمكنك تمكين هذا الخيار لتعيين مرحلة المشروع التقديري إلى **منتهية** بعد تشغيل الإزالة.</span><span class="sxs-lookup"><span data-stu-id="fde89-120">**Set stage to Finished** : Enable this option to set the estimate project’s stage to **Finished** after you run the elimination.</span></span>
   - <span data-ttu-id="fde89-121">**طباعة قائمة التقديرات** : حدد المعلومات التي سيتم تضمينها عند طباعة قائمة التقديرات‏‎.</span><span class="sxs-lookup"><span data-stu-id="fde89-121">**Print estimate list** : Select the information to be included when the estimate list is printed.</span></span>
   - <span data-ttu-id="fde89-122">**إظهار سجل المعلومات** : يمكنك تمكين هذا الخيار لعرض سجل المعلومات.</span><span class="sxs-lookup"><span data-stu-id="fde89-122">**Show Infolog** : Enable this option to display the Infolog.</span></span>
   - <span data-ttu-id="fde89-123">**تاريخ الترحيل** : اختر تاريخ ترحيل دفتر الأستاذ للتقدير.</span><span class="sxs-lookup"><span data-stu-id="fde89-123">**Posting date** : Choose the ledger posting date of the estimate.</span></span>

4.  <span data-ttu-id="fde89-124">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="fde89-124">Select **OK**.</span></span>
5. <span data-ttu-id="fde89-125">بعد اكتمال عملية الإزالة، يظهر المشروع التقدير المُزال مع قيمة سالبة.</span><span class="sxs-lookup"><span data-stu-id="fde89-125">After the elimination process is complete, the eliminated estimate project is displayed with a negative value.</span></span> 

<span data-ttu-id="fde89-126">إذا لم تكن تهدف إلى إزالة تقدير، فيمكنك تحديد التقدير المُزال وتحديد **عكس عملية الإزالة**.</span><span class="sxs-lookup"><span data-stu-id="fde89-126">If you did not intend to eliminate an estimate, you can select the eliminated estimate and select **Reverse elimination**.</span></span>   
