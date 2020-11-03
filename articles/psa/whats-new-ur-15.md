---
title: الجديد أو المتغير في إصدار التحديث 15، الإصدار 3 من Project Service Automation
description: يقدم هذا الموضوع معلومات حول الجديد في إصدار التحديث 15، الإصدار 3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 01/27/2020
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
ms.openlocfilehash: 6112e4874025e528a2bb583cf215fd9eff681534
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070601"
---
# <a name="project-service-automation-update-release-15-v3"></a><span data-ttu-id="cdd70-103">الإصدار 3 من Project Service Automation، إصدار التحديث 15</span><span class="sxs-lookup"><span data-stu-id="cdd70-103">Project Service Automation Update Release 15, V3</span></span>

<span data-ttu-id="cdd70-104">يسرنا الإعلان عن آخر تحديث لتطبيق Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="cdd70-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="cdd70-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="cdd70-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="cdd70-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="cdd70-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="cdd70-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="cdd70-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="cdd70-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="cdd70-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="cdd70-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في PSA V3، إصدار التحديث 15.</span><span class="sxs-lookup"><span data-stu-id="cdd70-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 15.</span></span> <span data-ttu-id="cdd70-110">يتضمن هذا الإصدار رقم البنية V3.10.5.28 وهو متوفر بشكل عام من خلال تحديث ذاتي في يناير 2020.</span><span class="sxs-lookup"><span data-stu-id="cdd70-110">This version has a build number of V3.10.5.28 and is generally available through a self-update in January 2020.</span></span>

## <a name="update-release-15"></a><span data-ttu-id="cdd70-111">إصدار التحديث 15</span><span class="sxs-lookup"><span data-stu-id="cdd70-111">Update Release 15</span></span> 

### <a name="enhancements"></a><span data-ttu-id="cdd70-112">التحسينات</span><span class="sxs-lookup"><span data-stu-id="cdd70-112">Enhancements</span></span>

- <span data-ttu-id="cdd70-113">إدارة المشروع</span><span class="sxs-lookup"><span data-stu-id="cdd70-113">Project Management</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="cdd70-114">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="cdd70-114">Bug fixes</span></span>

- <span data-ttu-id="cdd70-115">الوقت والمصروفات</span><span class="sxs-lookup"><span data-stu-id="cdd70-115">Time and Expense</span></span>

  - <span data-ttu-id="cdd70-116">إصلاح: إضافة التعامل مع أخطاء التحميل في طريقة عرض التسوية.</span><span class="sxs-lookup"><span data-stu-id="cdd70-116">Fixed: Add on-load error handling in the reconciliation view.</span></span>
  - <span data-ttu-id="cdd70-117">إصلاح: مركز موارد المشروع: إعادة تسمية **المبلغ** لتقليل الالتباس.</span><span class="sxs-lookup"><span data-stu-id="cdd70-117">Fixed: Project Resource Hub: Rename **Amount** to reduce ambiguity.</span></span>
  - <span data-ttu-id="cdd70-118">إصلاح: ضبط طريقة العرض **نسخ أعمدة إدخال الوقت** لتضمين النوع.</span><span class="sxs-lookup"><span data-stu-id="cdd70-118">Fixed: Adjust the view **Copy Time Entry Columns** to include the type.</span></span>
  - <span data-ttu-id="cdd70-119">إصلاح: يؤدي تحرير مدة إدخال الوقت في طريقة عرض الشبكة باستخدام الأرقام العشرية إلى حدوث خطأ غير معروف لبعض الأرقام.</span><span class="sxs-lookup"><span data-stu-id="cdd70-119">Fixed: Editing time entry duration in the grid view using decimal numbers results in unknown error for some numbers.</span></span>

