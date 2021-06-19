---
title: تكوين المحاسبة للمشروعات الداخلية
description: يقدم هذا الموضوع معلومات حول كيفية إعداد ممارسات المحاسبة للمشاريع الداخلية في Project Operations.
author: sigitac
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ad8b974ef75cb0a4e43af0aa254cec1bbcab154a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012840"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="e86c5-103">تكوين المحاسبة للمشروعات الداخلية</span><span class="sxs-lookup"><span data-stu-id="e86c5-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="e86c5-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="e86c5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e86c5-105">تسمح المشاريع الداخلية للشركات بتعقب التكلفة ذات الصلة بالأنشطة التي لم تتم فوترتها على العميل.</span><span class="sxs-lookup"><span data-stu-id="e86c5-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="e86c5-106">تتضمن الأمثلة عن المشاريع الداخلية:</span><span class="sxs-lookup"><span data-stu-id="e86c5-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="e86c5-107">تطوير منتج، مثل تطبيق أجهزة محمولة، وتعقب التكلفة المقترنة بالتطوير.</span><span class="sxs-lookup"><span data-stu-id="e86c5-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="e86c5-108">إدارة الوقت والمصروفات قبل البيع.</span><span class="sxs-lookup"><span data-stu-id="e86c5-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="e86c5-109">يمكن تحويل هذا المشروع الداخلي قبل البيع إلى مشروع قابل للفوترة في حالة الفوز به.</span><span class="sxs-lookup"><span data-stu-id="e86c5-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="e86c5-110">يتم التعامل مع أي مشروع غير مقترن بعقد في Dynamics 365 Project Operations على أنه مشروع داخلي.</span><span class="sxs-lookup"><span data-stu-id="e86c5-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="e86c5-111">لا تُستخدم ملفات تعريف إيرادات وتكلفة المشروع لتحديد القواعد المحاسبية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="e86c5-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="e86c5-112">يتم دائمًا ترحيل تكلفة المشروع الداخلي باستخدام مبادئ الأرباح والخسائر.</span><span class="sxs-lookup"><span data-stu-id="e86c5-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="e86c5-113">يتم تحديد حسابات دفتر الأستاذ لعمليات الترحيل في صفحة **إعداد ترحيل دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="e86c5-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="e86c5-114">يتم ترحيل حركات الوقت عبر الخصم من حساب **التكلفة** وإضافته إلى حساب **توزيع كشف الرواتب**.</span><span class="sxs-lookup"><span data-stu-id="e86c5-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="e86c5-115">يتم ترحيل حركات المصروفات عبر الخصم من حساب **التكلفة** وإضافته إلى **الحساب المقابل للمصروفات**.</span><span class="sxs-lookup"><span data-stu-id="e86c5-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>
- <span data-ttu-id="e86c5-116">يتم ترحيل حركات الأصناف عن طريق الخصم من حساب **التكلفة** والإضافة إلى حساب **التكلفة - الصنف**.</span><span class="sxs-lookup"><span data-stu-id="e86c5-116">Item transactions are posted by debiting the **Cost** account and crediting the **Cost - Item** account.</span></span>

<span data-ttu-id="e86c5-117">بعد ترحيل الحركات إلى المشروع، إذا كان المشروع مقترنًا بعقد مشروع، سيقوم النظام بعكس كافة الحركات التراكمية وإنشاء حركات جديدة قابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="e86c5-117">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="e86c5-118">تتبع الحركات القابلة للفوترة القواعد المحاسبية المحددة في ملف تعريف إيرادات وتكلفة المشروع.</span><span class="sxs-lookup"><span data-stu-id="e86c5-118">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
