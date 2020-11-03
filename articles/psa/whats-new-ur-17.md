---
title: الجديد أو المتغير في إصدار التحديث 17، الإصدار 3 من Project Service Automation
description: يسرد هذا الموضوع الميزات والإصلاحات المتوفرة في الإصدار 3 من Project Service Automation، إصدار التحديث 12.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 7ba685568692dafe117de42a71bb14d391cd7cc4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070600"
---
# <a name="project-service-automation-update-release-17-v3"></a><span data-ttu-id="85ea3-103">الإصدار 3 من Project Service Automation، إصدار التحديث 17</span><span class="sxs-lookup"><span data-stu-id="85ea3-103">Project Service Automation Update Release 17, V3</span></span>

<span data-ttu-id="85ea3-104">يسرنا الإعلان عن التحديث الأخير لتطبيق Project Service Automation لـ Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="85ea3-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="85ea3-105">يتضمن هذا الإصدار بعض التحسينات الهامة من ناحية الجودة والأداء وقابلية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="85ea3-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="85ea3-106">هذا الإصدار متوافق مع Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="85ea3-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="85ea3-107">للتحديث إلى هذا الإصدار، قم بزيارة مركز إدارة Dynamics 365 online، ثم انتقل إلى صفحة الحلول لتثبيت التحديث.</span><span class="sxs-lookup"><span data-stu-id="85ea3-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="85ea3-108">لمزيد من المعلومات، راجع [تثبيت حل مفضل أو تحديثه أو إزالته](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="85ea3-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="85ea3-109">يسرد هذا الموضوع الميزات والإصلاحات الجديدة أو التي تم تغييرها في PSA V3، إصدار التحديث 17.</span><span class="sxs-lookup"><span data-stu-id="85ea3-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 17.</span></span> <span data-ttu-id="85ea3-110">يتضمن هذا الإصدار رقم البنية V3.10.6.34 وهو متوفر بشكل عام من خلال تحديث ذاتي في مارس 2020.</span><span class="sxs-lookup"><span data-stu-id="85ea3-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-17"></a><span data-ttu-id="85ea3-111">إصدار التحديث 17</span><span class="sxs-lookup"><span data-stu-id="85ea3-111">Update Release 17</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="85ea3-112">إصلاحات الأخطاء</span><span class="sxs-lookup"><span data-stu-id="85ea3-112">Bug fixes</span></span>

<span data-ttu-id="85ea3-113">**عام**</span><span class="sxs-lookup"><span data-stu-id="85ea3-113">**General**</span></span>

- <span data-ttu-id="85ea3-114">‏‫تم الإصلاح‬: تحديث Project Service Automation لفرض تراخيص Team Member (سيتضمن مركز موارد المشروع بيانات تعريف خطة خدمة Team Member 3.x)</span><span class="sxs-lookup"><span data-stu-id="85ea3-114">Fixed: Update Project Service Automation to enforce Team Member licenses (Project Resource Hub will include Team Member Service plan metadata 3.x)</span></span>
 
<span data-ttu-id="85ea3-115">**الوقت والمصروفات**</span><span class="sxs-lookup"><span data-stu-id="85ea3-115">**Time and Expense**</span></span>

- <span data-ttu-id="85ea3-116">تم الإصلاح: لا يمكن تغيير تقدير مصروفات من سعر غير صفري إلى صفر (0).</span><span class="sxs-lookup"><span data-stu-id="85ea3-116">Fixed: It is not possible to change an expense estimate from a non-zero price to zero (0).</span></span> <span data-ttu-id="85ea3-117">تم تجاهل التغيير.</span><span class="sxs-lookup"><span data-stu-id="85ea3-117">The change is ignored.</span></span>

<span data-ttu-id="85ea3-118">**إدارة المشروع**</span><span class="sxs-lookup"><span data-stu-id="85ea3-118">**Project Management**</span></span>

- <span data-ttu-id="85ea3-119">تم الإصلاح: تمت إضافة فحص القيم الفارغة على اسم منصب عضو الفريق.</span><span class="sxs-lookup"><span data-stu-id="85ea3-119">Fixed: A check for null values has been added on a team member's position name.</span></span>
- <span data-ttu-id="85ea3-120">تم الإصلاح: تم إهمال الحقل **msdyn_userresourceid** على الكيان **msdyn_resourceassignment**.</span><span class="sxs-lookup"><span data-stu-id="85ea3-120">Fixed: **msdyn_userresourceid** field on the **msdyn_resourceassignment** entity has been deprecated.</span></span>
- <span data-ttu-id="85ea3-121">تم الإصلاح: تعالج الآن الترقية من 2.x إلى 3.x حدود المجهود الفارغة على تعيينات المهام.</span><span class="sxs-lookup"><span data-stu-id="85ea3-121">Fixed: Upgrade from 2.x to 3.x now handles empty effort contours on task assignments.</span></span>

<span data-ttu-id="85ea3-122">**المبيعات**</span><span class="sxs-lookup"><span data-stu-id="85ea3-122">**Sales**</span></span>

- <span data-ttu-id="85ea3-123">تم الإصلاح: يعالج **Invoice.PreValidateInvoiceUpdate** الآن سيناريو إعادة تعيين مالكي السجلات بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="85ea3-123">Fixed: **Invoice.PreValidateInvoiceUpdate** now handles the scenario of reassigning record owners properly.</span></span>
- <span data-ttu-id="85ea3-124">تم الإصلاح: عندما تكون فئة المعاملة **الوقت** ، تكون **UnitGroup** غير قابلة للتحرير لجميع الكيانات، بما فيها **QuoteLineDetails** و **JournalLine** و **InvoiceLineDetail** و **ContractLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="85ea3-124">Fixed: When the transaction class is **Time** , **UnitGroup** is non-editable for all entities including, **QuoteLineDetails** , **JournalLine** , **InvoiceLineDetail** , and **ContractLineDetails**.</span></span> <span data-ttu-id="85ea3-125">ومع ذلك، فإن **الوحدة** غير قابلة للتحرير فقط لكل من **JournalLine** و **InvoiceLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="85ea3-125">However, **Unit** is non-editable only for **JournalLine** and **InvoiceLineDetails**.</span></span>


