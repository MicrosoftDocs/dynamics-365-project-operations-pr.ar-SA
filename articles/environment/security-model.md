---
title: نموذج الأمان
description: يقدم هذا الموضوع معلومات حول نموذج الأمان في Dynamics 365 Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 3f65d13809fef342be8bec682c11d95c4d9e9b19
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276782"
---
# <a name="security-model"></a><span data-ttu-id="a0687-103">نموذج الأمان</span><span class="sxs-lookup"><span data-stu-id="a0687-103">Security Model</span></span>

<span data-ttu-id="a0687-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="a0687-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="a0687-105">يحتوي Microsoft Dynamics 365 Project Operations على نموذج أمان فريد يسمح بنموذج أمان الأعمال المستند إلى الدور الذي يتعاون مع مجموعات Microsoft Office.</span><span class="sxs-lookup"><span data-stu-id="a0687-105">Microsoft Dynamics 365 Project Operations contains a unique security model that allows for a role-based business security model that collaborates with Microsoft Office Groups.</span></span> 


## <a name="security-roles"></a><span data-ttu-id="a0687-106">أدوار الأمان</span><span class="sxs-lookup"><span data-stu-id="a0687-106">Security roles</span></span>
<span data-ttu-id="a0687-107">تشمل إمكانات الواجهة الأمامية في Project Operations الأدوار التالية:</span><span class="sxs-lookup"><span data-stu-id="a0687-107">Project Operations front-end capabilities include the following roles:</span></span>

| <span data-ttu-id="a0687-108">الدور</span><span class="sxs-lookup"><span data-stu-id="a0687-108">Role</span></span>                          | <span data-ttu-id="a0687-109">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="a0687-109">Description</span></span>                                                                                                                                                                 | <span data-ttu-id="a0687-110">Scope</span><span class="sxs-lookup"><span data-stu-id="a0687-110">Scope</span></span> |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| <span data-ttu-id="a0687-111">مدير الممارسة</span><span class="sxs-lookup"><span data-stu-id="a0687-111">Practice manager</span></span>              | <span data-ttu-id="a0687-112">يدعم رفع التقارير عبر المشاريع.</span><span class="sxs-lookup"><span data-stu-id="a0687-112">Supports cross-project reporting.</span></span>                                                                                                            | <span data-ttu-id="a0687-113">وحدة العمل</span><span class="sxs-lookup"><span data-stu-id="a0687-113">Business unit</span></span>              |
| <span data-ttu-id="a0687-114">الموافق على المشروع</span><span class="sxs-lookup"><span data-stu-id="a0687-114">Project approver</span></span>              | <span data-ttu-id="a0687-115">يوافق على الوقت والمصروفات مقابل أحد المشاريع.</span><span class="sxs-lookup"><span data-stu-id="a0687-115">Approves time and expenses against a project.</span></span>                                                                                                                              | <span data-ttu-id="a0687-116">وحدة العمل</span><span class="sxs-lookup"><span data-stu-id="a0687-116">Business unit</span></span> |
| <span data-ttu-id="a0687-117">مسؤول فوترة المشروع</span><span class="sxs-lookup"><span data-stu-id="a0687-117">Project billing administrator</span></span> | <span data-ttu-id="a0687-118">ينشئ مقترح الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="a0687-118">Creates the invoice proposal.</span></span>                                                                                                                                                 | <span data-ttu-id="a0687-119">وحدة العمل</span><span class="sxs-lookup"><span data-stu-id="a0687-119">Business unit</span></span> |
| <span data-ttu-id="a0687-120">مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="a0687-120">Project manager</span></span>               | <span data-ttu-id="a0687-121">يقوم بإنشاء خطة المشروع ويطلب الموارد.</span><span class="sxs-lookup"><span data-stu-id="a0687-121">Creates the project plan and requests resources.</span></span>                                                                                                                              | <span data-ttu-id="a0687-122">وحدة العمل</span><span class="sxs-lookup"><span data-stu-id="a0687-122">Business unit</span></span> |
| <span data-ttu-id="a0687-123">مورد المشروع</span><span class="sxs-lookup"><span data-stu-id="a0687-123">Project resource</span></span>              | <span data-ttu-id="a0687-124">أعضاء الفريق الذين يمكن حجزهم ووقت التقرير.</span><span class="sxs-lookup"><span data-stu-id="a0687-124">Team members who can be booked and report time.</span></span>                                                                                                          | <span data-ttu-id="a0687-125">وحدة العمل</span><span class="sxs-lookup"><span data-stu-id="a0687-125">Business unit</span></span>|
| <span data-ttu-id="a0687-126">مدير الموارد</span><span class="sxs-lookup"><span data-stu-id="a0687-126">Resource manager</span></span>              | <span data-ttu-id="a0687-127">تكون كافة وظائف إدارة الموارد، مثل استيفاء طلبات الموارد والحجوزات، مفصولة لدعم تكوين مدير مشروع مختلط + مدير الموارد ودعم دور مدير موارد واحد ومركزي.</span><span class="sxs-lookup"><span data-stu-id="a0687-127">All resource management functions, such as fulfill resource requests and bookings, separated to support a hybrid Project manager + Resource manager configuration and a single and centralized Resource manager role.</span></span> | <span data-ttu-id="a0687-128">وحدة العمل</span><span class="sxs-lookup"><span data-stu-id="a0687-128">Business unit</span></span> |


