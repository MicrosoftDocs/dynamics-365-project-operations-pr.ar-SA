---
title: حقول Project Operations كأبعاد تسعير
description: يقدم هذا الموضوع معلومات حول استخدام الحقول كأبعاد تسعير في Dynamics 365 Project Operations.
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
ms.openlocfilehash: 04b823e8237590a294ed0706e64d0ecb9d2cf56f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274622"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="9a763-103">حقول Project Operations كأبعاد تسعير</span><span class="sxs-lookup"><span data-stu-id="9a763-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="9a763-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="9a763-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9a763-105">يضم كيان **‏‫القيم الفعلية‬** العديد من الحقول التي يمكن استخدامها كأبعاد تسعير للأسعار المستندة إلى الموارد.</span><span class="sxs-lookup"><span data-stu-id="9a763-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="9a763-106">على سبيل المثال، حقل مشترك واحد هو **المورد القابل للحجز**.</span><span class="sxs-lookup"><span data-stu-id="9a763-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="9a763-107">قد تجد الشركات الصغيرة التي تحتوي على عدد أقل من 20-30 من الموارد القابلة للفوترة أن الحصول على أسعار التكلفة والفوترة الخاصة بكل مورد هي طريقة أبسط.</span><span class="sxs-lookup"><span data-stu-id="9a763-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="9a763-108">‏‫ومع ذلك، كلما زاد حجم القوة العاملة القابل للفوترة، فقد تصبح الأسعار الخاصة بالموارد غير واقعية للحفاظ عليه.</span><span class="sxs-lookup"><span data-stu-id="9a763-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="9a763-109">ويبدأ تغيير تكلفة الموارد وأسعار الفواتير مع ترقية الموارد أو الحصول على مزيد من الخبرة أو الحصول على مجموعة مختلفه من المهارات.</span><span class="sxs-lookup"><span data-stu-id="9a763-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="9a763-110">هناك مثال آخر لفئة الحركة.</span><span class="sxs-lookup"><span data-stu-id="9a763-110">Another example is that of transaction category.</span></span> <span data-ttu-id="9a763-111">قام العملاء والمنفذون باستخدام فئة الحركة لتصنيف العمل واستخدام الحقل لتحديد "السعر والتكلفة" حسب فئة العمل.</span><span class="sxs-lookup"><span data-stu-id="9a763-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]