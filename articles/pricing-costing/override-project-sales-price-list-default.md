---
title: تجاوز قوائم أسعار مبيعات المشروع
description: يقدم هذا الموضوع معلومات حول إنشاء قوائم أسعار مبيعات مخصصة.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: af9baca540d89f4e5e616bdfdd6111bef29abe28
ms.sourcegitcommit: 656a9d03f260c29e988e2ff05b6e07ae0365d6d0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "4672215"
---
# <a name="override-project-sales-price-lists"></a><span data-ttu-id="1087e-103">تجاوز قوائم أسعار مبيعات المشروع</span><span class="sxs-lookup"><span data-stu-id="1087e-103">Override project sales price lists</span></span>

<span data-ttu-id="1087e-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="1087e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="customer-specific-project-price-lists"></a><span data-ttu-id="1087e-105">قوائم أسعار مشروع خاصة بالعميل</span><span class="sxs-lookup"><span data-stu-id="1087e-105">Customer-specific project price lists</span></span>

<span data-ttu-id="1087e-106">يمكن إعداد اتفاقيات الأسعار الخاصة بالعميل كقوائم أسعار مشروع في سجل حساب في Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="1087e-106">Customer-specific price agreements can be set up as project price lists on an account record in Dynamics 365 Project Operations.</span></span>

<span data-ttu-id="1087e-107">لإعداد قائمه أسعار المشروع الخاصة بالعميل، في منطقة **المبيعات**، انتقل إلى سجل الحساب.</span><span class="sxs-lookup"><span data-stu-id="1087e-107">To set up a customer-specific project price list, in the **Sales** area, navigate to the account record.</span></span>

1. <span data-ttu-id="1087e-108">افتح صفحة قائمة **الحسابات**.</span><span class="sxs-lookup"><span data-stu-id="1087e-108">Open the **Accounts** list page.</span></span>
2. <span data-ttu-id="1087e-109">حدد موقع سجل عميل وانقر فوقه نقرًا مزدوجًا لفتح صفحة تفاصيل **الحساب**.</span><span class="sxs-lookup"><span data-stu-id="1087e-109">Locate and double-click a customer record to open the **Account** details page.</span></span>
3. <span data-ttu-id="1087e-110">على علامة التبويب **قوائم أسعار المشروع**، حدد **+ قائمة أسعار مشروع جديدة**.</span><span class="sxs-lookup"><span data-stu-id="1087e-110">On the **Project Price lists** tab, select **+ New Project Price List**.</span></span>
4. <span data-ttu-id="1087e-111">من صفحة **قائمة أسعار مشروع جديدة**، حدد قائمة أسعار من القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="1087e-111">On the **New Project Price List** page, select a price list from the drop-down.</span></span> <span data-ttu-id="1087e-112">يتم تضمين فقط قوائم الأسعار التي تم تعيين السياق فيها إلى **المبيعات** والتي تتطابق عملتها مع عملة الحساب.</span><span class="sxs-lookup"><span data-stu-id="1087e-112">Only price lists that have the context set to **Sales** and whose currency matches the account currency are included.</span></span>
5. <span data-ttu-id="1087e-113">أدخل اسمًا للاقتران، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="1087e-113">Name the association, and then select **Save**.</span></span> <span data-ttu-id="1087e-114">يتم إنشاء قائمة أسعار مشروع خاصة بالعميل.</span><span class="sxs-lookup"><span data-stu-id="1087e-114">A customer-specific project price list is created.</span></span> <span data-ttu-id="1087e-115">سيتم استخدام قائمة الأسعار هذه لتعيين أسعار المشروع بشكل افتراضي إلى عروض أسعار المشروع أو العقود التي تم إنشاؤها لهذا العميل حيث تاريخ إنشاء عرض الاسعار أو عقد المشروع يقع ضمن سريان تاريخ قائمة الأسعار.</span><span class="sxs-lookup"><span data-stu-id="1087e-115">This price list will be used to default project prices on project quotes or contracts created for this customer where the created date of the quote or project contract falls within the date effectivity of the price list.</span></span>

## <a name="custom-pricing-on-project-quotes"></a><span data-ttu-id="1087e-116">التسعير المخصص في عروض أسعار المشروع</span><span class="sxs-lookup"><span data-stu-id="1087e-116">Custom pricing on project quotes</span></span>

<span data-ttu-id="1087e-117">في عروض أسعار المشروع، يوجد تسعير مشروع يبدأ بقائمة أسعار قياسية افتراضية تم تعيينها بشكل افتراضي من معلمات العميل أو من معلمات المشروع.</span><span class="sxs-lookup"><span data-stu-id="1087e-117">On project quotes, you can have project pricing that starts with a default standard price list that defaults from the customer or from the project parameters.</span></span>

