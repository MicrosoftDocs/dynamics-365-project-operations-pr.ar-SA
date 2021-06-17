---
title: إنشاء إدخالات الوقت
description: يقدم هذا الموضوع معلومات عن كيفية إنشاء إدخالات الوقت.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: bc8e52fef0aa02505e412c746343ce1410c40ac3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999250"
---
# <a name="create-time-entries"></a><span data-ttu-id="73444-103">إنشاء إدخالات الوقت</span><span class="sxs-lookup"><span data-stu-id="73444-103">Create time entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="73444-104">في الإصدارات السابقة من Dynamics 365 Project Service Automation، تم إدخال إدخالات الوقت على أساس أسبوعي.</span><span class="sxs-lookup"><span data-stu-id="73444-104">In previous versions of Dynamics 365 Project Service Automation, time entries were entered on a weekly basis.</span></span> <span data-ttu-id="73444-105">في الإصدار 3 من Project Service Automation، يتم إدخال إدخالات الوقت على أساس يومي.</span><span class="sxs-lookup"><span data-stu-id="73444-105">In version 3 of Project Service Automation, time entries are entered on a daily basis.</span></span> <span data-ttu-id="73444-106">ومع ذلك، بعد أن يتم إنشاء إدخالات وقت قليلة، يمكنك إنشاء مجموعة منها أو نسخها بشكل مجمع.</span><span class="sxs-lookup"><span data-stu-id="73444-106">However, after a few time entries have been created, you can bulk create or copy them.</span></span>

## <a name="create-a-time-entry"></a><span data-ttu-id="73444-107">إنشاء إدخال وقت</span><span class="sxs-lookup"><span data-stu-id="73444-107">Create a time entry</span></span>

<span data-ttu-id="73444-108">اتبع هذه الخطوات لإنشاء إدخال وقت.</span><span class="sxs-lookup"><span data-stu-id="73444-108">Follow these steps to create a time entry.</span></span>

1. <span data-ttu-id="73444-109">في صفحة **إدخالات الوقت**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="73444-109">On the **Time Entries** page, select **New**.</span></span>
2. <span data-ttu-id="73444-110">في مربع الحوار **الإنشاء السريع: إدخال الوقت**، أدخل مدة إدخال الوقت بالدقائق أو الساعات أو الأيام.</span><span class="sxs-lookup"><span data-stu-id="73444-110">In the **Quick Create: Time Entry** dialog box, enter the duration of the time entry in minutes, hours, or days.</span></span> <span data-ttu-id="73444-111">يجب إدخال المدة بالتنسيق التالي: *x* من الدقائق *x* أو من الساعات أو *x* من الأيام.</span><span class="sxs-lookup"><span data-stu-id="73444-111">The duration must be entered in the following format: *x* minutes, *x* hours, or *x* days.</span></span> <span data-ttu-id="73444-112">يمكن أيضًا إدخال الساعات والأيام كقيم عشرية، مثل *x.x* من الساعات أو *x.x* من الأيام.</span><span class="sxs-lookup"><span data-stu-id="73444-112">Hours and days can also be entered as decimal values, such as *x.x* hours or *x.x* days.</span></span>
3. <span data-ttu-id="73444-113">حدد نوع إدخال الوقت والمشروع الذي تقوم بإدخال إدخال الوقت له.</span><span class="sxs-lookup"><span data-stu-id="73444-113">Select the type of time entry and the project that you're entering the time entry for.</span></span>
4. <span data-ttu-id="73444-114">في حقل **مهمة المشروع**، ابحث عن المهمة الخاصة بإدخال الوقت هذا.</span><span class="sxs-lookup"><span data-stu-id="73444-114">In the **Project Task** field, find the task for this time entry.</span></span>

    > [!NOTE]
    > <span data-ttu-id="73444-115">إذا كنت تقوم بإنشاء إدخال وقت لمهمة غير معينه لأحد المستخدمين، في حقل **مهمة المشروع**، حدد الزر **بحث**، وحدد **تغيير طريقة العرض**، ثم حدد **جميع مهام المشاريع النشطة** لسرد جميع المهام.</span><span class="sxs-lookup"><span data-stu-id="73444-115">If you're creating a time entry for a task that isn't assigned to a user, in the **Project Task** field, select the **Search** button, select **Change View**, and then select **All Active Project Tasks** to list all tasks.</span></span>

