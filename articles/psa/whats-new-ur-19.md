---
title: الجديد أو المتغير في الإصدار 3 من Project Service Automation، إصدار التحديث 19
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 19.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: e116bcbb8e9d184b7b894709c893aaf1dadefc2f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126805"
---
# <a name="project-service-automation-update-release-19-v3"></a><span data-ttu-id="df3be-103">الإصدار 3 من Project Service Automation، إصدار التحديث 19</span><span class="sxs-lookup"><span data-stu-id="df3be-103">Project Service Automation Update Release 19, V3</span></span>

<span data-ttu-id="df3be-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="df3be-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="df3be-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="df3be-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="df3be-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="df3be-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="df3be-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="df3be-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="df3be-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="df3be-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="df3be-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في PSA V3، إصدار التحديث 19.</span><span class="sxs-lookup"><span data-stu-id="df3be-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 19.</span></span> <span data-ttu-id="df3be-110">لدى هذا الإصدار رقم البنية V3.10.30.41 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر مايو 2020.</span><span class="sxs-lookup"><span data-stu-id="df3be-110">This version has a build number of V3.10.30.41 and is generally available through a self-update in May 2020.</span></span>

## <a name="update-release-19"></a><span data-ttu-id="df3be-111">إصدار التحديث 19</span><span class="sxs-lookup"><span data-stu-id="df3be-111">Update Release 19</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="df3be-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="df3be-112">Bug fixes</span></span>

<span data-ttu-id="df3be-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="df3be-113">**Time and Expense**</span></span>

<span data-ttu-id="df3be-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="df3be-114">The following issues have been fixed:</span></span> 

- <span data-ttu-id="df3be-115">الأخطاء المشتقة من عمليات استيراد إدخالات الوقت لا تظهر بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="df3be-115">Errors derived from time entry imports are not surfaced correctly.</span></span>
- <span data-ttu-id="df3be-116">لا تدعم شبكة إدخال الوقت سلوك حقل **التاريخ فقط**.</span><span class="sxs-lookup"><span data-stu-id="df3be-116">Time Entry Grid does not support **Date Only** field behavior.</span></span>
- <span data-ttu-id="df3be-117">يتعذر على موارد المشروع إنشاء مصروفات مع مشروع.</span><span class="sxs-lookup"><span data-stu-id="df3be-117">Project Resources are unable to create an expense with a project.</span></span>

<span data-ttu-id="df3be-118">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="df3be-118">**Project Management**</span></span>

<span data-ttu-id="df3be-119">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="df3be-119">The following issues have been fixed:</span></span> 

-  <span data-ttu-id="df3be-120">تتسبب مهمة فرعية كبيرة في تقدير جهد غير صحيح أثناء حساب الاكتمال (EAC).</span><span class="sxs-lookup"><span data-stu-id="df3be-120">Grandchild task causes an incorrect effort estimate during the Completion (EAC) Calculation.</span></span>

<span data-ttu-id="df3be-121">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="df3be-121">**Sales**</span></span>

<span data-ttu-id="df3be-122">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="df3be-122">The following issues have been fixed:</span></span> 

- <span data-ttu-id="df3be-123">لا يعمل إجراء **إعادة الحساب** مع تفاصيل شروط التعاقد أو تفاصيل بنود عرض الأسعار للمصروفات.</span><span class="sxs-lookup"><span data-stu-id="df3be-123">The **Recalculate** action does not work with expense contract line details or quote line details.</span></span>
- <span data-ttu-id="df3be-124">خيار **تحديث الأسعار** غير موجود في تقديرات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="df3be-124">**Update Prices** is missing for expense estimates.</span></span>
-  <span data-ttu-id="df3be-125">يتعذر على العملاء تحديد أسباب حالة العقد المخصص من صفحة **عقد المشروع**.</span><span class="sxs-lookup"><span data-stu-id="df3be-125">Customers are unable to select custom contract status reasons from the **Project Contract** page.</span></span>
- <span data-ttu-id="df3be-126">يواجه العملاء انخفاضًا في مستوى الأداء عند إنشاء قائمة أسعار مخصصة من عرض أسعار.</span><span class="sxs-lookup"><span data-stu-id="df3be-126">Customers experience degraded performance when creating a custom price list from a quote.</span></span>
- <span data-ttu-id="df3be-127">يواجه العملاء عدم اتساق مع الإعدادات الافتراضية على **الوحدة** على الصفحتين **تفاصيل بنود عرض الأسعار** و **تفاصيل شروط التعاقد**.</span><span class="sxs-lookup"><span data-stu-id="df3be-127">Customers experience inconsistency with **unit** defaults on **Quote Line Details** and **Contract Line Details** pages.</span></span>
- <span data-ttu-id="df3be-128">لن تؤدي إضافة أصناف من فئة عملية لا يتحمل نفقتها العميل إلى شروط تعاقد يتحمل نفقتها العميل إلى مراعاة نوع الفوترة **غير خاضع للرسوم** لفئة العملية.</span><span class="sxs-lookup"><span data-stu-id="df3be-128">Adding non-chargeable transaction category items to a chargeable contract line will not respect the **Non-chargeable** billing type of the transaction category.</span></span>
- <span data-ttu-id="df3be-129">يتعذر على العملاء استخدام الأدوار والفئات المضافة حديثًا على العقود التي تم إنشاؤها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="df3be-129">Customers can't use the newly added roles and category on previously created contracts.</span></span>
- <span data-ttu-id="df3be-130">يواجه العملاء انخفاضًا في مستوى الأداء. استرداد غير ضروري في PreValidateProjectTeamMemberUpdate.cs</span><span class="sxs-lookup"><span data-stu-id="df3be-130">Customers experience degraded performance Unnecessary retrieve in PreValidateProjectTeamMemberUpdate.cs</span></span>
- <span data-ttu-id="df3be-131">يجب إضافة الأدوار التي تم إعدادها كأدوار غير خاضعة للرسوم في قائمة **فئات الموارد** إلى علامة التبويب **الأدوار الخاضعة للرسوم‬** كأدوار **غير خاضعة للرسوم‬** في شروط التعاقد الخاصة بمشروع.</span><span class="sxs-lookup"><span data-stu-id="df3be-131">Roles set up as non-chargeable in the **Resource Categories** list should be added to the **Chargeable Roles** tab as **Non0chargeable** on the contract line for a project.</span></span>
- <span data-ttu-id="df3be-132">قد يواجه العملاء انخفاضًا في مستوى الأداء عند إنشاء مشروع لأن **GetBookableResourceIdFromUser** يسترد جميع أعمدة الموارد القابلة للحجز بدلاً من المعرف الأساسي‬ فقط.</span><span class="sxs-lookup"><span data-stu-id="df3be-132">Customers may experience degraded performance when creating a project because **GetBookableResourceIdFromUser** retrieves all columns of bookable resources instead of just the primary ID.</span></span>
- <span data-ttu-id="df3be-133">يفتقد الكيان **TransactionType** المكون الإضافي لتحديث التحقق المسبق من الصحة‬ لمنع المستخدمين من إدخال **الوحدات** و **مجموعات الوحدات‏‎** غير الصالحة لنوع العملية.</span><span class="sxs-lookup"><span data-stu-id="df3be-133">**TransactionType** entity missing the pre-validation update plug-in to prevent users from entering **Units** and **UnitGroups** that are not valid for transaction types.</span></span>
- <span data-ttu-id="df3be-134">لا تعمل خطوة **الإزالة** لاستيراد إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="df3be-134">The **Remove** step does not work for time entry import.</span></span>
