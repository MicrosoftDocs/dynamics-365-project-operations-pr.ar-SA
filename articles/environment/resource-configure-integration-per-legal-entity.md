---
title: تكوين تكامل Project Operations لكل كيان قانوني
description: يقدم هذا الموضوع معلومات حول إعداد التكامل حسب الكيان القانوني في Project Operations.
author: sigitac
ms.date: 10/21/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e5a12de275a9f886434da45fbbed5140e3913d83
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000060"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a><span data-ttu-id="fef42-103">تكوين تكامل Project Operations لكل كيان قانوني</span><span class="sxs-lookup"><span data-stu-id="fef42-103">Configure Project Operations integration per legal entity</span></span> 

<span data-ttu-id="fef42-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="fef42-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="fef42-105">ينقلك هذا الموضع عبر الخطوات المطلوبة لتكوين Dynamics 365 Project Operations لكل كيان قانوني.</span><span class="sxs-lookup"><span data-stu-id="fef42-105">This topic walks you through the steps required to configure Dynamics 365 Project Operations per legal entity.</span></span>

## <a name="enable-feature-keys-in-dynamics-365-finance"></a><span data-ttu-id="fef42-106">تمكين مفاتيح الميزات في Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="fef42-106">Enable feature keys in Dynamics 365 Finance</span></span>

<span data-ttu-id="fef42-107">أكمل الخطوات التالية لتمكين الميزات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="fef42-107">Complete the following steps to enable required features.</span></span>

1. <span data-ttu-id="fef42-108">في Dynamics 365 Finance، انتقل إلى مساحة عمل **إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="fef42-108">In Dynamics 365 Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="fef42-109">في **قائمة الميزات**، ابحث عن الميزات التالية وقم بتمكينها:</span><span class="sxs-lookup"><span data-stu-id="fef42-109">In **Feature list**, find and enable the following features:</span></span>
  
    - <span data-ttu-id="fef42-110">**تمكين شروط تعاقد متعددة لمشروع**</span><span class="sxs-lookup"><span data-stu-id="fef42-110">**Enable multiple contract lines for a project**</span></span>
    - <span data-ttu-id="fef42-111">**تمكين Project Operations على Dynamics 365 Customer Engagement**</span><span class="sxs-lookup"><span data-stu-id="fef42-111">**Enable Project Operations on Dynamics 365 Customer Engagement**</span></span>

> [!NOTE]
> <span data-ttu-id="fef42-112">إذا لم تظهر **مفاتيح الميزات** مدرجة، فتحقق من ان إصدار Finance يفي بالحد الأدنى من متطلبات الإصدار (إصدار التطبيق 10.0.13 مع تطبيق جميع تحديثات الجودة أو إصدار أعلى).</span><span class="sxs-lookup"><span data-stu-id="fef42-112">If you don't see **Feature keys** listed, verify that your Finance version meets the minimum version requirement (application version 10.0.13 with all quality updates applied or higher).</span></span> <span data-ttu-id="fef42-113">حدد **التحقق من وجود تحديثات** لتحديث قائمة الميزات.</span><span class="sxs-lookup"><span data-stu-id="fef42-113">Select **Check for updates** to refresh the feature list.</span></span>

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a><span data-ttu-id="fef42-114">تعريف سيناريو نشر Project Operations لكيان قانوني</span><span class="sxs-lookup"><span data-stu-id="fef42-114">Define the Project Operations deployment scenario for a legal entity</span></span>

<span data-ttu-id="fef42-115">يمكنك تمكين Project Operations على Dynamics 365 Customer Engagement على مستوى الكيان القانوني.</span><span class="sxs-lookup"><span data-stu-id="fef42-115">You can enable Project Operations on Dynamics 365 Customer Engagement on a legal entity level.</span></span> <span data-ttu-id="fef42-116">يمكنك الحصول على كيان قانوني واحد يستخدم Project Operations على Dynamics 365 Customer Engagement للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬.</span><span class="sxs-lookup"><span data-stu-id="fef42-116">You can have one legal entity using Project Operations on Dynamics 365 Customer Engagement for resource/non-stocked based scenarios.</span></span> <span data-ttu-id="fef42-117">في نفس البيئة، يمكن أن يكون لديك كيان قانوني آخر يستخدم Project Operations لسيناريوهات المنتجات المخزنة/أوامر الإنتاج‬.</span><span class="sxs-lookup"><span data-stu-id="fef42-117">In the same environment, you can have another legal entity using Project Operations for stocked/production order scenarios.</span></span>

