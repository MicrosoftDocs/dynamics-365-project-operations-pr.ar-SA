---
title: استلام العناصر في أمر الشراء من متطلبات الصنف
description: يشرح هذا الموضوع كيفية استلام العناصر في أمر الشراء من أحد متطلبات الصنف.
author: Yowelle
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
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c2083516ff929113fd6db377acfe5aeb104666dd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288212"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="08c84-103">استلام العناصر في أمر الشراء من متطلبات الصنف</span><span class="sxs-lookup"><span data-stu-id="08c84-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="08c84-104">يشرح هذا الموضوع كيفية استلام العناصر في أمر الشراء من أحد متطلبات الصنف.</span><span class="sxs-lookup"><span data-stu-id="08c84-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="08c84-105">باستخدام متطلب صنف بدلاً من حركة صنف ، يمكنك التخطيط للتسليم قبل استخدام العنصر فعليًا مباشرةً ، وإنشاء أمر شراء ، وتضمين العنصر في إطار عمل اتفاقية التجارة ، وتضمين متطلب الصنف في تخطيط الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="08c84-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="08c84-106">تستخدم هذه المهمة مجموعة بيانات USSI.</span><span class="sxs-lookup"><span data-stu-id="08c84-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="08c84-107">في جزء التنقل، انتقل إلى **الوحدات > إدارة المشاريع ومحاسبتها > المشاريع > جميع المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="08c84-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="08c84-108">في القائمة ، حدد الارتباط في الصف المطلوب.</span><span class="sxs-lookup"><span data-stu-id="08c84-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="08c84-109">في جزء الإجراءات، حدد **خطة**.</span><span class="sxs-lookup"><span data-stu-id="08c84-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="08c84-110">حدد **متطلبات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="08c84-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="08c84-111">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="08c84-111">Select **New**.</span></span>
6. <span data-ttu-id="08c84-112">في الصف الجديد، أدخل قيمه أو حددها في حقل **رقم الصنف**.</span><span class="sxs-lookup"><span data-stu-id="08c84-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="08c84-113">في حقل **الكمية**، حدد رقمًا.</span><span class="sxs-lookup"><span data-stu-id="08c84-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="08c84-114">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="08c84-114">Select **Save**.</span></span>
9. <span data-ttu-id="08c84-115">في جزء الإجراءات، حدد **إدارة**.</span><span class="sxs-lookup"><span data-stu-id="08c84-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="08c84-116">حدد **الوظائف**.</span><span class="sxs-lookup"><span data-stu-id="08c84-116">Select **Functions**.</span></span>
11. <span data-ttu-id="08c84-117">حدد **إنشاء أمر شراء**.</span><span class="sxs-lookup"><span data-stu-id="08c84-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="08c84-118">حدد خانة الاختيار **تضمين الكل**.</span><span class="sxs-lookup"><span data-stu-id="08c84-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="08c84-119">في حقل **حساب المورد**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="08c84-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="08c84-120">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="08c84-120">Select **OK**.</span></span>
15. <span data-ttu-id="08c84-121">في جزء التنقل، انتقل إلى **الوحدات > الحسابات الدائنة > أوامر الشراء > جميع موردي الشراء**.</span><span class="sxs-lookup"><span data-stu-id="08c84-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="08c84-122">في القائمة ، حدد الارتباط في الصف المطلوب.</span><span class="sxs-lookup"><span data-stu-id="08c84-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="08c84-123">في جزء الإجراءات، حدد **شراء**.</span><span class="sxs-lookup"><span data-stu-id="08c84-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="08c84-124">حدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="08c84-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="08c84-125">في جزء الإجراءات، حدد **استلام**.</span><span class="sxs-lookup"><span data-stu-id="08c84-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="08c84-126">حدد **إيصال استلام المنتج**.</span><span class="sxs-lookup"><span data-stu-id="08c84-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="08c84-127">في حقل **إيصال استلام المنتج**، اكتب قيمة.</span><span class="sxs-lookup"><span data-stu-id="08c84-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="08c84-128">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="08c84-128">Select **OK**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]