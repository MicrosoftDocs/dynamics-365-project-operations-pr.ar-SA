---
title: إدارة عقود المشروع
description: يقدم هذا الموضوع معلومات حول عرض العقود القائمة على المشروع.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 441fbc378a423334f45bc65658811ef238515393
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177315"
---
# <a name="manage-project-contracts"></a><span data-ttu-id="27fb1-103">إدارة عقود المشروع</span><span class="sxs-lookup"><span data-stu-id="27fb1-103">Manage project contracts</span></span>

<span data-ttu-id="27fb1-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="27fb1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="27fb1-105">تلتقط عقود المشروع في Dynamics 365 Project Operations وتدير تفاصيل الالتزامات والفوترة في مشروع والتي تم الاتفاق عليها بطريقة تعاقدية.</span><span class="sxs-lookup"><span data-stu-id="27fb1-105">Project contracts in Dynamics 365 Project Operations capture and manage the contractually agreed on commitments and billing details of a project.</span></span> <span data-ttu-id="27fb1-106">تم تخصيص بنية عقد المشروع في Project Operations للعمل القائم على المشروع مع المكونات التالية:</span><span class="sxs-lookup"><span data-stu-id="27fb1-106">The structure of a project contract in Project Operations is tailored to project-based work with the following components:</span></span>

- <span data-ttu-id="27fb1-107">شروط التعاقد التي تحدد مكونات العمل المنفصلة التي سيتم تقديمها كمكونات عالية المستوى على فاتورة مشروع.</span><span class="sxs-lookup"><span data-stu-id="27fb1-107">Contract lines that identify the discrete components of work that will be presented as high-level components on a project invoice.</span></span>
- <span data-ttu-id="27fb1-108">تفاصيل شروط التعاقد التي تحدد العمل وتقيّمه لكل مكون أو شرط تعاقد عالي المستوى.</span><span class="sxs-lookup"><span data-stu-id="27fb1-108">Contract line details that identify and estimate the work for each high-level component or contract line.</span></span> <span data-ttu-id="27fb1-109">يشتمل التقدير الجدول والجوانب المالية للعمل المرتبط بشروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="27fb1-109">The estimate includes the schedule and the financial aspects for the work tied to the contract line.</span></span>
- <span data-ttu-id="27fb1-110">تم إعداد نماذج للتعاقد والمكونات الخاضعة للرسوم لكل شرط تعاقد يحتفظ بترتيب الفوترة لكل شرط تعاقد والعقد الإجمالي.</span><span class="sxs-lookup"><span data-stu-id="27fb1-110">Contracting models and chargeable components are set up for each contract line that holds the billing arrangement for each contract line and the overall contract.</span></span>

## <a name="view-all-project-based-contracts"></a><span data-ttu-id="27fb1-111">عرض جميع العقود القائمة على المشروع</span><span class="sxs-lookup"><span data-stu-id="27fb1-111">View all project-based contracts</span></span>

<span data-ttu-id="27fb1-112">يمكن رؤية قائمة بكافة عقود المشروع في صفحة قائمة **العقود**.</span><span class="sxs-lookup"><span data-stu-id="27fb1-112">A list of all project contracts can be seen on the **Contracts** list page.</span></span> 

1. <span data-ttu-id="27fb1-113">انتقل إلى **المبيعات** > **العقود**.</span><span class="sxs-lookup"><span data-stu-id="27fb1-113">Go to **Sales** > **Contracts**.</span></span> <span data-ttu-id="27fb1-114">تظهر قائمة بكافة عقود المشروع في النظام.</span><span class="sxs-lookup"><span data-stu-id="27fb1-114">A list of all your project Contracts in the system are shown.</span></span> 
2. <span data-ttu-id="27fb1-115">حدد **مبدّل طريقة العرض** (سهم القائمة المنسدلة الموجود بجوار اسم طريقة العرض) لتحديد طرق عرض أخرى مصفاة.</span><span class="sxs-lookup"><span data-stu-id="27fb1-115">Select the **View switcher** (the drop-down arrow next to the name of the view) to select other filtered views.</span></span> <span data-ttu-id="27fb1-116">يمكنك إنشاء طرق عرض خاصة بك باستخدام معايير التصفية المخصصة.</span><span class="sxs-lookup"><span data-stu-id="27fb1-116">You can create your own views with custom filter criteria.</span></span>

<span data-ttu-id="27fb1-117">يمكن إنشاء العقود أو حذفها من صفحة القائمة هذه أو صفحات التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="27fb1-117">Contracts can be created or deleted from this list page or detail pages.</span></span>