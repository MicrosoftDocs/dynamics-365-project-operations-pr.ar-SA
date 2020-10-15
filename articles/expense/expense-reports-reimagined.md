---
title: إعادة صياغة تقارير المصروفات
description: يقدم هذا الموضوع معلومات حول التجربة المعاد تصميمها وصياغتها لإدخال تقرير المصروفات.
author: suvaidya
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: cd0d415b9cc85bac91de8fb9427da290ae0c6108
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897120"
---
# <a name="expense-reports-reimagined"></a><span data-ttu-id="7d93e-103">إعادة صياغة تقارير المصروفات</span><span class="sxs-lookup"><span data-stu-id="7d93e-103">Expense reports reimagined</span></span>

<span data-ttu-id="7d93e-104">أعيد تصميم إدخال تقرير المصروفات لتبسيط العملية وتقليل الوقت اللازم لإكمال التقرير.</span><span class="sxs-lookup"><span data-stu-id="7d93e-104">Expense report entry has been redesigned to simplify the process and reduce the time needed to complete a report.</span></span> <span data-ttu-id="7d93e-105">إليك المكونات الرئيسية لتجربة المصروفات الجديدة:</span><span class="sxs-lookup"><span data-stu-id="7d93e-105">Here are the major components of the new expense experience:</span></span>

- <span data-ttu-id="7d93e-106">مساحة عمل جديدة لإدارة المصروفات تتيح لك الوصول إلى مصروفات المفوض.</span><span class="sxs-lookup"><span data-stu-id="7d93e-106">A new expense management workspace that lets you access your delegate's expenses.</span></span>
- <span data-ttu-id="7d93e-107">تجربة جديدة لمطابقة الإيصالات لإظهار إيصالات على مستوى الرأس بشكل أفضل وتبسيط عمليه إرفاق الإيصالات ببنود المصروفات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-107">A new receipt matching experience to better show header-level receipts and simplify the process of attaching receipts to expense lines.</span></span>
- <span data-ttu-id="7d93e-108">شبكة جديدة للقراءة فقط تسمح لك بعرض العديد من بنود المصروفات وأعمدة بيانات إضافية.</span><span class="sxs-lookup"><span data-stu-id="7d93e-108">A new read-only grid that lets you view many more expense lines and additional columns of data.</span></span> <span data-ttu-id="7d93e-109">يمكنك الآن رؤية جميع البنود المفصلة والمقسمة مع مصروفاتها الأصلية.</span><span class="sxs-lookup"><span data-stu-id="7d93e-109">You can now see all itemized and split lines, together with their parent expenses.</span></span>
- <span data-ttu-id="7d93e-110">جزء مبسط لتحرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-110">A simplified pane for editing expenses.</span></span>
- <span data-ttu-id="7d93e-111">رسائل خطأ وتحذيرات وسياسات معاد تصميمها لتوفير السياق والفهم الصحيحين للمشكلة وكيفية حلها.</span><span class="sxs-lookup"><span data-stu-id="7d93e-111">Redesigned error, warning, and policy messages to provide the correct context and understanding of the issue and how to resolve it.</span></span> <span data-ttu-id="7d93e-112">لقد أزلنا الكثير من الرسائل التي ظهرت قبل أن يتمكن المستخدمون من إكمال مهامهم ومعالجة المشكلات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-112">We have removed several of the messages that appeared before users could complete their tasks and address the issues.</span></span>
- <span data-ttu-id="7d93e-113">صفحة جديدة لتحديد الحقول المطلوبة والحقول الاختيارية والحقول التي لا يجب تضمينها.</span><span class="sxs-lookup"><span data-stu-id="7d93e-113">A new page to specify required fields, optional fields, and the fields that should not be included.</span></span> <span data-ttu-id="7d93e-114">تساعد هذه الصفحة على تقليل عدد الحقول التي يجب تعيينها.</span><span class="sxs-lookup"><span data-stu-id="7d93e-114">This page helps to reduce the number of fields that must be set.</span></span>
- <span data-ttu-id="7d93e-115">شكل وأسلوب عرض جديدان لتقارير المصروفات، بحيث لا تبدو المصروفات وكأنها مصممة لشخصيات الحسابات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-115">A new look and feel for expense reports, so that the reports no longer seem as though they were designed for accounting personas.</span></span>

