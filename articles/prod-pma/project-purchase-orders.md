---
title: أوامر الشراء لمشروع
description: توضح هذه المقالة الطرق المتنوعة التي يمكنك استخدامها لإنشاء أوامر شراء لمشروع. تعتمد الطريقة التي تستخدمها على الغرض من أمر الشراء ، ووقت استهلاك الأصناف المشتراة وتحميلها على المشروع.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bd891aec5bcab66c5801a5d9ca8abbbf632d662d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070632"
---
# <a name="purchase-orders-for-a-project"></a>أوامر الشراء لمشروع

[!include [banner](../includes/banner.md)]

توضح هذه المقالة الطرق المتنوعة التي يمكنك استخدامها لإنشاء أوامر شراء لمشروع. تعتمد الطريقة التي تستخدمها على الغرض من أمر الشراء ، ووقت استهلاك الأصناف المشتراة وتحميلها على المشروع.

### <a name="methods-for-creating-a-purchase-order"></a>طرق إنشاء أمر شراء

يمكنك استخدام أحدي الطرق التالية لإنشاء أمر شراء في أداره المشروعات والمحاسبة. يحدد الغرض من أمر الشراء الوقت الذي يكون فيه أمر الشراء مستهلكا ، التالي عند سداد الأصناف لمشروع.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>الطريقة</th>
<th>الغرض</th>
<th>استهلاك الأصناف</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>يمكنك إنشاء أمر شراء مباشرةً من مشروع.</td>
<td>استخدم هذه الطريقة لشراء أصناف من مورّد خارجي للاستهلاك في مشروع. يمكنك إنشاء أمر الشراء بطريقتين:
<ul>
<li>من المشروع نفسه. وفي هذه الحالة ، يكون المشروع محددا بالفعل لأمر الشراء.</li>
<li>من خلال التنقل إلى أمر شراء المشروع. يجب تحديد كل من المورد والمشروع لإنشاء أمر الشراء ل.</li>
</ul></td>
<td>يتم استهلاك الأصناف عند تحديث فاتورة المورد.</td>
</tr>
<tr class="even">
<td>قم بإنشاء أمر شراء من أمر مبيعات.</td>
<td>استخدم هذا الأسلوب لشراء الأصناف عند إنشاء أمر توريد من أحد المشروعات.</td>
<td>يتم استهلاك الأصناف عند فوتره أمر المبيعات إلى العميل.</td>
</tr>
<tr class="odd">
<td>إنشاء أمر شراء من أحد متطلبات الأصناف.</td>
<td>استخدم هذه الطريقة لشراء العناصر عند إنشاء متطلب عنصر من مشروع.</td>
<td>يتم استهلاك الأصناف عند تحديث إيصال تعبئة متطلبات الصنف.</td>
</tr>
</tbody>
</table>

> [!NOTE] 
> عند تحديث فاتورة المورد أو إيصال التعبئة ، ستتم مطالبتك بتحديث إيصال التعبئة في متطلبات الصنف.

لمزيد من المعلومات، راجع [استلام العناصر في أمر الشراء من متطلب الصنف](tasks/receive-items-purchase-order-item-requirement.md).
