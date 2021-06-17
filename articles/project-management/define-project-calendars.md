---
title: تحديد تقاويم المشاريع
description: يوفر هذا الموضوع معلومات حول كيفية تطبيق قالب تقويم على مشروع لتعقب جدول المشروع.
author: ruhercul
ms.date: 02/05/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 0d1a2c4bd2d4022bbf79afcef79170eb482e6418
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998980"
---
# <a name="define-project-calendars"></a><span data-ttu-id="e3389-103">تحديد تقاويم المشاريع</span><span class="sxs-lookup"><span data-stu-id="e3389-103">Define project calendars</span></span>

<span data-ttu-id="e3389-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="e3389-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e3389-105">لإنشاء مشروع وإدارته، يجب تطبيق قالب تقويم على المشروع.</span><span class="sxs-lookup"><span data-stu-id="e3389-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="e3389-106">يحدد قالب التقويم سمات المشروع التالية:</span><span class="sxs-lookup"><span data-stu-id="e3389-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="e3389-107">ساعات العمل، بما في ذلك وقت البدء والانتهاء</span><span class="sxs-lookup"><span data-stu-id="e3389-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="e3389-108">أيام العمل</span><span class="sxs-lookup"><span data-stu-id="e3389-108">Working days</span></span>
- <span data-ttu-id="e3389-109">استثناءات التقويم مثل الأيام غير المخصصة للعمل</span><span class="sxs-lookup"><span data-stu-id="e3389-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="e3389-110">قالب التقويم المطبق على مشروع هو نسخة من قالب التقويم المعرف في إعدادات المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="e3389-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="e3389-111">إذا قمت بتغيير قالب التقويم، فلا يتم نشر هذه التغييرات إلى ساعات عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="e3389-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="e3389-112">لتغيير ساعات عمل المشروع، يجب تطبيق قالب جديد.</span><span class="sxs-lookup"><span data-stu-id="e3389-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="e3389-113">لإنشاء قالب تقويم لمنظمتك، يوجد متطلبين أساسيين:</span><span class="sxs-lookup"><span data-stu-id="e3389-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="e3389-114">حدد ساعات العمل المطلوبة في القالب باستخدام مورد جديد أو موجود قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="e3389-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="e3389-115">قم بإنشاء قالب تقويم جديد وإقران القالب بالمورد القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="e3389-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="e3389-116">**تحديد ساعات عمل القالب**</span><span class="sxs-lookup"><span data-stu-id="e3389-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="e3389-117">انتقل إلى **الموارد** \> **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="e3389-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="e3389-118">قم بإنشاء مورد جديد للمرجع في قالب التقويم، أو حدد موردًا موجودًا.</span><span class="sxs-lookup"><span data-stu-id="e3389-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="e3389-119">حدد علامة التبويب **ساعات العمل** للمورد واستكمل الإرشادات في [تعيين ساعات العمل للمورد](/dynamics365/field-service/set-work-hours-resource.md) لتكوين قواعد التقويم.</span><span class="sxs-lookup"><span data-stu-id="e3389-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="e3389-120">**إنشاء قالب تكوين جديد.**</span><span class="sxs-lookup"><span data-stu-id="e3389-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="e3389-121">انتقل إلى **الإعدادات** \> **قالب التقويم**.</span><span class="sxs-lookup"><span data-stu-id="e3389-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="e3389-122">حدد **جديد**، وأدخل اسمًا ووصفًا ومورد القالب.</span><span class="sxs-lookup"><span data-stu-id="e3389-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="e3389-123">عند الرجوع إلى مورد في قالب تقويم، يتم ربط نسخة من تقويم المورد مع قالب التقويم.</span><span class="sxs-lookup"><span data-stu-id="e3389-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="e3389-124">إذا تم تغيير ساعات العمل للقالب المنسوخ، فلا يتم نشر هذه التغييرات إلى قالب التقويم.</span><span class="sxs-lookup"><span data-stu-id="e3389-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="e3389-125">يمكنك الآن إقران قالب العمل بقالب تقويم مشروع.</span><span class="sxs-lookup"><span data-stu-id="e3389-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

