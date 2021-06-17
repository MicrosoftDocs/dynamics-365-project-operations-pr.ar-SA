---
title: المصروفات بين الشركات الشقيقة
description: يوفر هذا الموضوع معلومات حول كيفية استخدام المصاريف المشتركة بين شركات لتعيين مصروفات العامل إلى الكيان القانوني الذي تم تنفيذ العمل من أجله.
author: ShylaThompson
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d2cdba8d5368a8b26bf4d98226bda76a58261cf0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005055"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="017f4-103">المصروفات بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="017f4-103">Intercompany expenses</span></span>

<span data-ttu-id="017f4-104">قد يقوم العامل الذي تم توظيفه من قبل كيان قانوني في إحدى المؤسسات بتنفيذ عمل لكيان قانوني آخر في نفس المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="017f4-104">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="017f4-105">يمكنك استخدام المصاريف المشتركة بين شركات لتعيين مصروفات العامل إلى الكيان القانوني الذي تم تنفيذ العمل من أجله.</span><span class="sxs-lookup"><span data-stu-id="017f4-105">You can use intercompany expenses to assign the worker’s expenses to the legal entity for which the  work was performed.</span></span> <span data-ttu-id="017f4-106">يسمى الكيان القانوني الذي يوظف العامل الكيان القانوني المقرض.</span><span class="sxs-lookup"><span data-stu-id="017f4-106">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="017f4-107">يسمى الكيان القانوني الذي يتكبد العامل المصروفات له الكيان القانوني المقترض.</span><span class="sxs-lookup"><span data-stu-id="017f4-107">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="017f4-108">قبل أن يتمكن العامل من إنشاء مصاريف مشتركة بين الشركات وإرسالها، يجب تمكين بنود المصاريف المشتركة بين الشركات.</span><span class="sxs-lookup"><span data-stu-id="017f4-108">Before a worker can create and submit intercompany expenses, you must enable intercompany expense lines.</span></span> <span data-ttu-id="017f4-109">في الكيان القانوني المُقرِّض، من صفحة **معلمات إدارة المصاريف**، قم بتحديد **السماح ببنود المصاريف المشتركة بين الشركات**.</span><span class="sxs-lookup"><span data-stu-id="017f4-109">In the loaning legal entity, on the **Expense management parameters** page, select **Allow intercompany expense lines**.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="017f4-110">ترحيل الضرائب للمصروفات بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="017f4-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="017f4-111">قبل أن تتمكن من استخدام مجموعات الضريبة المقترنة بالكيان القانوني المُقرِّض (المصدر) بدلا من الكيان القانوني المقترض (الوجهة) في تقرير مصروفاتك، يجب تمكين الوظيفة في إعداد ضريبة مبيعات دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="017f4-111">Before you can use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you must enable the functionality in the General ledger sales tax setup.</span></span> <span data-ttu-id="017f4-112">عندما يتم تعيين **معلمة الكيان القانوني لنشر الضريبة بين الشركات** على **المصدر** و **تطبيق قواعد زيادة الضريبة على المبيعات** على **لا**، يتم استخدام توليفة الضريبة للكيان القانوني المُقرِّض.</span><span class="sxs-lookup"><span data-stu-id="017f4-112">When the **Legal entity for intercompany tax posting** parameter is set to **Source** and **Apply sales tax taxation rules** is set to **No**, the tax combination for the loaning legal entity is used.</span></span> <span data-ttu-id="017f4-113">عندما يتم تعيين نفس المعلمة إلى **الوجهة**، سيتم استخدام مجموعه الضرائب للكيان القانوني المقترض.</span><span class="sxs-lookup"><span data-stu-id="017f4-113">When the same parameter is set to **Destination**, the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="017f4-114">بالنسبة إلى الكيانات القانونية في الولايات المتحدة، عندما يتم تعيين المعلمة إلى **المصدر**، يجب أيضًا تكوين الحقل **مقبوضات لضريبة المبيعات** في صفحة **مجموعات ترحيل دفتر الأستاذ العام** الجديدة.</span><span class="sxs-lookup"><span data-stu-id="017f4-114">For legal entities in the United States, when the parameter is set to **Source**, the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="017f4-115">سيستخدم محرك المحاسبة المعلومات من هذا الحقل للإدخال المحاسبي المتعلق بالضريبة.</span><span class="sxs-lookup"><span data-stu-id="017f4-115">The accounting engine will use the information from this field for tax-related accounting entry.</span></span>   
<span data-ttu-id="017f4-116">يكون السلوك متسقًا بالنسبة لبنود المصروفات التي تم ترحيلها مع مشروع أو بدونه.</span><span class="sxs-lookup"><span data-stu-id="017f4-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  


[!INCLUDE[footer-include](../includes/footer-banner.md)]