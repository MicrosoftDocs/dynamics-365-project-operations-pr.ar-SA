---
title: المفاهيم الأساسية لإدارة الموارد
description: يوفر هذا الموضوع معلومات حول وظائف إدارة الموارد في Microsoft Dynamics Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: a14f0ec328049d1b199201955c384df9fac61e39
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123857"
---
# <a name="resource-management-key-concepts"></a><span data-ttu-id="a8d84-103">المفاهيم الأساسية لإدارة الموارد</span><span class="sxs-lookup"><span data-stu-id="a8d84-103">Resource management key concepts</span></span>

<span data-ttu-id="a8d84-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="a8d84-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a8d84-105">وتعتبر الموارد الأصل الأكثر أهميةً في المؤسسة التي تستند إلى الخدمة.</span><span class="sxs-lookup"><span data-stu-id="a8d84-105">Resources are the most important asset of a service-based organization.</span></span> <span data-ttu-id="a8d84-106">تساعد إمكانية العثور على الموارد الصحيحة في الوقت المناسب وحجز هذه الموارد في المشاريع والاحتفاظ باستخدام الموارد المؤسسة على الوفاء بأهداف العائد وأهداف رضا العميل.</span><span class="sxs-lookup"><span data-stu-id="a8d84-106">The ability to find the right resources at the right time, book those resources on projects and keep them utilized, helps the organization meet revenue targets and customer satisfaction goals.</span></span> <span data-ttu-id="a8d84-107">يمكنك استخدام وظيفة تعيين موارد المشروع في Dynamics 365 Project Operations للقيام بالمهام التالية:</span><span class="sxs-lookup"><span data-stu-id="a8d84-107">You can use the project resourcing functionality in Dynamics 365 Project Operations to do the following tasks:</span></span>

- <span data-ttu-id="a8d84-108">تكوين فرق المشروع من خلال حجز الموارد المتوفرة والمؤهلة.</span><span class="sxs-lookup"><span data-stu-id="a8d84-108">Form project teams by booking available and qualified resources.</span></span>
- <span data-ttu-id="a8d84-109">إنشاء سجلات أعضاء الفريق العامة وتعريف الأدوار والوحدة التنظيمية للمورد.</span><span class="sxs-lookup"><span data-stu-id="a8d84-109">Create generic team member records and define their roles and resource organization unit.</span></span>
- <span data-ttu-id="a8d84-110">إنشاء متطلبات الموارد لأعضاء الفريق العام من تعيينات المهام الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="a8d84-110">Generate resource requirements for generic team members from their task assignments.</span></span>
- <span data-ttu-id="a8d84-111">مطابقه المهارات من خلال تحديد المهارات المحددة في طلب المورد مقابل مهارات الموارد المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="a8d84-111">Match skills by identifying the skills defined on the resource demand against available resource skills.</span></span>
- <span data-ttu-id="a8d84-112">استبدال الموارد.</span><span class="sxs-lookup"><span data-stu-id="a8d84-112">Substitute resources.</span></span>
- <span data-ttu-id="a8d84-113">محاذاة تعيينات جدول المشروع وحجوزات الموارد.</span><span class="sxs-lookup"><span data-stu-id="a8d84-113">Align project schedule assignments and resource bookings.</span></span>
- <span data-ttu-id="a8d84-114">تسوية الفروق في الحجوزات والتعيينات.</span><span class="sxs-lookup"><span data-stu-id="a8d84-114">Reconcile differences in bookings and assignments.</span></span>
- <span data-ttu-id="a8d84-115">تغيير حجوزات الموارد كاستجابة لحالة خارج المكتب.</span><span class="sxs-lookup"><span data-stu-id="a8d84-115">Change resource bookings in response to out-of-office status.</span></span>
- <span data-ttu-id="a8d84-116">التعاون بين مديري المشاريع ومديري الموارد.</span><span class="sxs-lookup"><span data-stu-id="a8d84-116">Collaborate between project managers and resource managers.</span></span>
- <span data-ttu-id="a8d84-117">عرض محفوظات استخدام الموارد مقابل هدف، بما في ذلك تصنيف لكيفية استهلاك وقت الموارد.</span><span class="sxs-lookup"><span data-stu-id="a8d84-117">View the history of resource utilization against a target, including a breakdown of how the resources' time was utilized.</span></span>
- <span data-ttu-id="a8d84-118">صيانة مستودع مهارات وكفاءة.</span><span class="sxs-lookup"><span data-stu-id="a8d84-118">Maintain a skills and proficiency repository.</span></span>


<span data-ttu-id="a8d84-119">يمكنك توظيف الأفراد في المشروع الخاص بك من فريق من الموارد العامة أو المسماة في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a8d84-119">You can staff your project with a team of generic or named resources in Project Operations.</span></span> <span data-ttu-id="a8d84-120">يمكنك استخدام العديد من الطرق لإضافة أعضاء الفريق وتعيينهم ولإدارة الحجوزات والتعيينات الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="a8d84-120">You can use various methods to add and assign team members and to manage their bookings and assignments.</span></span> 
