---
title: الجديد أو المتغير في إصدار التحديث 12، الإصدار 3 من Project Service Automation
description: يقدم هذا الموضوع معلومات حول الجديد في إصدار التحديث 12، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: 58a12ded135712d8194499ce4a9ba9e4e2aa99bd
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949483"
---
# <a name="project-service-automation-update-release-12-v3"></a><span data-ttu-id="340fd-103">الإصدار 3 من Project Service Automation، إصدار التحديث 12</span><span class="sxs-lookup"><span data-stu-id="340fd-103">Project Service Automation Update Release 12, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="340fd-104">يسرنا الإعلان عن آخر تحديث لتطبيق Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="340fd-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="340fd-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="340fd-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="340fd-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="340fd-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="340fd-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="340fd-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="340fd-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="340fd-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="340fd-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 12.</span><span class="sxs-lookup"><span data-stu-id="340fd-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 12.</span></span> <span data-ttu-id="340fd-110">يتضمن هذا الإصدار رقم البنية V3.10.2.34 وهو متوفر بشكل عام من خلال تحديث ذاتي في أكتوبر 2019.</span><span class="sxs-lookup"><span data-stu-id="340fd-110">This version has a build number of V3.10.2.34 and is generally available through a self-update in October 2019.</span></span>

## <a name="update-release-12"></a><span data-ttu-id="340fd-111">إصدار التحديث 12</span><span class="sxs-lookup"><span data-stu-id="340fd-111">Update Release 12</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="340fd-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="340fd-112">Bug fixes</span></span>

- <span data-ttu-id="340fd-113">الوقت والمصروفات</span><span class="sxs-lookup"><span data-stu-id="340fd-113">Time and Expense</span></span>

    - <span data-ttu-id="340fd-114">إصلاح: تم تحديث المراسلة الخاصة بخطأ إدخال الوقت بواسطة سياق أكثر ملاءمة.</span><span class="sxs-lookup"><span data-stu-id="340fd-114">Fixed: Time entry error messaging has been updated with more relevant context.</span></span>
    - <span data-ttu-id="340fd-115">إصلاح: تعرض شبكة إدخال الوقت والجدول شريط التمرير العمودي بشكل صحيح عند الضرورة.</span><span class="sxs-lookup"><span data-stu-id="340fd-115">Fixed: Time entry grid and schedule correctly displays the vertical scrollbar when required.</span></span>
    - <span data-ttu-id="340fd-116">إصلاح: يمكن الموافقة على إدخال الوقت والمصروفات المرسلة.</span><span class="sxs-lookup"><span data-stu-id="340fd-116">Fixed: Submitted expense and time entries can be approved.</span></span>
    - <span data-ttu-id="340fd-117">إصلاح: تم تصحيح رسالة مربع حوار تأكيد إلغاء الموافقة لإظهار حالة الموافقة عند تغييرها من **معتمد‬‬** إلى **مرسل**.</span><span class="sxs-lookup"><span data-stu-id="340fd-117">Fixed: Cancel approval confirmation dialog message has been corrected to reflect the status of the approval when changed from **Approved** to **Submitted**.</span></span>
    - <span data-ttu-id="340fd-118">إصلاح: أصبحت الآن حقول **السعر** و **الوحدة** و **الكمية** مقفلة على سجل المصروفات بعد الموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="340fd-118">Fixed: **Price**, **Unit**, and **Quantity** fields are now locked on the Expense record after it is has been approved.</span></span>

- <span data-ttu-id="340fd-119">إدارة المشروع</span><span class="sxs-lookup"><span data-stu-id="340fd-119">Project Management</span></span>

    - <span data-ttu-id="340fd-120">إصلاح: تمت إزالة إجراء **جديد** على النموذج الرئيسي **عضو الفريق**.</span><span class="sxs-lookup"><span data-stu-id="340fd-120">Fixed: **New** action on **Team member** main form has been removed.</span></span>
    - <span data-ttu-id="340fd-121">إصلاح: تم تحديث تعيينات الموارد بحيث تأخذ في الاعتبار أخطاء التقريب غير الدقيقة، مما يؤدي إلى تغيير في تاريخ انتهاء المهمة.</span><span class="sxs-lookup"><span data-stu-id="340fd-121">Fixed: Resource assignments have been updated to account for inaccurate rounding errors, which lead to a shift in a task’s end date.</span></span>
    - <span data-ttu-id="340fd-122">إصلاح: في شريط المهمة، سوف تظهر للمستخدم الأخطاء ذات الصلة من جانب الخادم.</span><span class="sxs-lookup"><span data-stu-id="340fd-122">Fixed: In the task grid, relevant server-side errors will be surfaced to the user.</span></span>
    - <span data-ttu-id="340fd-123">إصلاح: يظهر الآن اسم عضو الفريق في منتقي أشخاص المهمة بدلاً من اسم المنصب.</span><span class="sxs-lookup"><span data-stu-id="340fd-123">Fixed: The team member’s name now renders in the task people picker instead of the position name.</span></span>

- <span data-ttu-id="340fd-124">إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="340fd-124">Resource Management</span></span>

    - <span data-ttu-id="340fd-125">إصلاح: تفاصيل متطلبات الموارد للمشاريع التي تم إنشاؤها من قالب تستخدم الآن تقويم المشروع.</span><span class="sxs-lookup"><span data-stu-id="340fd-125">Fixed: Resource requirement details for projects created from a template now use the project calendar.</span></span>
    - <span data-ttu-id="340fd-126">إصلاح: تعرض الآن المهارات والاختصاصات بشكل افتراضي متطلبات الموارد المنشأة للدور بدلاً من البيانات الرئيسية للدور.</span><span class="sxs-lookup"><span data-stu-id="340fd-126">Fixed: Skills and competencies now default from role master data to the resource requirement created for that role.</span></span>

- <span data-ttu-id="340fd-127">‏‏Sales</span><span class="sxs-lookup"><span data-stu-id="340fd-127">Sales</span></span>

    - <span data-ttu-id="340fd-128">إصلاح: توجد معرفات كائنات متكررة على نموذج **العقد الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="340fd-128">Fixed: Duplicate object IDs found on the **Contract main** form.</span></span>
    - <span data-ttu-id="340fd-129">إصلاح: تم تحديث المنطق لجعل علامة تبويب **تحليل عرض الاسعار** مرئية بحيث تعرض إعداد بيانات التعريف الخاصة بعلامة التبويب</span><span class="sxs-lookup"><span data-stu-id="340fd-129">Fixed: Logic has been updated to make the **Quote Analysis** tab visible so that it displays the metadata setup of the tab.</span></span>
    - <span data-ttu-id="340fd-130">إصلاح: التاريخ المحاسبي الخاص بالسجل الفعلي يأتي الآن من تاريخ إدخال المصروفات/الوقت وليس تاريخ الموافقة.</span><span class="sxs-lookup"><span data-stu-id="340fd-130">Fixed: Accounting date on the actual record now comes from the date of the time/expense entry date and not the date of the approval.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]