---
title: تحديد تقاويم المشاريع
description: يوفر هذا الموضوع معلومات حول كيفية تطبيق قالب تقويم على مشروع لتعقب جدول المشروع.
author: ruhercul
manager: AnnBe
ms.date: 02/05/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: 1d5642d7a2246dc878b2bc4f504f138b71d29a69
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981284"
---
# <a name="define-project-calendars"></a><span data-ttu-id="e1357-103">تحديد تقاويم المشاريع</span><span class="sxs-lookup"><span data-stu-id="e1357-103">Define project calendars</span></span>

<span data-ttu-id="e1357-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="e1357-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e1357-105">لإنشاء مشروع وإدارته، يجب تطبيق قالب تقويم على المشروع.</span><span class="sxs-lookup"><span data-stu-id="e1357-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="e1357-106">يحدد قالب التقويم سمات المشروع التالية:</span><span class="sxs-lookup"><span data-stu-id="e1357-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="e1357-107">ساعات العمل، بما في ذلك وقت البدء والانتهاء</span><span class="sxs-lookup"><span data-stu-id="e1357-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="e1357-108">أيام العمل</span><span class="sxs-lookup"><span data-stu-id="e1357-108">Working days</span></span>
- <span data-ttu-id="e1357-109">استثناءات التقويم مثل الأيام غير المخصصة للعمل</span><span class="sxs-lookup"><span data-stu-id="e1357-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="e1357-110">قالب التقويم المطبق على مشروع هو نسخة من قالب التقويم المعرف في إعدادات المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="e1357-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="e1357-111">إذا قمت بتغيير قالب التقويم، فلا يتم نشر هذه التغييرات إلى ساعات عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="e1357-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="e1357-112">لتغيير ساعات عمل المشروع، يجب تطبيق قالب جديد.</span><span class="sxs-lookup"><span data-stu-id="e1357-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="e1357-113">لإنشاء قالب تقويم لمنظمتك، يوجد متطلبين أساسيين:</span><span class="sxs-lookup"><span data-stu-id="e1357-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="e1357-114">حدد ساعات العمل المطلوبة في القالب باستخدام مورد جديد أو موجود قابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="e1357-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="e1357-115">قم بإنشاء قالب تقويم جديد وإقران القالب بالمورد القابل للحجز.</span><span class="sxs-lookup"><span data-stu-id="e1357-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="e1357-116">**تحديد ساعات عمل القالب**</span><span class="sxs-lookup"><span data-stu-id="e1357-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="e1357-117">انتقل إلى **الموارد** \> **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="e1357-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="e1357-118">قم بإنشاء مورد جديد للمرجع في قالب التقويم، أو حدد موردًا موجودًا.</span><span class="sxs-lookup"><span data-stu-id="e1357-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="e1357-119">حدد علامة التبويب **ساعات العمل** للمورد واستكمل الإرشادات في [تعيين ساعات العمل للمورد](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) لتكوين قواعد التقويم.</span><span class="sxs-lookup"><span data-stu-id="e1357-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="e1357-120">**إنشاء قالب تكوين جديد.**</span><span class="sxs-lookup"><span data-stu-id="e1357-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="e1357-121">انتقل إلى **الإعدادات** \> **قالب التقويم**.</span><span class="sxs-lookup"><span data-stu-id="e1357-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="e1357-122">حدد **جديد**، وأدخل اسمًا ووصفًا ومورد القالب.</span><span class="sxs-lookup"><span data-stu-id="e1357-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="e1357-123">عند الرجوع إلى مورد في قالب تقويم، يتم ربط نسخة من تقويم المورد مع قالب التقويم.</span><span class="sxs-lookup"><span data-stu-id="e1357-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="e1357-124">إذا تم تغيير ساعات العمل للقالب المنسوخ، فلا يتم نشر هذه التغييرات إلى قالب التقويم.</span><span class="sxs-lookup"><span data-stu-id="e1357-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="e1357-125">يمكنك الآن إقران قالب العمل بقالب تقويم مشروع.</span><span class="sxs-lookup"><span data-stu-id="e1357-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

