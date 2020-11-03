---
title: تنفيذ الحقول المخصصة لتطبيق الأجهزة المحمولة لـ Microsoft Dynamics 365 Project Timesheet على iOS وAndroid
description: يقدم هذا الموضوع الأنماط الشائعة لاستخدام الملحقات لتنفيذ الحقول المخصصة.
author: Yowelle
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 1ea1ca002a8f68f86808831b398e452244471322
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070698"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a>تنفيذ الحقول المخصصة لتطبيق الأجهزة المحمولة لـ Microsoft Dynamics 365 Project Timesheet على iOS وAndroid

[!include [banner](../includes/banner.md)]

يقدم هذا الموضوع الأنماط الشائعة لاستخدام الملحقات لتنفيذ الحقول المخصصة. يتم تغطيه الموضوعات التالية:

- العديد من أنواع البيانات التي يدعمها اطار عمل الحقل المخصص
- كيفيه إظهار حقول للقراءة فقط أو قابله للتحرير في إدخالات الجدول الزمني ، وحفظ القيم التي تم توفيرها بالنسبة للمستخدم مره أخرى إلى قاعده البيانات
- كيفيه إظهار حقول القراءة فقط في راس الجدول الزمني
- كيفيه دمج منطق الاعمال المخصصة الأخرى لإدخال القيم الافتراضية في الحقول وإجراء مزيد من التحقق من الصحة

## <a name="audience"></a>الجمهور

وهذا الموضوع مخصص للمطورين الذين يقومون بدمج الحقول المخصصة الخاصة بهم في تطبيق الأجهزة المحمولة لـ Microsoft Dynamics 365 Project Timesheet المتوفر لشركة Apple iOS وGoogle Android. الافتراض هو أن القراء على دراية بتطوير X ++ ووظائف الجدول الزمني للمشروع.

## <a name="data-contract--tstimesheetcustomfield-x-class"></a>عقد البيانات - فئة TSTimesheetCustomField X ++

فئة **TSTimesheetCustomField** هي فئة عقد بيانات X ++ التي تمثل معلومات حول حقل مخصص لوظائف الجدول الزمني. يتم تمرير قوائم كائنات الحقول المخصصة في كل من عقد بيانات TSTimesheetDetails وعقد بيانات TSTimesheetEntry لإظهار الحقول المخصصة في تطبيق الأجهزة المحمولة.

- **TSTimesheetDetails** - عقد رأس الجدول الزمني.
- **TSTimesheetEntry** - عقد معاملة الجدول الزمني. مجموعات من هذه الكائنات لها نفس معلومات المشروع وقيمة **timesheetLineRecId** تشكل البند.

### <a name="fieldbasetype-types"></a>fieldBaseType (الأنواع)

تحدد خاصية **FieldBaseType** في كائن **TsTimesheetCustom** نوع الحقل الذي يظهر في التطبيق. قيم **الأنواع** التالية التي يتم دعمها.

| قيمة الأنواع | كتابة              | ملاحظات |
|-------------|-------------------|-------|
| 1           | السلسلة (والتعداد) | يظهر الحقل كحقل نص. |
| 1           | Integer           | يتم عرض القيمة كرقم بدون منازل عشرية. |
| 2           | حقيقي              | يتم عرض القيمة كرقم بمنازل عشرية.<p>لإظهار القيمة الفعلية كعملة في التطبيق، استخدم خاصية **fieldExtenededType**. يمكنك استخدام خاصية **numberOfDecimals** لتعيين عدد المنازل العشرية المعروضة.</p> |
| 3           | التاريخ              | يتم تحديد تنسيقات التاريخ بواسطة إعداد **التاريخ والأوقات وتنسيق الأرقام** الخاص بالمستخدم والذي تم تحديده ضمن **تفضيلات اللغة والبلد/المنطقة** في **خيارات المستخدم**. |
| 4           | Boolean           | |
| 15          | GUID              | |
| 16          | Int64             | |

- إذا لم يتم توفير خاصية **stringOptions** في كائن **TSTimesheetCustomField** ، يتم توفير حقل نص حر للمستخدم.

    يمكن استخدام خاصية **stringLength** لتعيين الحد الأقصى لطول السلسلة الذي يمكن للمستخدمين إدخاله.