<span data-ttu-id="1087e-118">عندما تحتاج إلى تسعير مخصص للعمل المرتبط بالمشروع في عرض أسعار معين، يمكنك الحصول عليه من الكيان المقترن لقوائم أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="1087e-118">When you need custom pricing for project-related work on a particular quote, you can get that from the project price lists associated entity.</span></span>

<span data-ttu-id="1087e-119">أكمل الخطوات التالية لإعداد تسعير المشروع الخاص بعرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="1087e-119">Complete the following steps to set up quote-specific project pricing.</span></span>

1. <span data-ttu-id="1087e-120">افتح عرض أسعار المشروع، وحدد علامة التبويب **قوائم أسعار المشروع**.</span><span class="sxs-lookup"><span data-stu-id="1087e-120">Open the project quote and select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="1087e-121">في الشبكة الفرعية، حدد **إنشاء تسعير مخصص**.</span><span class="sxs-lookup"><span data-stu-id="1087e-121">In the subgrid, select **Create custom pricing**.</span></span>

<span data-ttu-id="1087e-122">يتم نسخ كافة قوائم أسعار المشروع المرفقة بعرض الأسعار إلى قوائم أسعار جديدة.</span><span class="sxs-lookup"><span data-stu-id="1087e-122">All the project price lists that are attached to the quote are copied to new price lists.</span></span> <span data-ttu-id="1087e-123">تعكس أسماء قوائم الأسعار الجديدة اسم عرض الأسعار الذي يحتوي على طابع التاريخ والوقت الذي تم فيه إنشاء قوائم الأسعار هذه.</span><span class="sxs-lookup"><span data-stu-id="1087e-123">The names of the new price lists reflect the name of quote with a date-time stamp for when these price lists were created.</span></span>

<span data-ttu-id="1087e-124">يمكنك استخدام كل واحدة من قوائم الأسعار هذه وإجراء تحديثات لأسعار العمالة (سعر الدور) والمصروفات (سعر الفئة).</span><span class="sxs-lookup"><span data-stu-id="1087e-124">You can use each of those price lists and make updates to labor (role price) and expense (category price) prices.</span></span> <span data-ttu-id="1087e-125">ستنطبق هذه الأسعار فقط على عقد المشروع هذا.</span><span class="sxs-lookup"><span data-stu-id="1087e-125">These prices will only be applicable to this project quote.</span></span>

## <a name="price-lists-on-a-project-contract"></a><span data-ttu-id="1087e-126">قوائم الأسعار على عقد المشروع</span><span class="sxs-lookup"><span data-stu-id="1087e-126">Price lists on a project contract</span></span>

<span data-ttu-id="1087e-127">في عقد المشروع، يتم تعيين تسعير المشروع دائمًا بشكل افتراضي كقائمة أسعار مخصص مع اسم العقد وطابع تاريخ ووقت الإنشاء تم الحاقه بالاسم.</span><span class="sxs-lookup"><span data-stu-id="1087e-127">On a project contract, project pricing always defaults as a custom price list with the name of contract and the created date time stamp appended to the name.</span></span> <span data-ttu-id="1087e-128">هذا صواب سواء تم إنشاء العقد عند فوز عرض الأسعار أو تم إنشاء العقد من البداية.</span><span class="sxs-lookup"><span data-stu-id="1087e-128">This is true whether the contract was created when the quote was won or if the contract was created from scratch.</span></span> <span data-ttu-id="1087e-129">إذا لزم الأمر، يمكنك إزالة هذا الاقتران بقائمة الأسعار المخصصة وإقران قائمة أسعار قياسية بعقد المشروع بدلاً من ذلك.</span><span class="sxs-lookup"><span data-stu-id="1087e-129">If needed, you can remove this association to the custom price list and associate a standard price list to the project contract instead.</span></span>

<span data-ttu-id="1087e-130">عند إقران قائمة أسعار قياسية بقوائم أسعار المشروع في عرض الأسعار أو العقد، ستؤثر أي تغييرات يتم إدخالها على الأسعار في قائمة الأسعار على جميع عروض الأسعار والعقود التي تستخدم قائمة الأسعار.</span><span class="sxs-lookup"><span data-stu-id="1087e-130">When you associate a standard price list to the project price lists on quote or contract, any changes made to the prices in the price list will impact all quotes and contracts that use the price list.</span></span>
