---
title: ما الجديد أو المتغير في إصدار التحديث Project Service Automation 32، V3
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في إصدار التحديث 31 Project Service Automation، V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 11bf451ef4f24e2301ffde4f86a556a8a4fe30b0
ms.sourcegitcommit: 886102894244887d72e5a6213071e8d8a52c9d48
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/01/2021
ms.locfileid: "6129650"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a><span data-ttu-id="6920e-103">ما الجديد أو المتغير في إصدار التحديث Project Service Automation 32، V3</span><span class="sxs-lookup"><span data-stu-id="6920e-103">What's new or changed in Project Service Automation Update Release 32, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="6920e-104">يسرنا أن نعلن عن آخر تحديث للتطبيق Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="6920e-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="6920e-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="6920e-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="6920e-106">وهو متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="6920e-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="6920e-107">لتحديث هذا الإصدار، قم بزيارة صفحة حل Dynamics 365 online في مركز إدارة، ثم قم بتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="6920e-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="6920e-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="6920e-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="6920e-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في Project Service Automation V3، إصدار التحديث 32.</span><span class="sxs-lookup"><span data-stu-id="6920e-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 32.</span></span> <span data-ttu-id="6920e-110">يحتوي هذا الإصدار على رقم الإصدار V3.10.53.108، ويتوفر بشكل عام من خلال التحديث الذاتي في يونيو 2021.</span><span class="sxs-lookup"><span data-stu-id="6920e-110">This version has a build number of V3.10.53.108 and is generally available through a self-update in June 2021.</span></span>

## <a name="update-release-32"></a><span data-ttu-id="6920e-111">إصدار التحديث 32</span><span class="sxs-lookup"><span data-stu-id="6920e-111">Update Release 32</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="6920e-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="6920e-112">Bug fixes</span></span>

#### <a name="general"></a><span data-ttu-id="6920e-113">عام </span><span class="sxs-lookup"><span data-stu-id="6920e-113">General</span></span>

- <span data-ttu-id="6920e-114">في حالة فشل عملية تحديث رئيسية، فإنه يجب حظر نقاط إدخال التطبيق الرئيسية فقط، لضمان استمرار الوصول إلى الكيانات المشتركة.</span><span class="sxs-lookup"><span data-stu-id="6920e-114">When a major upgrade fails, only the main application entry points should be blocked, to ensure that shared entities are still accessible.</span></span>

#### <a name="time-and-expense"></a><span data-ttu-id="6920e-115">الوقت والمصروفات</span><span class="sxs-lookup"><span data-stu-id="6920e-115">Time and Expense</span></span>

<span data-ttu-id="6920e-116">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="6920e-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="6920e-117">لا يحافظ **TimeEntriesImportFromResourceAssignment** على وقت البدء ووقت الانتهاء لشريحة محيط تعيين المورد.</span><span class="sxs-lookup"><span data-stu-id="6920e-117">**TimeEntriesImportFromResourceAssignment** doesn't maintain the start and end times of the resource assignment contour slice.</span></span>
- <span data-ttu-id="6920e-118">عندما تقوم بتحديد **فتح الإدخال** في الشبكة **إدخال الوقت**، فقد يتم منعك من تحديد نماذج أخرى.</span><span class="sxs-lookup"><span data-stu-id="6920e-118">When you select **Open Entry** on the **Time Entry** grid, you might be prevented from selecting other forms.</span></span>
- <span data-ttu-id="6920e-119">أثناء استيراد تعيينات إلى إدخالات الوقت، قد يقوم استعلام رمز العميل بإنشاء عنوان URL طويل يتسبب في فشل الاستعلام.</span><span class="sxs-lookup"><span data-stu-id="6920e-119">While you import assignments to time entries, the client code query could generate a long URL that fails the query.</span></span>
- <span data-ttu-id="6920e-120">في شبكة **إدخال الوقت**، بعد حذف قيمة من خلية، لا يظل التركيز في الشبكة.</span><span class="sxs-lookup"><span data-stu-id="6920e-120">In the **Time Entry** grid, after a value is deleted from a cell, the focus doesn't remain in the grid.</span></span>
- <span data-ttu-id="6920e-121">تمت إزالة الزر **رفض** من طريقة عرض **الموافقات قيد المعالجة** للموافقات الحديثة.</span><span class="sxs-lookup"><span data-stu-id="6920e-121">The **Reject** button has been removed from the **Processing approvals** view for modern approvals.</span></span>
- <span data-ttu-id="6920e-122">يتأثر الاستقرار والأداء للموافقة المجمعة لإدخال الوقت بسبب إخفاقات الوصول وفشل التعامل على نحو ملائم مع التخصيصات المرتبطة بالكيان **إدخال الوقت**.</span><span class="sxs-lookup"><span data-stu-id="6920e-122">The stability and performance of time entry bulk approval are affected by deadlocks and a failure to appropriately handle customizations that are related to the **Time Entry** entity.</span></span>

