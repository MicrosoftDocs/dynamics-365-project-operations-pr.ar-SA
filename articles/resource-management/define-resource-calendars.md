---
title: تحديد تقاويم الموارد
description: يقدم هذا الموضوع معلومات حول كيفية تحديد تقويمات ساعات العمل للموارد في Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ab39d7e5dc2d8c01ed49ca0f1a4d1691aaf15637
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070492"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="25321-103">تحديد تقاويم الموارد</span><span class="sxs-lookup"><span data-stu-id="25321-103">Define resource calendars</span></span>

<span data-ttu-id="25321-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="25321-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="25321-105">يجب أن يتوفر لدى كل مورد قابل للحجز يعمل على مشروع تقويم ساعات عمل لتحديد توفره.</span><span class="sxs-lookup"><span data-stu-id="25321-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="25321-106">يمكن تحديد ساعات عمل المورد من خلال طريقتين:</span><span class="sxs-lookup"><span data-stu-id="25321-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="25321-107">تحديد قواعد التقويم الفردي لأحد الموارد</span><span class="sxs-lookup"><span data-stu-id="25321-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="25321-108">تطبيق قالب تقويم موجود للمورد</span><span class="sxs-lookup"><span data-stu-id="25321-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="25321-109">تحديد ساعات عمل مورد</span><span class="sxs-lookup"><span data-stu-id="25321-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="25321-110">من قائمة **الموارد** ، حدد **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="25321-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="25321-111">من طريقة عرض الشبكة، حدد **مورد قابل للحجز** .</span><span class="sxs-lookup"><span data-stu-id="25321-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="25321-112">من الصفحة **تفاصيل المورد** ، حدد علامة تبويب **ساعات العمل**. بشكل افتراضي، يتم تعيين تقويم الموارد القابل للحجز بشكل افتراضي إلى ساعات عمل قالب ساعات العمل الافتراضية المحدد للمؤسسة.</span><span class="sxs-lookup"><span data-stu-id="25321-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="25321-113">لتحديث ساعات العمل، انقر بزر الماوس الأيمن فوق تاريخ البدء لقاعدة التقويم المقترحة المطلوب تحديدها.</span><span class="sxs-lookup"><span data-stu-id="25321-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="25321-114">استخدم قائمة قاعدة التقويم لتحديد قاعدة تقويم ليوم محدد أو بقية السلسلة أو التقويم بكامله.</span><span class="sxs-lookup"><span data-stu-id="25321-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="25321-115">بعد تحديد الخيار، يمكنك بعد ذلك تعريف:</span><span class="sxs-lookup"><span data-stu-id="25321-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="25321-116">يوم الأسبوع الذي سيتم فيه تطبيق ساعات العمل.</span><span class="sxs-lookup"><span data-stu-id="25321-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="25321-117">أوقات العمل خلال كل يوم.</span><span class="sxs-lookup"><span data-stu-id="25321-117">The working times within each day.</span></span>
    - <span data-ttu-id="25321-118">المنطقة الزمنية لقاعدة التقويم.</span><span class="sxs-lookup"><span data-stu-id="25321-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="25321-119">يمكن أيضًا تحديد وقت غير وقت العمل للقاعدة، إذا أمكن.</span><span class="sxs-lookup"><span data-stu-id="25321-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="25321-120">تطبيق قالب تقويم على مورد</span><span class="sxs-lookup"><span data-stu-id="25321-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="25321-121">من قائمة **الموارد** ، حدد **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="25321-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="25321-122">من طريقة عرض الشبكة، حدد عددًا من **الموارد القابلة للحجز** يصل إلى 25 لتحديثها.</span><span class="sxs-lookup"><span data-stu-id="25321-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="25321-123">حدد **تعيين التقويم** ، وسيظهر مربع حوار مع قائمة من قوالب ساعات العمل المتاحة.</span><span class="sxs-lookup"><span data-stu-id="25321-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="25321-124">حدد القالب الذي تريد استخدامه، ثم حدد **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="25321-124">Select the template you want to use, and then select **Apply**.</span></span>
