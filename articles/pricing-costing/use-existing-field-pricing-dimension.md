---
title: حقول Project Operations كأبعاد تسعير
description: يوفر هذا الموضوع معلومات حول استخدام الحقول كأبعاد التسعير في Dynamics 365 Project operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 59367b35f15f806b109f606e912edc487d9e7685
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4119222"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="b2dd8-103">حقول Project Operations كأبعاد تسعير</span><span class="sxs-lookup"><span data-stu-id="b2dd8-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="b2dd8-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="b2dd8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b2dd8-105">يضم كيان **‏‫القيم الفعلية‬** العديد من الحقول التي يمكن استخدامها كأبعاد تسعير للأسعار المستندة إلى الموارد.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="b2dd8-106">على سبيل المثال، حقل مشترك واحد هو **المورد القابل للحجز**.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="b2dd8-107">قد تجد الشركات الصغيرة التي تحتوي على عدد أقل من 20-30 من الموارد القابلة للفوترة أن الحصول على أسعار التكلفة والفوترة الخاصة بكل مورد هي طريقة أبسط.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="b2dd8-108">‏‫ومع ذلك، كلما زاد حجم القوة العاملة القابل للفوترة، فقد تصبح الأسعار الخاصة بالموارد غير واقعية للحفاظ عليه.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="b2dd8-109">ويبدأ تغيير تكلفة الموارد وأسعار الفواتير مع ترقية الموارد أو الحصول على مزيد من الخبرة أو الحصول على مجموعة مختلفه من المهارات.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="b2dd8-110">هناك مثال آخر لفئة الحركة.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-110">Another example is that of transaction category.</span></span> <span data-ttu-id="b2dd8-111">قام العملاء والمنفذون باستخدام فئة الحركة لتصنيف العمل واستخدام الحقل لتحديد "السعر والتكلفة" حسب فئة العمل.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>
