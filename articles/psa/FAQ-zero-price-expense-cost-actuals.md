---
title: لماذا يتم تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات؟
description: استكشاف الأخطاء وإصلاحها عند تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات.
author: rumant
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 306f169ee25d42ac3c9e63fa70956b9c50315829
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122102"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="3ba73-103">لماذا يتم تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="3ba73-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3ba73-104">تنطبق هذه الأسئلة المتداولة على القيم الفعلية للمصروفات حيث يتم تعيين فئة الحركة إلى "مصروفات" ونوع الحركة إلى "تكلفة".</span><span class="sxs-lookup"><span data-stu-id="3ba73-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="3ba73-105">استكشاف الأخطاء وإصلاحها في معدلات التكلفة على القيم الفعلية لتكلفة المصروفات</span><span class="sxs-lookup"><span data-stu-id="3ba73-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="3ba73-106">انتقل إلى إدخال المصروفات ذات الصلة وتأكد من وجود مبلغ في حقل إدخال المصروفات.</span><span class="sxs-lookup"><span data-stu-id="3ba73-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="3ba73-107">إذا لم يتم ملء حقل المبلغ في إدخال المصروفات الأصلي، فهذا يعني أنك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="3ba73-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="3ba73-108">لحل هذه المشكلة، قم بإعادة إنشاء إدخال المصروفات مع مبلغ صالح ووافق عليه.</span><span class="sxs-lookup"><span data-stu-id="3ba73-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