- <span data-ttu-id="cdd70-120">إدارة المشروع</span><span class="sxs-lookup"><span data-stu-id="cdd70-120">Project Management</span></span>

  - <span data-ttu-id="cdd70-121">إصلاح: تتوسع الآن القائمة المنسدلة **استخدام في طريقة عرض التعقب** استنادًا إلى عرض الخيارات.</span><span class="sxs-lookup"><span data-stu-id="cdd70-121">Fixed: The drop-down menu for **Use in Tracking View** now expands based on the width of the options.</span></span>
  - <span data-ttu-id="cdd70-122">إصلاح: عند إدارة المشروعات في المنطقة الزمنية +13، قد تعرض حسابات المهام نتائج غير دقيقة.</span><span class="sxs-lookup"><span data-stu-id="cdd70-122">Fixed: When managing projects in the +13 time zone, tasks calculations can display inaccurate results.</span></span>
  - <span data-ttu-id="cdd70-123">إصلاح: تم تصحيح **وقت انتهاء عضو الفريق** عند استخدام تقويم بنظام 24 ساعة.</span><span class="sxs-lookup"><span data-stu-id="cdd70-123">Fixed: **Team Member End Time** has been corrected when using a 24-hour calendar.</span></span>
  - <span data-ttu-id="cdd70-124">إصلاح: أعيد تنشيط **BPF** في النموذج الرئيسي **msdyn_project**.</span><span class="sxs-lookup"><span data-stu-id="cdd70-124">Fixed: Re-activated the **BPF** in **msdyn_project** main form.</span></span>
  - <span data-ttu-id="cdd70-125">إصلاح: لم يعد حساب التعيينات يتجاهل يومًا واحدًا.</span><span class="sxs-lookup"><span data-stu-id="cdd70-125">Fixed: Assignments calculation no longer ignores one day.</span></span>
  - <span data-ttu-id="cdd70-126">إصلاح: تمت إضافة شعار إعلام جديد إلى نموذج المشروع عندما تختلف المنطقة الزمنية بين المستخدم والمشروع.</span><span class="sxs-lookup"><span data-stu-id="cdd70-126">Fixed: A new notification banner has been added to the project form when the time zone differs between user and project.</span></span>

- <span data-ttu-id="cdd70-127">‏‏Sales</span><span class="sxs-lookup"><span data-stu-id="cdd70-127">Sales</span></span>

  - <span data-ttu-id="cdd70-128">إصلاح: يمكن استخدام بحث فئة تقديرات المصروفات لتصفية التكرارات.</span><span class="sxs-lookup"><span data-stu-id="cdd70-128">Fixed: Expense estimate category lookup can be used to filter duplicates.</span></span>
  - <span data-ttu-id="cdd70-129">إصلاح: لم تعد التعليمات البرمجية في **PluginDomain.ExecuteInTryCatchBlock(..)** تخفي أصل الاستثناء.</span><span class="sxs-lookup"><span data-stu-id="cdd70-129">Fixed: Code in **PluginDomain.ExecuteInTryCatchBlock(..)** no longer hides the origin of the exception.</span></span>
  - <span data-ttu-id="cdd70-130">إصلاح: لم تعد تظهر رسالة الخطأ في **البحث عن المشروع‬** في النموذج **بند عرض الأسعار‬** عند وجود أكثر من 1000 مشروع.</span><span class="sxs-lookup"><span data-stu-id="cdd70-130">Fixed: No longer get an error message in **Project lookup** in the **Quote Line** form when there are more than 1000 projects.</span></span>
  - <span data-ttu-id="cdd70-131">إصلاح: تعرض الآن شبكة **التقديرات** لتقديرات العملات وتقديرات المصروفات رمز العملة الصحيح.</span><span class="sxs-lookup"><span data-stu-id="cdd70-131">Fixed: **Estimates** grid for labor estimates and expense estimates now displays the correct currency symbol.</span></span>
  - <span data-ttu-id="cdd70-132">إصلاح: بعد قيام مؤسسة بتحديث PSA من إصدار التحديث 14 إلى إصدار التحديث 15، يتوقف ظهور علامة التبويب **الجدول** كفارغة على نموذج **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="cdd70-132">Fixed: After an organization updates PSA from Update Release 14 to Update Release 15, the **Schedule** tab no longer appears as blank on the **Project** form.</span></span>
