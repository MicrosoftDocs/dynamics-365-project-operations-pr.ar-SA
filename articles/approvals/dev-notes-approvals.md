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
ms.openlocfilehash: 9e4e910d0ff0a5f2603148fcc5daa0d423a4d174
ms.sourcegitcommit: a9dbcd3aff4c6ae495412e4980e105ae160fd1ec
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/10/2020
ms.locfileid: "4483932"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="36db6-103">ملاحظات المطور للموافقات</span><span class="sxs-lookup"><span data-stu-id="36db6-103">Developer notes for Approvals</span></span>

<span data-ttu-id="36db6-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="36db6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="36db6-105">يتضمن Dynamics 365 Project Operations منطق التحقق من الصحة الذي يضمن انتقال السجلات الصحيح من خلال مراحل الموافقة.</span><span class="sxs-lookup"><span data-stu-id="36db6-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="36db6-106">يضمن الانتقال الصحيح للسجلات:</span><span class="sxs-lookup"><span data-stu-id="36db6-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="36db6-107">إنشاء كافة صفوف الداعمة في الجداول ذات الصلة، مثل دفاتر اليومية والقيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="36db6-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="36db6-108">توضع على الموافق علامة **الموافق على المشروع** في المشروع قبل المتابعة.</span><span class="sxs-lookup"><span data-stu-id="36db6-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>