<span data-ttu-id="a0687-129">يتضمن Microsoft Project للويب الأدوار التالية:</span><span class="sxs-lookup"><span data-stu-id="a0687-129">Microsoft Project for the Web includes the following roles:</span></span>

| <span data-ttu-id="a0687-130">الدور</span><span class="sxs-lookup"><span data-stu-id="a0687-130">Role</span></span>           | <span data-ttu-id="a0687-131">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="a0687-131">Description</span></span>                                                                                                        | <span data-ttu-id="a0687-132">Scope</span><span class="sxs-lookup"><span data-stu-id="a0687-132">Scope</span></span>  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| <span data-ttu-id="a0687-133">مستخدم المشروع</span><span class="sxs-lookup"><span data-stu-id="a0687-133">Project user</span></span>   | <span data-ttu-id="a0687-134">المستخدم التعاوني للمشروع الذي يمكنه إنشاء المشروعات الخاصة به وعرض أية مشاريع مشتركة معه.</span><span class="sxs-lookup"><span data-stu-id="a0687-134">Collaborative user of Project   who is able to create their own projects and view any projects shared with   them.</span></span> | <span data-ttu-id="a0687-135">المستخدم</span><span class="sxs-lookup"><span data-stu-id="a0687-135">User</span></span>   |
| <span data-ttu-id="a0687-136">نظام المشروع</span><span class="sxs-lookup"><span data-stu-id="a0687-136">Project system</span></span> | <span data-ttu-id="a0687-137">الدور المستخدم لسياق التطبيق.</span><span class="sxs-lookup"><span data-stu-id="a0687-137">Role used for application   context.</span></span> <span data-ttu-id="a0687-138">لا ينبغي أن يستخدم العملاء دور النظام هذا.</span><span class="sxs-lookup"><span data-stu-id="a0687-138">Customers should not use this system role.</span></span>                                    | <span data-ttu-id="a0687-139">عمومي</span><span class="sxs-lookup"><span data-stu-id="a0687-139">Global</span></span> |

## <a name="security-enforcement"></a><span data-ttu-id="a0687-140">فرض الأمان</span><span class="sxs-lookup"><span data-stu-id="a0687-140">Security enforcement</span></span>
<span data-ttu-id="a0687-141">الإجراءات التي يتم تنفيذها على مستوي المشروع يتم تنفيذها في سياق المستخدم الذي قام بتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="a0687-141">Actions that are performed at the project level are performed in the context of the logged in user.</span></span> <span data-ttu-id="a0687-142">وهذا يعني أنه لإنشاء مشروع أو فتحه أو حذفه، سيكون المستخدم مطالبا بتوفر حق الوصول له إلى CDS.</span><span class="sxs-lookup"><span data-stu-id="a0687-142">This means that in order to create, open, or delete a project, the user is required to have access available in CDS.</span></span> <span data-ttu-id="a0687-143">قد يتم منح الوصول إلى CDS من خلال أي من الأليات المحتملة المضمنة في النظام الأساسي.</span><span class="sxs-lookup"><span data-stu-id="a0687-143">Access in CDS may be granted through any of the possible mechanisms included in the platform.</span></span> <span data-ttu-id="a0687-144">على سبيل المثال، قد يصل مستخدم ذو نطاق أكبر إلى المشروع أو تم تنفيذ إجراء مشاركة مشروع واضح والذي يمنح الوصول للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="a0687-144">For example, a user with a larger scope may access the project or if an explicit project share action has been performed which grants the user access.</span></span>

<span data-ttu-id="a0687-145">من المهم وضع ذلك في الاعتبار عند إنشاء المشروعات في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a0687-145">It's important to consider this when creating projects in Project Operations.</span></span>

## <a name="modern-group-collaboration-with-project-operations"></a><span data-ttu-id="a0687-146">تعاون المجموعة الحديثة باستخدام Project Operations</span><span class="sxs-lookup"><span data-stu-id="a0687-146">Modern group collaboration with Project Operations</span></span>
<span data-ttu-id="a0687-147">يدعم تطبيق Project for the Web و Project Operations المجموعات الحديثة للتعاون.</span><span class="sxs-lookup"><span data-stu-id="a0687-147">Project for the Web and Project Operations support modern groups for collaboration.</span></span> <span data-ttu-id="a0687-148">يمكن للمستخدمين الذين تتم إضافتهم إلى المشروع من خلال مجموعة تحرير خطة المشروع.</span><span class="sxs-lookup"><span data-stu-id="a0687-148">Users added to the project through a group are able to edit the project plan.</span></span>

<span data-ttu-id="a0687-149">يضيف Project for the Web المستخدمين إلى المجموعة تلقائيًا عند التعيين.</span><span class="sxs-lookup"><span data-stu-id="a0687-149">Project for the Web adds users to the group automatically upon assignment.</span></span>

