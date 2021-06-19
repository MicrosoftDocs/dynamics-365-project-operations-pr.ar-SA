---
title: إرسال طلب المورد
description: يمكنك إرسال متطلب مورد تم إنشاؤه كطلب مورد. ثم يتم إرسال الطلب إلى مدير مورد لاستيفائه.
author: ruhercul
ms.date: 10/04/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 6ac0044a27d1e506c9c62c477014017fd0ca06cb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014010"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="3c01c-104">إرسال طلب المورد</span><span class="sxs-lookup"><span data-stu-id="3c01c-104">Submit a resource request</span></span>

<span data-ttu-id="3c01c-105">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="3c01c-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3c01c-106">يمكنك إرسال متطلب مورد تم إنشاؤه كطلب مورد.</span><span class="sxs-lookup"><span data-stu-id="3c01c-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="3c01c-107">ثم يتم إرسال الطلب إلى مدير مورد لاستيفائه.</span><span class="sxs-lookup"><span data-stu-id="3c01c-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="3c01c-108">في Dynamics 365 Project Operations، في صفحة **المشاريع**، حدد علامة التبويب **فريق** لعرض قائمة بالموارد القابلة للحجز.</span><span class="sxs-lookup"><span data-stu-id="3c01c-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="3c01c-109">حدد المورد العام الذي يحتوي على متطلب مورد من القائمة، ثم انقر فوق **إرسال طلب**.</span><span class="sxs-lookup"><span data-stu-id="3c01c-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="3c01c-110">ستتغير حالة طلب عضو الفريق العام إلى **تم الإرسال**.</span><span class="sxs-lookup"><span data-stu-id="3c01c-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="3c01c-111">بعد استيفاء الطلب، سيتم استبدال المورد العام بمورد مسمى إذا كان مدير الموارد يفي بالطلب من خلال حجز مورد مسمي.</span><span class="sxs-lookup"><span data-stu-id="3c01c-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="3c01c-112">بخلاف ذلك، إذا اقترح مدير الموارد موردًا مسمى، سيظل المورد العام في الفريق وستتغير حالة الطلب إلى **في حاجة إلى المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="3c01c-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]