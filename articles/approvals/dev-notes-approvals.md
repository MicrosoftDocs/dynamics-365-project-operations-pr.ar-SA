---
title: ملاحظات المطور للموافقات
description: يقدم هذا الموضوع معلومات مطور إضافية حول العمل مع الموافقات.
author: stsporen
manager: Annbe
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: d58c776b0341c08b0292e1b459a7d7ebac550bcc
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290253"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="f7519-103">ملاحظات المطور للموافقات</span><span class="sxs-lookup"><span data-stu-id="f7519-103">Developer notes for Approvals</span></span>

<span data-ttu-id="f7519-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="f7519-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f7519-105">يتضمن Dynamics 365 Project Operations منطق التحقق من الصحة الذي يضمن انتقال السجلات الصحيح من خلال مراحل الموافقة.</span><span class="sxs-lookup"><span data-stu-id="f7519-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="f7519-106">يضمن الانتقال الصحيح للسجلات:</span><span class="sxs-lookup"><span data-stu-id="f7519-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="f7519-107">إنشاء كافة صفوف الداعمة في الجداول ذات الصلة، مثل دفاتر اليومية والقيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="f7519-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="f7519-108">توضع على الموافق علامة **الموافق على المشروع** في المشروع قبل المتابعة.</span><span class="sxs-lookup"><span data-stu-id="f7519-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]