<span data-ttu-id="a0687-150">تسمح المجموعات لأذونات المشروع وتدعم العمل على البيانات الاصطناعية للتعاون بشكل تعاوني.</span><span class="sxs-lookup"><span data-stu-id="a0687-150">Groups allow the permissions of the project and supporting collaboration artifacts to be worked on collaboratively.</span></span> <span data-ttu-id="a0687-151">يصف المخطط التالي الأحداث وتغييرات الحالة التي تحدث أثناء عملية تعيين المجموعة.</span><span class="sxs-lookup"><span data-stu-id="a0687-151">The following diagram depicts the events and state changes that happen during the group assignment process.</span></span>

<span data-ttu-id="a0687-152">لا يقوم Project Operations بإنشاء مجموعة من خلال إجراء ضمني وإنما يقوم بذلك من خلال الإجراء الصريح للمجموعات الضاغطة.</span><span class="sxs-lookup"><span data-stu-id="a0687-152">Project Operations does not create a group through implicit action and only does so through the explicit action of pressing groups.</span></span>

<span data-ttu-id="a0687-153">يقتصر بحث أعضاء المجموعة في مربع الحوار **إدارة المجموعات** على هؤلاء الذين تم تعيينهم كجزء من مجموعة أمان البيئة.</span><span class="sxs-lookup"><span data-stu-id="a0687-153">Group member search in the **Group management** dialog, is limited to those who are set as part of the environment's security group.</span></span> <span data-ttu-id="a0687-154">لمزيد من المعلومات، راجع [التحكم في وصول المستخدم إلى البيئات: مجموعات الأمان والتراخيص](https://docs.microsoft.com/power-platform/admin/control-user-access).</span><span class="sxs-lookup"><span data-stu-id="a0687-154">For more information, see [Control user access to environments: security groups and licenses](https://docs.microsoft.com/power-platform/admin/control-user-access).</span></span>

![وضع المجموعة](./media/groupsmode.png)

1. <span data-ttu-id="a0687-156">يتم إنشاء المشروع وامتلاكه بواسطة المستخدم الذي قام بالإنشاء.</span><span class="sxs-lookup"><span data-stu-id="a0687-156">The Project is created and owned by the creating User.</span></span>
2. <span data-ttu-id="a0687-157">يتم تحديث مالك المشروع إلى الفريق.</span><span class="sxs-lookup"><span data-stu-id="a0687-157">The Project owner is updated to the team.</span></span>
3. <span data-ttu-id="a0687-158">تم تعيين الفريق المالك إلى مجموعة Office المحددة أو التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="a0687-158">The Owner team is mapped to the specified or created Office Group.</span></span>
4. <span data-ttu-id="a0687-159">تتم إضافة المالك الأصلي للمشروع إلى مجموعة Office.</span><span class="sxs-lookup"><span data-stu-id="a0687-159">The original owner of the Project is added to the Office Group.</span></span>

## <a name="deployment-recommendation"></a><span data-ttu-id="a0687-160">توصيات التوزيع</span><span class="sxs-lookup"><span data-stu-id="a0687-160">Deployment recommendation</span></span>
<span data-ttu-id="a0687-161">مع تطوير نموذج تعاون مجموعة Office، ستتم إضافة الوظائف لتوفير مزيد من التحكم المفصل بمرور الوقت.</span><span class="sxs-lookup"><span data-stu-id="a0687-161">As the Office group collaboration model evolves, functionality will be added to provide more detailed control over time.</span></span> <span data-ttu-id="a0687-162">سيتم تشجيع العملاء الذين يقومون بنشر Project Operations اليوم على التركيز على نموذج أمان Microsoft Dynamics 365 التقليدي.</span><span class="sxs-lookup"><span data-stu-id="a0687-162">Customers that deploy Project Operations today are encouraged to focus on a traditional Microsoft Dynamics 365 security model.</span></span>

<span data-ttu-id="a0687-163">لمزيد من المعلومات، انظر [الأمان في Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).</span><span class="sxs-lookup"><span data-stu-id="a0687-163">For more information, see [Security in Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).</span></span>

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a><span data-ttu-id="a0687-164">أمان Project Operations وMicrosoft Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="a0687-164">Project Operations and Microsoft Dynamics 365 Finance security</span></span>
<span data-ttu-id="a0687-165">يشمل Project Operations الأدوار التالية:</span><span class="sxs-lookup"><span data-stu-id="a0687-165">Project Operations includes the following roles:</span></span>

- <span data-ttu-id="a0687-166">مدير المشروع</span><span class="sxs-lookup"><span data-stu-id="a0687-166">Project manager</span></span>
- <span data-ttu-id="a0687-167">محاسب المشروع</span><span class="sxs-lookup"><span data-stu-id="a0687-167">Project accountant</span></span>

<span data-ttu-id="a0687-168">للحصول على مزيد من المعلومات حول الأمان في Finance، راجع [الأمان المستند إلى الدور](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span><span class="sxs-lookup"><span data-stu-id="a0687-168">For more information about security in Finance, see [Role-based security](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]