#### <a name="project-planning"></a><span data-ttu-id="6920e-123">تخطيط المشروع</span><span class="sxs-lookup"><span data-stu-id="6920e-123">Project Planning</span></span>

- <span data-ttu-id="6920e-124">يتم إنشاء استثناء مرجع فارغ عند تحديث مشروع يحتوي على قيمة فارغة في الحقل **الوحدة المتعاقدة**.</span><span class="sxs-lookup"><span data-stu-id="6920e-124">A null reference exception is generated when you update a project that has a null value in the **Contracting Unit** field.</span></span>
- <span data-ttu-id="6920e-125">يقوم **تحديث إجماليات المشروع** بحساب التكلفة المتبقية والمبيعات المتبقية على مشروع بشكل غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="6920e-125">**Refresh Project Totals** incorrectly calculates the remaining cost and remaining sales on a project.</span></span>
- <span data-ttu-id="6920e-126">تؤثر حسابات التسعير التكرارية على الأداء المرتبط بتحديثات في محيطات تعيين الموارد.</span><span class="sxs-lookup"><span data-stu-id="6920e-126">Redundant pricing calculations affect performance that is related to updates on resource assignment contours.</span></span>

#### <a name="resource-management"></a><span data-ttu-id="6920e-127">إدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="6920e-127">Resource Management</span></span>

<span data-ttu-id="6920e-128">تم إصلاح المشاكل التالية:</span><span class="sxs-lookup"><span data-stu-id="6920e-128">The following issue has been fixed:</span></span>

- <span data-ttu-id="6920e-129">عندما تكون سعة التقويم الخاصة بالموارد القابلة للحجز أكثر من 1، يتعرف Project Service Automation بشكل غير صحيح على السعة على أنها 0 (صفر).</span><span class="sxs-lookup"><span data-stu-id="6920e-129">When a bookable resource's calendar capacity is more than 1, Project Service Automation incorrectly recognizes the capacity as 0 (zero).</span></span> <span data-ttu-id="6920e-130">ولذلك، يحدث تكرار لا نهائي في طريقة عرض الجدولة.</span><span class="sxs-lookup"><span data-stu-id="6920e-130">Therefore, an infinite loop occurs in the schedule view.</span></span>

#### <a name="sales"></a><span data-ttu-id="6920e-131">‏المبيعات</span><span class="sxs-lookup"><span data-stu-id="6920e-131">Sales</span></span>

<span data-ttu-id="6920e-132">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="6920e-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="6920e-133">عند إنشاء سطر دفتر يومية يحتوي على نوع معاملة مخصص، يحدث استثناء المرجع الفارغ التالي: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span><span class="sxs-lookup"><span data-stu-id="6920e-133">When a journal line is created that has a custom transaction type, the following null reference exception occurs: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span></span>
- <span data-ttu-id="6920e-134">يجب عدم إضافة الأدوار والفئات التي يتم تنشيطها قبل نسخ عرض الأسعار إلى الأدوار والفئات الخاضعة للرسوم من عروض الأسعار التي تم نسخها حديثًا.</span><span class="sxs-lookup"><span data-stu-id="6920e-134">Roles and categories that are inactivated before a quotation is copied should not be added to chargeable roles and categories of the newly copied quotation.</span></span>
- <span data-ttu-id="6920e-135">لا يتم محاذاة تاريخ المستند وتاريخ المحاسبة مع تاريخ البدء المقدم في تفاصيل بند الفاتورة التي يتم إنشاؤها مباشرة على فاتورة المسودة.</span><span class="sxs-lookup"><span data-stu-id="6920e-135">The document date and accounting date aren't aligned with the start date that is provided on an invoice line detail that is created directly on a draft invoice.</span></span>
- <span data-ttu-id="6920e-136">يتم إنشاء الاستثناءات المرجعية الفارغة في السيناريوهات المرتبطة بتعطيل الأدوار والفئات قبل نسخ عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="6920e-136">Null reference exceptions are generated in scenarios that are related to inactivation of roles and categories before a quotation is copied.</span></span>
- <span data-ttu-id="6920e-137">لا يقم إجراء **تحديث الأسعار** في الصفحة **مشروعات** بتحديث تقديرات المصروفات وتقديرات المواد.</span><span class="sxs-lookup"><span data-stu-id="6920e-137">The **Update Prices** action on the **Projects** page doesn't update expense estimates and material estimates.</span></span>