- في حالة توفير خاصية **stringOptions** في كائن **TSTimesheetCustomField** ، عناصر هذه القائمة هي القيم الوحيدة التي يمكن للمستخدمين تحديدها باستخدام أزرار الخيارات (الأزرار التبادلية).

    في هذه الحالة ، يمكن أن يعمل حقل السلسلة كقيمة تعداد لغرض إدخال المستخدم. لحفظ القيمة في قاعدة البيانات كتعداد ، قم يدويًا بتعيين قيمة السلسلة إلى قيمة التعداد قبل الحفظ في قاعدة البيانات باستخدام سلسلة الأوامر (راجع "استخدام سلسلة الأوامر في فئة TSTimesheetEntryService لحفظ إدخال جدول زمني من التطبيق مرة أخرى إلى قسم قاعدة البيانات "لاحقًا في هذا الموضوع على سبيل المثال).

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a>fieldExtendedType ‏(TSCustomFieldExtendedType)

يمكنك استخدام هذه الخاصية لتنسيق القيم الفعلية كعمله. يكون هذا الأسلوب قابلا للتطبيق فقط عندما تكون قيمة **fieldBaseType** هي **حقيقية**.

- **TSCustomFieldExtendedType:None** – لم يتم تطبيق أي تنسيق.
- **TSCustomFieldExtendedType::العملة** – تنسيق القيمة كعملة.

    عندما يكون تنسيق العملة نشطًا، يمكن استخدام حقل **stringValue** لتمرير رمز العملة الذي يجب ان يظهر في التطبيق. القيمة هي قيمه للقراءة فقط.

    يحتوي حقل **realValue** على المبلغ النقدي الذي ينبغي حفظه إلى قاعدة البيانات.

### <a name="fieldsection-tscustomfieldsection"></a>fieldSection (TSCustomFieldSection)

يمكنك استخدام هذه الخاصية لتحديد المكان الذي ينبغي ان يظهر فيه الحقل المخصص في التطبيق.

- **TSCustomFieldSection::الرأس** – سيظهر الحقل في قسم **عرض المزيد من التفاصيل** في التطبيق. هذه الحقول دائمًا للقراءة فقط.
- **TSCustomFieldSection::البند** – سيظهر الحقل بعد كل الحقول الجاهزة في إدخالات الجدول الزمني. يمكن ان تكون هذه الحقول اما قابله للتحرير أو للقراءة فقط.

### <a name="fieldname-fieldnameshort"></a>fieldName (FieldNameShort)

تحدد هذه الخاصية الحقل عندما يتم حفظ القيم التي يوفرها التطبيق مره أخرى إلى قاعده البيانات.

### <a name="tablename-tablenameshort"></a>tableName (TableNameShort)

تحدد هذه الخاصية الحقل عندما يتم حفظ القيم التي يوفرها التطبيق مره أخرى إلى قاعده البيانات.

### <a name="iseditable-noyes"></a>isEditable (NoYes)

قم بتعيين هذه الخاصية إلى **نعم** لتحديد أن الحقل الموجود في مقطع "إدخال الجدول الزمني" يجب ان يكون قابلا للتحرير من قبل المستخدمين. قم بتعيين الخاصية إلى **لا** لجعل الحقل للقراءة فقط.

### <a name="ismandatory-noyes"></a>isMandatory (NoYes)

قم بتعيين هذه الخاصية إلى **نعم** لتحديد أن الحقل في قسم إدخال الجدول الزمني يجب أن يكون إلزاميًا.

### <a name="label-str"></a>التسمية (سلسلة)

تحدد هذه الخاصية التسمية التي تظهر بعد الحقل في التطبيق.

### <a name="stringoptions-list-of-strings"></a>stringOptions (قائمة السلاسل)

تكون هذه الخاصية قابله للتطبيق فقط عندما يتم تعيين **fieldBaseType** إلى **السلسلة**. إذا تم تعيين **stringOptions** ، يتم تحديد قيم السلسلة المتاحة للتحديد عبر أزرار الخيارات (أزرار الاختيار) بواسطة السلاسل الموجودة في القائمة. يتم تحديد قيم السلسلة المتاحة للتحديد عبر أزرار الخيارات (أزرار الاختيار) بواسطة السلاسل الموجودة في القائمة.

### <a name="stringlength-int"></a>stringLength (int)

تحدد هذه الخاصية الحد الأقصى لطول حقل السلسلة. هذه الخاصية قابله للتطبيق فقط عندما يتم تعيين **fieldBaseType** إلى **السلسلة**.

### <a name="numberofdecimals-int"></a>numberOfDecimals (int)

