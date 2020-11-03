---
title: نظرة عامة على الموافقات
description: يقدم هذا الموضوع معلومات حول العمل مع الموافقات في Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 37994422e9146765076fdbb77f5c763b4f1d0802
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070504"
---
# <a name="approvals-overview"></a><span data-ttu-id="9ac70-103">نظرة عامة على الموافقات</span><span class="sxs-lookup"><span data-stu-id="9ac70-103">Approvals overview</span></span>

<span data-ttu-id="9ac70-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="9ac70-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9ac70-105">يتم نقل عمليات إرسال الوقت والمصروفات عبر سير عمل الموافقة.</span><span class="sxs-lookup"><span data-stu-id="9ac70-105">Time and Expense submissions move through an approval workflow.</span></span> <span data-ttu-id="9ac70-106">بعد الموافقة على الإدخالات، يتم تسجيل الحركات في القيم الفعلية أو الوقت المحجوز في الجدول.</span><span class="sxs-lookup"><span data-stu-id="9ac70-106">After the entries are approved, transactions are recorded in actuals or time is booked in the schedule.</span></span>

## <a name="approvals-workflow"></a><span data-ttu-id="9ac70-107">سير عمل الموافقات</span><span class="sxs-lookup"><span data-stu-id="9ac70-107">Approvals workflow</span></span>
<span data-ttu-id="9ac70-108">عند إنشاء إدخال وقت أو مصروفات وإرساله، يتم إنشاء إدخال الموافقة.</span><span class="sxs-lookup"><span data-stu-id="9ac70-108">When you create and submit a time or expense entry, an approval entry is created.</span></span> <span data-ttu-id="9ac70-109">يقوم الموافق على المشروع أو المدير بمراجعة إدخالك والموافقة عليه.</span><span class="sxs-lookup"><span data-stu-id="9ac70-109">The Project approver or your manager reviews and approves your entry.</span></span> <span data-ttu-id="9ac70-110">إذا كان الإدخال يتعلق بمشروع، فسيتم إنشاء القيم الفعلية عند الموافقة عليه.</span><span class="sxs-lookup"><span data-stu-id="9ac70-110">If the entry is related to a project, when it's approved, the actuals will be created.</span></span> <span data-ttu-id="9ac70-111">يتيح لك ذلك تعقب التكلفة والفوترة.</span><span class="sxs-lookup"><span data-stu-id="9ac70-111">This allows the cost and billing to be tracked.</span></span> 

## <a name="approve-an-entry"></a><span data-ttu-id="9ac70-112">الموافقة على إدخال</span><span class="sxs-lookup"><span data-stu-id="9ac70-112">Approve an entry</span></span>
<span data-ttu-id="9ac70-113">يسمح لك نموذج **الموافقات** بالتبديل بين طرق العرض المختلفة حتى تتمكن من عرض أنواع الموافقات المختلفة.</span><span class="sxs-lookup"><span data-stu-id="9ac70-113">The **Approvals** form allows you to switch between different views so that you can view the different types of approvals.</span></span>
  
1. <span data-ttu-id="9ac70-114">انتقل إلى نموذج **الموافقات** ، وحدد **المصروفات** أو **الوقت** أو **الاستدعاءات**.</span><span class="sxs-lookup"><span data-stu-id="9ac70-114">Go to the **Approvals** form and select **Expenses** , **Time** , or **Recalls**.</span></span>
2. <span data-ttu-id="9ac70-115">راجع كل موافقة، وحدد تلك التي تريد الموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="9ac70-115">Review each approval, and select the ones you want to approve.</span></span>
3. <span data-ttu-id="9ac70-116">حدد **موافقة** للموافقة على الإدخالات المحددة.</span><span class="sxs-lookup"><span data-stu-id="9ac70-116">Select **Approve** to approve the selected entries.</span></span>
<span data-ttu-id="9ac70-117">يعالج النظام هذه الإدخالات وينشئ القيم الفعلية أو الحجز.</span><span class="sxs-lookup"><span data-stu-id="9ac70-117">The system will process these entries and create actuals or a booking.</span></span>

## <a name="reject-an-entry"></a><span data-ttu-id="9ac70-118">رفض إدخال</span><span class="sxs-lookup"><span data-stu-id="9ac70-118">Reject an entry</span></span>
<span data-ttu-id="9ac70-119">بصفتك الموافق على المشروع، قد تحتاج إلى إعادة إرسال أحد الإدخال إلى المستخدم كي يصححه.</span><span class="sxs-lookup"><span data-stu-id="9ac70-119">As the Project approver, you may have to send an entry back to a user for correction.</span></span>
  
