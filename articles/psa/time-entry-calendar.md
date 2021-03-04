---
title: تقويم إدخال الوقت
description: يقدم هذا الموضوع معلومات حول كيفية استخدام تقويم إدخال الوقت.
author: rumant
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 94e580955b83b9f2eaf6c0487cc9fe8a30f51ce0
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150157"
---
# <a name="time-entry-calendar"></a><span data-ttu-id="8b71d-103">تقويم إدخال الوقت</span><span class="sxs-lookup"><span data-stu-id="8b71d-103">Time entry calendar</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8b71d-104">في صفحة **إدخالات الوقت**، يمكنك عرض إدخالات الوقت في التقويم عن طريق تحديد **عرض كـ**\> **عنصر تحكم التقويم**.</span><span class="sxs-lookup"><span data-stu-id="8b71d-104">On the **Time Entries** page, you can view the time entries on the calendar by selecting **Show as** \> **Calendar Control**.</span></span>

## <a name="updated-calendar-control"></a><span data-ttu-id="8b71d-105">عنصر تحكم التقويم المحدث</span><span class="sxs-lookup"><span data-stu-id="8b71d-105">Updated calendar control</span></span>

<span data-ttu-id="8b71d-106">يقدم Dynamics 365 Project Service Automation تجربة إدخال وقت جديده وقابله للتوسيع.</span><span class="sxs-lookup"><span data-stu-id="8b71d-106">Dynamics 365 Project Service Automation offers a new and extensible time entry experience.</span></span> <span data-ttu-id="8b71d-107">وتحل هذه التجربة الجديدة محل عنصر تحكم التقويم المخصص الذي تم استخدامه في الإصدارات السابقة.</span><span class="sxs-lookup"><span data-stu-id="8b71d-107">This new experience replaces the Custom Calendar Control that was used in earlier versions.</span></span> <span data-ttu-id="8b71d-108">ومع ذلك، لا يزال بإمكانك عرض إدخالات الوقت من خلال عنصر تحكم تقويم للقراءة فقط والذي يوفره إطار الواجهة الموحدة لطرق العرض اليومية أو الأسبوعيه أو الشهرية.</span><span class="sxs-lookup"><span data-stu-id="8b71d-108">However, you can still view time entries through a read-only calendar control that the Unified Interface Framework provides for daily, weekly, or monthly views.</span></span>

<span data-ttu-id="8b71d-109">لا يدعم التقويم الإجراءات في عناصر التقويم الفردية، ولا يمكنك تحديد عنصر تقويم واحد أو أكثر للإرسال أو الحذف.</span><span class="sxs-lookup"><span data-stu-id="8b71d-109">The calendar doesn't support actions on individual calendar items, and you can't select one or more calendar items for submission or deletion.</span></span> <span data-ttu-id="8b71d-110">بدلاً من ذلك، حدد عنصر تقويم لفتح صفحة كيان **إدخال الوقت**، حيث يمكنك إكمال الإجراءات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="8b71d-110">Instead, select a calendar item to open the **Time Entry** entity page, where you can complete the required actions.</span></span>

## <a name="extensibility"></a><span data-ttu-id="8b71d-111">إمكانية التوسعة</span><span class="sxs-lookup"><span data-stu-id="8b71d-111">Extensibility</span></span>

<span data-ttu-id="8b71d-112">في صفحة **إدخالات الوقت** التي تحتوي على شبكة إدخال الوقت، يمكنك إضافة حقول مخصصة وإعداد حقول البحث وإنشاء طرق عرض مخصصة.</span><span class="sxs-lookup"><span data-stu-id="8b71d-112">On the **Time Entries** page that has the time entry grid, you can add custom fields, set up lookup fields, and create custom views.</span></span> <span data-ttu-id="8b71d-113">يمكنك أيضًا إعداد منطق عمل مخصص يستند إلى القيم التي تم تحديدها أو إدخالها في حقول مخصصة.</span><span class="sxs-lookup"><span data-stu-id="8b71d-113">You can also set up custom business logic that is based on the values that are selected or entered in custom fields.</span></span>