<span data-ttu-id="7d93e-116">لتشغيل التجربة الجديدة، استخدم مساحة عمل **إدارة الميزات** لتشغيل ميزة **إعادة صياغة تقارير المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="7d93e-116">To turn on the new experience, use the **Feature management** workspace to turn on the **Expense reports reimagined** feature.</span></span> <span data-ttu-id="7d93e-117">عند تشغيل هذه الميزة، تحدث الإجراءات التالية:</span><span class="sxs-lookup"><span data-stu-id="7d93e-117">When you turn on this feature, the following actions occur:</span></span>

- <span data-ttu-id="7d93e-118">يتم استبدال مساحة عمل المصروفات الموجودة بمساحة العمل الجديدة.</span><span class="sxs-lookup"><span data-stu-id="7d93e-118">The existing expense workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="7d93e-119">تتم إضافة عنصر قائمة جديد لرؤية حقل المصروفات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-119">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="7d93e-120">لا تتم إزالة عناصر القائمة الموجودة لتقارير المصروفات (الصفحة الحالية) أو حقول تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-120">No existing menu items for expense reports (the existing page) or expense report fields are removed.</span></span>
- <span data-ttu-id="7d93e-121">وتستمر عمليات سير العمل وأي موافقات في الانتقال إلى صفحه تقارير المصروفات الموجودة.</span><span class="sxs-lookup"><span data-stu-id="7d93e-121">Workflows and any approvals still take you to the existing expense reports page.</span></span>

## <a name="getting-started-video-for-new-users"></a><span data-ttu-id="7d93e-122">مقاطع فيديو الشروع في العمل للمستخدمين الجدد</span><span class="sxs-lookup"><span data-stu-id="7d93e-122">Getting started video for new users</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2Y7gO]

