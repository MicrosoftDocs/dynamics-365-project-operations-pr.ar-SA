---
title: لماذا يتم تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة الوقت؟
description: استكشاف الأخطاء وإصلاحها عند تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة الوقت.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 44d4952b77ac0a541cdf8e3e55f202c9209efdf4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070663"
---
# <a name="why-is-the-price-defaulting-to-zero-on-time-cost-actuals"></a><span data-ttu-id="47133-103">لماذا يتم تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة الوقت؟</span><span class="sxs-lookup"><span data-stu-id="47133-103">Why is the price defaulting to zero on time cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="47133-104">تنطبق هذه الأسئلة المتداولة على القيم الفعلية حيث يتم تعيين فئة الحركة إلى "وقت" ونوع الحركة إلى "تكلفة"‬.</span><span class="sxs-lookup"><span data-stu-id="47133-104">This FAQ applies to actuals where the transaction class is set to Time and transaction type is Cost.</span></span> <span data-ttu-id="47133-105">ستساعدك عمليات التحقق الثلاث التالية في استكشاف أسباب تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة الوقت وإصلاح المشكلة.</span><span class="sxs-lookup"><span data-stu-id="47133-105">The following three checks will help you troubleshoot why the price is defaulting to 0 on time cost actuals.</span></span>
 
## <a name="check-1-identify-the-cost-price-list-for-the-project"></a><span data-ttu-id="47133-106">عملية التحقق 1: تحديد قائمة أسعار التكلفة للمشروع</span><span class="sxs-lookup"><span data-stu-id="47133-106">Check 1: Identify the cost price list for the project</span></span>

<span data-ttu-id="47133-107">ابحث عن المشروع من حقل المشروع للقيم الفعلية ثم انتقل إلى صفحة المشروع.</span><span class="sxs-lookup"><span data-stu-id="47133-107">Find the project from the project field of the actual and then go to the project page.</span></span> <span data-ttu-id="47133-108">انقر فوق ارتباط الوحدة المتعاقدة‬ في الحقل.</span><span class="sxs-lookup"><span data-stu-id="47133-108">Click on the contracting unit link in the field.</span></span> <span data-ttu-id="47133-109">في صفحة "الوحدة المتعاقدة‬"، تحقق مما إذا كان لدى الوحدة المتعاقدة‬ قائمة أسعار في شبكة "قوائم أسعار التكلفة".</span><span class="sxs-lookup"><span data-stu-id="47133-109">On the Contracting Unit page, check if the contracting unit has a price list in the Cost Price Lists grid.</span></span>

<span data-ttu-id="47133-110">في حال وجود أكثر من قائمة أسعار واحدة، فهذا يعني أنك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="47133-110">If there is more than one price list, you have isolated the problem.</span></span> <span data-ttu-id="47133-111">تسمح لك Project Service بدعم قائمة أسعار واحدة فقط لكل وحدة تنظيمية.</span><span class="sxs-lookup"><span data-stu-id="47133-111">Project Service only supports one price list per organizational unit.</span></span> <span data-ttu-id="47133-112">قم بإزالة جميع قوائم الأسعار من هذا الكيان حتى الحصول على قائمة أسعار واحدة فقط مرفقة بشبكة "قوائم أسعار التكلفة" للوحدة التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="47133-112">Remove all prices lists from this entity until there is only one price list attached in the Cost Price Lists grid of the Organizational Unit.</span></span>

<span data-ttu-id="47133-113">وفي حال عدم وجود قوائم أسعار مرفقة بالوحدة التنظيمية"، فدوّن عملة الوحدة التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="47133-113">If there are no price lists attached to the Organizational Unit, make a note of the currency of the Organizational unit.</span></span> <span data-ttu-id="47133-114">انتقل إلى Project Service، ثم "المعلمات" وافتح علامة تبويب "قوائم الأسعار". تحقق من وجود أي قوائم أسعار تم فيها تعيين السياق إلى"تكلفة" وذات عملة تطابق عملة الوحدة التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="47133-114">Go to the Project Service and then Parameters and open the Price Lists tab. Check if there are any price lists with context set to Cost and currency that matches the currency of the Organizational Unit.</span></span>
 
