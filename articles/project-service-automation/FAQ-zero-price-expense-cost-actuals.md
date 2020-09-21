---
title: لماذا يتم تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات؟
description: استكشاف الأخطاء وإصلاحها عند تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
ms.topic: article
ms.prod: Project Service
ms.technology: ''
ms.assetid: bc1ebc58-c733-4310-8435-572ed9a9fef9
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 3fb678822877a61d141de75aea29b7d5cdf292c4
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748647"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="f0f0a-103">لماذا يتم تعيين السعر إلى صفر بشكل افتراضي في القيم الفعلية لتكلفة المصروفات؟</span><span class="sxs-lookup"><span data-stu-id="f0f0a-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="f0f0a-104">تنطبق هذه الأسئلة المتداولة على القيم الفعلية للمصروفات حيث يتم تعيين فئة الحركة إلى "مصروفات" ونوع الحركة إلى "تكلفة".</span><span class="sxs-lookup"><span data-stu-id="f0f0a-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="f0f0a-105">استكشاف الأخطاء وإصلاحها في معدلات التكلفة على القيم الفعلية لتكلفة المصروفات</span><span class="sxs-lookup"><span data-stu-id="f0f0a-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="f0f0a-106">انتقل إلى إدخال المصروفات ذات الصلة وتأكد من وجود مبلغ في حقل إدخال المصروفات.</span><span class="sxs-lookup"><span data-stu-id="f0f0a-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="f0f0a-107">إذا لم يتم ملء حقل المبلغ في إدخال المصروفات الأصلي، فهذا يعني أنك عزلت المشكلة.</span><span class="sxs-lookup"><span data-stu-id="f0f0a-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="f0f0a-108">لحل هذه المشكلة، قم بإعادة إنشاء إدخال المصروفات مع مبلغ صالح ووافق عليه.</span><span class="sxs-lookup"><span data-stu-id="f0f0a-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
