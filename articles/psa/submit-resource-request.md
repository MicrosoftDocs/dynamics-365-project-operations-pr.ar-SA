---
title: إرسال طلب مورد
description: يوفر هذا الموضوع معلومات حول إرسال طلب لمورد مشروع.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: 173572be43149aea253bf7beddb993f8c50ab337
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149707"
---
# <a name="submitting-a-resource-request"></a><span data-ttu-id="1c207-103">إرسال طلب مورد</span><span class="sxs-lookup"><span data-stu-id="1c207-103">Submitting a resource request</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="1c207-104">يمكنك إرسال متطلب مورد تم إنشاؤه كطلب مورد.</span><span class="sxs-lookup"><span data-stu-id="1c207-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="1c207-105">ثم يتم إرسال الطلب إلى مدير مورد لاستيفائه.</span><span class="sxs-lookup"><span data-stu-id="1c207-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="1c207-106">في Project Service Automation (PSA)، في صفحة **المشاريع**، انقر فوق علامة التبويب **فريق** لعرض قائمة بالموارد القابلة للحجز.</span><span class="sxs-lookup"><span data-stu-id="1c207-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="1c207-107">حدد المورد العام الذي يحتوي على متطلب مورد من القائمة ثم انقر فوق **إرسال طلب**.</span><span class="sxs-lookup"><span data-stu-id="1c207-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![إرسال طلب مورد](media/RM-how-to-18.png)

<span data-ttu-id="1c207-109">ستتغير حالة طلب عضو الفريق العام إلى **تم الإرسال**.</span><span class="sxs-lookup"><span data-stu-id="1c207-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="1c207-110">بعد استيفاء الطلب بواسطة مدير الموارد، سيتم استبدال المورد العام بمورد محدد إذا كان مدير الموارد يفي بالطلب مع حجز مورد مسمي.</span><span class="sxs-lookup"><span data-stu-id="1c207-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="1c207-111">وبخلاف ذلك، سيظل المورد العام في الفريق وستتغير حالة الطلب إلى **في حاجة إلى المراجعة**، إذا اقترح مدير المورد موردًا مسمى.</span><span class="sxs-lookup"><span data-stu-id="1c207-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review**, if the resource manager has proposed a named resource.</span></span>
