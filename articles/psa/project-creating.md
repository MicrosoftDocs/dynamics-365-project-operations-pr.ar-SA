---
title: جداول المشاريع
description: يقدم هذا الموضوع معلومات عن كيفية إنشاء جدول.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 3/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 9a6b27050a19d8a7f2ed35f74b42bb4f371ad069
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070679"
---
# <a name="project-schedules"></a>جداول المشاريع 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

يوضح جدول المشروع ما العمل الذي يجب إكماله ، والموارد التي ستؤدي العمل ، والإطار الزمني الذي يجب الانتهاء من العمل فيه. يعكس جميع الأعمال المرتبطة بتسليم المشروع في الوقت المحدد. في Dynamics 365 Project Service Automation، يمكنك إنشاء جدول مشروع وذلك بتقسيم العمل إلى المهام القابلة للإدارة وتقدير الوقت المطلوب لتنفيذ كل مهمة وتعيين تبعيات المهام وتعيين مدد المهام وتقدير الموارد العامة التي ستقوم بتنفيذ المهام. يتم إنشاء جدول المشروع في علامة التبويب **الجدولة** في صفحة المشروع.
 
## <a name="tasks"></a>المهام

تتمثل الخطوة الأولى في إنشاء جدول مشروع في تقسيم العمل إلى أجزاء قابلة للإدارة. يدعم الجدول في PSA الميزات التالية:

- عقدة الجذر للمشروع.
- المهام الموجزة أو مهام الحاوية
- مهام العقدة الطرفية

### <a name="project-root-node"></a>عقدة الجذر للمشروع.

عقدة جذر المشروع هي مهمة الملخص ذات المستوى الأعلى للمشروع. يتم إنشاء كافة مهام المشروع تحتها. يتم تعيين اسم العقدة الجذر إلى اسم المشروع دائمًا. يتم تلخيص المجهود والتواريخ ومدة عقدة الجذر استنادًا إلى القيم الموجودة في التدرج الهرمي أدناها. لا يمكنك تحرير خصائص العقدة الجذر. لا يمكنك أيضًا حذف العقدة الجذر.

### <a name="summary-or-container-tasks"></a>المهام الموجزة أو مهام الحاوية 

تشتمل مهام الملخص على مهام فرعية أو مهام حاوية ضمنها. وليس لديهم جهد عمل أو تكلفة خاصة بهم. بدلاً من ذلك ، فإن جهد العمل والتكلفة هما مجموعة من جهد العمل وتكلفة مهام الحاوية الخاصة به. تاريخ بدء مهمة التلخيص هو تاريخ بدء مهام الحاوية ، وتاريخ الانتهاء هو تاريخ الانتهاء من مهام الحاوية. يمكن تحرير اسم مهمة تلخيصية ، لكن لا يمكن تحرير خصائص الجدولة (الجهد والتواريخ والمدة). إذا قمت بحذف مهمة تلخيصية ، يمكنك أيضًا حذف جميع مهام الحاوية الخاصة بها.

### <a name="leaf-node-tasks"></a>مهام العقدة الطرفية

تمثل مهام عقدة الورقة العمل الأكثر تفصيلاً في المشروع. إنها تتميز بمجهود مقدّر والموارد وتواريخ بدء وانتهاء مخططين ومدة.
 
## <a name="creating-a-task-hierarchy"></a>إنشاء التدرج الهرمي للمهام

يمكنك إنشاء تدرج هرمي للمهام باستخدام الخيارات التالية:

- الزر **إضافة مهمة**
- الزر **تحريك المهمة إلى مستوى أدنى**.
- الزر **تحريك المهمة إلى مستوى أعلى**.
- الزران **تحريك لأعلى** و **تحريك لأسفل**
- اختصارات لوحة المفاتيح وذوي الاحتياجات الخاصة

### <a name="add-task"></a>إضافة مهمة

يتيح لك الزر **إضافة مهمة** إمكانية إنشاء مهمة جديدة في التدرج الهرمي. إذا لم تقم بتحديد موضع، فإنه يتم إدراج المهمة في النهاية. 

يتم تعيين معرف الجدول لكل مهمة. يمثل معرف الجدول عمق وموضع المهمة في التدرج الهرمي. ويستخدم ترقيم المخططات التفصيلية. بالنسبة للمهام الموجودة في المستوي الأول أسفل العقدة الجذر للمشروع ، يتم استخدام نظام ترقيم من 1 و2 و3 وهكذا. بالنسبة للمهام ضمن المستوى الأول، يتم استخدام نظام ترقيم من 1.1 و1.2 و1.3 وهكذا.

