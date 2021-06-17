---
title: مزامنة سعة الموارد
description: يقدم هذا الموضوع معلومات حول كيفية مزامنة سعة مورد عبر التقويمات والمشروعات.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8bde3c434680f0651293cbce13ecdce945c3a743
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997495"
---
# <a name="synchronize-resource-capacity"></a><span data-ttu-id="fbc78-103">مزامنة سعة الموارد</span><span class="sxs-lookup"><span data-stu-id="fbc78-103">Synchronize resource capacity</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="fbc78-104">تساعد عمليات مزامنة الموارد على ضمان أن المعلومات الخاصة بالتقويم والتقويم الأساسي تتدفق إلى أسفل في جدولة موارد المشروع.</span><span class="sxs-lookup"><span data-stu-id="fbc78-104">The processes for resource synchronization help guarantee that information for the calendar and base calendar trickles down into project resource scheduling.</span></span> <span data-ttu-id="fbc78-105">إذا تم تغيير التقويم ، تقوم العمليات بإجراء التحديثات المطلوبة لجدولة موارد المشروع.</span><span class="sxs-lookup"><span data-stu-id="fbc78-105">If the calendar is changed, the processes make the required updates to the scheduling of project resources.</span></span> <span data-ttu-id="fbc78-106">تساعد العمليات أيضًا في تحسين الأداء ، لأن معلومات موارد التقويم تتم مزامنتها مسبقًا.</span><span class="sxs-lookup"><span data-stu-id="fbc78-106">The processes also help improve performance, because the calendar's resource information is synchronized in advance.</span></span> <span data-ttu-id="fbc78-107">لذلك ، تحدث تحديثات معلومات جدولة الموارد بسرعة أكبر.</span><span class="sxs-lookup"><span data-stu-id="fbc78-107">Therefore, updates to resource scheduling information occur more quickly.</span></span> <span data-ttu-id="fbc78-108">نوصي بجدولة العمليات كدفعة بدلاً من واحدة في كل مرة.</span><span class="sxs-lookup"><span data-stu-id="fbc78-108">We recommend that you schedule the processes as a batch instead of one at a time.</span></span> <span data-ttu-id="fbc78-109">خلاف ذلك ، هناك خطر أن ينسى شخص ما التواريخ الشاملة التي تمت فيها مزامنة المعلومات آخر مرة.</span><span class="sxs-lookup"><span data-stu-id="fbc78-109">Otherwise, there is a risk that someone will forget the inclusive dates when the information was last synchronized.</span></span> <span data-ttu-id="fbc78-110">إذا لم يتم استخدام التواريخ الشاملة ، فقد تحدث فجوات أثناء مزامنة التاريخ.</span><span class="sxs-lookup"><span data-stu-id="fbc78-110">If inclusive dates aren't used, gaps can occur during date synchronization.</span></span>

![مزامنة التقويم](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a><span data-ttu-id="fbc78-112">قم بمزامنة عمليات تجميع القدرة الإنتاجية للموارد</span><span class="sxs-lookup"><span data-stu-id="fbc78-112">Synchronize resource capacity roll-ups</span></span>

<span data-ttu-id="fbc78-113">تم تصميم عملية المزامنة لمزامنة كافة معلومات تقويم المورد.</span><span class="sxs-lookup"><span data-stu-id="fbc78-113">The synchronization process is designed to synchronize all resource calendar information.</span></span> <span data-ttu-id="fbc78-114">تتضمن هذه المعلومات معلومات التقويم الاساسيه حول إيه تغييرات في جدول "التقويم" الخاص بالمشروع "المصدر الأصل".</span><span class="sxs-lookup"><span data-stu-id="fbc78-114">This information includes base calendar information about any changes to the project's Resource calendar capacity table.</span></span> <span data-ttu-id="fbc78-115">في حاله أضافه موارد جديده في المشروع ، تساعد المزامنة علي ضمان توفر معلومات التقويم المحدثة.</span><span class="sxs-lookup"><span data-stu-id="fbc78-115">If new resources are added in the project, synchronization helps guarantee that the updated calendar information is available.</span></span> <span data-ttu-id="fbc78-116">يمكن القيام بهذه المزامنة في اي وقت.</span><span class="sxs-lookup"><span data-stu-id="fbc78-116">This synchronization can be done at any time.</span></span>

<span data-ttu-id="fbc78-117">نوصي باستخدام دفعة.</span><span class="sxs-lookup"><span data-stu-id="fbc78-117">We recommend that you use a batch.</span></span> <span data-ttu-id="fbc78-118">تتوفر الخيارات اثناء مزامنة عمليات الحفاظ علي القدرة الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="fbc78-118">The options are available during synchronization of capacity reservations.</span></span>

1. <span data-ttu-id="fbc78-119">حدد **إدارة المشاريع والمحاسبة** &gt; **دوري** &gt; **مزامنة القدرة الإنتاجية** &gt; **مزامنة عمليات تجميع القدرة الإنتاجية للموارد‬**.</span><span class="sxs-lookup"><span data-stu-id="fbc78-119">Select **Project management and accounting** &gt; **Periodic** &gt; **Capacity synchronization** &gt; **Synchronize resources capacity roll-ups**.</span></span>
2. <span data-ttu-id="fbc78-120">قم بتعيين الخيارات في الجدول التالي.</span><span class="sxs-lookup"><span data-stu-id="fbc78-120">Set the options in the following table.</span></span>

    | <span data-ttu-id="fbc78-121">خيار</span><span class="sxs-lookup"><span data-stu-id="fbc78-121">Option</span></span>      | <span data-ttu-id="fbc78-122">‏‏الوصف</span><span class="sxs-lookup"><span data-stu-id="fbc78-122">Description</span></span> |
    |-------------|-------------|
    | <span data-ttu-id="fbc78-123">كود الفترة</span><span class="sxs-lookup"><span data-stu-id="fbc78-123">Period code</span></span> | <span data-ttu-id="fbc78-124">حدد كود الفترة الزمنية لدفتر الأستاذ العام بشكل اختياري لتعيين تاريخي البدء والانتهاء لعمليه المزامنة الخاصة باللفات الانتاجيه للقدرة علي الموارد.</span><span class="sxs-lookup"><span data-stu-id="fbc78-124">Optionally select the General ledger date interval code to set the start and end dates for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="fbc78-125">تاريخ البدء</span><span class="sxs-lookup"><span data-stu-id="fbc78-125">Start date</span></span>  | <span data-ttu-id="fbc78-126">ادخل تاريخ البدء الخاص بعمليه المزامنة الخاصة بلفات الموارد والموردين.</span><span class="sxs-lookup"><span data-stu-id="fbc78-126">Enter the start date for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="fbc78-127">تاريخ الانتهاء</span><span class="sxs-lookup"><span data-stu-id="fbc78-127">End date</span></span>    | <span data-ttu-id="fbc78-128">ادخل تاريخ الانتهاء الخاص بعمليه المزامنة الخاصة بلفات الموارد والموردين.</span><span class="sxs-lookup"><span data-stu-id="fbc78-128">Enter the end date for the synchronization process for resource capacity roll-ups.</span></span> |

<span data-ttu-id="fbc78-129">[![عملية المزامنة](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span><span class="sxs-lookup"><span data-stu-id="fbc78-129">[![Synchronization process](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]