تحدد هذه الخاصية عدد المنازل العشرية التي يتم عرضها للحقل الحقيقي. هذه الخاصية قابله للتطبيق فقط عندما يتم تعيين **fieldBaseType** إلى **حقيقي**.

### <a name="ordersequence-int"></a>orderSequence (int)

تتحكم هذه الخاصية بالترتيب الذي يتم به عرض الحقول المخصصة في التطبيق عندما يتم تحديد أكثر من حقل مخصص واحد. يتم عرض الحقول التي تحتوي علي أرقام اقل أولا.

### <a name="booleanvalue-boolean"></a>booleanValue (منطقية)

بالنسبة للحقول التي لها النوع **المنطقي** ، تمرر هذه الخاصية القيمة المنطقية للحقل بين الخادم والتطبيق.

### <a name="guidvalue-guid"></a>guidValue (guid)

بالنسبة للحقول التي لها النوع **GUID** ، تمرر هذه الخاصية قيمة المعرف الفريد العمومي (GUID) للحقل بين الخادم والتطبيق.

### <a name="int64value-int64"></a>int64Value (int64)

بالنسبة للحقول التي لها النوع **Int64** ، تمرر هذه الخاصية قيمة int64 للحقل بين الخادم والتطبيق.

### <a name="intvalue-int"></a>intValue (int)

بالنسبة للحقول التي لها النوع **Int** ، تمرر هذه الخاصية القيمة int للحقل بين الخادم والتطبيق.

### <a name="realvalue-real"></a>realValue (حقيقي)

بالنسبة للحقول التي لها النوع **حقيقي** ، تمرر هذه الخاصية القيمة الحقيقية للحقل بين الخادم والتطبيق.

### <a name="stringvalue-str"></a>stringValue (السلسلة)

بالنسبة للحقول التي لها النوع **سلسلة** ، تمرر هذه الخاصية قيمة سلسلة الحقل بين الخادم والتطبيق. ويستخدم أيضا للحقول التي لها نوع **حقيقي** والتي تم تنسيقها كعملة. بالنسبة لهذه الحقول ، يتم استخدام الخاصية لتمرير رمز العملة إلى التطبيق.

### <a name="datevalue-date"></a>dateValue (التاريخ)

بالنسبة للحقول التي لها نوع **التاريخ** ، تمرر هذه الخاصية قيمة تاريخ الحقل بين الخادم والتطبيق.

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a>إظهار حقل مخصص في مقطع إدخال الجدول الزمني وحفظه

فيما يلي لقطه شاشه من تطبيق الجوال لإنشاء إدخال لجدول زمني. يعرض الحقول الجاهزة وحقلًا مخصصًا في قسم "إدخال الوقت" المسمى "سلسلة الاختبار" مع تعيين قيمة تعداد "الخيار الثاني" بالفعل.

![الحقل المخصص لسلسله الاختبار في التطبيق](media/timesheet-entry.jpg)



يوجد أدناه لقطة شاشة من تطبيق الجوال للمستخدم الذي يختار أحد خيارات التعداد المتاحة للحقل المخصص "اختبار السلسلة".  ويكون الخياران هما "الخيار الأول" و "الخيار الثاني" الظاهرين كازرار خيارات. الخيار الثاني محدد حاليا.

