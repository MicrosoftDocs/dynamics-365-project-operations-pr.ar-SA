---
title: إنشاء قالب ساعات عمل
description: يصف هذا الموضوع كيفية إنشاء قالب ساعات العمل في Project Service.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 105e3cb2ef7b904e96dc21013906e0b7444e3b88
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997180"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="43080-103">إنشاء قالب ساعات العمل (Project Service)</span><span class="sxs-lookup"><span data-stu-id="43080-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="43080-104">لإنشاء مشروع وإدارته، يجب تطبيق قالب تقويم على المشروع.</span><span class="sxs-lookup"><span data-stu-id="43080-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="43080-105">يحدد قالب التقويم سمات المشروع التالية:</span><span class="sxs-lookup"><span data-stu-id="43080-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="43080-106">ساعات العمل، بما في ذلك وقت البدء والانتهاء</span><span class="sxs-lookup"><span data-stu-id="43080-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="43080-107">أيام العمل</span><span class="sxs-lookup"><span data-stu-id="43080-107">Working days</span></span>
- <span data-ttu-id="43080-108">استثناءات التقويم مثل الأيام غير المخصصة للعمل</span><span class="sxs-lookup"><span data-stu-id="43080-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="43080-109">قالب التقويم المطبق على مشروع هو نسخة من قالب التقويم المعرف في إعدادات المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="43080-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="43080-110">إذا قمت بتغيير قالب التقويم، فلا يتم نشر هذه التغييرات إلى ساعات عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="43080-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="43080-111">لتغيير ساعات عمل المشروع، يجب تطبيق قالب جديد.</span><span class="sxs-lookup"><span data-stu-id="43080-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="43080-112">لإنشاء قالب تقويم لمنظمتك، يوجد متطلبين أساسيين:</span><span class="sxs-lookup"><span data-stu-id="43080-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="43080-113">حدد ساعات العمل المطلوبة في القالب باستخدام مورد جديد أو موجود قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="43080-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="43080-114">قم بإنشاء قالب تقويم جديد وإقران القالب بالمورد القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="43080-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="43080-115">**تحديد ساعات عمل القالب**</span><span class="sxs-lookup"><span data-stu-id="43080-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="43080-116">انتقل إلى **الموارد** \> **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="43080-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="43080-117">قم بإنشاء مورد جديد للمرجع في قالب التقويم، أو حدد موردًا موجودًا.</span><span class="sxs-lookup"><span data-stu-id="43080-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="43080-118">حدد علامة التبويب **ساعات العمل** للمورد واستكمل الإرشادات في [تعيين ساعات العمل للمورد](/dynamics365/field-service/set-work-hours-resource.md) لتكوين قواعد التقويم.</span><span class="sxs-lookup"><span data-stu-id="43080-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="43080-119">**إنشاء قالب تكوين جديد.**</span><span class="sxs-lookup"><span data-stu-id="43080-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="43080-120">انتقل إلى **الإعدادات** \> **قالب التقويم**.</span><span class="sxs-lookup"><span data-stu-id="43080-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="43080-121">حدد **جديد**، وأدخل اسمًا ووصفًا ومورد القالب.</span><span class="sxs-lookup"><span data-stu-id="43080-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="43080-122">عند الرجوع إلى مورد في قالب تقويم، يتم ربط نسخة من تقويم المورد مع قالب التقويم.</span><span class="sxs-lookup"><span data-stu-id="43080-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="43080-123">إذا تم تغيير ساعات العمل للقالب المنسوخ، فلا يتم نشر هذه التغييرات إلى قالب التقويم.</span><span class="sxs-lookup"><span data-stu-id="43080-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="43080-124">راجع أيضًا</span><span class="sxs-lookup"><span data-stu-id="43080-124">See Also</span></span>  
 [<span data-ttu-id="43080-125">إعداد الموارد</span><span class="sxs-lookup"><span data-stu-id="43080-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
