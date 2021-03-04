---
title: الجديد أو المتغير في إصدار التحديث 21، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 21.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: b1194c1cf1997b68030fe88360c6ebb756c715fd
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147007"
---
# <a name="project-service-automation-update-release-21-v3"></a><span data-ttu-id="d3ba2-103">الإصدار 3 من Project Service Automation، إصدار التحديث 21</span><span class="sxs-lookup"><span data-stu-id="d3ba2-103">Project Service Automation Update Release 21, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="d3ba2-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="d3ba2-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="d3ba2-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="d3ba2-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="d3ba2-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="d3ba2-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="d3ba2-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 21.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 21.</span></span> <span data-ttu-id="d3ba2-110">لدى هذا الإصدار رقم البنية V 3.10.32.50 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر يونيو 2020.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-110">This version has a build number of V 3.10.32.50 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-21"></a><span data-ttu-id="d3ba2-111">إصدار التحديث 21</span><span class="sxs-lookup"><span data-stu-id="d3ba2-111">Update Release 21</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="d3ba2-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="d3ba2-112">Bug fixes</span></span>

<span data-ttu-id="d3ba2-113">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="d3ba2-113">**Time and Expense**</span></span>

<span data-ttu-id="d3ba2-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="d3ba2-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="d3ba2-115">وعند استضافة **عنصر تحكم شبكة إدخال الوقت** في لوحات المعلومات، فإن الشبكة لا تستخدم العرض الكامل لحاوية شبكة لوحة المعلومات.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-115">When hosting the **Time Entry Grid Control** in Dashboards, the grid does not utilize the full width of the dashboard grid container.</span></span>
- <span data-ttu-id="d3ba2-116">بالنسبة لمناطق زمنية محددة، لا يعرض عنصر تحكم شبكة **إدخال الوقت** السجلات.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-116">For specific time zones, the **Time Entry** grid control does not display records.</span></span>
- <span data-ttu-id="d3ba2-117">تظهر إدخالات الوقت بعد 9:00 مساءً في يوم غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-117">Time entries that are after 9:00 PM appear on the wrong day.</span></span>
- <span data-ttu-id="d3ba2-118">يتعذر على المستخدمين إرسال المصروفات إذا كانت فئة المصروفات، **إيصال استلام المصروفات**، لا تشتمل على قيمة.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-118">Users are unable to submit expenses if the expense category, **Expense receipt required** has no value.</span></span>

<span data-ttu-id="d3ba2-119">**إدارة الموارد**</span><span class="sxs-lookup"><span data-stu-id="d3ba2-119">**Resource Management**</span></span>

<span data-ttu-id="d3ba2-120">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="d3ba2-120">The following issues have been fixed:</span></span>

- <span data-ttu-id="d3ba2-121">يتم عرض عمليات الحجز غير النشطة في طريقة عرض **التسوية**.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-121">Inactive bookings are displayed in the **Reconciliation** view.</span></span>
- <span data-ttu-id="d3ba2-122">يفتقد تنفيذ المورد العام إلى التحقق من الصحة لضمان وجود حالة حجز صالحة.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-122">Generic resource fulfillment was missing validation to ensure that a valid booking status exists.</span></span>

<span data-ttu-id="d3ba2-123">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="d3ba2-123">**Project Management**</span></span>

