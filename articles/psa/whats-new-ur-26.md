---
title: ما الجديد أو المتغير في إصدار التحديث 26 من Project Service Automation، الإصدار 3
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 26، الإصدار V3 من Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
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
ms.openlocfilehash: 669b3ca4601bdac483db4e1d7f55a8bf5b3d9661
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948808"
---
# <a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="a3c46-103">إصدار التحديث 26 من Project Service Automation، الإصدار 3</span><span class="sxs-lookup"><span data-stu-id="a3c46-103">Project Service Automation Update Release 26, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="a3c46-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a3c46-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a3c46-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="a3c46-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a3c46-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="a3c46-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a3c46-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="a3c46-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="a3c46-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a3c46-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a3c46-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو المتغيرة لإصدار التحديث 26 من Project Service Automation، الإصدار 3‬</span><span class="sxs-lookup"><span data-stu-id="a3c46-109">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="a3c46-110">يحتوي هذا الإصدار على رقم إصدار V3.10.44.59 وهو متاح بشكل عام من خلال التحديث الذاتي في ديسمبر 2020.</span><span class="sxs-lookup"><span data-stu-id="a3c46-110">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

## <a name="update-release-26"></a><span data-ttu-id="a3c46-111">إصدار التحديث 26</span><span class="sxs-lookup"><span data-stu-id="a3c46-111">Update Release 26</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a3c46-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="a3c46-112">Bug fixes</span></span>

<span data-ttu-id="a3c46-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="a3c46-113">**Time and Expense**</span></span>

<span data-ttu-id="a3c46-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="a3c46-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="a3c46-115">يمكن للمستخدمين تغيير المهمة في إدخال الوقت الذي تمت الموافقة عليه/إرساله.</span><span class="sxs-lookup"><span data-stu-id="a3c46-115">Users are able to change the task on a time entry that has been approved/submitted.</span></span>
- <span data-ttu-id="a3c46-116">حدث خطأ "لم يتم تعيين مرجع الكائن" عند حفظ إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="a3c46-116">"Object Reference Not Set" error when saving time entry.</span></span>
- <span data-ttu-id="a3c46-117">يقوم استيراد إدخال الوقت من تعيينات الموارد بإنشاء إدخالات الوقت بقيم التاريخ/الوقت غير الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="a3c46-117">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>
- <span data-ttu-id="a3c46-118">عندما يتم تثبيت كلٍّ من Project Service Automation وتطبيق Field Service، فإنه يتم عرض الزر **جديد** مرتين على شريط الأوامر لإدخالات الوقت في تطبيق Field Service.</span><span class="sxs-lookup"><span data-stu-id="a3c46-118">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>
- <span data-ttu-id="a3c46-119">تعمل تحديثات خلايا **السماح بالوحدة** و **مجموعة الوحدة** في شبكة **تقديرات المصاريف**.</span><span class="sxs-lookup"><span data-stu-id="a3c46-119">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>
- <span data-ttu-id="a3c46-120">يشتمل نموذج **تحرير إدخال وقت التحديث** على **المخطط الزمني**.</span><span class="sxs-lookup"><span data-stu-id="a3c46-120">**Update Time Entry Edit** form includes **Timeline**.</span></span>
- <span data-ttu-id="a3c46-121">تؤدي الموافقة على إدخالات الوقت لغير المشروع إلى حظر النظام عند البحث عن دور مانح على المشروع.</span><span class="sxs-lookup"><span data-stu-id="a3c46-121">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="a3c46-122">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="a3c46-122">**Resource Management**</span></span>

<span data-ttu-id="a3c46-123">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="a3c46-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="a3c46-124">تمت إضافة عملية التحقق من الصحة في المكون الإضافي لـ **PostProjectCreate** للتحقق من المتطلبات الأساسية قبل إنشاء واحدة.</span><span class="sxs-lookup"><span data-stu-id="a3c46-124">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>
- <span data-ttu-id="a3c46-125">يطرح نموذج الإنشاء السريع لـ **عضو فريق المشروع** استثناء مرجعيًا فارغًا إذا تمت إزالة الحقول من النموذج.</span><span class="sxs-lookup"><span data-stu-id="a3c46-125">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>
- <span data-ttu-id="a3c46-126">سيفشل إنشاء متطلبات لمدة 12 ساعة على مدى عام واحد.</span><span class="sxs-lookup"><span data-stu-id="a3c46-126">Generate requirements for 12 hours over 1 year will fail.</span></span>
- <span data-ttu-id="a3c46-127">تم تحسين استثناء مرجع فارغ لرسالة الخطأ أثناء إنشاء متطلبات المورد.</span><span class="sxs-lookup"><span data-stu-id="a3c46-127">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="a3c46-128">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="a3c46-128">**Project Management**</span></span>

<span data-ttu-id="a3c46-129">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="a3c46-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="a3c46-130">تم تحسين التحقق من صحة لمعالجة استثناء مرجع فارغ تم إنشاؤه في المكون الإضافي لـ **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="a3c46-130">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>
- <span data-ttu-id="a3c46-131">تحذف المشروعات المنشورة بواسطة الوظيفة الإضافية لسطح مكتب Microsoft Project التعيينات غير المعينة.</span><span class="sxs-lookup"><span data-stu-id="a3c46-131">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>
- <span data-ttu-id="a3c46-132">تمت إضافة تحقق جديد عندما يكون مرجع مشروع المهمة غير صالح بسبب استثناء مرجع فارغ في المكون الإضافي لـ **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="a3c46-132">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>
- <span data-ttu-id="a3c46-133">لا تعرض شبكة أعضاء الفريق التعيينات المميزة في سجل عضو الفريق.</span><span class="sxs-lookup"><span data-stu-id="a3c46-133">Team Member grid does not show distinct assignments on the team member record.</span></span>
- <span data-ttu-id="a3c46-134">تمت إضافة رسائل تحقق وأخطاء جديدة بسبب استثناء مرجعي فارغ في المكون الإضافي لـ **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="a3c46-134">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="a3c46-135">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="a3c46-135">**Sales**</span></span>

<span data-ttu-id="a3c46-136">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="a3c46-136">The following issues have been fixed:</span></span>

- <span data-ttu-id="a3c46-137">عند اختيار بند قائم على المشروع في عرض أسعار أو عقد، فإن الزر **اقتراح** يجب أن يكون مرئيًا فقط عند تحديد خط مستند إلى منتج مرتبط بمنتج موجود.</span><span class="sxs-lookup"><span data-stu-id="a3c46-137">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>
- <span data-ttu-id="a3c46-138">قم بتقسم امتياز **Create_Product** من امتياز **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="a3c46-138">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>
- <span data-ttu-id="a3c46-139">يؤدي حذف بند فاتورة إلى فشل مرجع فارغ في **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="a3c46-139">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]