5. <span data-ttu-id="73444-116">قم بإدخال وصف، وإذا كان الوصف مطلوبًا، فحدد **حفظ وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="73444-116">Enter a description, if a description is required, and then select **Save and Close**.</span></span>

<span data-ttu-id="73444-117">وبعد إنشاء إدخال الوقت وحفظه، يمكنك تحريره في شبكة إدخالات الوقت.</span><span class="sxs-lookup"><span data-stu-id="73444-117">After the time entry is created and saved, you can edit it in the time entry grid.</span></span> <span data-ttu-id="73444-118">تدعم شبكة إدخالات الوقت التنسيقين التاليين:</span><span class="sxs-lookup"><span data-stu-id="73444-118">The time entry grid supports two formats:</span></span>

- <span data-ttu-id="73444-119">يمكنك إدخال إدخالات الوقت بتنسيق **hh:mm**.</span><span class="sxs-lookup"><span data-stu-id="73444-119">You can enter time entries in **hh:mm** format.</span></span> <span data-ttu-id="73444-120">يتم تحويل هذا التنسيق بعد ذلك إلى ساعات وكسور.</span><span class="sxs-lookup"><span data-stu-id="73444-120">This format is then converted to hours and fractions.</span></span>
- <span data-ttu-id="73444-121">يمكنك إدخال الساعات والكسور مباشرةً.</span><span class="sxs-lookup"><span data-stu-id="73444-121">You can enter hours and fractions directly.</span></span>

<span data-ttu-id="73444-122">لاحظ أن كسور الساعة ليس دقائق.</span><span class="sxs-lookup"><span data-stu-id="73444-122">Note that the fractions of an hour aren't minutes.</span></span> <span data-ttu-id="73444-123">وبالتالي، 1.5 ساعات تمثل 1 ساعة و30 دقيقة.</span><span class="sxs-lookup"><span data-stu-id="73444-123">Therefore, 1.5 hours represents 1 hour and 30 minutes.</span></span> <span data-ttu-id="73444-124">تنطبق نفس القاعدة على كسور اليوم.</span><span class="sxs-lookup"><span data-stu-id="73444-124">The same rule applies to fractions of a day.</span></span> <span data-ttu-id="73444-125">اليوم الواحد هو 24 ساعة، ويمثل 0.5 يوم 12 ساعة.</span><span class="sxs-lookup"><span data-stu-id="73444-125">One day is 24 hours, and 0.5 days represents 12 hours.</span></span>

## <a name="bulk-create-time-entries"></a><span data-ttu-id="73444-126">الإنشاء المجمع لإدخالات الوقت</span><span class="sxs-lookup"><span data-stu-id="73444-126">Bulk create time entries</span></span>

<span data-ttu-id="73444-127">بعد أن يتم إنشاء إدخالات وقت قليلة، يمكنك نسخها لإنشاء إدخالات وقت إضافية بشكل مجمع.</span><span class="sxs-lookup"><span data-stu-id="73444-127">After a few time entries have been created, you can copy them to create additional time entries in bulk.</span></span>

