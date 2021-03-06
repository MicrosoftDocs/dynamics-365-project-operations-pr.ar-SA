---
title: إدخال المصروفات (خفيفة)
description: يقدم هذا الموضوع معلومات حول كيفية العمل مع إدخال المصروفات في عملية نشر خفيفة.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 746d5d9ff56222e7d6b9b6e264db75d5814365c7
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965713"
---
# <a name="expense-entry-lite"></a>إدخال المصروفات (خفيفة)

_**ينطبق على:** النشر الخفيف – التعامل مع الفواتير الأولية_

إدارة المصروفات الأساسية، أو الخفيفة، هي القدرة على تسجيل المصروفات البسيطة. يمكنك تسجيل المصروفات في مقابل مشروع، ومن ثم يقوم الموافق على المشروع بمراجعتها والموافقة عليها.

لمزيد من المعلومات حول قدرات المصروفات في Dynamics 365 Project Operations، راجع [نظرة عامة حول المصروفات](expense-overview.md).

## <a name="capture-a-basic-expense"></a>تسجيل مصروفات أساسية

يمكنك تسجيل المصروفات بحيث يمكنك إرسالها إلى الموافق.

1. انتقل إلى **المصروفات**، وحدد **جديد**.
2. في صفحة **المصروفات الجديدة**، أدخل معلومات المصروفات المطلوبة، ثم حدد **حفظ**.

## <a name="submit-a-basic-expense"></a>إرسال مصروفات أساسية

بعد أن تنتهي من تسجيل كافة المصروفات، يجب عليك إرسالها للموافقة عليها.

1. انتقل إلى **المصروفات**، وحدد أحدها. أو حدد كافة المصروفات باستخدام خانة الاختيار الموجودة في الرأس.
2. حدد **إرسال**. يعالج النظام الإدخالات المحددة ثم ينشئ طلبات الموافقة على المصروفات.

## <a name="recall-a-basic-expense"></a>استدعاء مصروفات أساسية

عند إرسال مصروفات عن طريق الخطأ، يمكنك استدعاؤها. يتوقف الوقت المطلوب لاستدعاء إدخال المصروفات على مرحلة الموافقة عليه.  إذا لم يكن الموافق قد وافق بعد على الإدخال، فيمكن أن يحدث الاستدعاء على الفور. ومع ذلك، إذا كانت قد تمت الموافقة على الإدخال، فيجب على الموافق الموافقة على الاستدعاء وإلغاء الحركات.

1. انتقل إلى **المصروفات**، ثم في قائمة المصروفات، حدد إدخال المصروفات الذي ترغب استدعائه.
2. حدد **استرجاع**. إذا لم تكن الموافقة على إدخال المصروفات قد حدثت بعد، فسيقوم النظام باستدعائه على الفور. إذا كانت قد تمت الموافقة على إدخال المصروفات، فسيتم إنشاء طلب استدعاء لإعلام الموافق برغبتك في إلغاء إدخال المصروفات. سيؤكد الموافق عندئذٍ أنه يمكن تنفيذ الإلغاء، وسيتم إرجاع الإدخال.

## <a name="delete-a-basic-expense"></a>حذف مصروفات أساسية

يمكن حذف المصروفات التي لم يتم إرسالها بعد. لحذف إدخال مصروفات تم إرساله، يجب أولاً استدعاؤه.

## <a name="see-also"></a>راجع أيضًا

- [نظرة عامة على الموافقات](../approvals/approvals-overview.md)