<span data-ttu-id="7d93e-123">تم تضمين فيديو [تجربة المصروفات في Dynamics 365 for Finance and Operations](https://youtu.be/Ocy-MsTvEE0) (يظهر أعلاه) في [Finance and Operations قائمة التشغيل](https://www.youtube.com/playlist?list=PLcakwueIHoT_SYfIaPGoOhloFoCXiUSyW) المتوفرة على YouTube.</span><span class="sxs-lookup"><span data-stu-id="7d93e-123">The [Expense experience in Dynamics 365 for Finance and Operations](https://youtu.be/Ocy-MsTvEE0) video (shown above) is included in the [Finance and Operations playlist](https://www.youtube.com/playlist?list=PLcakwueIHoT_SYfIaPGoOhloFoCXiUSyW) available on YouTube.</span></span>

## <a name="new-features"></a><span data-ttu-id="7d93e-124">الميزات الجديدة</span><span class="sxs-lookup"><span data-stu-id="7d93e-124">New features</span></span>

| <span data-ttu-id="7d93e-125">الميزة الجديدة</span><span class="sxs-lookup"><span data-stu-id="7d93e-125">New feature</span></span> | <span data-ttu-id="7d93e-126">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="7d93e-126">Description</span></span> |
|---|----|
| <span data-ttu-id="7d93e-127">رؤية حقل المصروفات</span><span class="sxs-lookup"><span data-stu-id="7d93e-127">Expense field visibility</span></span> | <span data-ttu-id="7d93e-128">تسمح لك صفحة إعداد جديدة بتحديد الحقول التي يجب تعطيلها لمؤسسة، والحقول التي يجب أن تكون مطلوبة، والحقول الموصى بها.</span><span class="sxs-lookup"><span data-stu-id="7d93e-128">A new setup page lets you specify which fields should be disabled for an organization, which fields should be required, and which fields are recommended.</span></span> |
| <span data-ttu-id="7d93e-129">الحقول المطلوبة</span><span class="sxs-lookup"><span data-stu-id="7d93e-129">Required fields</span></span> | <span data-ttu-id="7d93e-130">يتيح لك التكوين البسيط الجديد جعل بعض الحقول مطلوبة من دون الحاجة إلى استخدام إطار عمل السياسة.</span><span class="sxs-lookup"><span data-stu-id="7d93e-130">New simple configuration lets you make some fields required without having to use the policy framework.</span></span> |
| <span data-ttu-id="7d93e-131">الحقول الاختيارية</span><span class="sxs-lookup"><span data-stu-id="7d93e-131">Optional fields</span></span> | <span data-ttu-id="7d93e-132">تمت إضافة صحفة ثانية للحقول الاختيارية.</span><span class="sxs-lookup"><span data-stu-id="7d93e-132">A second page for optional fields is added.</span></span> <span data-ttu-id="7d93e-133">بهذه الطريقة، لن يشعر الموظفون بأنه عليهم تعيين الحقول، ولكن يبقى الوصول إلى الحقول سهلاً.</span><span class="sxs-lookup"><span data-stu-id="7d93e-133">In this way, employees won't feel as if they must set the fields, but the fields are still easily accessible.</span></span> |
| <span data-ttu-id="7d93e-134">إضافة إيصالات غير مرفقة</span><span class="sxs-lookup"><span data-stu-id="7d93e-134">Add unattached receipts</span></span> | <span data-ttu-id="7d93e-135">تظهر القدرة على إضافة إيصالات غير مرفقة إلى تقرير المصروفات بشكل افضل على مساحة العمل وعلى تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-135">The ability to add unattached receipts to expense report is more visible from the workspace and on the expense report.</span></span> |
| <span data-ttu-id="7d93e-136">مراسلة محسنة</span><span class="sxs-lookup"><span data-stu-id="7d93e-136">Improved messaging</span></span> | <span data-ttu-id="7d93e-137">هناك رؤية أفضل في بنود المصروفات التي بها تحذيرات أو أخطاء.</span><span class="sxs-lookup"><span data-stu-id="7d93e-137">There is better visibility into expense lines that have warnings or errors.</span></span> |
| <span data-ttu-id="7d93e-138">تخفيض عدد الرسائل في شريط الرسائل</span><span class="sxs-lookup"><span data-stu-id="7d93e-138">Reduction in messages in the message bar</span></span>| <span data-ttu-id="7d93e-139">تم تقليل عدد رسائل سجل المعلومات، وتم بذل جهود لمنع ظهور الرسائل المكررة في العديد من الحالات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-139">The number of Infolog messages was decreased, and an effort was made to prevent duplicate messages from appearing in many cases.</span></span> |
| <span data-ttu-id="7d93e-140">تجميع الإجراءات الشائعة معًا</span><span class="sxs-lookup"><span data-stu-id="7d93e-140">Grouped together common actions</span></span> | <span data-ttu-id="7d93e-141">تم تنظيف الواجهة بإضافة زر إجراءات جديد لمعظم الإجراءات على مستوى البنود وإضافة زر علامة القطع (...) للرأس وإجراءات أخرى أقل تكرارًا.</span><span class="sxs-lookup"><span data-stu-id="7d93e-141">The interface was cleaned up with the addition of a new actions button for most of the common line-level actions and the addition of an ellipsis button (...) for header and other less frequent actions.</span></span> |
| <span data-ttu-id="7d93e-142">مساحة عمل جديدة لزيادة الرؤية</span><span class="sxs-lookup"><span data-stu-id="7d93e-142">New workspace to increase visibility</span></span> | <span data-ttu-id="7d93e-143">توحد مساحة العمل الجديدة الميزات والارتباطات التي تتيح للمستخدمين الانتقال إلى مناطق مختلفة.</span><span class="sxs-lookup"><span data-stu-id="7d93e-143">A new workspace unifies features and links that let users move to different areas.</span></span> |
| <span data-ttu-id="7d93e-144">إضافة مصروفات وإيصالات موجودة أثناء إنشاء المصروفات</span><span class="sxs-lookup"><span data-stu-id="7d93e-144">Add existing expenses and receipts during expense creation</span></span> | <span data-ttu-id="7d93e-145">عند إنشاء تقارير المصروفات، يمكنك إضافة كافة المصروفات والإيصالات أو المحددة منها.</span><span class="sxs-lookup"><span data-stu-id="7d93e-145">When you create expense reports, you can add all or selected expenses and receipts.</span></span> |
| <span data-ttu-id="7d93e-146">حاسبة سعر الصرف</span><span class="sxs-lookup"><span data-stu-id="7d93e-146">Exchange rate calculator</span></span> | <span data-ttu-id="7d93e-147">تمت إضافة حاسبة سعر الصرف التي تسمح لك بحساب سعر الصرف للحركات الضرورية متعددة العملات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-147">An exchange rate calculator is added that lets you calculate the exchange rate for out-of-pocket multicurrency transactions.</span></span> |
| <span data-ttu-id="7d93e-148">حفظ وإضافة بنود مصروفات جديدة</span><span class="sxs-lookup"><span data-stu-id="7d93e-148">Save and add new expense lines</span></span> | <span data-ttu-id="7d93e-149">يتوفر الزران **حفظ** و**جديد** عند إدخال مصروفات جديدة، لمساعدتك على إدخال بنود المصروفات بسرعة.</span><span class="sxs-lookup"><span data-stu-id="7d93e-149">**Save** and **New** buttons are available when new expenses are entered, to help you quickly enter expense lines.</span></span> |
| <span data-ttu-id="7d93e-150">رؤية أفضل للبنود المقسمة والمفصلة</span><span class="sxs-lookup"><span data-stu-id="7d93e-150">Better visibility into split and itemized lines</span></span> | <span data-ttu-id="7d93e-151">تُضاف البنود المفصلة والمقسمة مباشرةً إلى قائمة المصروفات لزيادة الرؤية ومساعدتك على تحديد وجود الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="7d93e-151">Itemized and split lines are added directly to the list of expenses to increase visibility and help you easily determine whether there are any errors.</span></span> |
| <span data-ttu-id="7d93e-152">إظهار الإيصالات اثناء تفصيل البنود</span><span class="sxs-lookup"><span data-stu-id="7d93e-152">Show receipts during itemization</span></span> | <span data-ttu-id="7d93e-153">يمكن إظهار الإيصالات اثناء تفصيل البنود.</span><span class="sxs-lookup"><span data-stu-id="7d93e-153">Receipts can be shown during itemization.</span></span> |

<span data-ttu-id="7d93e-154">يركز الإصدار الأولي على سيناريوهات إدخال المصروفات.</span><span class="sxs-lookup"><span data-stu-id="7d93e-154">The initial release is focused on expense entry scenarios.</span></span> <span data-ttu-id="7d93e-155">سيستمر أي سيناريو لمراجعة تقرير المصروفات أو الموافقة عليه في استخدام صفحة إدخال المصروفات الموجودة.</span><span class="sxs-lookup"><span data-stu-id="7d93e-155">Any expense report review or approval scenario will continue to use the existing expense entry page.</span></span>

<span data-ttu-id="7d93e-156">الميزات التالية موجودة على الصفحة الحالية ولكنها غير موجودة بعد على الصفحة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="7d93e-156">The following features are present on the existing page but aren't yet present on the new page.</span></span> <span data-ttu-id="7d93e-157">سيُعاد تقديم هذه الميزات خلال الإصدارات العديدة التالية:</span><span class="sxs-lookup"><span data-stu-id="7d93e-157">These features will be reintroduced over the next several releases:</span></span>

- <span data-ttu-id="7d93e-158">الموافقات</span><span class="sxs-lookup"><span data-stu-id="7d93e-158">Approvals</span></span>
- <span data-ttu-id="7d93e-159">الموافقات على حسابات المدفوعات والقدرة على تحرير المحاسبة</span><span class="sxs-lookup"><span data-stu-id="7d93e-159">Accounts payable approvals and the ability to edit the accounting</span></span>
- <span data-ttu-id="7d93e-160">نقاط إدخال متعددة</span><span class="sxs-lookup"><span data-stu-id="7d93e-160">Multiple entry points</span></span>
- <span data-ttu-id="7d93e-161">تكامل طلب السفر</span><span class="sxs-lookup"><span data-stu-id="7d93e-161">Travel requisition integration</span></span>
- <span data-ttu-id="7d93e-162">كيان البيانات لرؤية حقل المصروفات</span><span class="sxs-lookup"><span data-stu-id="7d93e-162">Data entity for expense field visibility</span></span>
- <span data-ttu-id="7d93e-163">إدخال المصروفات باستخدام المصروف اليومي‬</span><span class="sxs-lookup"><span data-stu-id="7d93e-163">Entry for per-diem expenses</span></span>
- <span data-ttu-id="7d93e-164">سير عمل على مستوى البنود</span><span class="sxs-lookup"><span data-stu-id="7d93e-164">Line-level workflow</span></span>
- <span data-ttu-id="7d93e-165">دعم الموافق المؤقت</span><span class="sxs-lookup"><span data-stu-id="7d93e-165">Interim approver support</span></span>
- <span data-ttu-id="7d93e-166">التفصيل المتقدم</span><span class="sxs-lookup"><span data-stu-id="7d93e-166">Advanced itemization</span></span>