1. <span data-ttu-id="73444-128">في صفحة **إدخالات الوقت**، حدد **نسخ أسبوع**.</span><span class="sxs-lookup"><span data-stu-id="73444-128">On the **Time Entries** page, select **Copy Week**.</span></span>
2. <span data-ttu-id="73444-129">في المجموعة حقل **من الفترة**، في حقلي **تاريخ البدء** و **تاريخ الانتهاء**، حدد نطاق التاريخ لنسخ إدخالات الوقت منه.</span><span class="sxs-lookup"><span data-stu-id="73444-129">In the **From Period** field group, in the **Start Date** and **End Date** fields, define the date range to copy time entries from.</span></span>
3. <span data-ttu-id="73444-130">في مجموعة حقل **من الفترة**، في حقل **تاريخ البدء**، حدد التاريخ المراد إنشاء إدخالات الوقت له.</span><span class="sxs-lookup"><span data-stu-id="73444-130">In the **To Period** field group, in the **Start Date** field, specify the date to create time entries for.</span></span>
4. <span data-ttu-id="73444-131">حدد **نسخ** لإنشاء نسخة من إدخالات الوقت التي تتوافق مع يوم الأسبوع المحدد في مجموعة حقل **إلى الفترة**.</span><span class="sxs-lookup"><span data-stu-id="73444-131">Select **Copy** to create a copy of the time entries that correspond to the day of the week that is specified in the **To Period** field group.</span></span> <span data-ttu-id="73444-132">على سبيل المثال، يتم نسخ إدخال الوقت ليوم الإثنين من أيام الأسبوع الماضية إلى الأسبوع المحدد في مجموعة حقل **إلى الفترة**.</span><span class="sxs-lookup"><span data-stu-id="73444-132">For example, the time entry for Monday of last week is copied to Monday of the week that is specified in the **To Period** field group.</span></span>

## <a name="import-data-for-time-entries"></a><span data-ttu-id="73444-133">استيراد البيانات لإدخالات الوقت</span><span class="sxs-lookup"><span data-stu-id="73444-133">Import data for time entries</span></span>

<span data-ttu-id="73444-134">يمكنك استيراد البيانات من حجوزات المشروع وتعييناته.</span><span class="sxs-lookup"><span data-stu-id="73444-134">You can import data from project bookings and assignments.</span></span> <span data-ttu-id="73444-135">عند استيراد البيانات، يمكنك تحديد نطاق التاريخ لعمليات الحجز التي سيتم استيرادها ثم تحديد الحجوزات التي ينبغي إنشاؤها في شكل إدخالات وقت **مسودة**.</span><span class="sxs-lookup"><span data-stu-id="73444-135">When you import data, you can specify the date range of the bookings to import and then explicitly select the bookings that should be created as **Draft** time entries.</span></span>

## <a name="group-by-sort-search-and-filter-capabilities"></a><span data-ttu-id="73444-136">التجميع حسب، والفرز، والبحث، وإمكانات التصفية</span><span class="sxs-lookup"><span data-stu-id="73444-136">Group by, sort, search, and filter capabilities</span></span>

<span data-ttu-id="73444-137">يمكنك تجميع وتصفية إدخالات الوقت بواسطة الأبعاد المحددة في الأعمدة.</span><span class="sxs-lookup"><span data-stu-id="73444-137">You can group and filter time entries by the dimensions that are specified in the columns.</span></span> <span data-ttu-id="73444-138">في الحقل **تجميع حسب**، حدد البُعد المطلوب استخدامه لتصفية إدخالات الوقت.</span><span class="sxs-lookup"><span data-stu-id="73444-138">In the **Group by** field, select the dimension to use to filter time entries.</span></span> <span data-ttu-id="73444-139">يمكنك أيضًا فرز سجلات إدخالات الوقت في ترتيب تصاعدي أو تنازلي باستخدام سهم الفرز في عناوين الأعمدة.</span><span class="sxs-lookup"><span data-stu-id="73444-139">You can also sort the time entry records in ascending or descending order by using the sort arrow on the column headings.</span></span> <span data-ttu-id="73444-140">بالإضافة إلى ذلك، يمكنك إظهار الإدخالات أو إخفاؤها بتحديد الزر **تصفية** في عناوين الأعمدة، ثم في مربع **البحث**، ثم إدخال النص الذي يجب استخدامه للبحث عن إدخالات الوقت حسب اسم المشروع ومهمة المشروع وإدخال الوقت أو المورد.</span><span class="sxs-lookup"><span data-stu-id="73444-140">Additionally, you can show or hide entries by selecting the **Filter** button on the column headings, and then, in the **Search** box, entering the text that should be used to search for time entries by project name, project task, time entry, or resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]