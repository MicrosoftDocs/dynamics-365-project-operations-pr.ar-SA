---
title: نظرة عامة على الفوترة بين الشركات الشقيقة
description: يوفر هذا الموضوع معلومات وأمثلة حول الفوترة بين الشركات الشقيقة للمشاريع.
author: sigitac
ms.date: 11/19/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: c1dcf642f79ce64cb83285ac6dc6d7eaf815145c
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369360"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="f9167-103">نظرة عامة على الفوترة بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="f9167-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="f9167-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="f9167-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f9167-105">قد يكون لدي مؤسستك أقسام وشركات متعددة وكيانات قانونيه أخرى تقوم بنقل المنتجات والخدمات إلى بعضها البعض للمشاريع.</span><span class="sxs-lookup"><span data-stu-id="f9167-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="f9167-106">ويطلق علي الكيان القانوني الذي يوفر الخدمة أو المنتج *الكيان القانوني المقرض*.</span><span class="sxs-lookup"><span data-stu-id="f9167-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="f9167-107">ويطلق علي الكيان القانوني الذي يستلم الخدمة أو المنتج *الكيان القانوني المقترض*.</span><span class="sxs-lookup"><span data-stu-id="f9167-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="f9167-108">يوضح الشكل التوضيحي التالي سيناريو نموذجي حيث يتشارك كيانات قانونيان، Contoso Robotics الولايات المتحدة الأمريكية (the borrowing legal entity) و Contoso Robotics المملكة المتحدة (الكيان القانوني المستقل) في الموارد لتسليم مشروع إلى العميل، Adventure works.</span><span class="sxs-lookup"><span data-stu-id="f9167-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="f9167-109">لهذا السيناريو، تم التعاقد مع شركة Contoso Robotics الولايات المتحدة الأمريكية لتسليم العمل إلى الشركة Adventure Works.</span><span class="sxs-lookup"><span data-stu-id="f9167-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![الفوترة بين الشركات الشقيقة](./media/IntercompanyScenario.png) 

<span data-ttu-id="f9167-111">يستخدم Dynamics 365 Project Operations التدفق التالي لمعالجه الحركات بين الشركات الشقيقة:</span><span class="sxs-lookup"><span data-stu-id="f9167-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="f9167-112">تسجل الموارد من الكيان القانوني للإقراض معاملات الوقت أو المصروفات بين الشركات الشقيقة عن طريق حجز الوقت والمصروفات مقابل المشاريع في الكيان القانوني المقترض.</span><span class="sxs-lookup"><span data-stu-id="f9167-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="f9167-113">يتم تسجيل تكاليف الوقت والمصروفات في الشركة المُقرضة باستخدام قائمة أسعار تكلفة الوحدة للشركة المقترضة.</span><span class="sxs-lookup"><span data-stu-id="f9167-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="f9167-114">يتم تسجيل معاملات البيع غير المفوترة بين الشركات الشقيقة في الشركة المُقرضة باستخدام قائمة أسعار تكلفة الوحدة للشركة المقترضة.</span><span class="sxs-lookup"><span data-stu-id="f9167-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="f9167-115">يتم تسجيل الإيرادات غير المفوترة في الشركة المقترضة باستخدام قائمة أسعار مبيعات عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="f9167-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="f9167-116">يمكن إصدار فاتورة للعميل عند تسجيل الإيرادات غير المفوترة.</span><span class="sxs-lookup"><span data-stu-id="f9167-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="f9167-117">لا يتعين على العميل الانتظار حتى اكتمال معالجة الفواتير بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="f9167-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="f9167-118">يتم إنشاء فواتير العملاء بين الشركات الشقيقة على أساس دوري في الشركة المُقرضة.</span><span class="sxs-lookup"><span data-stu-id="f9167-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="f9167-119">يتم إنشاء الفواتير يدويًا أو باستخدام عملية آلية دورية.</span><span class="sxs-lookup"><span data-stu-id="f9167-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="f9167-120">يمكن إنشاء فاتورة واحدة لكل كيان قانوني مقترض أو يمكن إنشاء فواتير منفصلة بواسطة المشروع.</span><span class="sxs-lookup"><span data-stu-id="f9167-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="f9167-121">عندما يتم ترحيل فاتورة العميل بين الشركات الشقيقة في الكيان القانوني للإقراض ، يتم إنشاء فاتورة المورد المعلقة المقابلة في الكيان القانوني المقترض.</span><span class="sxs-lookup"><span data-stu-id="f9167-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="f9167-122">سيتم تسجيل التكاليف الموجودة في فاتورة البائع المعلقة في دفتر الأستاذ الفرعي للمشروع عند ترحيل الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="f9167-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="f9167-123">يوضح الرسم التخطيطي التالي الفواتير بين الشركات الشقيقة من حيث ارتباطها بأحداث المحاسبة والترحيلات المتوقعة إلى دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="f9167-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![التدفق بين الشركات الشقيقة](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="f9167-125">الموارد الإضافية</span><span class="sxs-lookup"><span data-stu-id="f9167-125">Additional resources</span></span>

- [<span data-ttu-id="f9167-126">تكوين الفوترة بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="f9167-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="f9167-127">تسجيل حركات بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="f9167-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="f9167-128">إنشاء فواتير العميل والمورّد بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="f9167-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]