### <a name="indent-task"></a>تحريك المهمة إلى مستوى أدنى

عند تحريك مهمة لأسفل، تصبح تابعة للمهمة التي فوقها مباشرةً. ثم تتم إعادة حساب الجدول الزمني للمهمة بحيث يستند إلى معرف الجدول الأصلي الجديد ويتبع مخطط ترقيم المخطط التفصيلي. تعتبر المهمة الأصل الآن مهمة ملخص أو مهمة حاوية. ولذلك، تصبح قيمة محتسبة للمهام التابعة لها.

### <a name="outdent-task"></a>تحريك المهمة إلى مستوى أعلى 

عندما يتم تحريك أحدي المهام إلى مستوى أعلى، تصبح المهمة تابعة للمهمة الأصلية. ثم يتم بعد ذلك إعادة حساب معرف الجدول حتى يعكس عمق وموضع المهمة اللذين تم تحديثهما في التدرج الهرمي. تتم إعادة حساب الجهد والتكلفة والتواريخ الخاصة بالمهمة الأصل السابقة التالي لا تتضمن هذه المهمة.

### <a name="move-up-and-move-down"></a>تحريك لأعلى وتحريك لأسفل 

ويقوم الزران **تحريك لأعلى** و **تحريك لأسفل** بتغيير موضع المهمة في التدرج الهرمي الأصل. لا تؤثر التغييرات من هذا النوع على مجهود المهمة أو تكلفتها أو تواريخها أو مدتها. يتأثر فقط معرف الجدول الخاص بالمهمة. تتم إعادة حساب معرف الجدول حتى يعكس الموضع الجديد للمهمة في قائمة المهام التابعة للأصل.

### <a name="accessibility-and-keyboard-shortcuts"></a>اختصارات لوحة المفاتيح وذوي الاحتياجات الخاصة

إن شبكة **الجدولة** يمكن الوصول اليها بالكامل ويمكن استخدامها مع قارئات الشاشة مثل المسرد أو JAWS أو NVDA. يمكنك التنقل خلال منطقه الشبكة باستخدام مفاتيح الأسهم (كما في Microsoft Excel)، يمكنك استخدام المفتاح Tab للتقدم من خلال عناصر واجهة المستخدم التفاعلية، ويمكنك استخدام مفتاح السهم لأسفل، أو مفتاح Enter، أو Spacebar لتحديد واستدعاء القوائم المنسدلة. وتكون رؤوس الأعمدة أيضا تفاعلية. يمكنك إخفاء الأعمدة وإظهارها، واستخدام المفتاح Tab ومفاتيح الأسهم للتنقل بين رؤوس الأعمدة، واستخدام أزرار الإجراء على شريط الأدوات. بالإضافه إلى ذلك، يمكنك استخدام مفاتيح الاختصارات التالية:

- **تحديث** :‏ ALT+SHIFT+F5
- **إضافة** :‏ ALT+SHIFT+Insert
- **حذف** :‏ ALT+SHIFT+Delete
- **تحريك لأعلى/لأسفل** : أسهم‏ ALT+SHIFT+Up/Down
- **التحريك لمستوى أدنى/أعلى** : أسهم ALT_SHIFT+Left/Right
- **توسيع/طي التدرجات الهرمية** : مفاتيح ALT+SHIFT+Plus/Minus

## <a name="task-attributes"></a>سمات المهمة

يصف اسم المهمة العمل الذي يجب إكماله. في PSA ، تصف السمات المرتبطة بالمهمة جدول المهمة ومتطلبات التوظيف الخاصة بها.

> ![سمات المهمة](media/project-2.png)
 
### <a name="schedule-attributes"></a>سمات الجدولة

تحدد سمات **المجهود** و **تاريخ البدء** و **تاريخ الانتهاء** و **المدة** الجدول الخاص بالمهمة.

وتتضمن سمات الجدولة الاضافية ما يلي:

- **ساعات المجهود** : أدخل تقديرا للساعات المطلوبة لإكمال المهمة. 
- **المدة** : حدد عدد أيام الإنجاز المطلوبة لإكمال المهمة.
- **معرف الجدول** : يتم استخدام المعرف الذي تم إنشاؤه تلقائيًا لطلب المهام في التدرج الهرمي. تدير التبعيات بين المهام الترتيب الفعلي الذي تم العمل على المهام فيه.
 
