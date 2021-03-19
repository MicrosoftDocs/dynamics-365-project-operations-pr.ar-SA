---
title: تكوين المحاسبة للمشروعات الداخلية
description: يقدم هذا الموضوع معلومات حول كيفية إعداد ممارسات المحاسبة للمشاريع الداخلية في Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 9f1cc75b12fec81d726e46f8d970dcfe030f6b29
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287582"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="a5b5b-103">تكوين المحاسبة للمشروعات الداخلية</span><span class="sxs-lookup"><span data-stu-id="a5b5b-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="a5b5b-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="a5b5b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a5b5b-105">تسمح المشاريع الداخلية للشركات بتعقب التكلفة ذات الصلة بالأنشطة التي لم تتم فوترتها على العميل.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="a5b5b-106">تتضمن الأمثلة عن المشاريع الداخلية:</span><span class="sxs-lookup"><span data-stu-id="a5b5b-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="a5b5b-107">تطوير منتج، مثل تطبيق أجهزة محمولة، وتعقب التكلفة المقترنة بالتطوير.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="a5b5b-108">إدارة الوقت والمصروفات قبل البيع.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="a5b5b-109">يمكن تحويل هذا المشروع الداخلي قبل البيع إلى مشروع قابل للفوترة في حالة الفوز به.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="a5b5b-110">يتم التعامل مع أي مشروع غير مقترن بعقد في Dynamics 365 Project Operations على أنه مشروع داخلي.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="a5b5b-111">لا تُستخدم ملفات تعريف إيرادات وتكلفة المشروع لتحديد القواعد المحاسبية للمشروع.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="a5b5b-112">يتم دائمًا ترحيل تكلفة المشروع الداخلي باستخدام مبادئ الأرباح والخسائر.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="a5b5b-113">يتم تحديد حسابات دفتر الأستاذ لعمليات الترحيل في صفحة **إعداد ترحيل دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="a5b5b-114">يتم ترحيل حركات الوقت عبر الخصم من حساب **التكلفة** وإضافته إلى حساب **توزيع كشف الرواتب**.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="a5b5b-115">يتم ترحيل حركات المصروفات عبر الخصم من حساب **التكلفة** وإضافته إلى **الحساب المقابل للمصروفات**.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>

<span data-ttu-id="a5b5b-116">بعد ترحيل الحركات إلى المشروع، إذا كان المشروع مقترنًا بعقد مشروع، سيقوم النظام بعكس كافة الحركات التراكمية وإنشاء حركات جديدة قابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-116">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="a5b5b-117">تتبع الحركات القابلة للفوترة القواعد المحاسبية المحددة في ملف تعريف إيرادات وتكلفة المشروع.</span><span class="sxs-lookup"><span data-stu-id="a5b5b-117">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]