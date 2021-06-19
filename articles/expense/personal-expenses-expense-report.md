---
title: العمل مع المصروفات الشخصية في تقرير المصروفات
description: يوفر هذا الموضوع معلومات حول كيفية التعامل مع المصاريف الشخصية التي يتحملها الموظفون أثناء السفر لأغراض العمل.
author: suvaidya
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: ae25eca08089d224f1e17e95eeb571054de8a5c0
ms.sourcegitcommit: fd6e9ff78392c7bac35591d9130c00d2750438ae
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025668"
---
# <a name="work-with-personal-expenses-on-an-expense-report"></a><span data-ttu-id="b3279-103">العمل مع المصروفات الشخصية في تقرير المصروفات</span><span class="sxs-lookup"><span data-stu-id="b3279-103">Work with personal expenses on an expense report</span></span>

<span data-ttu-id="b3279-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="b3279-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b3279-105">أثناء السفر للعمل، قد يقوم موظف بقيد مصاريف شخصية على بطاقة ائتمان الشركة الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="b3279-105">During business travel, an employee might charge personal expenses to their corporate credit card.</span></span> <span data-ttu-id="b3279-106">إذا لم يتم تحديد عملية لمعالجة المصاريف الشخصية، فقد تتعطل عملية الموافقة على تقرير المصروفات عندما يقوم أحد الموظفين بإرسال تقرير مصروفات مفصل خاص به.</span><span class="sxs-lookup"><span data-stu-id="b3279-106">If a process hasn't been defined for handling personal expenses, the expense report approval process might be disrupted when an employee submits their itemized expense report.</span></span>

<span data-ttu-id="b3279-107">هناك طريقتان يمكنك استخدامها للعمل مع المصاريف الشخصية الخاصة بالموظف:</span><span class="sxs-lookup"><span data-stu-id="b3279-107">There are two methods you can use to work with an employee's personal expenses:</span></span>

  - <span data-ttu-id="b3279-108">**مدفوعة بواسطة الموظف**: لا تسدد مؤسستك المصروفات الشخصية التي تظهر على فاتورة بطاقة الائتمان الخاصة بالشركة.</span><span class="sxs-lookup"><span data-stu-id="b3279-108">**Paid by employee**: Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="b3279-109">وبدلا من ذلك، يدفع الموظف لمورد بطاقة الائتمان مباشرة مقابل المصاريف.</span><span class="sxs-lookup"><span data-stu-id="b3279-109">Instead, the employee pays the credit card vendor directly for the expenses.</span></span> 
  - <span data-ttu-id="b3279-110">**مدفوعة بواسطة الشركة**: تدفع مؤسستك الفاتورة الكاملة لبطاقة ائتمان الشركة، ثم تقوم بدفع حساب العامل للمصاريف الشخصية.</span><span class="sxs-lookup"><span data-stu-id="b3279-110">**Paid by company**: Your organization pays the full bill for the corporate credit card, and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="b3279-111">يمكنك تحديد الطريقة التي تستخدمها مؤسستك في صفحة **معلمات إدارة المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="b3279-111">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>


## <a name="enable-split-expense-function-when-personal-amount-field-has-value-defined"></a><span data-ttu-id="b3279-112">تمكين وظيفة المصروفات المقسمة عندما يكون يحتوي حقل المبلغ الشخصي على قيمة محددة</span><span class="sxs-lookup"><span data-stu-id="b3279-112">Enable split expense function when personal amount field has value defined</span></span>

<span data-ttu-id="b3279-113">الميزة، **تمكين وظيفة مصروفات مقسمة عندما يحتوي حقل المبلغ الشخصي على قيمة محددة** تنطبق على تقارير المصروفات التي يتم الموافقة عليها باستخدام سير عمل على مستوى البند.</span><span class="sxs-lookup"><span data-stu-id="b3279-113">The feature, **Enable split expense function when personal amount field has value defined** only applies to expense reports that are approved using a line-level workflow.</span></span> <span data-ttu-id="b3279-114">تتم الموافقة على التقارير عن طريق الانتقال **معالجة تقارير المصروفات** > **تقارير المصروفات المعينة إليّ** > **فتح تقرير المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="b3279-114">Reports are approved by going to **Process expense reports** > **Expense reports assigned to me** > **Open expense report**.</span></span> 

<span data-ttu-id="b3279-115">لتمكين هذه الميزة، انتقل إلى **مساحات العمل** > **إدارة الميزان**، حدد **‏‫تمكين وظيفة المصروفات المقسمة عندما يكون يحتوي حقل المبلغ الشخصي على قيمة محددة‬**، ثم حدد **تمكين الآن**.</span><span class="sxs-lookup"><span data-stu-id="b3279-115">To enable this feature, go to **Workspaces** > **Feature Management**, select **Enable split expense function when personal amount field has value defined**, and then select **Enable now**.</span></span> 

<span data-ttu-id="b3279-116">عندما يتم تمكين الميزة، تعمل بنود المصروفات التي تستخدم هذه الوظيفة على إنشاء بندين عند إرسال التقرير.</span><span class="sxs-lookup"><span data-stu-id="b3279-116">When the feature is enabled, expense lines that use this functionality generate two lines when the report is submitted.</span></span> <span data-ttu-id="b3279-117">يتم إنشاء بندين بحيث يمكن للموافق الموافقة على كل بند بشكل منفصل.</span><span class="sxs-lookup"><span data-stu-id="b3279-117">Two lines are generated so that the approver can approve each line separately.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
