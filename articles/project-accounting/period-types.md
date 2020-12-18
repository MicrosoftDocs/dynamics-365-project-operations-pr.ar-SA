---
title: أنواع الفترات
description: يقدم هذا الموضوع معلومات حول كيفيه اعداد أنواع الفترات لتقدير الإيرادات.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6bcd988fbd074c66d64f7e327b4329d3de27e950
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531341"
---
# <a name="period-types"></a><span data-ttu-id="a4e90-103">أنواع الفترات</span><span class="sxs-lookup"><span data-stu-id="a4e90-103">Period types</span></span>

<span data-ttu-id="a4e90-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="a4e90-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a4e90-105">يحدد نوع الفترة الطريقة التي يتم بها تقدير الإيراد في المشروع.</span><span class="sxs-lookup"><span data-stu-id="a4e90-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="a4e90-106">يقدم هذا الموضوع معلومات حول كيفيه اعداد أنواع الفترات لتقدير الإيرادات.</span><span class="sxs-lookup"><span data-stu-id="a4e90-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="a4e90-107">إنشاء أنواع الفترة الزمنية والعمل معها</span><span class="sxs-lookup"><span data-stu-id="a4e90-107">Create and work with period types</span></span>
<span data-ttu-id="a4e90-108">لإنشاء والعمل مع أنواع الفترات، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="a4e90-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="a4e90-109">في بيئة Dynamics 365 Finance الخاصة بك، انتقل إلى **إدارة المشاريع والمحاسبة** > **الإعداد** > **التقديرات** > **أنواع الفترات**.</span><span class="sxs-lookup"><span data-stu-id="a4e90-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="a4e90-110">حدد **جديد** لإنشاء نوع فترة جديد.</span><span class="sxs-lookup"><span data-stu-id="a4e90-110">Select **New** to create new period type.</span></span> <span data-ttu-id="a4e90-111">أدخل اسمًا ووصفًا.</span><span class="sxs-lookup"><span data-stu-id="a4e90-111">Enter a name and description.</span></span>
3. <span data-ttu-id="a4e90-112">في حقل **التكرار**، حدد قيمة:</span><span class="sxs-lookup"><span data-stu-id="a4e90-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="a4e90-113">إذا حددت **أسبوع** أو **نصف أسبوعي** أو **نصف شهري** أو **شهر** أو **يوم** أو **ربع سنة** أو **سنة**، سيتم استخدام التقويم لإنشاء الفترات.</span><span class="sxs-lookup"><span data-stu-id="a4e90-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="a4e90-114">إذا قمت بتحديد **فتره دفتر الأستاذ**، سيتم استخدام فترات دفتر الأستاذ من تكوين دفتر الأستاذ العام لإنشاء فترات.</span><span class="sxs-lookup"><span data-stu-id="a4e90-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="a4e90-115">إذا قمت بتحديد **غير محدود**، فيمكنك تحديد فترات مخصصة.</span><span class="sxs-lookup"><span data-stu-id="a4e90-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="a4e90-116">حدد سجل نوع الفترة، ثم حدد **إنشاء فترات** لإنشاء فترات لنوع الفترة.</span><span class="sxs-lookup"><span data-stu-id="a4e90-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="a4e90-117">استنادًا إلى فترة التكرار التي حددتها، قد يكون لديك خيار تحديد تاريخ البدء أو عدد الفترات المطلوب إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="a4e90-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="a4e90-118">حدد **فترات** لمراجعة الفترات التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="a4e90-118">Select **Periods** to review generated periods.</span></span>

