---
title: فهم حالة المشروع
description: يوفر هذا الموضوع معلومات حول الحالة المعينة للمشاريع في Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ad8c012b93bc65595dca33df1770562916c557e0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993400"
---
# <a name="understand-project-status"></a><span data-ttu-id="1bcd0-103">فهم حالة المشروع</span><span class="sxs-lookup"><span data-stu-id="1bcd0-103">Understand project status</span></span>

<span data-ttu-id="1bcd0-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="1bcd0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="1bcd0-105">يوفر قسم **الحالة** في صفحة **كيان المشروع** ملخصًا لسلامة المشروع استنادًا إلى التكلفة والجهد.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="1bcd0-106">حقول ملخص الحالة</span><span class="sxs-lookup"><span data-stu-id="1bcd0-106">Status summary fields</span></span>

- <span data-ttu-id="1bcd0-107">يعتبر حقل **حالة المشروع الإجمالية** حقلا قابلا للتحرير يوضح الحالة الإجمالية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="1bcd0-108">يستخدم هذا الحقل ترميز اللون، مثل الأخضر، والأصفر، والأحمر، للإشارة إلى زيادة المخاطرة.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="1bcd0-109">يتيح حقل **التعليقات** لمدير المشروع إدخال تعليقات معينة حول الحالة.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="1bcd0-110">حقل **تاريخ تحديث الحالة** غير قابل للتحرير.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="1bcd0-111">القيمة الموجودة في هذا الحقل عبارة عن طابع زمني يشير إلى آخر تاريخ تم فيه تحديث الحالة.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="1bcd0-112">يتم تعيين حقل **أداء الجدولة** و **أداء التكلفة** من شبكة التعقب.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="1bcd0-113">عندما يكون تباين الجدول والتكلفة للعقدة الجذر في طريقة عرض **تعقب الجهد** موجبًا، يتم تحديث هذه الحقول إلى **متقدم**.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="1bcd0-114">عندما يكون تباين الجدول والتكلفة للعقدة الجذر سالبًا، يتم تعيين هذه الحقول إلى **متأخر**.</span><span class="sxs-lookup"><span data-stu-id="1bcd0-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]