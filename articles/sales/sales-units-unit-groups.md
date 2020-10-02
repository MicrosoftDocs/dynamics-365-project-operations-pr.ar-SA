---
title: الوحدات ومجموعات الوحدات
description: يقدم هذا الموضوع معلومات عن كيفية إنشاء الوحدات ومجموعات الوحدات في Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: ea5399368214a293ca7c10fabf21d82407b5c76f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898740"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="755ed-103">الوحدات ومجموعات الوحدات</span><span class="sxs-lookup"><span data-stu-id="755ed-103">Units and unit groups</span></span>

<span data-ttu-id="755ed-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="755ed-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="755ed-105">الوحدات هي الكميات أو القياسات التي تقوم ببيع المنتجات أو الخدمات فيها.</span><span class="sxs-lookup"><span data-stu-id="755ed-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="755ed-106">على سبيل المثال، إذا كنت تبيع لوازم الحدائق، قد تبيع البذور في وحدات من الحزم والصناديق والبالتات.</span><span class="sxs-lookup"><span data-stu-id="755ed-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="755ed-107">وتعد مجموعة الوحدات مجموعة من هذه الوحدات المختلفة.</span><span class="sxs-lookup"><span data-stu-id="755ed-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="755ed-108">لإكمال الخطوات الواردة في هذا الموضوع، تأكد من أنه قد تم تعيينك إلى مسؤول النظام أو لدور مدير Sales Professional أو أن لديك الأذونات المكافئة.</span><span class="sxs-lookup"><span data-stu-id="755ed-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="755ed-109">إنشاء مجموعة وحدة</span><span class="sxs-lookup"><span data-stu-id="755ed-109">Create a unit group</span></span>

1. <span data-ttu-id="755ed-110">في مخطط الموقع، حدد **الوحدات**.</span><span class="sxs-lookup"><span data-stu-id="755ed-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="755ed-111">حدد **جديد** وفي مربع الحوار **إنشاء مجموعة وحدات** أدخل اسم الوحدة.</span><span class="sxs-lookup"><span data-stu-id="755ed-111">Select **New**, and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="755ed-112">في حقل **‏‫الوحدة الأساسية‬** أدخل أصغر وحدة قياس شائعة سيتم بيع المنتج بها.</span><span class="sxs-lookup"><span data-stu-id="755ed-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="755ed-113">على سبيل المثال، يمكنك إدخال "قطعة" أو "أونصة".</span><span class="sxs-lookup"><span data-stu-id="755ed-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="755ed-114">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="755ed-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="755ed-115">إضافة وحدات إلى مجموعة وحدة</span><span class="sxs-lookup"><span data-stu-id="755ed-115">Add units to a unit group</span></span>

1. <span data-ttu-id="755ed-116">افتح مجموعة وحدات، وفي علامة التبويب **ذات صلة‬‏‫** حدد **الوحدات**.</span><span class="sxs-lookup"><span data-stu-id="755ed-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="755ed-117">سوف ترى أن الوحدة الأساسية تمت إضافتها بالفعل.</span><span class="sxs-lookup"><span data-stu-id="755ed-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="755ed-118">حدد **إضافة وحدة جديدة** وفي صفحة **الإنشاء السريع: وحدة‬‏‫** في حقل **الاسم** أدخل اسم الوحدة.</span><span class="sxs-lookup"><span data-stu-id="755ed-118">Select **Add New Unit**, and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="755ed-119">في حقل **الكمية** أدخل الكمية التي ستحتويها الوحدة.</span><span class="sxs-lookup"><span data-stu-id="755ed-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="755ed-120">على سبيل المثال، إذا كان الصندوق يحتوي على قطعتين، أدخل "2."</span><span class="sxs-lookup"><span data-stu-id="755ed-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="755ed-121">في حقل **‏‫الوحدة الأساسية‬** حدد وحدة أساسية لإنشاء اقل وحده قياس للوحدة.</span><span class="sxs-lookup"><span data-stu-id="755ed-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="755ed-122">على سبيل المثال، يمكنك تحديد "قطعة".</span><span class="sxs-lookup"><span data-stu-id="755ed-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="755ed-123">حدد **حفظ**:</span><span class="sxs-lookup"><span data-stu-id="755ed-123">Select **Save**:</span></span>
