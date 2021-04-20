---
title: إلغاء تنشيط قوائم الأسعار
description: يشرح هذا الموضوع كيفية إزالة أو إلغاء تنشيط قوائم الأسعار القديمة أو غير المستخدمة.
author: rumant
manager: AnnBe
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Professional Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 3fa902e93815002be7d6915880cd7759dbbde5ef
ms.sourcegitcommit: 386921f44f1e9a8a828b140206d52945de07aee7
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2021
ms.locfileid: "5701902"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="6afc3-103">إلغاء تنشيط قوائم الأسعار</span><span class="sxs-lookup"><span data-stu-id="6afc3-103">Deactivate price lists</span></span> 

<span data-ttu-id="6afc3-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="6afc3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6afc3-105">لإزالة قوائم أسعار قديمة أو غير مستخدمة من Dynamics 365 Project Operations، هناك خطوتان يجب إكمالهما.</span><span class="sxs-lookup"><span data-stu-id="6afc3-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="6afc3-106">إزالة قائمة الأسعار أو حذفها من صفحات محددة.</span><span class="sxs-lookup"><span data-stu-id="6afc3-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="6afc3-107">إلغاء تنشيط قائمة الأسعار أو حذفها من قوائم الأسعار النشطة في صفحة **قوائم الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="6afc3-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="6afc3-108">يجب إكمال الخطوتين لإزالة قائمة أسعار بالكامل.</span><span class="sxs-lookup"><span data-stu-id="6afc3-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="6afc3-109">لا يُعد تنفيذ الخطوة 2 فقط، وهي حذف قائمة الأسعار أو إلغاء تنشيطها مباشرة من طريقة عرض قوائم الأسعار النشطة، كافيًا.</span><span class="sxs-lookup"><span data-stu-id="6afc3-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="6afc3-110">يجب عليك أيضًا حذف اقتران قائمة الأسعار هذه من جميع الأماكن المذكورة في الخطوة 1.</span><span class="sxs-lookup"><span data-stu-id="6afc3-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="6afc3-111">حذف قائمة الأسعار من صفحات محددة</span><span class="sxs-lookup"><span data-stu-id="6afc3-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="6afc3-112">لحذف قائمة أسعار من Project Operations، انتقل إلى الصفحات التالية:</span><span class="sxs-lookup"><span data-stu-id="6afc3-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="6afc3-113">صفحة **معلمات المشروع** > علامة تبويب **قوائم الأسعار**</span><span class="sxs-lookup"><span data-stu-id="6afc3-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="6afc3-114">صفحة **الوحدة التنظيمية‬** > شبكة **قوائم الأسعار**</span><span class="sxs-lookup"><span data-stu-id="6afc3-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="6afc3-115">صفحة **الحساب** > شبكة **قوائم أسعار المشروع**</span><span class="sxs-lookup"><span data-stu-id="6afc3-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="6afc3-116">صفحة **عروض أسعار المشروع** > شبكة **قوائم أسعار المشروع**: ينطبق هذا على جميع عروض أسعار المشروع.</span><span class="sxs-lookup"><span data-stu-id="6afc3-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="6afc3-117">صفحة **عقود المشروع** > شبكة **قوائم أسعار المشروع**: ينطبق هذا على جميع عقود المشروع النشطة.</span><span class="sxs-lookup"><span data-stu-id="6afc3-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="6afc3-118">بالنسبة لكل صفحة، حدد قائمة الأسعار التي تريد حذفها، ثم حدد **حذف**.</span><span class="sxs-lookup"><span data-stu-id="6afc3-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="6afc3-119">حذف قائمة الأسعار أو إلغاء تنشيطها من صفحة قوائم الأسعار</span><span class="sxs-lookup"><span data-stu-id="6afc3-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="6afc3-120">لحذف قائمة أسعار من قوائم الأسعار النشطة، انتقل إلى **المبيعات** > **العملاء** > **قوائم الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="6afc3-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="6afc3-121">حدد قائمة التي تريد حذفها، ثم حدد **حذف**.</span><span class="sxs-lookup"><span data-stu-id="6afc3-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="6afc3-122">إذا كانت قائمة الأسعار مشار إليها في أية حركات موجودة، فلن تتمكن من حذفها.</span><span class="sxs-lookup"><span data-stu-id="6afc3-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="6afc3-123">وإذا حدث ذلك، يمكنك إلغاء تنشيط قائمة الأسعار حتى لا تظهر في أية طرق عرض.</span><span class="sxs-lookup"><span data-stu-id="6afc3-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="6afc3-124">لإلغاء تنشيط قائمة الأسعار، حدد قائمة الأسعار مرة أخرى، ثم حدد **إلغاء تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="6afc3-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
