---
title: نظرة عامة على المصروفات
description: يوفر هذا الموضوع معلومات حول وظيفة المصروفات في Project Operations.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: c4e2f441e1c4b1bcba5bca292b8075b4334a004d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276557"
---
# <a name="expense-home-page"></a><span data-ttu-id="e84d8-103">الصفحة الرئيسية للمصروفات</span><span class="sxs-lookup"><span data-stu-id="e84d8-103">Expense home page</span></span>

<span data-ttu-id="e84d8-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="e84d8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="e84d8-105">يدعم Dynamics 365 Project Operations إمكانية معالجة المصاريف.</span><span class="sxs-lookup"><span data-stu-id="e84d8-105">Dynamics 365 Project Operations supports the ability to process expenses.</span></span> <span data-ttu-id="e84d8-106">تحدث معالجة المصروفات مع أو بدون مشاريع باستخدام سير عمل قابل للتخصيص للسياسات وفئات الحركات وعمليات الموافقة.</span><span class="sxs-lookup"><span data-stu-id="e84d8-106">Expense processing occurs with or without projects by using a customizable workflow of policies, transaction categories, and approvals.</span></span>

<span data-ttu-id="e84d8-107">في Project Operations، هناك نموذجا نشر مدعومان للمصروفات:</span><span class="sxs-lookup"><span data-stu-id="e84d8-107">In Project Operations, there are two supported deployment models for Expense:</span></span> 

- <span data-ttu-id="e84d8-108">**كامل**: يتوفر النشر الكامل لـ **Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬** أو **Project Operations للسيناريوهات المستندة إلى الإنتاج‬**.</span><span class="sxs-lookup"><span data-stu-id="e84d8-108">**Full**: Full deployment is available for **Project Operations for resource/non-stocked based scenarios** or **Project Operations for production order-based scenarios**.</span></span>
- <span data-ttu-id="e84d8-109">**أساسي**: يتوفر النشر الأساسي لـ **Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة** و **النشر الخفيف – التعامل مع الفواتير الأولية**.</span><span class="sxs-lookup"><span data-stu-id="e84d8-109">**Basic**: Basic deployment is available for **Project Operations for resource/non-stocked based scenarios** and **Lite deployment – deal to proforma invoicing**.</span></span>

## <a name="full"></a><span data-ttu-id="e84d8-110">كامل</span><span class="sxs-lookup"><span data-stu-id="e84d8-110">Full</span></span> 
<span data-ttu-id="e84d8-111">يوفر نشر المصروفات الكاملة تطبيق سياسة تامة تشمل القدرة على إنشاء سياسات، مثل:</span><span class="sxs-lookup"><span data-stu-id="e84d8-111">Full Expense deployment provides a complete policy enforcement that includes the ability to create policies, such as:</span></span>

  - <span data-ttu-id="e84d8-112">حدود فئة المصروفات</span><span class="sxs-lookup"><span data-stu-id="e84d8-112">Expense category limits</span></span>
  - <span data-ttu-id="e84d8-113">السفر</span><span class="sxs-lookup"><span data-stu-id="e84d8-113">Travel</span></span>
  - <span data-ttu-id="e84d8-114">مصروف يومي</span><span class="sxs-lookup"><span data-stu-id="e84d8-114">Per diem</span></span>
  - <span data-ttu-id="e84d8-115">استيراد بطاقات الائتمان</span><span class="sxs-lookup"><span data-stu-id="e84d8-115">Credit card imports</span></span>
  - <span data-ttu-id="e84d8-116">التعرف البصري على الأحرف في الإيصالات</span><span class="sxs-lookup"><span data-stu-id="e84d8-116">Receipt optical character recognition</span></span>

## <a name="basic"></a><span data-ttu-id="e84d8-117">أساسي</span><span class="sxs-lookup"><span data-stu-id="e84d8-117">Basic</span></span> 
<span data-ttu-id="e84d8-118">يتيح لك سيناريو نشر المصروفات الأساسي فقط تسجيل المصروفات الأساسية في مقابل مشروع.</span><span class="sxs-lookup"><span data-stu-id="e84d8-118">Basic Expense deployment scenario only allows you to record basic expenses against a project.</span></span> 

<span data-ttu-id="e84d8-119">لمزيد من المعلومات، راجع [إدخال المصروفات (خفيف)](basic-expense.md)</span><span class="sxs-lookup"><span data-stu-id="e84d8-119">For more information, see [Expense entry (lite)](basic-expense.md)</span></span>

## <a name="determine-your-expense-deployment"></a><span data-ttu-id="e84d8-120">تحديد نشر المصروفات</span><span class="sxs-lookup"><span data-stu-id="e84d8-120">Determine your Expense deployment</span></span>
<span data-ttu-id="e84d8-121">لتحديد ما إذا كنت تقوم بتشغيل نشر إدارة المصروفات الأساسية، تأكد من أن عنوان URL ينتهي بـ **.crm.dynamics.com**.</span><span class="sxs-lookup"><span data-stu-id="e84d8-121">To determine if you're running the Basic Expense management deployment, verify that the address URL ends with **.crm.dynamics.com**.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]