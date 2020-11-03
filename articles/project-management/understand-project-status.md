---
title: فهم حالة المشروع
description: يوفر هذا الموضوع معلومات حول الحالة المعينة للمشاريع في Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 336e479ad39653af14cca7930fe63e906b7de489
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070516"
---
# <a name="understand-project-status"></a><span data-ttu-id="5927d-103">فهم حالة المشروع</span><span class="sxs-lookup"><span data-stu-id="5927d-103">Understand project status</span></span>

<span data-ttu-id="5927d-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="5927d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="5927d-105">يوفر قسم  **الحالة** في صفحة  **كيان المشروع** ملخصًا لسلامة المشروع استنادًا إلى التكلفة والجهد.</span><span class="sxs-lookup"><span data-stu-id="5927d-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="5927d-106">حقول ملخص الحالة</span><span class="sxs-lookup"><span data-stu-id="5927d-106">Status summary fields</span></span>

- <span data-ttu-id="5927d-107">يعتبر حقل  **حالة المشروع الإجمالية**  حقلا قابلا للتحرير يوضح الحالة الإجمالية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="5927d-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="5927d-108">يستخدم هذا الحقل ترميز اللون، مثل الأخضر، والأصفر، والأحمر، للإشارة إلى زيادة المخاطرة.</span><span class="sxs-lookup"><span data-stu-id="5927d-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="5927d-109">يتيح حقل  **التعليقات** لمدير المشروع إدخال تعليقات معينة حول الحالة.</span><span class="sxs-lookup"><span data-stu-id="5927d-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="5927d-110">لا يكون حقل  **تاريخ تحديث الحالة** قابلا للتحرير.</span><span class="sxs-lookup"><span data-stu-id="5927d-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="5927d-111">القيمة الموجودة في هذا الحقل عبارة عن طابع زمني يشير إلى آخر تاريخ تم فيه تحديث الحالة.</span><span class="sxs-lookup"><span data-stu-id="5927d-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="5927d-112">يتم تعيين حقلي  **أداء الجدولة** و **أداء التكلفة** من شبكة التعقب.</span><span class="sxs-lookup"><span data-stu-id="5927d-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="5927d-113">عندما يكون تباين الجدول وتباين للعقدة الجذر في طريقة عرض  **تعقب الجهد** موجبًا، يتم تحديث هذه الحقول إلى  **متقدم**.</span><span class="sxs-lookup"><span data-stu-id="5927d-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="5927d-114">عندما يكون تباين الجدول التكلفة للعقدة الجذر سالبًا، يتم تعيين هذه الحقول إلى  **متأخر**.</span><span class="sxs-lookup"><span data-stu-id="5927d-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>