### <a name="staffing-attributes"></a>سمات التوظيف

يتم الوصول إلى سمات التوظيف من خلال حقل **الموارد** في الجدول. يمكنك إما البحث عن مورد موجود، أو النقر فوق **إنشاء** وفي جزء **الإنشاء السريع** ، أضف عضو فريق مشروع كمورد جديد.

يتم استخدام حقول **الدور** و **وحدة تعيين الموارد‬** و **اسم المنصب** لوصف متطلبات الموظفين للمهمة. يتم استخدام سمات التوظيف هذه مع جداول المهام للعثور على الموارد المتوفرة لتنفيذ هذه المهمة.

**الدور** -حدد نوع المورد المطلوب لتنفيذ المهمة.

**وحدة تعيين الموارد** - حدد الوحدة التي ينبغي تعيين الموارد الخاصة بالمهمة منها. تؤثر هذه السمة على تقدير التكلفة والمبيعات الخاصة بالمهمة في حالة تعيين التكلفة وسعر الفاتورة للمورد بناء على وحدات تعيين الموارد.

**اسم المنصب** – ادخل اسما مألوفا للمورد العام الذي يعمل كعنصر نائب للمورد الذي سيقوم بالعمل في النهاية.

يحتوي حقل **الموارد** على اسم المنصب الخاص بالمورد العام أو المورد المسمى عند العثور على واحد.

ويحتوي حقل **الفئة** على القيم التي تشير إلى نوع أكبر من العمل الذي يمكن تجميع المهمة فيه. لا يؤثر هذا الحقل في الجدولة أو الموظفين. ويُستخدم لإعداد التقارير فقط.

### <a name="task-dependencies"></a>تبعيات المهمة 

يمكنك استخدام الجدول في PSA لإنشاء العلاقات السابقة بين المهام. يأخذ حقل **النشاط السابق** ضمن **المهام** قيمه واحدة أو أكثر للإشارة إلى المهام التي تعتمد عليها المهمة. عند تعيين قيم أنشطة سابقة لمهمة، يمكن بدء المهمة فقط بعد إكمال كافة المهام السابقة. وبسبب التبعية، تتم إعادة تعيين تاريخ البدء المخطط للمهمة إلى تاريخ إتمام المهام السابقة.

لا يؤثر وضع المهمة على التحديثات التي يتم إجراؤها على تاريخي البدء والانتهاء للمهام السابقة/التابعة.

## <a name="task-mode"></a>وضع المهمة 

يحدد وضع المهمة جدولة مهام العقدة الطرفية. يدعم PSA وضعي مهام لكل مهمة: الجدولة التلقائية والجدولة اليدوية.

### <a name="auto-scheduling"></a>الجدولة التلقائية 
 
عند تعيين وضع المهمة إلى **تمت الجدولة تلقائيًا** ، يستخدم محرك جدولة المهمة قواعد الجدولة على سمات المهمة التالية لتحديد الجدول الزمني للمهمة.

#### <a name="scheduling-rules"></a>قواعد الجدولة

بشكل افتراضي، لا تشتمل مهمة عقدة طرفية على مهام سابقة، تم تعيين تاريخ البدء الخاص بها إلى تاريخ البدء المجدول للمشروع. يتم حساب مدة مهمة العقدة الطرفية دائمًا كعدد أيام العمل بين تاريخي البدء والانتهاء. عندما تتم جدولة مهمة تلقائيًا، يتبع محرك الجدولة القواعد التالية:

- يجب أن يكون تاريخي بدء وانتهاء المهمة عبارة عن أيام عمل وفقًا لتقويم جدولة المشروع. 
- بالنسبة إلى أي مهمة لها مهام سابقة، يتم تعيين تاريخ البدء تلقائيًا على آخر تاريخ نهاية لسابقاتها.
- يتم حساب الجهد باستخدام هذه الصيغة: عدد الأشخاص × المدة × ساعة في يوم عمل قياسي في تقويم المشروع.

### <a name="manual-scheduling"></a>الجدولة اليدوية

إذا كانت قواعد الجدولة التلقائية لا تفي بمتطلباتك، فيمكنك تعيين وضع المهمة للهمهة المُراد **جدولتها يدويًا**. يؤدي هذا الإعداد إلى توقف محرك الجدولة عن حساب القيم لسمات جدولة أخرى. وبغض النظر عن وضع المهمة، إذا قمت بتعيين المهام السابقة على المهام، فسيؤثر دائمًا على تاريخ البدء للمهمة التابعة.