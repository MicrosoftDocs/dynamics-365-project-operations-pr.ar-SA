---
title: تأكيد عقد مشروع
description: يوفر هذا الموضوع معلومات حول كيفية تأكيد عقد في Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d807d3631f40a93ec7dbd918b64c287fd4875c79
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273812"
---
# <a name="confirm-a-project-contract"></a><span data-ttu-id="df00c-103">تأكيد عقد مشروع</span><span class="sxs-lookup"><span data-stu-id="df00c-103">Confirm a project contract</span></span>

<span data-ttu-id="df00c-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="df00c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="df00c-105">بإمكان عقد المشروع في Dynamics 365 Project Operations أن يكون نشطًا مع السبب **مؤكد**، أو مغلقًا مع السبب **خاسر**.</span><span class="sxs-lookup"><span data-stu-id="df00c-105">A project contract in Dynamics 365 Project Operations can be active with a reason of **Confirmed**, or closed with a reason of **Lost**.</span></span> <span data-ttu-id="df00c-106">عند تأكيد عقد مشروع، يتم تحديث الحالة من **مسودة** إلى **نشط** وسبب الحالة هو **مؤكد**.</span><span class="sxs-lookup"><span data-stu-id="df00c-106">When you confirm a project contract, the status updates from **Draft** to **Active** and the status reason is **Confirmed**.</span></span> <span data-ttu-id="df00c-107">لا يمكن تحرير عقد نشط أو مغلق أو إعادة فتحه.</span><span class="sxs-lookup"><span data-stu-id="df00c-107">An active or closed contract can't be edited or reopened.</span></span> 

### <a name="financial-impact-of-confirming-a-project-contract"></a><span data-ttu-id="df00c-108">التأثير المالي لتأكيد عقد مشروع</span><span class="sxs-lookup"><span data-stu-id="df00c-108">Financial impact of confirming a project contract</span></span>

<span data-ttu-id="df00c-109">بعد تأكيد عقد المشروع، يعيد التطبيق حساب إغلاق التكاليف من خلال عكس القيم الفعلية للتكلفة القديمة وإعادة إنشاء قيم فعلية للتكلفة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="df00c-109">After a project contract is confirmed, the application recalculates the costs by reversing the older cost actuals and creating new cost actuals.</span></span> <span data-ttu-id="df00c-110">ستتم عندئذٍ معالجة القيم الفعلية للتكلفة الجديدة استنادا إلى أسلوب الفوترة لشرط تعاقد المشروع المقترن.</span><span class="sxs-lookup"><span data-stu-id="df00c-110">The new cost actuals are then processed based on the billing method of the associated project contract line.</span></span> <span data-ttu-id="df00c-111">إذا كانت القيم الفعلية للتكلفة تشير إلى شرط تعاقد الوقت والمواد، يعيد التطبيق إنشاء قيم فعلية للمبيعات غير المفوترة بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="df00c-111">If the cost actuals reference a Time and Material contract line, the application automatically re-creates corresponding unbilled sales actuals.</span></span> <span data-ttu-id="df00c-112">إذا كانت القيم الفعلية للتكلفة تشير إلى شرط تعاقد ثابت السعر، يتوقف التطبيق عن إعادة معالجة القيم الفعلية للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="df00c-112">If the cost actuals reference a Fixed Price contract line, the application stops reprocessing the cost actuals.</span></span>

<span data-ttu-id="df00c-113">يتم تقييم الحدود التي يجب عدم تجاوزها وإعداد الخضوع للرسوم والتسعير والتكلفة على القيم الفعلية، ويتم تحديثها كجزء من عملية التأكيد.</span><span class="sxs-lookup"><span data-stu-id="df00c-113">Not-to-exceed limits, chargeability setup, and pricing and costing on the actuals is evaluated and then updated as part of the confirmations process.</span></span>

## <a name="close-a-project-contract-as-lost"></a><span data-ttu-id="df00c-114">إغلاق عقد مشروع كخاسر</span><span class="sxs-lookup"><span data-stu-id="df00c-114">Close a project contract as lost</span></span>

<span data-ttu-id="df00c-115">عند إغلاق عقد مشروع كخاسر، يتم تحديث حالة العقد إلى **مغلق** وسبب الحالة هو **خاسر**.</span><span class="sxs-lookup"><span data-stu-id="df00c-115">When you close a project contract as lost, the contract status is updated to **Closed** and the status reason is **Lost**.</span></span> <span data-ttu-id="df00c-116">يصبح عقد المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="df00c-116">The project contract becomes read-only.</span></span> <span data-ttu-id="df00c-117">يتم توفير مربع حوار تأكيد قبل اكتمال التغييرات لأنه لا يمكنك إعادة فتح عقد مشروع مغلق.</span><span class="sxs-lookup"><span data-stu-id="df00c-117">A confirmation dialog is provided before the changes are complete because you can't reopen a closed project contract.</span></span>

<span data-ttu-id="df00c-118">إذا كان عقد المشروع الذي تم إغلاقه كخاسر يشير إلى مشروع على بنوده، توضع علامة أيضًا على هذا المشروع كمغلق.</span><span class="sxs-lookup"><span data-stu-id="df00c-118">If the project contract that is closed as lost references a project on its lines, that project is also marked as closed.</span></span> <span data-ttu-id="df00c-119">يتم إلغاء حجوزات الموارد من هذا اليوم.</span><span class="sxs-lookup"><span data-stu-id="df00c-119">Any resource bookings from that day forward are canceled.</span></span> <span data-ttu-id="df00c-120">سيتم إلغاء أي قيم فعلية للمبيعات غير المفوترة على عقد المشروع غير الموجودة على فاتورة.</span><span class="sxs-lookup"><span data-stu-id="df00c-120">Any unbilled sales actuals on the project contract that aren't already on an invoice, will be reversed.</span></span>

> [!NOTE]
> <span data-ttu-id="df00c-121">في Dynamics 365 Project Operations، لن يؤثر إغلاق عقد مشروع كخاسر على حالة الفرصة المقترنة.</span><span class="sxs-lookup"><span data-stu-id="df00c-121">In Dynamics 365 Project Operations, closing a project contract as lost will not impact that status of the associated opportunity.</span></span> <span data-ttu-id="df00c-122">ستظل الفرصة مفتوحة ويجب إغلاقها يدويًا.</span><span class="sxs-lookup"><span data-stu-id="df00c-122">The opportunity will remain open and must be manually closed.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]