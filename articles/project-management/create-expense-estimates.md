---
title: تقديرات المصروفات
description: يوفر هذا الموضوع معلومات حول تحديد المصروفات المستندة إلى المشروع أو تقييمها.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3f0429366c69346113003355679c055cd2c74ca3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287042"
---
# <a name="expense-estimates"></a><span data-ttu-id="52ec4-103">تقديرات المصروفات</span><span class="sxs-lookup"><span data-stu-id="52ec4-103">Expense estimates</span></span>
<span data-ttu-id="52ec4-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="52ec4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="52ec4-105">بالإضافة إلى تعريف التقديرات المستندة إلى الموارد، يسمح Dynamics 365 Project Operations لمدراء المشاريع تحديد المصروفات المستندة إلى المشروع لكل مشروع.</span><span class="sxs-lookup"><span data-stu-id="52ec4-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="52ec4-106">يمكن ربط كل بند مصروفات بمهمة مشروع أو فئة مصروفات معينة.</span><span class="sxs-lookup"><span data-stu-id="52ec4-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="52ec4-107">يتم عادةً تعريف فئات المصروفات على مستوى المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="52ec4-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="52ec4-108">يتم عادةً تعريف التسعير لكل فئة مصروفات في التدرج الهرمي التالي:</span><span class="sxs-lookup"><span data-stu-id="52ec4-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="52ec4-109">المؤسسة</span><span class="sxs-lookup"><span data-stu-id="52ec4-109">Organization</span></span>
- <span data-ttu-id="52ec4-110">العميل</span><span class="sxs-lookup"><span data-stu-id="52ec4-110">Customer</span></span>
- <span data-ttu-id="52ec4-111">عرض الأسعار/العقد</span><span class="sxs-lookup"><span data-stu-id="52ec4-111">Quote/contract</span></span>

<span data-ttu-id="52ec4-112">أكمل الخطوات التالية لعرض مصروفات المشروع أو إضافتها أو حذفها.</span><span class="sxs-lookup"><span data-stu-id="52ec4-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="52ec4-113">انتقل إلى **المشاريع**، وحدد المشروع الذي تريد العمل عليه.</span><span class="sxs-lookup"><span data-stu-id="52ec4-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="52ec4-114">حدد علامة التبويب **تقديرات المشروع**، واستعرض قائمة مصروفات المشروع.</span><span class="sxs-lookup"><span data-stu-id="52ec4-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="52ec4-115">حدد **مصروفات جديدة** لإضافة مصروفات.</span><span class="sxs-lookup"><span data-stu-id="52ec4-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="52ec4-116">أو حدد مصروفات لحذفها، ثم حدد **حذف المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="52ec4-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="52ec4-117">يتم تحديد السمات التالية لكل عنصر من بند مصروفات:</span><span class="sxs-lookup"><span data-stu-id="52ec4-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="52ec4-118">**الفئة**: هي التجميعات الشائعة المستخدمة لوصف كافة المصروفات التي يتم تحملها في مشروع.</span><span class="sxs-lookup"><span data-stu-id="52ec4-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="52ec4-119">**تاريخ البدء**: التاريخ الذي تم فيه التنبؤ بتحمل المصروفات.</span><span class="sxs-lookup"><span data-stu-id="52ec4-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="52ec4-120">**الكمية**: العدد المقدّر لبنود المصروفات لفئة معينة.</span><span class="sxs-lookup"><span data-stu-id="52ec4-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="52ec4-121">**سعر تكلفة الوحدة**: سعر الوحدة المستخدم لاحتساب تكلفة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="52ec4-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="52ec4-122">**سعر مبيعات الوحدة**: سعر الوحدة المستخدم لاحتساب أسعار مبيعات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="52ec4-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]