![أزرار الخيارات (الأزرار التبادلية) الخاصة بالحقل المخصص لسلسله الاختبار](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a>قم بتوسيع الجدول TSTimesheetLine بحيث يحتوي على حقل مخصص

في السيناريوهات النموذجية ، من المحتمل أن يتم حفظ البيانات الخاصة بالحقل المخصص في قسم إدخال الجدول الزمني في جدول TSTimesheetLine. ومع ذلك ، يمكن استخدام جداول أخرى إذا كان من الممكن استرداد البيانات بناءً على سجل TSTimesheetTrans الذي تم توفيره ، أو إذا لم يكن لديه سياق سجل محدد (على سبيل المثال ، إذا تم تعيين الحقل للقراءة فقط في معلمات المشروع) .

لاحظ أن الحقول المخصصة لا يجب أن تحتوي على أي سجلات قاعدة بيانات داعمة. يمكن إنشاؤها ديناميكيًا بناءً على منطق X ++. يمكن أن يكون هذا الأسلوب مفيدًا في سيناريوهات القراءة فقط (راجع قسم "استخدام سلسلة الأوامر في فئة TSTimesheetDetails ، طريقة buildCustomFieldListForHeader لملء تفاصيل الجدول الزمني" للحصول على مثال لقيم الحقول المخصصة التي تم إنشاؤها ديناميكيًا.)

فيما يلي لقطه شاشة من Visual Studio لشجرة كائنات التطبيق. يعرض امتدادًا لجدول TSTimesheetLine مع إضافة حقل TestLineString كحقل مخصص.

![سلسلة السطر](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a>استخدم سلسلة الأوامر في طريقة buildCustomFieldList لفئة TSTimesheetSettings لإظهار حقل في قسم إدخال الجدول الزمني

يتحكم هذا الرمز في إعدادات العرض للحقل في التطبيق. على سبيل المثال ، يتحكم في نوع الحقل ، والتسمية ، وما إذا كان الحقل إلزاميًا ، وما القسم الذي يظهر فيه الحقل.

يوضح المثال التالي حقل سلسله في إدخالات الوقت. يشتمل هذا الحقل علي خيارين، **الخيار الأول** و **الخيار الثاني** ، والتي تتوفر من خلال أزرار الخيارات (الأزرار التبادلية). ويقترن الحقل الموجود في التطبيق بحقل **TestLineString** الذي تمت اضافته إلى جدول TSTimesheetLine.

لاحظ استخدام أسلوب **TSTimesheetCustomField::newFromMetatdata()** لتبسيط تهيئة خصائص الحقول المخصصة: **fieldBaseType** ، و **tableName** ، و **fieldname** ، و **label** ، و **isEditable** ، و **isMandatory** , **stringLength** ، و **numberOfDecimals**. يمكنك أيضا تعيين هذه المعلمات يدويا ، كما تفضل.

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('Second option');
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a>استخدم سلسلة الأوامر في طريقة buildCustomFieldListForEntry لفئة TSTimesheetEntry لإدخال القيم في إدخال الجدول الزمني

يتم استخدام أسلوب **buildCustomFieldListForEntry** لإدخال القيم في سطور الجدول الزمني المحفوظة في تطبيق الهاتف المحمول. يستغرق سجل TSTimesheetTrans كمعلمة. يمكن استخدام الحقول من هذا السجل لملء قيمة الحقل المخصص في التطبيق.

```xpp
...
[ExtensionOf(classStr(TsTimesheetEntry))]
final class TsTimesheetEntry_Extension
{
    protected List buildCustomFieldListForEntry(TSTimesheetTrans _tsTimesheetTrans)
    {
        List customFieldList = next buildCustomFieldListForEntry(_tsTimesheetTrans);
        TSTimesheetLine tsTimesheetLine = _tsTimesheetTrans.timesheetLine();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        tsTimesheetCustomField.parmStringValue(tsTimesheetLine.TestLineString);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('second option;);
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a>استخدم سلسلة الأوامر في فئة TSTimesheetEntryService لحفظ إدخال الجدول الزمني من التطبيق إلى قاعدة البيانات

لحفظ حقل مخصص مرة أخرى إلى قاعدة البيانات في الاستخدام المعتاد ، يجب توسيع طرق متعددة:

- يتم استخدام أسلوب **timesheetLineNeedsUpdating** لتحديد ما إذا كان قد تم تغيير سجل الخط بواسطة المستخدم في التطبيق ويجب حفظه في قاعدة البيانات. إذا لم يكن الأداء مصدر قلق ، فيمكن تبسيط هذه الطريقة بحيث تُرجع دائمًا **حقيقي**.
- يمكن توسيع أسلوبي **populateTimesheetLineFromEntryDuringCreate** و **populateTimesheetLineFromEntryDuringUpdate** بحيث يقومون بإدخال القيم في سجل قاعدة بيانات TSTimesheetLine من سجل عقد بيانات TSTimesheetEntry الذي يتم توفيره. في المثال التالي ، لاحظ كيف يتم التعيين بين حقل قاعدة البيانات وحقل الإدخال يدويًا عبر كود X ++.
- كما يمكن توسيع أسلوب **populateTimesheetWeekFromEntry** إذا كان الحقل المخصص المعين لكائن **TSTimesheetEntry** يجب إعادة الكتابة إلى جدول قاعدة البيانات TSTimesheetLineweek.

> [!NOTE]
> يقوم المثال التالي بحفظ قيمة **firstOption** أو **secondOption** التي يقوم المستخدم بتحديدها لقاعده بيانات كقيمه سلسلة بسيطة. إذا كان حقل قاعده البيانات هو حقل من نوع **التعداد** ، فيمكن تعيين هذه القيم يدويًا إلى قيمه التعداد ثم حفظها في حقل تعداد في جدول قاعده البيانات.

```xpp
...
[ExtensionOf(classStr(TSTimesheetEntryService))]
final class TSTimesheetEntryService_Extension
{
    protected boolean timesheetLineNeedsUpdating(TSTimesheetLine _tsTimesheetLine,
    TsTimesheetEntry _tsTimesheetEntry)
    {
        boolean ret = next timesheetLineNeedsUpdating(_tsTimesheetLine,
        _tsTimesheetEntry);
        if (!ret)
        {
            */ Loop through custom fields to see if value needs updating*/
            ListEnumerator enumerator =  _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    */ If Custom field value for TestLineString field has changed, We need to update the timesheet line.*/
                    if (_tsTimesheetLine.TestLineString != customField.parmStringValue())
                    {
                        ret = true;
                    }
                }
            }
        }
        return ret;
    }
    protected void populateTimesheetLineFromEntryDuringCreate(TSTimesheetLine
    _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
    {
        next populateTimesheetLineFromEntryDuringCreate(_tsTimesheetLine,
        _tsTimesheetEntry);
        this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
        _tsTimesheetEntry);
        }
        protected void populateTimesheetLineFromEntryDuringUpdate(TSTimesheetLine
        \_tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            next populateTimesheetLineFromEntryDuringUpdate(_tsTimesheetLine,
            _tsTimesheetEntry);
            this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
            _tsTimesheetEntry);
        }
        private void populateTimesheetLineFromCustomFields(TSTimesheetLine
        _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            ListEnumerator enumerator =
            _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    _tsTimesheetLine.TestLineString = customField.parmStringValue();
                }
            }
        }
    }
