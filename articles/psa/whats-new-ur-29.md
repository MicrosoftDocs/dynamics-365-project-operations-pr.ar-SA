---
title: الجديد أو المتغير في إصدار التحديث 29، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 29، الإصدار V3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 2ac47974b9cc8386c7446136faf48724de73efce
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948556"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a><span data-ttu-id="ca60e-103">الجديد أو المتغير في إصدار التحديث 29، الإصدار 3 من Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="ca60e-103">What's new or changed in Project Service Automation Update Release 29, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="ca60e-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="ca60e-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="ca60e-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="ca60e-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="ca60e-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="ca60e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="ca60e-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="ca60e-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="ca60e-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="ca60e-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="ca60e-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار V3 من Project Service Automation، إصدار التحديث 29.</span><span class="sxs-lookup"><span data-stu-id="ca60e-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.</span></span> <span data-ttu-id="ca60e-110">يحتوي هذا الإصدار على رقم إصدار V3.10.47.7 وهو متاح بشكل عام من خلال التحديث الذاتي في فبراير 2021.</span><span class="sxs-lookup"><span data-stu-id="ca60e-110">This version has a build number of V3.10.47.7 and is generally available through a self-update in February 2021.</span></span>

## <a name="update-release-29"></a><span data-ttu-id="ca60e-111">إصدار التحديث 29</span><span class="sxs-lookup"><span data-stu-id="ca60e-111">Update Release 29</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="ca60e-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="ca60e-112">Bug fixes</span></span>

<span data-ttu-id="ca60e-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="ca60e-113">**Time and Expense**</span></span>

<span data-ttu-id="ca60e-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="ca60e-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="ca60e-115">يتعذر على للمستخدمين رؤية ساعات العمل المسجلة في أيام خارج أيام العمل في شبكة إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="ca60e-115">Users can't see working hours logged on non-working days in the time entry grid.</span></span>
- <span data-ttu-id="ca60e-116">يمكن تحرير إدخالات المصروفات الموافق عليها على الشبكة.</span><span class="sxs-lookup"><span data-stu-id="ca60e-116">Approved expense entries can be edited on the grid.</span></span>

<span data-ttu-id="ca60e-117">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="ca60e-117">**Project Management**</span></span>

<span data-ttu-id="ca60e-118">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="ca60e-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="ca60e-119">منطق التحقق من الصحة مفقود للتأكد من أن ساعات مجهود تعيين الموارد لا يمكن أن تكون سالبة.</span><span class="sxs-lookup"><span data-stu-id="ca60e-119">Missing validation logic to ensure resource assignment effort hours can't be negative.</span></span>
- <span data-ttu-id="ca60e-120">يقوم الإجراء المخصص، **AssignResourcesForTask** بتحديث جميع الحقول بدلاً من الحقول المتغيرة فقط.</span><span class="sxs-lookup"><span data-stu-id="ca60e-120">The custom action, **AssignResourcesForTask** updates all fields instead of only changed fields.</span></span>
- <span data-ttu-id="ca60e-121">عند نسخ مشروع في بيئة بها مكونات إضافية أو عمليات سير عمل مسجلة في الحدث **CreateProject**، لا يتم تحديث السمة **msdyn_bulkgenerationstatus** عند فشل **CopyWBSToProject**.</span><span class="sxs-lookup"><span data-stu-id="ca60e-121">When copying a project in an environment with plug-ins or workflows that are registered on the **CreateProject** event, the **msdyn_bulkgenerationstatus** attribute isn't updated if the **CopyWBSToProject** fails.</span></span>
- <span data-ttu-id="ca60e-122">عند توسيع تقويم المشروع، لا يتم فرز أيام العمل بالترتيب التصاعدي مما يتسبب في فشل بعض تحديثات مهام المشروع.</span><span class="sxs-lookup"><span data-stu-id="ca60e-122">When you expand the project calendar, the working days aren't sorted in ascending order causing some project task updates to fail.</span></span>
- <span data-ttu-id="ca60e-123">يؤدي تغيير مدير المشروع في مشروع موجود إلى تشغيل المنطق الافتراضية للوحدة المؤسسية.</span><span class="sxs-lookup"><span data-stu-id="ca60e-123">Changing the Project Manager on an existing project triggers the organizational unit defaulting logic.</span></span>

<span data-ttu-id="ca60e-124">**‏المبيعات**</span><span class="sxs-lookup"><span data-stu-id="ca60e-124">**Sales**</span></span>

<span data-ttu-id="ca60e-125">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="ca60e-125">The following issues have been fixed:</span></span>

- <span data-ttu-id="ca60e-126">تفشل علامة التبويب **أداء العقد** في صفحة **العقد‏‎** بشكل صامت أثناء التهيئة عند عدم وجود شروط تعاقد.</span><span class="sxs-lookup"><span data-stu-id="ca60e-126">The **Contract Performance** tab on the **Contract** page fails silently during initialization when no contract lines are present.</span></span>