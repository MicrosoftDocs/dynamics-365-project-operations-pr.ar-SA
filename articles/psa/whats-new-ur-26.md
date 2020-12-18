---
title: ما الجديد أو المتغير في إصدار التحديث 26 من Project Service Automation، الإصدار 3
ms.openlocfilehash: 849e7288ee91d3e9360c0b03f6b8b37ff29338e7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643247"
---
<a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="f0e40-102">إصدار التحديث 26 من Project Service Automation، الإصدار 3</span><span class="sxs-lookup"><span data-stu-id="f0e40-102">Project Service Automation Update Release 26, V3</span></span>
================================================

<span data-ttu-id="f0e40-103">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f0e40-103">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="f0e40-104">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="f0e40-104">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="f0e40-105">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f0e40-105">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f0e40-106">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="f0e40-106">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="f0e40-107">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f0e40-107">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f0e40-108">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو المتغيرة لإصدار التحديث 26 من Project Service Automation، الإصدار 3‬</span><span class="sxs-lookup"><span data-stu-id="f0e40-108">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="f0e40-109">يحتوي هذا الإصدار على رقم إصدار V3.10.44.59 وهو متاح بشكل عام من خلال التحديث الذاتي في ديسمبر 2020.</span><span class="sxs-lookup"><span data-stu-id="f0e40-109">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

<a name="update-release-26"></a><span data-ttu-id="f0e40-110">إصدار التحديث 26</span><span class="sxs-lookup"><span data-stu-id="f0e40-110">Update Release 26</span></span>
-----------------

### <a name="bug-fixes"></a><span data-ttu-id="f0e40-111">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="f0e40-111">Bug fixes</span></span>

<span data-ttu-id="f0e40-112">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="f0e40-112">**Time and Expense**</span></span>

<span data-ttu-id="f0e40-113">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="f0e40-113">The following issues have been fixed:</span></span>

-   <span data-ttu-id="f0e40-114">يمكن للمستخدمين تغيير المهمة في إدخال الوقت الذي تمت الموافقة عليه/إرساله.</span><span class="sxs-lookup"><span data-stu-id="f0e40-114">Users are able to change the task on a time entry that has been approved/submitted.</span></span>

-   <span data-ttu-id="f0e40-115">حدث خطأ "لم يتم تعيين مرجع الكائن" عند حفظ إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="f0e40-115">"Object Reference Not Set" error when saving time entry.</span></span>

-   <span data-ttu-id="f0e40-116">يقوم استيراد إدخال الوقت من تعيينات الموارد بإنشاء إدخالات الوقت بقيم التاريخ/الوقت غير الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="f0e40-116">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>

-   <span data-ttu-id="f0e40-117">عندما يتم تثبيت كلٍّ من Project Service Automation وتطبيق Field Service، فإنه يتم عرض الزر **جديد** مرتين على شريط الأوامر لإدخالات الوقت في تطبيق Field Service.</span><span class="sxs-lookup"><span data-stu-id="f0e40-117">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>

-   <span data-ttu-id="f0e40-118">تعمل تحديثات خلايا **السماح بالوحدة** و **مجموعة الوحدة** في شبكة **تقديرات المصاريف**.</span><span class="sxs-lookup"><span data-stu-id="f0e40-118">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>

-   <span data-ttu-id="f0e40-119">يشتمل نموذج **تحرير إدخال وقت التحديث** على **المخطط الزمني**.</span><span class="sxs-lookup"><span data-stu-id="f0e40-119">**Update Time Entry Edit** form includes **Timeline**.</span></span>

-   <span data-ttu-id="f0e40-120">تؤدي الموافقة على إدخالات الوقت لغير المشروع إلى حظر النظام عند البحث عن دور مانح على المشروع.</span><span class="sxs-lookup"><span data-stu-id="f0e40-120">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="f0e40-121">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="f0e40-121">**Resource Management**</span></span>

<span data-ttu-id="f0e40-122">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="f0e40-122">The following issues have been fixed:</span></span>

-   <span data-ttu-id="f0e40-123">تمت إضافة عملية التحقق من الصحة في المكون الإضافي لـ **PostProjectCreate** للتحقق من المتطلبات الأساسية قبل إنشاء واحدة.</span><span class="sxs-lookup"><span data-stu-id="f0e40-123">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>

-   <span data-ttu-id="f0e40-124">يطرح نموذج الإنشاء السريع لـ **عضو فريق المشروع** استثناء مرجعيًا فارغًا إذا تمت إزالة الحقول من النموذج.</span><span class="sxs-lookup"><span data-stu-id="f0e40-124">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>

-   <span data-ttu-id="f0e40-125">سيفشل إنشاء متطلبات لمدة 12 ساعة على مدى عام واحد.</span><span class="sxs-lookup"><span data-stu-id="f0e40-125">Generate requirements for 12 hours over 1 year will fail.</span></span>

-   <span data-ttu-id="f0e40-126">تم تحسين استثناء مرجع فارغ لرسالة الخطأ أثناء إنشاء متطلبات المورد.</span><span class="sxs-lookup"><span data-stu-id="f0e40-126">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="f0e40-127">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="f0e40-127">**Project Management**</span></span>

<span data-ttu-id="f0e40-128">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="f0e40-128">The following issues have been fixed:</span></span>

-   <span data-ttu-id="f0e40-129">تم تحسين التحقق من صحة لمعالجة استثناء مرجع فارغ تم إنشاؤه في المكون الإضافي لـ **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="f0e40-129">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>

-   <span data-ttu-id="f0e40-130">تحذف المشروعات المنشورة بواسطة الوظيفة الإضافية لسطح مكتب Microsoft Project التعيينات غير المعينة.</span><span class="sxs-lookup"><span data-stu-id="f0e40-130">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>

-   <span data-ttu-id="f0e40-131">تمت إضافة تحقق جديد عندما يكون مرجع مشروع المهمة غير صالح بسبب استثناء مرجع فارغ في المكون الإضافي لـ **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="f0e40-131">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>

-   <span data-ttu-id="f0e40-132">لا تعرض شبكة أعضاء الفريق التعيينات المميزة في سجل عضو الفريق.</span><span class="sxs-lookup"><span data-stu-id="f0e40-132">Team Member grid does not show distinct assignments on the team member record.</span></span>

-   <span data-ttu-id="f0e40-133">تمت إضافة رسائل تحقق وأخطاء جديدة بسبب استثناء مرجعي فارغ في المكون الإضافي لـ **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="f0e40-133">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="f0e40-134">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="f0e40-134">**Sales**</span></span>

<span data-ttu-id="f0e40-135">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="f0e40-135">The following issues have been fixed:</span></span>

-   <span data-ttu-id="f0e40-136">عند اختيار بند قائم على المشروع في عرض أسعار أو عقد، فإن الزر **اقتراح** يجب أن يكون مرئيًا فقط عند تحديد خط مستند إلى منتج مرتبط بمنتج موجود.</span><span class="sxs-lookup"><span data-stu-id="f0e40-136">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>

-   <span data-ttu-id="f0e40-137">قم بتقسم امتياز **Create_Product** من امتياز **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="f0e40-137">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>

-   <span data-ttu-id="f0e40-138">يؤدي حذف بند فاتورة إلى فشل مرجع فارغ في **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="f0e40-138">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>
