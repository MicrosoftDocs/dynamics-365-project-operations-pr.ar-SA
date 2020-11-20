---
title: الحجوزات في مقابل التعيينات
description: يوفر هذا الموضوع معلومات حول الاختلافات بين حجوزات الموارد وتعيينات الموارد.
author: ruhercul
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8fe6937dfdfe137f28917c16da1d7dc6155284ae
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130202"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="ecf8b-103">الحجوزات في مقابل التعيينات</span><span class="sxs-lookup"><span data-stu-id="ecf8b-103">Bookings vs assignments</span></span>

<span data-ttu-id="ecf8b-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="ecf8b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ecf8b-105">الحجوزات هي تخصيص الموارد الثابت أو المبدئي لمشروع.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="ecf8b-106">تستهلك الحجوزات الثابتة سعة المورد.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="ecf8b-107">تمثل الحجوزات المفاهيم المؤسسية للفرق بحيث يمكنها أن تفهم كيفية تفاعل الموارد عبر العديد من المشاريع.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="ecf8b-108">يعتبر Dynamics 365 Project Operations الحجوزات بمثابة مفهوم على مستوى المشروع.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="ecf8b-109">بخلاف الحجوزات، التعيينات هي التزام الموارد بمهام المشروع في جدول المشروع.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="ecf8b-110">بإمكان الموارد أن تكون مسماة أو عامة.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-110">The resources can be named or generic.</span></span> 

<span data-ttu-id="ecf8b-111">وبشكل عام، سيكون مجموع الحجوزات لمورد مساويًا لمجموع تعيينات المورد عبر مهمة أو أكثر.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-111">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="ecf8b-112">ومع ذلك، لا يفرض Project Operations هذه الاتفاقية.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-112">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="ecf8b-113">تعرض طريقة عرض **التسوية** لمدير المشروع الأماكن حيث لا تتطابق حجوزات وتعيينات المورد.</span><span class="sxs-lookup"><span data-stu-id="ecf8b-113">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>
