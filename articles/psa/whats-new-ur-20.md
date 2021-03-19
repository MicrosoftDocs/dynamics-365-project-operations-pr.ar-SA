---
title: الجديد أو المتغير في الإصدار 3 من Project Service Automation، إصدار التحديث 20
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 20.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: db416343ac9ac2591007e83be80493a48f9ae904
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280652"
---
# <a name="project-service-automation-update-release-20-v3"></a><span data-ttu-id="3d11c-103">الإصدار 3 من Project Service Automation، إصدار التحديث 20</span><span class="sxs-lookup"><span data-stu-id="3d11c-103">Project Service Automation Update Release 20, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="3d11c-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="3d11c-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="3d11c-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="3d11c-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="3d11c-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="3d11c-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="3d11c-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="3d11c-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="3d11c-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="3d11c-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="3d11c-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في الإصدار 3 من Project Service Automation، إصدار التحديث 20.</span><span class="sxs-lookup"><span data-stu-id="3d11c-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 20.</span></span> <span data-ttu-id="3d11c-110">لدى هذا الإصدار رقم البنية V 3.10.31.37 وهو متوفر بشكل عام من خلال تحديث ذاتي في شهر يونيو 2020.</span><span class="sxs-lookup"><span data-stu-id="3d11c-110">This version has a build number of V 3.10.31.37 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-20"></a><span data-ttu-id="3d11c-111">إصدار التحديث 20</span><span class="sxs-lookup"><span data-stu-id="3d11c-111">Update Release 20</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="3d11c-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="3d11c-112">Bug fixes</span></span>

<span data-ttu-id="3d11c-113">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="3d11c-113">**Project Management**</span></span>

<span data-ttu-id="3d11c-114">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="3d11c-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="3d11c-115">يؤدي استيراد أعضاء فريق المشروع الذين لديهم طريقة تخصيص تحتاج إلى ساعات ساعات إلى ظهور رسالة خطأ غير واضحة عندما تكون قيمة الساعات المحددة صفرية.</span><span class="sxs-lookup"><span data-stu-id="3d11c-115">Importing project team members with an allocation method that requires hours results in an unclear error message when the specified hours are zero.</span></span>
- <span data-ttu-id="3d11c-116">يتلقى المستخدمون رسالة خطأ غير صحيحة عند إدخال الحد الأقصى لعدد الأحرف في حقل **الوصف** لمهمة مشروع.</span><span class="sxs-lookup"><span data-stu-id="3d11c-116">Users receive an incorrect error when the maximum number of characters have been entered into the **Description** field for a project task.</span></span>
- <span data-ttu-id="3d11c-117">تقوم صفحة **تنزيل الوظيفة الإضافية Microsoft Dynamics 365 Project Service Automation** بإعادة التوجيه إلى صفحة التنزيل باللغة الإنجليزية عند تعيين إعدادات لغة المستخدم إلى اللغة اليابانية.</span><span class="sxs-lookup"><span data-stu-id="3d11c-117">The **Microsoft Dynamics 365 Project Service Automation add-in download** page redirects to the English download page when the user’s language settings are set to Japanese.</span></span>
- <span data-ttu-id="3d11c-118">عند حدوث خطأ في الخادم، تبقى في بعض الأحيان تسمية المزامنة على علامة تبويب **الجدول** في نموذج **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="3d11c-118">When a server error occurs, the synchronization label on the **Schedule** tab of the **Projects** form sometimes remains.</span></span>
- <span data-ttu-id="3d11c-119">يتم إرسال تحديثات المهمة المتكررة إلى الخادم عند تعديل مهمة.</span><span class="sxs-lookup"><span data-stu-id="3d11c-119">Redundant task updates are being sent to the server when a task is modified.</span></span>

<span data-ttu-id="3d11c-120">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="3d11c-120">**Sales**</span></span>

