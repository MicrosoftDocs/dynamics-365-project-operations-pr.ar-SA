---
title: المصروفات بين الشركات الشقيقة
description: قد يقوم العامل الذي تم توظيفه من قبل كيان قانوني في إحدى المؤسسات بتنفيذ عمل لكيان قانوني آخر في نفس المؤسسة. وفي هذه الحالة، يمكنك استخدام ميزه مصروفات بين الشركات الشقيقة لتعيين مصروفات العامل للكيان القانوني الذي تم تنفيذ العمل له.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070795"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="3d5b8-104">المصروفات بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="3d5b8-104">Intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="3d5b8-105">قد يقوم العامل الذي تم توظيفه من قبل كيان قانوني في إحدى المؤسسات بتنفيذ عمل لكيان قانوني آخر في نفس المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-105">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="3d5b8-106">وفي هذه الحالة، يمكنك استخدام ميزه مصروفات بين الشركات الشقيقة لتعيين مصروفات العامل للكيان القانوني الذي تم تنفيذ العمل له.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-106">In this situation, you can use the intercompany expense feature to assign the worker’s expenses to the legal entity for which the work was performed.</span></span> <span data-ttu-id="3d5b8-107">يسمى الكيان القانوني الذي يوظف العامل الكيان القانوني المقرض.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-107">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="3d5b8-108">يسمى الكيان القانوني الذي يتكبد العامل المصروفات له الكيان القانوني المقترض.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-108">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="3d5b8-109">قبل أن يتمكن العامل من إنشاء مصروفات للعمل الذي يتم تنفيذه لكيان قانوني مختلف، في الكيان القانوني المقرض، في الصفحة **معلمات إدارة المصروفات** ، حدد الخيار **السماح ببنود المصروفات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-109">Before a worker can create and submit expenses for work that is performed for a different legal entity, in the loaning legal entity, on the **Expense management parameters** page, select the **Allow intercompany expense lines** option.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="3d5b8-110">ترحيل الضرائب للمصروفات بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="3d5b8-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="3d5b8-111">إذا كنت ترغب في استخدام مجموعات الضرائب المقترنة بالكيان القانوني المقرض (المصدر) بدلاً من الكيان القانوني المقترض (الوجهة) في تقرير المصروفات، ستحتاج إلى تكوينها في إعداد ضريبة مبيعات دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-111">If you want to use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you will need to configure this in the General ledger sales tax set up.</span></span> <span data-ttu-id="3d5b8-112">عند تعيين معلمة دفتر الأستاذ العام، **الكيان القانوني لترحيل الضرائب بين الشركات الشقيقة** إلى **المصدر** و **تطبيق قواعد ضريبة المبيعات** إلى **لا** ، سيتم استخدام مجموعة الضرائب للكيان القانوني المقرض.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-112">When the General ledger parameter, **Legal entity for intercompany tax posting** is set to **Source** and **Apply sales tax taxation rules** is set to **No** , the tax combination for the loaning legal entity will be used.</span></span> <span data-ttu-id="3d5b8-113">عندما يتم تعيين نفس المعلمة إلى **الوجهة** ، سيتم استخدام مجموعه الضرائب للكيان القانوني المقترض.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-113">When the same parameter is set to **Destination** , the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="3d5b8-114">بالنسبة إلى الكيانات القانونية في الولايات المتحدة، عندما يتم تعيين المعلمة إلى **المصدر** ، يجب أيضًا تكوين الحقل **مقبوضات لضريبة المبيعات** في صفحة **مجموعات ترحيل دفتر الأستاذ العام** الجديدة.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-114">For legal entities in the United States, when the parameter is set to **Source** , the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="3d5b8-115">سيستخدم محرك المحاسبة المعلومات من هذا الحقل للإدخال المحاسبي المتعلق بالضريبة.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-115">The accounting engine will use the information from this field for tax related accounting entry.</span></span>   
<span data-ttu-id="3d5b8-116">يكون السلوك متسقًا بالنسبة لبنود المصروفات التي تم ترحيلها مع مشروع أو بدونه.</span><span class="sxs-lookup"><span data-stu-id="3d5b8-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
