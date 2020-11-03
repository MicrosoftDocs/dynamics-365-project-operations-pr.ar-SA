---
title: الجديد أو المتغير في إصدار التحديث 24، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 24.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 6c8348e65307f63a251f97bf1ea17578e7026da8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070596"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="89b5c-103">الإصدار 3 من Project Service Automation، إصدار التحديث 24</span><span class="sxs-lookup"><span data-stu-id="89b5c-103">Project Service Automation Update Release 24, V3</span></span>

<span data-ttu-id="89b5c-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="89b5c-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="89b5c-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="89b5c-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="89b5c-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="89b5c-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="89b5c-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="89b5c-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="89b5c-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="89b5c-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="89b5c-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 24.</span><span class="sxs-lookup"><span data-stu-id="89b5c-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="89b5c-110">يتضمن هذا الإصدار رقم البنية V 3.10.42.43 وهو متوفر بشكل عام من خلال تحديث ذاتي في أكتوبر 2020.</span><span class="sxs-lookup"><span data-stu-id="89b5c-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="89b5c-111">إصدار التحديث 24</span><span class="sxs-lookup"><span data-stu-id="89b5c-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="89b5c-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="89b5c-112">Bug fixes</span></span>

<span data-ttu-id="89b5c-113">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="89b5c-113">**Sales**</span></span>

<span data-ttu-id="89b5c-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="89b5c-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="89b5c-115">تحدث مشكلة أثناء إعداد قائمة الأسعار الافتراضية للمنتجات.</span><span class="sxs-lookup"><span data-stu-id="89b5c-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="89b5c-116">أداء الفوز بعرض الأسعار بطيء بسبب قائمة الأسعار المضمنة ونسخة سجلات أسعار الدور.</span><span class="sxs-lookup"><span data-stu-id="89b5c-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="89b5c-117">يتم تقريب **عقد المشروع/مركز المبيعات** > **بند سطر المنتج/كمية بند الأمر** إلى أقرب عدد صحيح بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="89b5c-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="89b5c-118">رفع امتيازات النظام عند قراءة قوائم الأسعار.</span><span class="sxs-lookup"><span data-stu-id="89b5c-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="89b5c-119">نسخ حقول عنوان العميل **address1_freighttermscode** و **address1_shippingmethodcode** إلى عرض الأسعار/الأمر.</span><span class="sxs-lookup"><span data-stu-id="89b5c-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="89b5c-120">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="89b5c-120">**Time and Expense**</span></span>

<span data-ttu-id="89b5c-121">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="89b5c-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="89b5c-122">لا تدعم شبكة **إدخال الوقت** سلوك الوقت **التاريخ فقط**.</span><span class="sxs-lookup"><span data-stu-id="89b5c-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="89b5c-123">لا يتم تحديث **إدخال الوقت** بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="89b5c-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="89b5c-124">يلزم إجراء تحديث يدوي.</span><span class="sxs-lookup"><span data-stu-id="89b5c-124">A manual refresh is required.</span></span>
- <span data-ttu-id="89b5c-125">يتعذر استيراد إدخالات الوقت من تعيين عند وجود فاصل (0 ساعات) في تعيينات المورد.</span><span class="sxs-lookup"><span data-stu-id="89b5c-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="89b5c-126">عند إنشاء إدخال الوقت، عيّن وقت البدء بحيث يكون **msdyn_date** نفسه.</span><span class="sxs-lookup"><span data-stu-id="89b5c-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="89b5c-127">إعادة تمكين التحرير المجمع لإدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="89b5c-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="89b5c-128">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="89b5c-128">**Resource Management**</span></span>

<span data-ttu-id="89b5c-129">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="89b5c-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="89b5c-130">ستؤدي محاولة تحديث حالة حجز خلال اليوم من دون طلب إلى طرح استثناء مرجع خالٍ.</span><span class="sxs-lookup"><span data-stu-id="89b5c-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="89b5c-131">خطأ في تحميل **طريقة عرض التسوية**.</span><span class="sxs-lookup"><span data-stu-id="89b5c-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="89b5c-132">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="89b5c-132">**Project Management**</span></span>

<span data-ttu-id="89b5c-133">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="89b5c-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="89b5c-134">في **جدول المشروع** ، عند التغيير من **يدوي** إلى **تلقائي** ، لا يكتمل الحفظ التلقائي.</span><span class="sxs-lookup"><span data-stu-id="89b5c-134">In the **Project Schedule** , when changing from **Manual** to **Auto** , auto save is not completing.</span></span>
- <span data-ttu-id="89b5c-135">يجب ألا يتم حساب تكاليف المصروفات نحو التباين في **شبكة تعقب المشروع**.</span><span class="sxs-lookup"><span data-stu-id="89b5c-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="89b5c-136">سلوك غير متناسق لأعمدة **علامة التقديرات** أثناء التحميل في مقابل تغيير نوع **التوزيع على الوقت**.</span><span class="sxs-lookup"><span data-stu-id="89b5c-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="89b5c-137">قد لا تعكس التكلفة الفعلية في المشروع الإجماليات من **القيم الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="89b5c-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="89b5c-138">لا يتطابق **تاريخ الانتهاء المقدر** على علامة تبويب **الملخص** مع **جدول WBS**.</span><span class="sxs-lookup"><span data-stu-id="89b5c-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="89b5c-139">لا يعمل **تحديث الساعات الفعلية** بالمستوى الأعلى بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="89b5c-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="89b5c-140">لا يستطيع مدير المشروع خارج **BU** الجذر إنشاء مشروع.</span><span class="sxs-lookup"><span data-stu-id="89b5c-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="89b5c-141">لا تدوم التغييرات التي يتم إدخالها على المهمة أو الفئة في **تقديرات المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="89b5c-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="89b5c-142">يؤدي اختيار **نسخ العقد** إلى نسخ جداول الفواتير وحالة التشغيل.</span><span class="sxs-lookup"><span data-stu-id="89b5c-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="89b5c-143">يحسب الزر **تحديث القيم الفعلية** المهام الموجزة بشكل غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="89b5c-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="89b5c-144">الوظيفة الإضافية Microsoft Project: إصلاح خطأ مرجعي خالٍ عند وجود وحدة تعيين موارد فارغة لدي أي من أعضاء الفريق.</span><span class="sxs-lookup"><span data-stu-id="89b5c-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>