<span data-ttu-id="3d11c-121">تم إصلاح المشكلات التالية:</span><span class="sxs-lookup"><span data-stu-id="3d11c-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="3d11c-122">في نموذج **العقد**، يؤدي النقر المزدوج فوق **إنشاء فاتورة** إلى إنشاء فاتورتين لسجل القيمة الفعلية الفردية.</span><span class="sxs-lookup"><span data-stu-id="3d11c-122">On the **Contract** form, double-clicking **Create Invoice** creates two invoices for a single actuals record.</span></span>
- <span data-ttu-id="3d11c-123">في Internet Explorer 11، يتعذر على المستخدمين إنشاء إدخالات مصروفات.</span><span class="sxs-lookup"><span data-stu-id="3d11c-123">In Internet Explorer 11, users are unable to create expense entries.</span></span>
- <span data-ttu-id="3d11c-124">عكس التكلفة وعكس قيم المبيعات الفعلية غير المفوترة غير مرتبطين.</span><span class="sxs-lookup"><span data-stu-id="3d11c-124">Reversal of Cost and reversal of Unbilled Sales Actuals are not linked.</span></span>
- <span data-ttu-id="3d11c-125">لا يؤدي الضغط على الزر **تحديث القيم الفعلية** على نموذج **المشروع** إلى تحديث **الساعات الفعلية‬ للمهمة**.</span><span class="sxs-lookup"><span data-stu-id="3d11c-125">The **Refresh Actuals** button on the **Project** form does not refresh **Task Actual Hours**.</span></span>
- <span data-ttu-id="3d11c-126">بإمكان المكون الإضافي **PreValidateProjectTeamMemberCreate** إنشاء موارد عامة قابلة للحجز عند تعيين السمة **msdyn_isgenericresourceprojectscoped** إلى **خطأ**.</span><span class="sxs-lookup"><span data-stu-id="3d11c-126">The **PreValidateProjectTeamMemberCreate** plug-in can create duplicate generic bookable resources when the attribute **msdyn_isgenericresourceprojectscoped** is set to **False**.</span></span>
- <span data-ttu-id="3d11c-127">يقوم الخيار **إعادة الحساب** بمسح التكاليف الخاضعة للرسوم لتفاصيل بنود عرض أسعار يستند إلى منتج وتفاصيل شروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="3d11c-127">**Recalculate** clears chargeable costs of product-based quote line details and contract line details.</span></span>
- <span data-ttu-id="3d11c-128">في سيناريوهات معينة، يعرض المكون الإضافي **PostEstimateLineUpdate** خطأ استثناء مرجعيُا.</span><span class="sxs-lookup"><span data-stu-id="3d11c-128">In specific scenarios, the **PostEstimateLineUpdate** plug-in displays a null teference exception error.</span></span>
- <span data-ttu-id="3d11c-129">لا تتطابق مدة المرحلة الزمنية على **مخطط تحليل الربحية** مع مدة التكاليف في تفاصيل بنود عرض الأسعار الثابتة السعر في عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="3d11c-129">Time phase duration on the **Profitability Analysis Chart** does not match duration of the costs in the fixed-price quote line detail of the quote.</span></span>
- <span data-ttu-id="3d11c-130">لا يتم تحديد قيم الوحدة ومجموعات الوحدات بشكل افتراضي صحيح لفئات المصروفات في النموذجين **تفاصيل شروط التعاقد** و **تفاصيل بنود عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="3d11c-130">Unit and unit group values do not default correctly for expense categories on the **Contract Line Details** and **Quote Line Details** forms.</span></span>
- <span data-ttu-id="3d11c-131">تسمح قوائم **سعر تكلفة الوحدة التنظيمية** بحالات تداخل في سريان التاريخ.‬</span><span class="sxs-lookup"><span data-stu-id="3d11c-131">**Org Unit Cost Price** lists permit overlaps in the date effectivity.</span></span>
- <span data-ttu-id="3d11c-132">لا يُسمح للمستخدمين بتغيير **OrgUnit** عندما لا يكون نوع الأمر قائمًا على العمل لأنه سيؤدي إلى خطأ استثناء مرجعي فارغ.</span><span class="sxs-lookup"><span data-stu-id="3d11c-132">Users are not permitted to change the **OrgUnit** when the order type is not work-based because it will lead to a null reference exception error.</span></span>
- <span data-ttu-id="3d11c-133">عند محاولة الانتقال من نموذج **تفاصيل بنود عرض الأسعار**، والعودة إلى علامة تبويب **عرض الأسعار**، يتم تحديث النموذج ويعرض علامة تبويب **الملخص**.</span><span class="sxs-lookup"><span data-stu-id="3d11c-133">When attempting to navigate from the **Quote Line Details** form, back to the **Quote** tab, the form refreshes and displays the **Summary** tab.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]