---
title: السلفة النقدية
description: يقدم هذا الموضوع معلومات حول السلف النقدية.
author: suvaidya
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 209fe0b8a79b2c0689c458c423664cb292da249b
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070527"
---
# <a name="cash-advance"></a>السلفة النقدية

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

تسمح السلفة النقدية للموظفين باقتراض أموال من شركتهم قبل تكبد أي مصروفات. وعند الموافقة على السلفة النقدية المطلوبة ودفعها، يستطيع الموظف استخدام الأموال الخاصة بمصروفات العمل التي قد تكون على وشك تحملها. 

## <a name="create-and-submit-a-cash-advance-request"></a>إنشاء طلب سلفة نقدية وإرساله

1. ضمن **مصروفاتي‏‎** ، حدد **السلف النقدية** > **جديد** لإنشاء سلفة نقدية جديدة. 
2. في الصفحة **طلب سلفة نقدية جديدة** ، أدخل غرض المصروفات وحدد الموقع الذي سيتم تكبد المصروفات فيه.
3. ادخل المبلغ المطلوب والعملة المطلوبة، ثم حدد **حفظ**. 
4. عندما تكون جاهزًا لإرسال طلب السلفة النقدية، في الصفحة **طلب سلفة نقدية** ، حدد **سير عمل** > **إرسال**.

## <a name="modify-a-cash-advance-request"></a>تعديل طلب سلفة نقدية

يمكنك تعديل طلب سلفة نقدية إذا لم يتم إرساله للموافقة عليه.

1. ضمن **مصروفاتي: السلف النقدية** ، حدد موقع السلفة النقدية التي ترغب في تحريرها وحددها.
2. حدد **تحرير** ، وأدخل التغييرات اللازمة على طلب السلفة النقدية. 
3. حدد **حفظ وإغلاق**.


## <a name="view-cash-advance-requests"></a>عرض طلبات السلف النقدية
يمكنك مراجعة قائمة بجميع السلف النقدية في وضع المسودة أو المرسلة أو قيد المراجعة أو المدفوعة تحت **مصروفاتي: السلف النقدية‬‏‫**. 

## <a name="approve-cash-advance-requests"></a>الموافقة على طلبات السلف النقدية

سيتمكن المدراء أو المستخدمون الذين تم تكوينهم كموافقين في سير العمل من الموافقة على طلبات السلف النقدية المرسلة اليهم للمراجعة. 

1. للموافقة على سلفة نقدية، ضمن **معالجة السلف النقدية** ، حدد **السلف النقدية لمراجعتي**.
2. حدد السلفة النقدية التي ترغب في مراجعتها وحدد **موافقة**.  

## <a name="pay-cash-advances"></a>دفع السلف النقدية 
يتم عادةً إكمال الإجراء التالي بواسطة محاسب أو مستخدم له أذونات محاسبية.

1. لترحيل السلف النقدية الموافق عليها، حدد **السلف النقدية الموافق عليها** ، ثم حدد **دفع وتحويل**.  
2. قدم تفاصيل دفتر اليومية للسلف النقدية، ثم حدد **موافق**. 

## <a name="submit-an-expense-report-against-a-paid-cash-advance"></a>إرسال تقرير مصروفات في مقابل سلفة نقدية مدفوعة 

عندما تقوم بإنشاء تقرير مصروفات وإرساله لسلفة نقدية استلمتها، سيتم ضبط المصروفات بشكل تلقائي في مقابل هذه السلفة. إذا كانت السلفة النقدية أكبر من المبلغ المصروف، يجب عليك إرجاع الرصيد إلى الشركة باستخدام فئة المصروفات **إرجاع المبلغ النقدي**. إذا كانت السلفة النقدية المدفوعة من خلال الشركة أقل من المبلغ المصروف، فيجب على الشركة تعويض الرصيد. 

### <a name="example"></a>مثال
أنت تخطط للسفر لحضور مؤتمر من سياتل إلى مدينة نيويورك. يمكنك إنشاء طلب سلفة نقدية بمبلغ 3000.00 دولار إذ قمت بتقدير تكلفة التذكر والرحلات والفندق والوجبات وسيارات الإجراء بحيث تساوي هذا المبلغ تقريبًا. لن يتم دفع هذا المبلغ لك ما لم يوافق المدير على هذا الطلب. بعد موافقة المدير، يتم دفع المبلغ النقدي المطلوب وهو 3000.00 دولار في حسابك البنكي. ثم تحضر المؤتمر. بعد انتهاء رحلتك، يتبين لك أن إجمالي النفقات بلغ 2790.00 دولار فقط. حدد **نقدًا** في حقل **طريقة الدفع** وأرسل مصروفاتك بقيمة 2790.00 دولار. يتم ضبط مبلغ المصروفات المرسل بشكل تلقائي في مقابل السلفة النقدية بقيمة 3000.00 دولار التي تم إقراضها لك. يجب عليك الآن إرجاع مبلغ 210.00 دولار (3000.00-2790.00) للشركة، ويمكنك إرجاعه باستخدام فئة المصروفات **إرجاع المبلغ النقدي**. 