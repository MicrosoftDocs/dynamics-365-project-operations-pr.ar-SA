---
title: استلام العناصر في أمر الشراء من متطلبات الصنف
description: يشرح هذا الموضوع كيفية استلام العناصر في أمر الشراء من أحد متطلبات الصنف.
author: KimANelson
manager: AnnBe
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.assetid: c61e3a5e-da3d-4f4c-87fa-03dea19f6936
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c5ed287aa24aff647ef1dc625f9e9f5f086ee662
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748590"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="5bda7-103">استلام العناصر في أمر الشراء من متطلبات الصنف</span><span class="sxs-lookup"><span data-stu-id="5bda7-103">Receive items on purchase order from item requirement</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="5bda7-104">يشرح هذا الموضوع كيفية استلام العناصر في أمر الشراء من أحد متطلبات الصنف.</span><span class="sxs-lookup"><span data-stu-id="5bda7-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="5bda7-105">باستخدام متطلب صنف بدلاً من حركة صنف ، يمكنك التخطيط للتسليم قبل استخدام العنصر فعليًا مباشرةً ، وإنشاء أمر شراء ، وتضمين العنصر في إطار عمل اتفاقية التجارة ، وتضمين متطلب الصنف في تخطيط الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="5bda7-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="5bda7-106">تستخدم هذه المهمة مجموعة بيانات USSI.</span><span class="sxs-lookup"><span data-stu-id="5bda7-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="5bda7-107">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > المشاريع > جميع المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="5bda7-108">في القائمة ، حدد الارتباط في الصف المطلوب.</span><span class="sxs-lookup"><span data-stu-id="5bda7-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="5bda7-109">في جزء الإجراءات، حدد **خطة**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="5bda7-110">حدد **متطلبات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="5bda7-111">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-111">Select **New**.</span></span>
6. <span data-ttu-id="5bda7-112">في الصف الجديد، أدخل قيمه أو حددها في حقل **رقم الصنف**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="5bda7-113">في حقل **الكمية**، حدد رقمًا.</span><span class="sxs-lookup"><span data-stu-id="5bda7-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="5bda7-114">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-114">Select **Save**.</span></span>
9. <span data-ttu-id="5bda7-115">في جزء الإجراءات، حدد **إدارة**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="5bda7-116">حدد **الوظائف**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-116">Select **Functions**.</span></span>
11. <span data-ttu-id="5bda7-117">حدد **إنشاء أمر شراء**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="5bda7-118">حدد خانة الاختيار **تضمين الكل**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="5bda7-119">في حقل **حساب المورد**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="5bda7-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="5bda7-120">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-120">Select **OK**.</span></span>
15. <span data-ttu-id="5bda7-121">في جزء التنقل، انتقل إلى **الوحدات > الحسابات الدائنة > أوامر الشراء > جميع موردي الشراء**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="5bda7-122">في القائمة ، حدد الارتباط في الصف المطلوب.</span><span class="sxs-lookup"><span data-stu-id="5bda7-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="5bda7-123">في جزء الإجراءات، حدد **شراء**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="5bda7-124">حدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="5bda7-125">في جزء الإجراءات، حدد **استلام**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="5bda7-126">حدد **إيصال استلام المنتج**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="5bda7-127">في حقل **إيصال استلام المنتج**، اكتب قيمة.</span><span class="sxs-lookup"><span data-stu-id="5bda7-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="5bda7-128">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5bda7-128">Select **OK**.</span></span>

