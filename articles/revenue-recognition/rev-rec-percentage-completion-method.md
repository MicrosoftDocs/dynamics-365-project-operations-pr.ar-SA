---
title: مشاريع تقدير الإيرادات ثابتة السعر
description: يوفر هذا الموضوع معلومات حول عائد السعر الثابت في المشاريع.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 80fe1d4171d80ca39e8b7ebb1eefaa524a4f2b07
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531342"
---
# <a name="fixed-price-revenue-estimate-projects"></a><span data-ttu-id="6f898-103">مشاريع تقدير الإيرادات ثابتة السعر</span><span class="sxs-lookup"><span data-stu-id="6f898-103">Fixed price revenue estimate projects</span></span> 

<span data-ttu-id="6f898-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="6f898-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="6f898-105">عند إنشاء بند عقد مشروع باستخدام السمات التالية في Dynamics 365 Project Operations في Microsoft Dataverse، يقوم النظام تلقائيا بإنشاء مشروع تقديري لإيراد السعر الثابت.</span><span class="sxs-lookup"><span data-stu-id="6f898-105">When you create a project contract line with the following attributes in Dynamics 365 Project Operations on Microsoft Dataverse, the system automatically creates a fixed price revenue estimate project.</span></span> <span data-ttu-id="6f898-106">تعتمد المعلومات الموجودة في هذا المشروع علي ما يلي:</span><span class="sxs-lookup"><span data-stu-id="6f898-106">The information in this project is based on the following:</span></span>

  - <span data-ttu-id="6f898-107">طريقة فوترة بسعر ثابت.</span><span class="sxs-lookup"><span data-stu-id="6f898-107">A fixed price billing method.</span></span>
  - <span data-ttu-id="6f898-108">مشروع مقترن.</span><span class="sxs-lookup"><span data-stu-id="6f898-108">An associated project.</span></span>
  - <span data-ttu-id="6f898-109">تم تحديد حدث رئيسي واحد على الأقل في علامة التبويب **جدولة الفواتير** في صفحة **شروط تعاقد المشروع**.</span><span class="sxs-lookup"><span data-stu-id="6f898-109">At least one milestone defined on the **Invoice schedule** tab on the **Project contract line** page.</span></span>

## <a name="review-fixed-price-revenue-estimates-projects"></a><span data-ttu-id="6f898-110">مراجعة المشاريع المقدرة بإيرادات السعر الثابت</span><span class="sxs-lookup"><span data-stu-id="6f898-110">Review fixed price revenue estimates projects</span></span>
<span data-ttu-id="6f898-111">لمراجعه المشروعات المقدرة لإيرادات الأسعار الثابتة، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="6f898-111">To review fixed price revenue estimates projects, complete the following steps:</span></span>

1. <span data-ttu-id="6f898-112">في بيئة Dynamics 365 Finance، انتقل إلى **إدارة المشاريع والمحاسبة** > **المشاريع** > **مشاريع تقدير الإيرادات ثابتة السعر‬**.</span><span class="sxs-lookup"><span data-stu-id="6f898-112">In the Dynamics 365 Finance environment, go to **Projects management and accounting** > **Projects** > **Fixed price revenue estimate projects**.</span></span>
2. <span data-ttu-id="6f898-113">حدد المشروع الذي ترغب في عرضه ثم انقر نقرا مزدوجا فوق **معرف مشروع التقدير** لفتح السجل ومراجعه تفاصيل المشروع.</span><span class="sxs-lookup"><span data-stu-id="6f898-113">Select the project that you want to view and double-click the **Estimate project ID** to open the record and review the details of the project.</span></span>
3. <span data-ttu-id="6f898-114">قم بتوسيع علامة التبويب **المشروع**. ستري مشروعا واحدا في شبكة **المشاريع المحددة**.</span><span class="sxs-lookup"><span data-stu-id="6f898-114">Expand the **Project** tab. You will see one project in the **Selected projects** grid.</span></span> <span data-ttu-id="6f898-115">يستخدم النظام هذا كمشروع افتراضي لأنه المشروع المقترن بسطر عقد المشروع.</span><span class="sxs-lookup"><span data-stu-id="6f898-115">The system uses this as default project because it is the project associated to the project contract line.</span></span> 
4. <span data-ttu-id="6f898-116">لتغيير الاقتران، قم بتحديد المشاريع الاضافيه وإضافتها إلى شبكة **المشاريع المحددة**.</span><span class="sxs-lookup"><span data-stu-id="6f898-116">To change the association, select additional projects and add them to the **Selected projects** grid.</span></span> <span data-ttu-id="6f898-117">إذا تم تحديد عدة مشاريع في هذه الشبكة، فسيتم حساب النسبة المئوية لإكمال المشروع وتقديرات الإيرادات معًا لكل المشاريع المحددة.</span><span class="sxs-lookup"><span data-stu-id="6f898-117">If multiple projects are selected in this grid, the project percentage completion and revenue estimates are calculated together for of the all selected projects.</span></span>

  <span data-ttu-id="6f898-118">يمكن تعيين تكلفة المشروع وملف تعريف الإيرادات ونموذج التكلفة ورمز الفترة يدويًا.</span><span class="sxs-lookup"><span data-stu-id="6f898-118">Project cost, revenue profile, cost template, and the period code can be set manually.</span></span> <span data-ttu-id="6f898-119">إذا لم يتم تعيينها يدويًا، فإن القيم الافتراضية أثناء حساب التقدير الأول للمشروع باستخدام القواعد المكونة لملفات تعريف الإيرادات وتكلفة المشروع.</span><span class="sxs-lookup"><span data-stu-id="6f898-119">If they aren't set manually, the values default during the first estimate calculation for the project using the rules configured for project cost and revenue profiles.</span></span>