1. <span data-ttu-id="9ac70-120">انتقل إلى نموذج **الموافقات** وحدد الإدخال الذي يجب رفضه.</span><span class="sxs-lookup"><span data-stu-id="9ac70-120">Go to the **Approvals** form and select the entry to reject.</span></span> 
2. <span data-ttu-id="9ac70-121">حدد **رفض**.</span><span class="sxs-lookup"><span data-stu-id="9ac70-121">Select **Reject**.</span></span>
3. <span data-ttu-id="9ac70-122">اختياري - أضف تعليقًا في مربع الحوار **تعليقات الرفض** لإعلام المستخدم بسبب رفض الإدخال.</span><span class="sxs-lookup"><span data-stu-id="9ac70-122">Optional - Add a comment in the **Rejection Comments** dialog to inform the user why the entry is being rejected.</span></span>
4. <span data-ttu-id="9ac70-123">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="9ac70-123">Select **OK**.</span></span> <span data-ttu-id="9ac70-124">سيتم إرجاع الإدخال إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="9ac70-124">The entry will be returned to the user.</span></span>
  
## <a name="recall-entries"></a><span data-ttu-id="9ac70-125">استدعاء الإدخالات</span><span class="sxs-lookup"><span data-stu-id="9ac70-125">Recall entries</span></span>
<span data-ttu-id="9ac70-126">في مرحلة ما، قد تحتاج إلى استدعاء إدخال تم إرساله.</span><span class="sxs-lookup"><span data-stu-id="9ac70-126">At some point, you might need to recall a submitted entry.</span></span> <span data-ttu-id="9ac70-127">إذا لم تتم الموافقة على الإدخال، سيتم إرجاعه على الفور.</span><span class="sxs-lookup"><span data-stu-id="9ac70-127">If the entry has not been approved, it will be returned immediately.</span></span> <span data-ttu-id="9ac70-128">ومع ذلك، فإن الإدخال الموافق عليه قد يكون ذا تأثير مادي.</span><span class="sxs-lookup"><span data-stu-id="9ac70-128">An approved entry however, may have a material impact.</span></span> <span data-ttu-id="9ac70-129">يجب على الموافق على المشروع الموافقة على الاستدعاء لإلغاء المعاملة في القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="9ac70-129">The Project approver is required to approve the recall in order to reverse the transaction in Actuals.</span></span>

## <a name="specify-project-approvers"></a><span data-ttu-id="9ac70-130">تحديد الموافقين على المشروع</span><span class="sxs-lookup"><span data-stu-id="9ac70-130">Specify Project approvers</span></span>
<span data-ttu-id="9ac70-131">يحتوي كل مشروع على عدد من أعضاء فريق المشروع.</span><span class="sxs-lookup"><span data-stu-id="9ac70-131">Each project has a number of project team members.</span></span> <span data-ttu-id="9ac70-132">يمكنك تحديد أعضاء الفريق الذين يؤدون أيضًا دور الموافقين على المشروع.</span><span class="sxs-lookup"><span data-stu-id="9ac70-132">You can specify which team members are also Project approvers.</span></span>

1. <span data-ttu-id="9ac70-133">انتقل إلى نموذج **المشاريع** وفتح المشروع من القائمة.</span><span class="sxs-lookup"><span data-stu-id="9ac70-133">Go to the **Projects** form and open the project from the list.</span></span>
2. <span data-ttu-id="9ac70-134">في علامة التبويب **فريق** ، حدد عضو الفريق الذي سيكون الموافق على المشروع، ثم حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="9ac70-134">On the **Team** tab, select the team member who will be a Project approver and then select **Edit**.</span></span>
3. <span data-ttu-id="9ac70-135">عيّن حقل **الموافق على المشروع** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9ac70-135">Set the **Project Approver** field to **Yes**.</span></span>
4. <span data-ttu-id="9ac70-136">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9ac70-136">Select **Save**.</span></span>
5. <span data-ttu-id="9ac70-137">كرر الخطوتين 2 و4 لإضافة المزيد من الموافقين على المشروع.</span><span class="sxs-lookup"><span data-stu-id="9ac70-137">Repeat steps 2-4 to add additional Project approvers.</span></span>

## <a name="configure-the-users-manager"></a><span data-ttu-id="9ac70-138">تكوين مدير المستخدم</span><span class="sxs-lookup"><span data-stu-id="9ac70-138">Configure the user's manager</span></span>

1. <span data-ttu-id="9ac70-139">انتقل إلى **الإعدادات** > **الأمان** > **المستخدمون**.</span><span class="sxs-lookup"><span data-stu-id="9ac70-139">Go to **Settings** > **Security** > **Users**.</span></span>
2. <span data-ttu-id="9ac70-140">حدد المستخدم الذي تقوم بتعيين مدير له وفي منطقة **معلومات المؤسسة** ، حدد المدير من القائمة.</span><span class="sxs-lookup"><span data-stu-id="9ac70-140">Select the user to whom you are assigning a manager and in the **Organization Information** area, select the manager from the list.</span></span> 
3. <span data-ttu-id="9ac70-141">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9ac70-141">Select **Save**.</span></span>