<span data-ttu-id="47133-115">في حال عدم وجود قوائم أسعار تطابق هذه المعايير، فهذا يعني أنك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="47133-115">If there are no price lists that match that criteria, you have isolated the problem.</span></span> <span data-ttu-id="47133-116">تأكد من وجود قائمة أسعار واحدة على الأقل تم فيها تعيين السياق إلى"تكلفة" وذات عملة تطابق عملة الوحدة التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="47133-116">Make sure to have at least one price list whose context is set to Cost and whose currency matches the currency of the Organizational Unit.</span></span>

<span data-ttu-id="47133-117">في حال وجود أكثر من قائمة أسعار واحدة تطابق هذه المعايير، فتابع قراءة هذا المستند لإجراء المزيد من عمليات التحقق.</span><span class="sxs-lookup"><span data-stu-id="47133-117">If there is more than one price list that match that criteria, continue reading this document to make more checks.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-cost-actual"></a><span data-ttu-id="47133-118">عملية التحقق 2: هل هناك أي قائمة من قوائم الأسعار المحددة أعلاه صالحة للتاريخ المحدد للقيم الفعلية لتكلفة الوقت؟</span><span class="sxs-lookup"><span data-stu-id="47133-118">Check 2: Are any of the price lists identified above valid for the specific date of the time cost actual?</span></span>

<span data-ttu-id="47133-119">لكي تأخذ خدمة Project Service قائمة أسعار للسعر الافتراضي في الاعتبار، يجب أن تكون قائمة الأسعار هذه قابلة للتطبيق على التاريخ في القيم الفعلية لتكلفة الوقت.</span><span class="sxs-lookup"><span data-stu-id="47133-119">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the time cost actual.</span></span> <span data-ttu-id="47133-120">تحقق مما يلي لمعرفة ما إذا كانت قائمة (قوائم) الأسعار المحدد أعلاه قابلة للتطبيق:</span><span class="sxs-lookup"><span data-stu-id="47133-120">Check the following to see if the price list(s) identified above are applicable:</span></span>

- <span data-ttu-id="47133-121">ابدأ بالتحقق مما إذا كانت تواريخ البدء والانتهاء على علامة التبويب " عام" لقوائم الأسعار المرفقة غير فارغة.</span><span class="sxs-lookup"><span data-stu-id="47133-121">Check if the start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="47133-122">إذا كانت تواريخ البدء والانتهاء على قوائم الأسعار المحددة أعلاه فارغة، فهذا يعني أنك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="47133-122">If the start and end dates on price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="47133-123">دوّن ملاحظة بشأن حقل "تاريخ البدء" على القيم الفعلية لتكلفة الوقت، وتأكد من أن أيًا من الأسعار المحددة تنطبق لهذا التاريخ.</span><span class="sxs-lookup"><span data-stu-id="47133-123">Make a note of the start date field on your time cost actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="47133-124">على سبيل المثال، يجب أن يقع تاريخ القيم الفعلية لتكلفة الوقت بين تاريخي البدء والانتهاء على قائمة الأسعار.</span><span class="sxs-lookup"><span data-stu-id="47133-124">For example, the date of the time cost actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="47133-125">وفي حال عدم وجود قائمة أسعار تغطي هذا التاريخ على القيم الفعلية لتكلفة الوقت، فهذا يعني انك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="47133-125">If there is no price list that covers that date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="47133-126">قم بتعديل تاريخي البدء والانتهاء لقائمة الأسعار للتأكد من أن قائمة الأسعار تغطي تاريخ القيم الفعلية لتكلفة الوقت.</span><span class="sxs-lookup"><span data-stu-id="47133-126">Modify the start and end dates of the price list to ensure that the price list covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="47133-127">وفي حال وجود أكثر من قائمة أسعار واحدة تغطي التاريخ على القيم الفعلية لتكلفة الوقت، فهذا يعني انك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="47133-127">If there is more than one price list that covers the date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="47133-128">يمكنك تصحيح ذلك عن طريق تحرير تاريخي البدء والانتهاء لقائمة (قوائم) الأسعار للحصول على قائمة أسعار واحدة فقط تغطي تاريخ القيم الفعلية لتكلفة الوقت.</span><span class="sxs-lookup"><span data-stu-id="47133-128">You can fix this by editing the start and end dates of the price list(s) so that there is only one price list that covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="47133-129">في حال وجود قائمة أسعار واحدة فقط تغطي هذا التاريخ للقيم الفعلية لتكلفة الوقت، فانتقل إلى عملية التحقق التالية في المستند.</span><span class="sxs-lookup"><span data-stu-id="47133-129">If there is only one price list that covers that date of the time cost actual, move to the next check in the document.</span></span>
<span data-ttu-id="47133-130">بمجرد الانتهاء من إجراء الإصلاحات المطلوبة، يجب إعادة إنشاء إدخال وقت والموافقة عليه والتأكد من أن القيم الفعلية لتكلفة الوقت تعرض سعرًا صالحًا.</span><span class="sxs-lookup"><span data-stu-id="47133-130">Once you’ve done made the required fixes, recreate a time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-cost-actual"></a><span data-ttu-id="47133-131">عملية التحقق 3: هل يوجد سعر في قائمة الأسعار لأبعاد التسعير على القيم الفعلية لتكلفة الوقت؟</span><span class="sxs-lookup"><span data-stu-id="47133-131">Check 3: Is there a price in the price list for the pricing dimensions on the time cost actual?</span></span>