1. <span data-ttu-id="fef42-118">في Dynamics 365 Finance، انتقل إلى **إدارة المشاريع والمحاسبة** > **الإعداد‏‎** > **معلمات إدارة المشاريع والمحاسبة العمومية**.</span><span class="sxs-lookup"><span data-stu-id="fef42-118">In Dynamics 365 Finance, go to **Project management and accounting** > **Setup** > **Global project management and accounting parameters**.</span></span>
2. <span data-ttu-id="fef42-119">في قائمة الكيانات القانونية المتاحة، حدد الكيانات التي سيتم فيها تمكين العديد من شروط التعاقد وProject Operations على ميزات Dynamics 365 Customer Engagement.</span><span class="sxs-lookup"><span data-stu-id="fef42-119">In the list of available legal entities, select entities where multiple contract lines and Project Operations on Dynamics 365 Customer Engagement features will be enabled.</span></span> <span data-ttu-id="fef42-120">اترك الكيانات القانونية التي ستستخدم Project Operations لسيناريوهات المنتجات المخزنة/أوامر الإنتاج‬ من دون تحديدها.</span><span class="sxs-lookup"><span data-stu-id="fef42-120">Leave legal entities that will be using Project Operations for stocked/production order scenarios unselected.</span></span>

> [!NOTE]
> <span data-ttu-id="fef42-121">لا يمكن تحديد الكيان القانوني الا إذا لم يكن لديه أي مشاريع موجودة.</span><span class="sxs-lookup"><span data-stu-id="fef42-121">A legal entity can be selected only if it doesn't have any existing projects.</span></span>

## <a name="configure-project-management-and-accounting-parameters"></a><span data-ttu-id="fef42-122">تكوين معلمات إدارة المشاريع والمحاسبة</span><span class="sxs-lookup"><span data-stu-id="fef42-122">Configure Project management and accounting parameters</span></span>

<span data-ttu-id="fef42-123">يحتاج كل كيان قانوني يستخدم Project Operations على Dynamics 365 Customer Engagement إلى مجموعة من المعلمات الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="fef42-123">Each legal entity using Project Operations on Dynamics 365 Customer Engagement needs a set of default parameters.</span></span> <span data-ttu-id="fef42-124">يتم تكوين هذه المعلمات على علامة تبويب **Project Operations** في صفحة **معلمات إدارة المشاريع والمحاسبة‬**.</span><span class="sxs-lookup"><span data-stu-id="fef42-124">These parameters are configured on the **Project Operations** tab on the **Project management and accounting parameters** page.</span></span> <span data-ttu-id="fef42-125">المعلمات هي:</span><span class="sxs-lookup"><span data-stu-id="fef42-125">The parameters are:</span></span>

  - <span data-ttu-id="fef42-126">**الإعدادات الافتراضية لنوع الفوترة**: يستخدم Project Operations مجموعة ثابتة من الإعدادات الافتراضية لنوع الفوترة التي يجب تعيها إلى خصائص البنود في Finance.</span><span class="sxs-lookup"><span data-stu-id="fef42-126">**Billing type defaults**: Project Operations uses a fixed set of billing type defaults that must be mapped to line properties Finance.</span></span> <span data-ttu-id="fef42-127">أنشئ سجلاً لكل نوع فوترة: **غير محدد** و **خاضع للرسوم** و **غير خاضع للرسوم** و **تكميلي‬** و **غير متوفر**.</span><span class="sxs-lookup"><span data-stu-id="fef42-127">Create a record for each billing type: **Not specified**, **Chargeable**, **Non-chargeable**, **Complimentary**, and **Not available**.</span></span>
  - <span data-ttu-id="fef42-128">**الإعدادات الافتراضية لفئة المشروع**: حدد الإعدادات الافتراضية لفئة المشروع التي يجب استخدامها لكل نوع حركة.</span><span class="sxs-lookup"><span data-stu-id="fef42-128">**Project category defaults**: Select the default project categories to be used for each transaction type.</span></span> <span data-ttu-id="fef42-129">سيتم استخدام هذه الإعدادات الافتراضية في **دفتر يومية تكامل Project Operations** وفي التقديرات التي لم يتم فيها تحديد فئة مشروع للقيمة الفعلية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="fef42-129">These defaults will be used in the **Project Operations Integration journal** and in estimates where no transaction category is specified for the project actual.</span></span>
  - <span data-ttu-id="fef42-130">**التنبؤات**: حدد نموذج التنبؤ الذي سيتم استخدامه لتقديرات الوقت والمصروفات.</span><span class="sxs-lookup"><span data-stu-id="fef42-130">**Forecasts**: Select the forecast model to be used for time and expense estimates.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]