...
```

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a>عرض حقل مخصص في قسم رأس الجدول الزمني

يوجد أدناه لقطة شاشة من تطبيق الهاتف المحمول لمستخدم يعرض الجدول الزمني. تم تحديد زر "مزيد من المعلومات" في الزاوية العلوية اليمنى لإظهار خيار "عرض المزيد من التفاصيل".  

![أمر عرض المزيد من التفاصيل](media/show-more.png)

يوجد أدناه لقطة شاشة من تطبيق الجوال تعرض قسم "المزيد" في الجدول الزمني. تمت إضافة حقل مخصص يسمى "معدل استخدام الجدول الزمني هذا (حقل مخصص محسوب)" إلى قسم رأس الجدول الزمني. تم تعيين قيمة للقراءة فقط "0.667" في الحقل المخصص.

![قسم المزيد](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a>توسيع جدول TSTimesheetTable بحيث يحتوي على حقل مخصص

في السيناريوهات النموذجية ، من المحتمل أن يتم سحب بيانات حقل مخصص في قسم الرأس من جدول TSTimesheetHeader. ومع ذلك ، يمكن استخدام جداول أخرى إذا كان من الممكن استرداد البيانات بناءً على سجل TSTimesheetTable الذي تم توفيره ، أو إذا لم يكن لديه سياق سجل محدد (على سبيل المثال ، إذا تم تعيين الحقل للقراءة فقط في معلمات المشروع) .

لاحظ أن الحقول المخصصة لا يجب أن تحتوي على أي سجلات قاعدة بيانات داعمة. يمكن إنشاؤها ديناميكيًا بناءً على منطق X ++. يوضح المثال التالي هذا الأسلوب.

الحقول الموجودة في قسم الرأس تكون دائمًا للقراءة فقط في التطبيق.

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a>استخدم سلسلة الأوامر في طريقة buildCustomFieldList لفئة TSTimesheetSettings لإظهار حقل في قسم الرأس

يتحكم هذا الرمز في إعدادات العرض للحقل في التطبيق. على سبيل المثال ، يتحكم في نوع الحقل ، والتسمية ، وما إذا كان الحقل إلزاميًا ، وما القسم الذي يظهر فيه الحقل.

يوضح المثال التالي قيمة محسوبة في قسم الرأس في التطبيق.

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a>استخدم سلسلة الأوامر في طريقة buildCustomFieldListForHeader لفئة TSTimesheetDetails لملء تفاصيل الجدول الزمني

يتم استخدام أسلوب **buildCustomFieldListForHeader** لملء تفاصيل رأس الجدول الزمني في تطبيق الهاتف المحمول. يستغرق سجل TSTimesheetTable كمعلمة. يمكن استخدام الحقول من هذا السجل لملء قيمة الحقل المخصص في التطبيق. المثال التالي لا يقرأ أي قيم من قاعدة البيانات. بدلاً من ذلك ، يستخدم منطق X ++ لإنشاء قيمة محسوبة تظهر بعد ذلك في التطبيق.


```xpp
...
[ExtensionOf(classStr(TSTimesheetDetails))]
final class TSTimesheetDetails_Extension
{
    protected List buildCustomFieldListForHeader(TSTimesheetTable
    _tsTimesheetTable)
    {
        List customFieldList = next buildCustomFieldListForHeader(_tsTimesheetTable);
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        real utilizationRate = 0;
        if (_tsTimesheetTable.totalHours() != 0)
        {
            utilizationRate = _tsTimesheetTable.totalHoursBillable() /
            _tsTimesheetTable.totalHours();
        }
        tsTimesheetCustomField.parmRealValue(utilizationRate);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

## <a name="other-configurabilityextensibility-opportunities"></a>فرص التكوين/القابلية للتوسعة الأخرى

### <a name="adding-additional-validation-for-the-app"></a>إضافة تحقق إضافي للتطبيق

سيظل المنطق الحالي لوظيفة الجدول الزمني على مستوى قاعدة البيانات يعمل كما هو متوقع. لمقاطعة اكتمال عمليات الحفظ أو الإرسال وإظهار رسالة خطأ معينة، يمكنك إضافة **خطأ الطرح ("رسالة إلى المستخدم")** إلى الكود عبر سلسلة من توسيع الأوامر. فيما يلي ثلاثة أمثلة للطرق المفيدة القابلة للتوسيع:

- إذا أرجع **validateWrite** في جدول TSTimesheetLine **خطأ** أثناء عملية حفظ سطر الجدول الزمني ، تظهر رسالة خطأ في تطبيق الهاتف المحمول.
- إذا أرجع **validateSubmit** في جدول TSTimesheetTable **خطأ** أثناء إرسال الجدول الزمني في التطبيق ، تظهر رسالة خطأ للمستخدم.
- المنطق الذي يملأ الحقول (على سبيل المثال، **خاصية البند** ) أثناء تشغيل أسلوب **الإدراج** في جدول TSTimesheetLine.

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a>إخفاء الحقول الجاهزة وتمييزها للقراءة فقط عبر التكوين

من معلمات المشروع ، يمكنك جعل الحقول الجاهزة للقراءة فقط أو مخفية في تطبيق الهاتف المحمول. قم بتعيين الخيارات في قسم **الجداول الزمنية** في علامة التبويب **الجدول الزمني** في صفحة **معلمات المحاسبة وإدارة المشاريع**.

![معلمات المشاريع](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a>تغيير الانشطه المتاحة للتحديد عبر الملحقات

يتم ملء الأنشطة المتاحة للاختيار للمشروع عبر أساليب **getActivitiesForProject()** و **getActivityQuery()** في فئة **TsTimesheetProjectService**. يمكنك استخدام سلسلة الأوامر لتغيير هذا السلوك لمطابقة سيناريو عملك للأنشطة المتاحة للاختيار لمشروع معين.

### <a name="entering-a-default-project-category-on-timesheet-entries"></a>إدخال فئة المشروع الافتراضية في إدخالات الجدول الزمني

يحدث إدخال فئة المشروع الافتراضية في إدخالات الجدول الزمني على ثلاثة مستويات. يمكنك استخدام سلسلة الأوامر لتوسيع السلوك في أي من هذه المستويات أو جميعها لتحقيق السلوك المطلوب. يتم استخدام التسلسل الهرمي التالي:

1. يحاول التطبيق وضع الفئة الافتراضية من مورد المشروع. يتم تعيين هذه الفئة الافتراضية في أسلوبي **getCurrentUserResource** و **getDelegatedResourcesForCurrentUser** في فئة **TSTimesheetSettingsService**.
2. إذا لم يتم توفير الفئة الافتراضية على مستوى موارد المشروع ، فسيحاول التطبيق سحبها من نشاط المشروع. تم تعيين هذه الفئة الافتراضية في أسلوب **getActivitiesForProject** في فئة **TSTimesheetProjectService**.
3. إذا لم يتم توفير الفئة الافتراضية على مستوى نشاط المشروع ، فإن الفئة الافتراضية المأخوذة من معلمات المشروع. تم تعيين هذه الفئة الافتراضية في أسلوب **getProjectDetailsbyRule** في فئة **TSTimesheetProjectService**.