<span data-ttu-id="47133-132">إذا أكملت عمليتي التحقق 1 و2 بنجاح، يجب أن يكون لديك الآن قائمة أسعار واحدة فقط للمشروع تنطبق على تاريخ القيم الفعلية لتكلفة الوقت.</span><span class="sxs-lookup"><span data-stu-id="47133-132">If you have successfully completed Check 1 and Check 2, you should now have only one price list that is applicable for the date of the time cost actual.</span></span> <span data-ttu-id="47133-133">افتح قائمة الأسعار هذه، وانتقل إلى علامة التبويب "أسعار الأدوار". تأكد من وجود صف في الشبكة لأبعاد التسعير على القيم الفعلية لتكلفة الوقت.</span><span class="sxs-lookup"><span data-stu-id="47133-133">Open this Price List and go to the Role Prices tab. Make sure that there is a row in the grid for the pricing dimensions on the time cost actual.</span></span>

<span data-ttu-id="47133-134">في حال عدم وجود صف في شبكة أسعار الأدوار لأبعاد التسعير على القيم الفعلية لتكلفة الوقت، فهذا يعني أنك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="47133-134">If there is no row in the role price grid for the pricing dimensions on the time cost actual, then you have isolated the problem.</span></span> <span data-ttu-id="47133-135">أنشئ صفًا في شبكة أسعار الأدوار لشبكة التسعير على القيم الفعلية لتكلفة الوقت.</span><span class="sxs-lookup"><span data-stu-id="47133-135">Create a row in the Role prices grid for the pricing dimensions on your time cost actual.</span></span> <span data-ttu-id="47133-136">بمجرد الانتهاء من ذلك، يجب إعادة إنشاء إدخال الوقت والموافقة عليه والتأكد من أن القيم الفعلية لتكلفة الوقت تعرض سعرًا صالحًا.</span><span class="sxs-lookup"><span data-stu-id="47133-136">Once this is done, recreate time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>
 
<span data-ttu-id="47133-137">إذا لم تتمكن من رؤية سعر صالح على القيم الفعلية لتكلفة الوقت بعد تنفيذ عمليات التحقق الثلاث أعلاه، فيُرجى تسجيل تذكرة دعم.</span><span class="sxs-lookup"><span data-stu-id="47133-137">If you still don't see a valid price on your time cost actual after you’ve done the three checks above, please log a support ticket.</span></span>