<span data-ttu-id="d3ba2-124">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="d3ba2-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="d3ba2-125">تظل شبكات نموذج **المشروع** (طريقة عرض **تعيين الموارد**، **المهمة**، **التسوية**، **تقديرات المصروفات**) قابلة للتحرير حتى عندما يكون المشروع غير نشط.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-125">The **Project** form grids (**Resource Assignment**, **Task**, **Reconciliation** view, **Expense Estimates**) remain editable even when a project is not active.</span></span>
- <span data-ttu-id="d3ba2-126">لا يمكن دمج العملاء المكررين مع العملاء المرتبطين بعقود المشاريع المؤكدة.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-126">Duplicate customers can't be merged with customers that are linked to confirmed project contracts.</span></span>
- <span data-ttu-id="d3ba2-127">عند إضافة مورد لا يشتمل على تقويم صالح، لا يقوم النظام بإرجاع رسالة خطأ سهلة الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-127">When a resource who does not have a valid calendar is added, the system does not return a user friendly-error message.</span></span>
- <span data-ttu-id="d3ba2-128">يتم تمكين الزر **إضافة مهمة** على شبكه المهمة عندما يكون المشروع مرتبطًا بـ **الوظيفة الإضافية لـ Microsoft project**.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-128">The **Add Task** button on the task grid is enabled when the project is linked to **Microsoft Project add-in**.</span></span>
- <span data-ttu-id="d3ba2-129">يتزايد الجهد بشكل لا يمكن التحكم فيه عند تعيين مهمة بفئة إلى مورد ذي دور تم تحديد سعر تكلفة له.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-129">Effort grows uncontrollably when a task with a category is assigned to a resource with a role for which there is a cost price defined.</span></span>

<span data-ttu-id="d3ba2-130">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="d3ba2-130">**Sales**</span></span>

<span data-ttu-id="d3ba2-131">تم إجراء التحسينات التالية:</span><span class="sxs-lookup"><span data-stu-id="d3ba2-131">The following enhancements have been made:</span></span>

- <span data-ttu-id="d3ba2-132">تم نقل **تكرار الفاتورة** و **بدء الفوترة** إلى علامة التبويب **جدولة الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-132">**Invoice Frequency** and **Billing Start** have been moved to the **Invoice Schedule** tab.</span></span>

<span data-ttu-id="d3ba2-133">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="d3ba2-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="d3ba2-134">**السعر الإجمالي للمبيعات** هو صفر (0) لـ **الفئة** على الرغم من أن **الدور** يحتوي على إجمالي سعر مبيعات ليس صفرًا.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-134">**Total Sales Price** is zero (0) for **Category** even though **Role** has a total sales price that is not zero.</span></span>
- <span data-ttu-id="d3ba2-135">لا يستطيع العملاء تغيير قيمة حقل **حالة الفاتورة** إلى **جاهز للفوترة** عند قيام عملية مخصصة أخرى بتحديث حقل إضافي.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-135">Customers can't change the value of the **Invoice Status** field to **Ready for invoicing** when another customized process is updating an additional field.</span></span>
- <span data-ttu-id="d3ba2-136">يمكن للزر **تحديث بنود الفاتورة** إنشاء عدة بنود مكررة إذا كانت محددة بشكل متكرر.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-136">The **Refresh Invoice Lines** button can create multiple duplicated lines if it is repeatedly selected.</span></span>
- <span data-ttu-id="d3ba2-137">لا يعمل زر **تحديث الأسعار** على الشبكة الفرعية **أسعار الأدوار** في نموذج **العرض السريع**.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-137">The **Update Prices** button doesn't work on the **Role Prices** subgrid in the **Quick View** form.</span></span>
- <span data-ttu-id="d3ba2-138">إن منطق **حل قائمة أسعار المبيعات** يعالج المناطق الزمنية بشكل غير صحيح، مما يؤدي إلى التحديد غير الصحيح لقوائم الأسعار.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-138">The **Sales Price List Resolution** logic improperly handles time zones, resulting in the incorrect selection of price lists.</span></span>
- <span data-ttu-id="d3ba2-139">يمكن إيقاف **التكلفة الفعلية الإجمالية للمشروع** بمبلغ كسري بعد اعتماد إدخال وقت واحد.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-139">A project’s **Total Actual Cost** can be off by a fractional amount after a single time entry is approved.</span></span>
- <span data-ttu-id="d3ba2-140">لا يوفر منطق **حل الأسعار** رسالة خطأ مألوفة للمستخدم إذا كان **سعر الدور المسترد** لا يشتمل على قيم في حقلي **"الوحدة الرئيسية"** و **"السعر في الوحدة الرئيسية"**.</span><span class="sxs-lookup"><span data-stu-id="d3ba2-140">The **Price Resolution** logic does not provide a user-friendly error message if **Retrieved RolePrice** doesn't have values in **'Primary Unit'** and **'Price In Primary Unit'** fields.</span></span>
