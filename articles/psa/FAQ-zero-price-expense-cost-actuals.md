---
title: لماذا يتم تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات؟
description: استكشاف الأخطاء وإصلاحها عند تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
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
ms.openlocfilehash: 9f4ff8a96250d675faeda3246c2d0a6c5bd83286
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070665"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="8e388-103">لماذا يتم تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="8e388-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8e388-104">تنطبق هذه الأسئلة المتداولة على القيم الفعلية للمصروفات حيث يتم تعيين فئة الحركة إلى "مصروفات" ونوع الحركة إلى "تكلفة".</span><span class="sxs-lookup"><span data-stu-id="8e388-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="8e388-105">استكشاف الأخطاء وإصلاحها في معدلات التكلفة على القيم الفعلية لتكلفة المصروفات</span><span class="sxs-lookup"><span data-stu-id="8e388-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="8e388-106">انتقل إلى إدخال المصروفات ذات الصلة وتأكد من وجود مبلغ في حقل إدخال المصروفات.</span><span class="sxs-lookup"><span data-stu-id="8e388-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="8e388-107">إذا لم يتم ملء حقل المبلغ في إدخال المصروفات الأصلي، فهذا يعني أنك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="8e388-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="8e388-108">لحل هذه المشكلة، قم بإعادة إنشاء إدخال المصروفات مع مبلغ صالح ووافق عليه.</span><span class="sxs-lookup"><span data-stu-id="8e388-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
