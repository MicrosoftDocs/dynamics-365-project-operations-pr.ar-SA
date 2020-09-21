---
title: استخدام حقل موجود في Project Service كبعد تسعير
description: يقدم هذا الموضوع معلومات حول استخدام حقول Project Service الموجودة كأبعاد تسعير.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: ed86e0c4-b2ea-4b3b-b9e3-cbfb3b512591
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: b280e2aeecc9d63fb65b77fad809edff817aff65
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748661"
---
# <a name="use-an-existing-field-in-project-service-as-a-pricing-dimension"></a><span data-ttu-id="f98cb-103">استخدام حقل موجود في Project Service كبعد تسعير</span><span class="sxs-lookup"><span data-stu-id="f98cb-103">Use an existing field in Project Service as a pricing dimension</span></span>

<span data-ttu-id="f98cb-104">يشتمل Project Service Automation (PSA) على العديد من الحقول في كيان **القيم الفعلية** والتي يمكن استخدامها كأبعاد تسعير للأسعار المستندة إلى الموارد في مؤسسات المشروع.</span><span class="sxs-lookup"><span data-stu-id="f98cb-104">Project Service Automation (PSA) has many fields on the **Actuals** entity that can be used as pricing dimensions for resource-based pricing in project organizations.</span></span> <span data-ttu-id="f98cb-105">على سبيل المثال، حقل مشترك واحد هو **المورد القابل للحجز**.</span><span class="sxs-lookup"><span data-stu-id="f98cb-105">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="f98cb-106">قد تجد الشركات الصغيرة التي تحتوي على عدد أقل من 20-30 من الموارد القابلة للفوترة أن الحصول على أسعار التكلفة والفوترة الخاصة بكل مورد هي طريقة أبسط.</span><span class="sxs-lookup"><span data-stu-id="f98cb-106">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="f98cb-107">ومع ذلك، كلما زاد حجم القوة العاملة القابل للفوترة، فقد يصبح هذا غير واقعي للحفاظ عليه لأن تكلفه المورد وأسعار الفواتير تبدأ في الاختلاف عند ترقية الموارد أو اكتساب مزيد من الخبرة أو اكتساب مجموعات مهارات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="f98cb-107">However, as the billable workforce grows, this could become unrealistic to maintain as resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different skill sets.</span></span> <span data-ttu-id="f98cb-108">ونظرا لأن هذا الأسلوب لا يزال مستمرًا في العمل مع الشركات التي لها حجم معين، راجع الموضوع [استخدام مورد قابل للحجز كبُعد تسعير](bookable-resource-pricing-dimension.md) لفهم كيفية استخدام Project Service موجود كبُعد تسعير.</span><span class="sxs-lookup"><span data-stu-id="f98cb-108">Because this approach still works for companies of a certain size, see the topic, [Use a bookable resource as a pricing dimension](bookable-resource-pricing-dimension.md) to understand how an existing Project Service field can be used as a pricing dimension.</span></span>

<span data-ttu-id="f98cb-109">هناك مثال آخر لفئة الحركة.</span><span class="sxs-lookup"><span data-stu-id="f98cb-109">Another example is that of transaction category.</span></span> <span data-ttu-id="f98cb-110">قام العملاء والمنفذون باستخدام فئة الحركة في PSA لتصنيف العمل واستخدام الحقل لتحديد "السعر والتكلفة" حسب فئة العمل.</span><span class="sxs-lookup"><span data-stu-id="f98cb-110">Customers and Implementers have used the transaction category in PSA to classify work and use the field to price and cost based on the category of work.</span></span> <span data-ttu-id="f98cb-111">لمزيد من المعلومات، راجع [استخدام فئة الحركة كبُعد تسعير](transaction-category-pricing-dimension.md).</span><span class="sxs-lookup"><span data-stu-id="f98cb-111">For more information, see [Use transaction category as a pricing dimension](transaction-category-pricing-dimension.md).</span></span>
