---
title: الفواتير المصححة
description: يقدم هذا الموضوع معلومات حول الفواتير المصححة.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e14da1c07d5b697de6caf1b9041c30581ecff102
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898065"
---
# <a name="corrected-invoices"></a><span data-ttu-id="8b0a0-103">الفواتير المصححة</span><span class="sxs-lookup"><span data-stu-id="8b0a0-103">Corrected invoices</span></span>

<span data-ttu-id="8b0a0-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="8b0a0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8b0a0-105">يمكن تحرير الفواتير المؤكدة.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="8b0a0-106">عندما تقوم بتحرير فاتورة مؤكدة، يتم إنشاء مسودة فاتورة مُصححة.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="8b0a0-107">نظرًا لأن الافتراض هو أنك تريد إلغاء جميع المعاملات والكميات من الفاتورة الأصلية، فمن ثم تتضمن الفاتورة المصححة جميع المعاملات من الفاتورة الأصلية، وتكون جميع الكميات الموجودة بها صفر (0).</span><span class="sxs-lookup"><span data-stu-id="8b0a0-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="8b0a0-108">عندما لا تتطلب المعاملات تصحيحًا، فيمكنك إزالتها من مسودة الفاتورة المُصححة.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="8b0a0-109">لإلغاء أو إرجاع كمية جزئية فقط، يمكنك تحرير حقل الكمية في تفاصيل البند.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="8b0a0-110">إذا قمت بفتح تفاصيل بند الفاتورة، فيمكنك الاطلاع على كمية الفاتورة الأصلية.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="8b0a0-111">يمكنك بعد ذلك تحرير كمية الفاتورة الحالية حتى تكون أقل من أو أكبر من كمية الفاتورة الأصلية.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="8b0a0-112">عندم تقوم بتأكيد فاتورة تصحيحية، يتم إلغاء القيمة الفعلية للمبيعات المفوترة الأصلية، وإنشاء القيمة الفعلية للمبيعات المفوترة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="8b0a0-113">إذا تم تخفيض الكمية، سيتسبب الفرق في إنشاء قمة فعلية لمبيعات غير مفوترة جديدة أيضًا.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="8b0a0-114">على سبيل المثال، إذا كان المبيعات الأصلية المفوتر لمدة ثماني ساعات، وكانت تفاصيل بند الفاتورة المُصححة تحتوي على كمية مخفضة تبلغ ست ساعات، فسيتم إلغاء بند المبيعات الأصلي المفوتر ويتم إنشاء عمليتين فعليتين جديدتين:</span><span class="sxs-lookup"><span data-stu-id="8b0a0-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="8b0a0-115">قيمة فعلية لمبيعات تمت فوترتها لست ساعات.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="8b0a0-116">قيمة فعلية لمبيعات غير مفوترة للساعتين المتبقيتين.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="8b0a0-117">ويمكن أن يتم فوترة هذه الحركة لاحقا أو وضع علامة عليها على أنها غير خاضعة للرسوم، وذلك وفقا لعمليات التفاوض مع العميل.</span><span class="sxs-lookup"><span data-stu-id="8b0a0-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
