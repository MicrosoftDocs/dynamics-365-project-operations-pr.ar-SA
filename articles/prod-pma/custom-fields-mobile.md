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
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a><span data-ttu-id="9e3bb-103">تنفيذ الحقول المخصصة لتطبيق الأجهزة المحمولة لـ Microsoft Dynamics 365 Project Timesheet على iOS وAndroid</span><span class="sxs-lookup"><span data-stu-id="9e3bb-103">Implement custom fields for the Microsoft Dynamics 365 Project Timesheet mobile app on iOS and Android</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="9e3bb-104">يقدم هذا الموضوع الأنماط الشائعة لاستخدام الملحقات لتنفيذ الحقول المخصصة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-104">This topic provides common patterns for using extensions to implement custom fields.</span></span> <span data-ttu-id="9e3bb-105">يتم تغطيه الموضوعات التالية:</span><span class="sxs-lookup"><span data-stu-id="9e3bb-105">The following topics are covered:</span></span>

- <span data-ttu-id="9e3bb-106">العديد من أنواع البيانات التي يدعمها اطار عمل الحقل المخصص</span><span class="sxs-lookup"><span data-stu-id="9e3bb-106">The various data types that the custom field framework supports</span></span>
- <span data-ttu-id="9e3bb-107">كيفيه إظهار حقول للقراءة فقط أو قابله للتحرير في إدخالات الجدول الزمني ، وحفظ القيم التي تم توفيرها بالنسبة للمستخدم مره أخرى إلى قاعده البيانات</span><span class="sxs-lookup"><span data-stu-id="9e3bb-107">How to show read-only or editable fields on timesheet entries, and save user-provided values back to the database</span></span>
- <span data-ttu-id="9e3bb-108">كيفيه إظهار حقول القراءة فقط في راس الجدول الزمني</span><span class="sxs-lookup"><span data-stu-id="9e3bb-108">How to show read-only fields on the timesheet header</span></span>
- <span data-ttu-id="9e3bb-109">كيفيه دمج منطق الاعمال المخصصة الأخرى لإدخال القيم الافتراضية في الحقول وإجراء مزيد من التحقق من الصحة</span><span class="sxs-lookup"><span data-stu-id="9e3bb-109">How to integrate other custom business logic to enter default values in fields and do additional validation</span></span>

## <a name="audience"></a><span data-ttu-id="9e3bb-110">الجمهور</span><span class="sxs-lookup"><span data-stu-id="9e3bb-110">Audience</span></span>

<span data-ttu-id="9e3bb-111">وهذا الموضوع مخصص للمطورين الذين يقومون بدمج الحقول المخصصة الخاصة بهم في تطبيق الأجهزة المحمولة لـ Microsoft Dynamics 365 Project Timesheet المتوفر لشركة Apple iOS وGoogle Android.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-111">This topic is intended for developers who are integrating their custom fields into the Microsoft Dynamics 365 Project Timesheet mobile application that is available for Apple iOS and Google Android.</span></span> <span data-ttu-id="9e3bb-112">الافتراض هو أن القراء على دراية بتطوير X ++ ووظائف الجدول الزمني للمشروع.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-112">The assumption is that readers are familiar with X++ development and project timesheet functionality.</span></span>

## <a name="data-contract--tstimesheetcustomfield-x-class"></a><span data-ttu-id="9e3bb-113">عقد البيانات - فئة TSTimesheetCustomField X ++</span><span class="sxs-lookup"><span data-stu-id="9e3bb-113">Data contract – TSTimesheetCustomField X++ class</span></span>

<span data-ttu-id="9e3bb-114">فئة **TSTimesheetCustomField** هي فئة عقد بيانات X ++ التي تمثل معلومات حول حقل مخصص لوظائف الجدول الزمني.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-114">The **TSTimesheetCustomField** class is the X++ data contract class that represents information about a custom field for timesheet functionality.</span></span> <span data-ttu-id="9e3bb-115">يتم تمرير قوائم كائنات الحقول المخصصة في كل من عقد بيانات TSTimesheetDetails وعقد بيانات TSTimesheetEntry لإظهار الحقول المخصصة في تطبيق الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-115">Lists of the custom field objects are passed on both the TSTimesheetDetails data contract and the TSTimesheetEntry data contract to show custom fields in the mobile app.</span></span>

- <span data-ttu-id="9e3bb-116">**TSTimesheetDetails** - عقد رأس الجدول الزمني.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-116">**TSTimesheetDetails** - The timesheet header contract.</span></span>
- <span data-ttu-id="9e3bb-117">**TSTimesheetEntry** - عقد معاملة الجدول الزمني.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-117">**TSTimesheetEntry** - The timesheet transaction contract.</span></span> <span data-ttu-id="9e3bb-118">مجموعات من هذه الكائنات لها نفس معلومات المشروع وقيمة **timesheetLineRecId** تشكل البند.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-118">Groups of these objects that have the same project information and **timesheetLineRecId** value constitute a line.</span></span>

### <a name="fieldbasetype-types"></a><span data-ttu-id="9e3bb-119">fieldBaseType (الأنواع)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-119">fieldBaseType (Types)</span></span>

<span data-ttu-id="9e3bb-120">تحدد خاصية **FieldBaseType** في كائن **TsTimesheetCustom** نوع الحقل الذي يظهر في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-120">The **FieldBaseType** property on the **TsTimesheetCustom** object determines the type of the field that appears in the app.</span></span> <span data-ttu-id="9e3bb-121">قيم **الأنواع** التالية التي يتم دعمها.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-121">The following **Types** values that are supported.</span></span>

| <span data-ttu-id="9e3bb-122">قيمة الأنواع</span><span class="sxs-lookup"><span data-stu-id="9e3bb-122">Types value</span></span> | <span data-ttu-id="9e3bb-123">كتابة</span><span class="sxs-lookup"><span data-stu-id="9e3bb-123">Type</span></span>              | <span data-ttu-id="9e3bb-124">ملاحظات</span><span class="sxs-lookup"><span data-stu-id="9e3bb-124">Notes</span></span> |
|-------------|-------------------|-------|
| <span data-ttu-id="9e3bb-125">1</span><span class="sxs-lookup"><span data-stu-id="9e3bb-125">0</span></span>           | <span data-ttu-id="9e3bb-126">السلسلة (والتعداد)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-126">String (and Enum)</span></span> | <span data-ttu-id="9e3bb-127">يظهر الحقل كحقل نص.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-127">The field appears as a text field.</span></span> |
| <span data-ttu-id="9e3bb-128">1</span><span class="sxs-lookup"><span data-stu-id="9e3bb-128">1</span></span>           | <span data-ttu-id="9e3bb-129">Integer</span><span class="sxs-lookup"><span data-stu-id="9e3bb-129">Integer</span></span>           | <span data-ttu-id="9e3bb-130">يتم عرض القيمة كرقم بدون منازل عشرية.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-130">The value is shown as a number without decimal places.</span></span> |
| <span data-ttu-id="9e3bb-131">2</span><span class="sxs-lookup"><span data-stu-id="9e3bb-131">2</span></span>           | <span data-ttu-id="9e3bb-132">حقيقي</span><span class="sxs-lookup"><span data-stu-id="9e3bb-132">Real</span></span>              | <span data-ttu-id="9e3bb-133">يتم عرض القيمة كرقم بمنازل عشرية.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-133">The value is shown as a number that has decimal places.</span></span><p><span data-ttu-id="9e3bb-134">لإظهار القيمة الفعلية كعملة في التطبيق، استخدم خاصية **fieldExtenededType**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-134">To show the real value as a currency in the app, use the **fieldExtenededType** property.</span></span> <span data-ttu-id="9e3bb-135">يمكنك استخدام خاصية **numberOfDecimals** لتعيين عدد المنازل العشرية المعروضة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-135">You can use the **numberOfDecimals** property to set the number of decimal places that are shown.</span></span></p> |
| <span data-ttu-id="9e3bb-136">3</span><span class="sxs-lookup"><span data-stu-id="9e3bb-136">3</span></span>           | <span data-ttu-id="9e3bb-137">التاريخ</span><span class="sxs-lookup"><span data-stu-id="9e3bb-137">Date</span></span>              | <span data-ttu-id="9e3bb-138">يتم تحديد تنسيقات التاريخ بواسطة إعداد **التاريخ والأوقات وتنسيق الأرقام** الخاص بالمستخدم والذي تم تحديده ضمن **تفضيلات اللغة والبلد/المنطقة** في **خيارات المستخدم**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-138">Date formats are determined by the user's **Date, times, and number format** setting that is specified under **Language and country/region preference** in **User options**.</span></span> |
| <span data-ttu-id="9e3bb-139">4</span><span class="sxs-lookup"><span data-stu-id="9e3bb-139">4</span></span>           | <span data-ttu-id="9e3bb-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e3bb-140">Boolean</span></span>           | |
| <span data-ttu-id="9e3bb-141">15</span><span class="sxs-lookup"><span data-stu-id="9e3bb-141">15</span></span>          | <span data-ttu-id="9e3bb-142">GUID</span><span class="sxs-lookup"><span data-stu-id="9e3bb-142">GUID</span></span>              | |
| <span data-ttu-id="9e3bb-143">16</span><span class="sxs-lookup"><span data-stu-id="9e3bb-143">16</span></span>          | <span data-ttu-id="9e3bb-144">Int64</span><span class="sxs-lookup"><span data-stu-id="9e3bb-144">Int64</span></span>             | |

- <span data-ttu-id="9e3bb-145">إذا لم يتم توفير خاصية **stringOptions** في كائن **TSTimesheetCustomField** ، يتم توفير حقل نص حر للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-145">If the **stringOptions** property isn't provided on the **TSTimesheetCustomField** object, a free-text field is provided to the user.</span></span>

    <span data-ttu-id="9e3bb-146">يمكن استخدام خاصية **stringLength** لتعيين الحد الأقصى لطول السلسلة الذي يمكن للمستخدمين إدخاله.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-146">The **stringLength** property can be used to set the maximum string length that users can enter.</span></span>

- <span data-ttu-id="9e3bb-147">في حالة توفير خاصية **stringOptions** في كائن **TSTimesheetCustomField** ، عناصر هذه القائمة هي القيم الوحيدة التي يمكن للمستخدمين تحديدها باستخدام أزرار الخيارات (الأزرار التبادلية).</span><span class="sxs-lookup"><span data-stu-id="9e3bb-147">If the **stringOptions** property is provided on the **TSTimesheetCustomField** object, those list elements are the only values that users can select by using option buttons (radio buttons).</span></span>

    <span data-ttu-id="9e3bb-148">في هذه الحالة ، يمكن أن يعمل حقل السلسلة كقيمة تعداد لغرض إدخال المستخدم.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-148">In this case, the string field can act as an enum value for the purpose of user entry.</span></span> <span data-ttu-id="9e3bb-149">لحفظ القيمة في قاعدة البيانات كتعداد ، قم يدويًا بتعيين قيمة السلسلة إلى قيمة التعداد قبل الحفظ في قاعدة البيانات باستخدام سلسلة الأوامر (راجع "استخدام سلسلة الأوامر في فئة TSTimesheetEntryService لحفظ إدخال جدول زمني من التطبيق مرة أخرى إلى قسم قاعدة البيانات "لاحقًا في هذا الموضوع على سبيل المثال).</span><span class="sxs-lookup"><span data-stu-id="9e3bb-149">To save the value to the database as an enum, manually map the string value back to the enum value before you save to the database by using chain of command (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a><span data-ttu-id="9e3bb-150">fieldExtendedType ‏(TSCustomFieldExtendedType)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-150">fieldExtendedType (TSCustomFieldExtendedType)</span></span>

<span data-ttu-id="9e3bb-151">يمكنك استخدام هذه الخاصية لتنسيق القيم الفعلية كعمله.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-151">You can use this property to format real values as currency.</span></span> <span data-ttu-id="9e3bb-152">يكون هذا الأسلوب قابلا للتطبيق فقط عندما تكون قيمة **fieldBaseType** هي **حقيقية**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-152">This approach is applicable only when the **fieldBaseType** value is **Real**.</span></span>

- <span data-ttu-id="9e3bb-153">**TSCustomFieldExtendedType:None** – لم يتم تطبيق أي تنسيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-153">**TSCustomFieldExtendedType:None** – No formatting is applied.</span></span>
- <span data-ttu-id="9e3bb-154">**TSCustomFieldExtendedType::العملة** – تنسيق القيمة كعملة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-154">**TSCustomFieldExtendedType::Currency** – Format the value as currency.</span></span>

    <span data-ttu-id="9e3bb-155">عندما يكون تنسيق العملة نشطًا، يمكن استخدام حقل **stringValue** لتمرير رمز العملة الذي يجب ان يظهر في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-155">When currency formatting is active, the **stringValue** field can be used pass the currency code that should be shown in the app.</span></span> <span data-ttu-id="9e3bb-156">القيمة هي قيمه للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-156">The value is a read-only value.</span></span>

    <span data-ttu-id="9e3bb-157">يحتوي حقل **realValue** على المبلغ النقدي الذي ينبغي حفظه إلى قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-157">The **realValue** field contains the money amount that should be saved to the database.</span></span>

### <a name="fieldsection-tscustomfieldsection"></a><span data-ttu-id="9e3bb-158">fieldSection (TSCustomFieldSection)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-158">fieldSection (TSCustomFieldSection)</span></span>

<span data-ttu-id="9e3bb-159">يمكنك استخدام هذه الخاصية لتحديد المكان الذي ينبغي ان يظهر فيه الحقل المخصص في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-159">You can use this property specify where the custom field should appear in the app.</span></span>

- <span data-ttu-id="9e3bb-160">**TSCustomFieldSection::الرأس** – سيظهر الحقل في قسم **عرض المزيد من التفاصيل** في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-160">**TSCustomFieldSection::Header** – The field will appear in the **View more details** section in the app.</span></span> <span data-ttu-id="9e3bb-161">هذه الحقول دائمًا للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-161">These fields are always read-only.</span></span>
- <span data-ttu-id="9e3bb-162">**TSCustomFieldSection::البند** – سيظهر الحقل بعد كل الحقول الجاهزة في إدخالات الجدول الزمني.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-162">**TSCustomFieldSection::Line** – The field will appear after all the out-of-box line fields on timesheet entries.</span></span> <span data-ttu-id="9e3bb-163">يمكن ان تكون هذه الحقول اما قابله للتحرير أو للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-163">These fields can be either editable or read-only.</span></span>

### <a name="fieldname-fieldnameshort"></a><span data-ttu-id="9e3bb-164">fieldName (FieldNameShort)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-164">fieldName (FieldNameShort)</span></span>

<span data-ttu-id="9e3bb-165">تحدد هذه الخاصية الحقل عندما يتم حفظ القيم التي يوفرها التطبيق مره أخرى إلى قاعده البيانات.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-165">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="tablename-tablenameshort"></a><span data-ttu-id="9e3bb-166">tableName (TableNameShort)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-166">tableName (TableNameShort)</span></span>

<span data-ttu-id="9e3bb-167">تحدد هذه الخاصية الحقل عندما يتم حفظ القيم التي يوفرها التطبيق مره أخرى إلى قاعده البيانات.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-167">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="iseditable-noyes"></a><span data-ttu-id="9e3bb-168">isEditable (NoYes)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-168">isEditable (NoYes)</span></span>

<span data-ttu-id="9e3bb-169">قم بتعيين هذه الخاصية إلى **نعم** لتحديد أن الحقل الموجود في مقطع "إدخال الجدول الزمني" يجب ان يكون قابلا للتحرير من قبل المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-169">Set this property to **Yes** to specify that the field in the timesheet entry section should be editable by users.</span></span> <span data-ttu-id="9e3bb-170">قم بتعيين الخاصية إلى **لا** لجعل الحقل للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-170">Set the property to **No** to make the field read-only.</span></span>

### <a name="ismandatory-noyes"></a><span data-ttu-id="9e3bb-171">isMandatory (NoYes)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-171">isMandatory (NoYes)</span></span>

<span data-ttu-id="9e3bb-172">قم بتعيين هذه الخاصية إلى **نعم** لتحديد أن الحقل في قسم إدخال الجدول الزمني يجب أن يكون إلزاميًا.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-172">Set this property to **Yes** to specify that the field in the timesheet entry section should be mandatory.</span></span>

### <a name="label-str"></a><span data-ttu-id="9e3bb-173">التسمية (سلسلة)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-173">label (str)</span></span>

<span data-ttu-id="9e3bb-174">تحدد هذه الخاصية التسمية التي تظهر بعد الحقل في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-174">This property specifies the label that is shown next the field in the app.</span></span>

### <a name="stringoptions-list-of-strings"></a><span data-ttu-id="9e3bb-175">stringOptions (قائمة السلاسل)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-175">stringOptions (List of Strings)</span></span>

<span data-ttu-id="9e3bb-176">تكون هذه الخاصية قابله للتطبيق فقط عندما يتم تعيين **fieldBaseType** إلى **السلسلة**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-176">This property is applicable only when **fieldBaseType** is set to **String**.</span></span> <span data-ttu-id="9e3bb-177">إذا تم تعيين **stringOptions** ، يتم تحديد قيم السلسلة المتاحة للتحديد عبر أزرار الخيارات (أزرار الاختيار) بواسطة السلاسل الموجودة في القائمة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-177">If **stringOptions** is set, the string values that are available for selection via option buttons (radio buttons) are specified by the strings in the list.</span></span> <span data-ttu-id="9e3bb-178">يتم تحديد قيم السلسلة المتاحة للتحديد عبر أزرار الخيارات (أزرار الاختيار) بواسطة السلاسل الموجودة في القائمة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-178">If no strings are provided, free-text entry in the string field is allowed (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="stringlength-int"></a><span data-ttu-id="9e3bb-179">stringLength (int)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-179">stringLength (int)</span></span>

<span data-ttu-id="9e3bb-180">تحدد هذه الخاصية الحد الأقصى لطول حقل السلسلة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-180">This property specifies the maximum length for a string field.</span></span> <span data-ttu-id="9e3bb-181">هذه الخاصية قابله للتطبيق فقط عندما يتم تعيين **fieldBaseType** إلى **السلسلة**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-181">It's applicable only when **fieldBaseType** is set to **String**.</span></span>

### <a name="numberofdecimals-int"></a><span data-ttu-id="9e3bb-182">numberOfDecimals (int)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-182">numberOfDecimals (int)</span></span>

<span data-ttu-id="9e3bb-183">تحدد هذه الخاصية عدد المنازل العشرية التي يتم عرضها للحقل الحقيقي.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-183">This property specifies the number of decimal places that are shown for a real field.</span></span> <span data-ttu-id="9e3bb-184">هذه الخاصية قابله للتطبيق فقط عندما يتم تعيين **fieldBaseType** إلى **حقيقي**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-184">It's applicable only when **fieldBaseType** is set to **Real**.</span></span>

### <a name="ordersequence-int"></a><span data-ttu-id="9e3bb-185">orderSequence (int)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-185">orderSequence (int)</span></span>

<span data-ttu-id="9e3bb-186">تتحكم هذه الخاصية بالترتيب الذي يتم به عرض الحقول المخصصة في التطبيق عندما يتم تحديد أكثر من حقل مخصص واحد.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-186">This property controls the order in which the custom fields are shown in the app when more than one custom field is specified.</span></span> <span data-ttu-id="9e3bb-187">يتم عرض الحقول التي تحتوي علي أرقام اقل أولا.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-187">Fields that have lower numbers are shown first.</span></span>

### <a name="booleanvalue-boolean"></a><span data-ttu-id="9e3bb-188">booleanValue (منطقية)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-188">booleanValue (boolean)</span></span>

<span data-ttu-id="9e3bb-189">بالنسبة للحقول التي لها النوع **المنطقي** ، تمرر هذه الخاصية القيمة المنطقية للحقل بين الخادم والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-189">For fields of the **Boolean** type, this property passes the Boolean value of the field between the server and the app.</span></span>

### <a name="guidvalue-guid"></a><span data-ttu-id="9e3bb-190">guidValue (guid)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-190">guidValue (guid)</span></span>

<span data-ttu-id="9e3bb-191">بالنسبة للحقول التي لها النوع **GUID** ، تمرر هذه الخاصية قيمة المعرف الفريد العمومي (GUID) للحقل بين الخادم والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-191">For fields of the **GUID** type, this property passes the globally unique identifier (GUID) value of the field between the server and the app.</span></span>

### <a name="int64value-int64"></a><span data-ttu-id="9e3bb-192">int64Value (int64)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-192">int64Value (int64)</span></span>

<span data-ttu-id="9e3bb-193">بالنسبة للحقول التي لها النوع **Int64** ، تمرر هذه الخاصية قيمة int64 للحقل بين الخادم والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-193">For fields of the **Int64** type, this property passes the int64 value of the field between the server and the app.</span></span>

### <a name="intvalue-int"></a><span data-ttu-id="9e3bb-194">intValue (int)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-194">intValue (int)</span></span>

<span data-ttu-id="9e3bb-195">بالنسبة للحقول التي لها النوع **Int** ، تمرر هذه الخاصية القيمة int للحقل بين الخادم والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-195">For fields of the **Int** type, this property passes the int value of the field between the server and the app.</span></span>

### <a name="realvalue-real"></a><span data-ttu-id="9e3bb-196">realValue (حقيقي)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-196">realValue (real)</span></span>

<span data-ttu-id="9e3bb-197">بالنسبة للحقول التي لها النوع **حقيقي** ، تمرر هذه الخاصية القيمة الحقيقية للحقل بين الخادم والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-197">For fields of the **Real** type, this property passes the real value of the field between the server and the app .</span></span>

### <a name="stringvalue-str"></a><span data-ttu-id="9e3bb-198">stringValue (السلسلة)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-198">stringValue (str)</span></span>

<span data-ttu-id="9e3bb-199">بالنسبة للحقول التي لها النوع **سلسلة** ، تمرر هذه الخاصية قيمة سلسلة الحقل بين الخادم والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-199">For fields of the **String** type, this property passes the string value of the field between the server and the app.</span></span> <span data-ttu-id="9e3bb-200">ويستخدم أيضا للحقول التي لها نوع **حقيقي** والتي تم تنسيقها كعملة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-200">It's also used for fields of the **Real** type that are formatted as currency.</span></span> <span data-ttu-id="9e3bb-201">بالنسبة لهذه الحقول ، يتم استخدام الخاصية لتمرير رمز العملة إلى التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-201">For those fields, the property is used to pass the currency code to the app.</span></span>

### <a name="datevalue-date"></a><span data-ttu-id="9e3bb-202">dateValue (التاريخ)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-202">dateValue (date)</span></span>

<span data-ttu-id="9e3bb-203">بالنسبة للحقول التي لها نوع **التاريخ** ، تمرر هذه الخاصية قيمة تاريخ الحقل بين الخادم والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-203">For fields of the **Date** type, this property passes the date value of the field between the server and the app.</span></span>

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a><span data-ttu-id="9e3bb-204">إظهار حقل مخصص في مقطع إدخال الجدول الزمني وحفظه</span><span class="sxs-lookup"><span data-stu-id="9e3bb-204">Show and save a custom field in the timesheet entry section</span></span>

<span data-ttu-id="9e3bb-205">فيما يلي لقطه شاشه من تطبيق الجوال لإنشاء إدخال لجدول زمني.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-205">Below is a screenshot from the mobile app of a timesheet entry creation.</span></span> <span data-ttu-id="9e3bb-206">يعرض الحقول الجاهزة وحقلًا مخصصًا في قسم "إدخال الوقت" المسمى "سلسلة الاختبار" مع تعيين قيمة تعداد "الخيار الثاني" بالفعل.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-206">It shows the out-of-box fields and a custom field in the "Time entry" section called "Test string" with an enum value of "Second option" already set.</span></span>

![الحقل المخصص لسلسله الاختبار في التطبيق](media/timesheet-entry.jpg)



<span data-ttu-id="9e3bb-208">يوجد أدناه لقطة شاشة من تطبيق الجوال للمستخدم الذي يختار أحد خيارات التعداد المتاحة للحقل المخصص "اختبار السلسلة".</span><span class="sxs-lookup"><span data-stu-id="9e3bb-208">Below is a screenshot from the mobile app of the user selecting one of the enum options available for the "Test string" custom field.</span></span>  <span data-ttu-id="9e3bb-209">ويكون الخياران هما "الخيار الأول" و "الخيار الثاني" الظاهرين كازرار خيارات.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-209">The two options are "First option" and "Second option" shown as radio buttons.</span></span> <span data-ttu-id="9e3bb-210">الخيار الثاني محدد حاليا.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-210">The second option is currently selected.</span></span>

![أزرار الخيارات (الأزرار التبادلية) الخاصة بالحقل المخصص لسلسله الاختبار](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="9e3bb-212">قم بتوسيع الجدول TSTimesheetLine بحيث يحتوي على حقل مخصص</span><span class="sxs-lookup"><span data-stu-id="9e3bb-212">Extend the TSTimesheetLine table so that it has a custom field</span></span>

<span data-ttu-id="9e3bb-213">في السيناريوهات النموذجية ، من المحتمل أن يتم حفظ البيانات الخاصة بالحقل المخصص في قسم إدخال الجدول الزمني في جدول TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-213">In typical scenarios, it's likely that the data for a custom field in the timesheet entry section will be saved to the TSTimesheetLine table.</span></span> <span data-ttu-id="9e3bb-214">ومع ذلك ، يمكن استخدام جداول أخرى إذا كان من الممكن استرداد البيانات بناءً على سجل TSTimesheetTrans الذي تم توفيره ، أو إذا لم يكن لديه سياق سجل محدد (على سبيل المثال ، إذا تم تعيين الحقل للقراءة فقط في معلمات المشروع) .</span><span class="sxs-lookup"><span data-stu-id="9e3bb-214">However, other tables can be used if the data can be retrieved based on a TSTimesheetTrans record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="9e3bb-215">لاحظ أن الحقول المخصصة لا يجب أن تحتوي على أي سجلات قاعدة بيانات داعمة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-215">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="9e3bb-216">يمكن إنشاؤها ديناميكيًا بناءً على منطق X ++.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-216">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="9e3bb-217">يمكن أن يكون هذا الأسلوب مفيدًا في سيناريوهات القراءة فقط (راجع قسم "استخدام سلسلة الأوامر في فئة TSTimesheetDetails ، طريقة buildCustomFieldListForHeader لملء تفاصيل الجدول الزمني" للحصول على مثال لقيم الحقول المخصصة التي تم إنشاؤها ديناميكيًا.)</span><span class="sxs-lookup"><span data-stu-id="9e3bb-217">This approach can be useful in read-only scenarios (see the “Use chain of command on the TSTimesheetDetails class, buildCustomFieldListForHeader method to fill in timesheet details” section for an example of dynamically generated custom field values.)</span></span>

<span data-ttu-id="9e3bb-218">فيما يلي لقطه شاشة من Visual Studio لشجرة كائنات التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-218">Below is a screenshot from Visual Studio of the Application Object Tree.</span></span> <span data-ttu-id="9e3bb-219">يعرض امتدادًا لجدول TSTimesheetLine مع إضافة حقل TestLineString كحقل مخصص.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-219">It shows an extension of the TSTimesheetLine table with the TestLineString field added as a custom field.</span></span>

![سلسلة السطر](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a><span data-ttu-id="9e3bb-221">استخدم سلسلة الأوامر في طريقة buildCustomFieldList لفئة TSTimesheetSettings لإظهار حقل في قسم إدخال الجدول الزمني</span><span class="sxs-lookup"><span data-stu-id="9e3bb-221">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the timesheet entry section</span></span>

<span data-ttu-id="9e3bb-222">يتحكم هذا الرمز في إعدادات العرض للحقل في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-222">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="9e3bb-223">على سبيل المثال ، يتحكم في نوع الحقل ، والتسمية ، وما إذا كان الحقل إلزاميًا ، وما القسم الذي يظهر فيه الحقل.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-223">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="9e3bb-224">يوضح المثال التالي حقل سلسله في إدخالات الوقت.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-224">The following example shows a string field on time entries.</span></span> <span data-ttu-id="9e3bb-225">يشتمل هذا الحقل علي خيارين، **الخيار الأول** و **الخيار الثاني** ، والتي تتوفر من خلال أزرار الخيارات (الأزرار التبادلية).</span><span class="sxs-lookup"><span data-stu-id="9e3bb-225">This field has two options, **First option** and **Second option** , that are available via option buttons (radio buttons).</span></span> <span data-ttu-id="9e3bb-226">ويقترن الحقل الموجود في التطبيق بحقل **TestLineString** الذي تمت اضافته إلى جدول TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-226">The field in the app is associated with the **TestLineString** field that is added to the TSTimesheetLine table.</span></span>

<span data-ttu-id="9e3bb-227">لاحظ استخدام أسلوب **TSTimesheetCustomField::newFromMetatdata()** لتبسيط تهيئة خصائص الحقول المخصصة: **fieldBaseType** ، و **tableName** ، و **fieldname** ، و **label** ، و **isEditable** ، و **isMandatory** , **stringLength** ، و **numberOfDecimals**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-227">Note the use of the **TSTimesheetCustomField::newFromMetatdata()** method to simplify the initialization of the custom field properties: **fieldBaseType** , **tableName** , **fieldname** , **label** , **isEditable** , **isMandatory** , **stringLength** , and **numberOfDecimals**.</span></span> <span data-ttu-id="9e3bb-228">يمكنك أيضا تعيين هذه المعلمات يدويا ، كما تفضل.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-228">You can also set these parameters manually, as you prefer.</span></span>

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a><span data-ttu-id="9e3bb-229">استخدم سلسلة الأوامر في طريقة buildCustomFieldListForEntry لفئة TSTimesheetEntry لإدخال القيم في إدخال الجدول الزمني</span><span class="sxs-lookup"><span data-stu-id="9e3bb-229">Use chain of command on the buildCustomFieldListForEntry method of the TSTimesheetEntry class to enter values in a timesheet entry</span></span>

<span data-ttu-id="9e3bb-230">يتم استخدام أسلوب **buildCustomFieldListForEntry** لإدخال القيم في سطور الجدول الزمني المحفوظة في تطبيق الهاتف المحمول.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-230">The **buildCustomFieldListForEntry** method is used to enter values on the saved timesheet lines in the mobile app.</span></span> <span data-ttu-id="9e3bb-231">يستغرق سجل TSTimesheetTrans كمعلمة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-231">It takes a TSTimesheetTrans record as a parameter.</span></span> <span data-ttu-id="9e3bb-232">يمكن استخدام الحقول من هذا السجل لملء قيمة الحقل المخصص في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-232">Fields from that record can be used to fill in the custom field value in the app.</span></span>

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

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a><span data-ttu-id="9e3bb-233">استخدم سلسلة الأوامر في فئة TSTimesheetEntryService لحفظ إدخال الجدول الزمني من التطبيق إلى قاعدة البيانات</span><span class="sxs-lookup"><span data-stu-id="9e3bb-233">Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database</span></span>

<span data-ttu-id="9e3bb-234">لحفظ حقل مخصص مرة أخرى إلى قاعدة البيانات في الاستخدام المعتاد ، يجب توسيع طرق متعددة:</span><span class="sxs-lookup"><span data-stu-id="9e3bb-234">To save a custom field back to the database in typical usage, you must extend multiple methods:</span></span>

- <span data-ttu-id="9e3bb-235">يتم استخدام أسلوب **timesheetLineNeedsUpdating** لتحديد ما إذا كان قد تم تغيير سجل الخط بواسطة المستخدم في التطبيق ويجب حفظه في قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-235">The **timesheetLineNeedsUpdating** method is used to determine whether the line record has been changed by the user in the app and must be saved to the database.</span></span> <span data-ttu-id="9e3bb-236">إذا لم يكن الأداء مصدر قلق ، فيمكن تبسيط هذه الطريقة بحيث تُرجع دائمًا **حقيقي**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-236">If performance isn't a concern, this method can be simplified so that it always returns **true**.</span></span>
- <span data-ttu-id="9e3bb-237">يمكن توسيع أسلوبي **populateTimesheetLineFromEntryDuringCreate** و **populateTimesheetLineFromEntryDuringUpdate** بحيث يقومون بإدخال القيم في سجل قاعدة بيانات TSTimesheetLine من سجل عقد بيانات TSTimesheetEntry الذي يتم توفيره.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-237">The **populateTimesheetLineFromEntryDuringCreate** and **populateTimesheetLineFromEntryDuringUpdate** methods can be extended so that they enter values in the TSTimesheetLine database record from the TSTimesheetEntry data contract record that is provided.</span></span> <span data-ttu-id="9e3bb-238">في المثال التالي ، لاحظ كيف يتم التعيين بين حقل قاعدة البيانات وحقل الإدخال يدويًا عبر كود X ++.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-238">In the example that follows, notice how the mapping between the database field and the entry field is manually done via X++ code.</span></span>
- <span data-ttu-id="9e3bb-239">كما يمكن توسيع أسلوب **populateTimesheetWeekFromEntry** إذا كان الحقل المخصص المعين لكائن **TSTimesheetEntry** يجب إعادة الكتابة إلى جدول قاعدة البيانات TSTimesheetLineweek.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-239">The **populateTimesheetWeekFromEntry** method can also be extended if the custom field that is mapped to the **TSTimesheetEntry** object must write back to the TSTimesheetLineweek database table.</span></span>

> [!NOTE]
> <span data-ttu-id="9e3bb-240">يقوم المثال التالي بحفظ قيمة **firstOption** أو **secondOption** التي يقوم المستخدم بتحديدها لقاعده بيانات كقيمه سلسلة بسيطة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-240">The following example saves the **firstOption** or **secondOption** value that the user selects to the database as a raw string value.</span></span> <span data-ttu-id="9e3bb-241">إذا كان حقل قاعده البيانات هو حقل من نوع **التعداد** ، فيمكن تعيين هذه القيم يدويًا إلى قيمه التعداد ثم حفظها في حقل تعداد في جدول قاعده البيانات.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-241">If the database field is a field of the **Enum** type, those values can be manually mapped to an enum value and then saved to an enum field on the database table.</span></span>

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

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a><span data-ttu-id="9e3bb-242">عرض حقل مخصص في قسم رأس الجدول الزمني</span><span class="sxs-lookup"><span data-stu-id="9e3bb-242">Show a custom field in the timesheet header section</span></span>

<span data-ttu-id="9e3bb-243">يوجد أدناه لقطة شاشة من تطبيق الهاتف المحمول لمستخدم يعرض الجدول الزمني.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-243">Below is a screenshot from the mobile app of a user viewing a timesheet.</span></span> <span data-ttu-id="9e3bb-244">تم تحديد زر "مزيد من المعلومات" في الزاوية العلوية اليمنى لإظهار خيار "عرض المزيد من التفاصيل".</span><span class="sxs-lookup"><span data-stu-id="9e3bb-244">The "More information" button has been selected in the upper-right corner to show the "View more details" option.</span></span>  

![أمر عرض المزيد من التفاصيل](media/show-more.png)

<span data-ttu-id="9e3bb-246">يوجد أدناه لقطة شاشة من تطبيق الجوال تعرض قسم "المزيد" في الجدول الزمني.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-246">Below is a screenshot from the mobile app showing the “More” section of a timesheet.</span></span> <span data-ttu-id="9e3bb-247">تمت إضافة حقل مخصص يسمى "معدل استخدام الجدول الزمني هذا (حقل مخصص محسوب)" إلى قسم رأس الجدول الزمني.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-247">A custom field called “Utilization rate of this timesheet (computed custom field)” has been added to the timesheet header section.</span></span> <span data-ttu-id="9e3bb-248">تم تعيين قيمة للقراءة فقط "0.667" في الحقل المخصص.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-248">A read-only value of "0.667" is set on the custom field.</span></span>

![قسم المزيد](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="9e3bb-250">توسيع جدول TSTimesheetTable بحيث يحتوي على حقل مخصص</span><span class="sxs-lookup"><span data-stu-id="9e3bb-250">Extend the TSTimesheetTable table so that it has a custom field</span></span>

<span data-ttu-id="9e3bb-251">في السيناريوهات النموذجية ، من المحتمل أن يتم سحب بيانات حقل مخصص في قسم الرأس من جدول TSTimesheetHeader.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-251">In typical scenarios, it's likely that the data for a custom field in the header section will be pulled from the TSTimesheetHeader table.</span></span> <span data-ttu-id="9e3bb-252">ومع ذلك ، يمكن استخدام جداول أخرى إذا كان من الممكن استرداد البيانات بناءً على سجل TSTimesheetTable الذي تم توفيره ، أو إذا لم يكن لديه سياق سجل محدد (على سبيل المثال ، إذا تم تعيين الحقل للقراءة فقط في معلمات المشروع) .</span><span class="sxs-lookup"><span data-stu-id="9e3bb-252">However, other tables can be used if the data can be retrieved based on a TSTimesheetTable record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="9e3bb-253">لاحظ أن الحقول المخصصة لا يجب أن تحتوي على أي سجلات قاعدة بيانات داعمة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-253">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="9e3bb-254">يمكن إنشاؤها ديناميكيًا بناءً على منطق X ++.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-254">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="9e3bb-255">يوضح المثال التالي هذا الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-255">The example that follows shows this approach.</span></span>

<span data-ttu-id="9e3bb-256">الحقول الموجودة في قسم الرأس تكون دائمًا للقراءة فقط في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-256">Fields in the header section are always read-only in the app.</span></span>

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a><span data-ttu-id="9e3bb-257">استخدم سلسلة الأوامر في طريقة buildCustomFieldList لفئة TSTimesheetSettings لإظهار حقل في قسم الرأس</span><span class="sxs-lookup"><span data-stu-id="9e3bb-257">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the header section</span></span>

<span data-ttu-id="9e3bb-258">يتحكم هذا الرمز في إعدادات العرض للحقل في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-258">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="9e3bb-259">على سبيل المثال ، يتحكم في نوع الحقل ، والتسمية ، وما إذا كان الحقل إلزاميًا ، وما القسم الذي يظهر فيه الحقل.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-259">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="9e3bb-260">يوضح المثال التالي قيمة محسوبة في قسم الرأس في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-260">The following example shows a computed value in the header section in the app.</span></span>

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a><span data-ttu-id="9e3bb-261">استخدم سلسلة الأوامر في طريقة buildCustomFieldListForHeader لفئة TSTimesheetDetails لملء تفاصيل الجدول الزمني</span><span class="sxs-lookup"><span data-stu-id="9e3bb-261">Use chain of command on the buildCustomFieldListForHeader method of the TSTimesheetDetails class to fill in timesheet details</span></span>

<span data-ttu-id="9e3bb-262">يتم استخدام أسلوب **buildCustomFieldListForHeader** لملء تفاصيل رأس الجدول الزمني في تطبيق الهاتف المحمول.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-262">The **buildCustomFieldListForHeader** method is used to fill in the timesheet header details in the mobile app.</span></span> <span data-ttu-id="9e3bb-263">يستغرق سجل TSTimesheetTable كمعلمة.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-263">It takes a TSTimesheetTable record as a parameter.</span></span> <span data-ttu-id="9e3bb-264">يمكن استخدام الحقول من هذا السجل لملء قيمة الحقل المخصص في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-264">Fields from that record can be used to fill in the custom field value in the app.</span></span> <span data-ttu-id="9e3bb-265">المثال التالي لا يقرأ أي قيم من قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-265">The following example doesn't read any values from the database.</span></span> <span data-ttu-id="9e3bb-266">بدلاً من ذلك ، يستخدم منطق X ++ لإنشاء قيمة محسوبة تظهر بعد ذلك في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-266">Instead, it uses X++ logic to generate a computed value that is then shown in the app.</span></span>


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

## <a name="other-configurabilityextensibility-opportunities"></a><span data-ttu-id="9e3bb-267">فرص التكوين/القابلية للتوسعة الأخرى</span><span class="sxs-lookup"><span data-stu-id="9e3bb-267">Other configurability/extensibility opportunities</span></span>

### <a name="adding-additional-validation-for-the-app"></a><span data-ttu-id="9e3bb-268">إضافة تحقق إضافي للتطبيق</span><span class="sxs-lookup"><span data-stu-id="9e3bb-268">Adding additional validation for the app</span></span>

<span data-ttu-id="9e3bb-269">سيظل المنطق الحالي لوظيفة الجدول الزمني على مستوى قاعدة البيانات يعمل كما هو متوقع.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-269">Existing logic for timesheet functionality at the database level will still work as expected.</span></span> <span data-ttu-id="9e3bb-270">لمقاطعة اكتمال عمليات الحفظ أو الإرسال وإظهار رسالة خطأ معينة، يمكنك إضافة **خطأ الطرح ("رسالة إلى المستخدم")** إلى الكود عبر سلسلة من توسيع الأوامر.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-270">To interrupt the completion of save or submit operations and show a specific error message, you can add **throw error("message to user")** to the code via a chain of command extension.</span></span> <span data-ttu-id="9e3bb-271">فيما يلي ثلاثة أمثلة للطرق المفيدة القابلة للتوسيع:</span><span class="sxs-lookup"><span data-stu-id="9e3bb-271">Here are three examples of useful extensible methods:</span></span>

- <span data-ttu-id="9e3bb-272">إذا أرجع **validateWrite** في جدول TSTimesheetLine **خطأ** أثناء عملية حفظ سطر الجدول الزمني ، تظهر رسالة خطأ في تطبيق الهاتف المحمول.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-272">If **validateWrite** on the TSTimesheetLine table returns **false** during a save operation for a timesheet line, an error message is shown in the mobile app.</span></span>
- <span data-ttu-id="9e3bb-273">إذا أرجع **validateSubmit** في جدول TSTimesheetTable **خطأ** أثناء إرسال الجدول الزمني في التطبيق ، تظهر رسالة خطأ للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-273">If **validateSubmit** on the TSTimesheetTable table returns **false** during timesheet submission in the app, an error message is shown to the user.</span></span>
- <span data-ttu-id="9e3bb-274">المنطق الذي يملأ الحقول (على سبيل المثال، **خاصية البند** ) أثناء تشغيل أسلوب **الإدراج** في جدول TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-274">Logic that fills in fields (for example, **Line Property** ) during the **insert** method on the TSTimesheetLine table will still run.</span></span>

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a><span data-ttu-id="9e3bb-275">إخفاء الحقول الجاهزة وتمييزها للقراءة فقط عبر التكوين</span><span class="sxs-lookup"><span data-stu-id="9e3bb-275">Hiding and marking out-of-box fields as read-only via configuration</span></span>

<span data-ttu-id="9e3bb-276">من معلمات المشروع ، يمكنك جعل الحقول الجاهزة للقراءة فقط أو مخفية في تطبيق الهاتف المحمول.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-276">From the project parameters, you can make out-of-box fields read-only or hidden in the mobile app.</span></span> <span data-ttu-id="9e3bb-277">قم بتعيين الخيارات في قسم **الجداول الزمنية** في علامة التبويب **الجدول الزمني** في صفحة **معلمات المحاسبة وإدارة المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-277">Set the options in the **Mobile timesheets** section on the **Timesheet** tab of the **Project management and accounting parameters** page.</span></span>

![معلمات المشاريع](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a><span data-ttu-id="9e3bb-279">تغيير الانشطه المتاحة للتحديد عبر الملحقات</span><span class="sxs-lookup"><span data-stu-id="9e3bb-279">Changing the activities that are available for selection via extensions</span></span>

<span data-ttu-id="9e3bb-280">يتم ملء الأنشطة المتاحة للاختيار للمشروع عبر أساليب **getActivitiesForProject()** و **getActivityQuery()** في فئة **TsTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-280">The activities that are available for selection for a project are filled in via the **getActivitiesForProject()** and **getActivityQuery()** methods in the **TsTimesheetProjectService** class.</span></span> <span data-ttu-id="9e3bb-281">يمكنك استخدام سلسلة الأوامر لتغيير هذا السلوك لمطابقة سيناريو عملك للأنشطة المتاحة للاختيار لمشروع معين.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-281">You can use chain of command to change this behavior to match your business scenario for the activities that are available for selection for a specific project.</span></span>

### <a name="entering-a-default-project-category-on-timesheet-entries"></a><span data-ttu-id="9e3bb-282">إدخال فئة المشروع الافتراضية في إدخالات الجدول الزمني</span><span class="sxs-lookup"><span data-stu-id="9e3bb-282">Entering a default project category on timesheet entries</span></span>

<span data-ttu-id="9e3bb-283">يحدث إدخال فئة المشروع الافتراضية في إدخالات الجدول الزمني على ثلاثة مستويات.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-283">Entry of a default project category on timesheet entries occurs at three levels.</span></span> <span data-ttu-id="9e3bb-284">يمكنك استخدام سلسلة الأوامر لتوسيع السلوك في أي من هذه المستويات أو جميعها لتحقيق السلوك المطلوب.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-284">You can use chain of command to extend the behavior at any or all of these levels to achieve the desired behavior.</span></span> <span data-ttu-id="9e3bb-285">يتم استخدام التسلسل الهرمي التالي:</span><span class="sxs-lookup"><span data-stu-id="9e3bb-285">The following hierarchy is used:</span></span>

1. <span data-ttu-id="9e3bb-286">يحاول التطبيق وضع الفئة الافتراضية من مورد المشروع.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-286">The app tries to put the default category from the project resource.</span></span> <span data-ttu-id="9e3bb-287">يتم تعيين هذه الفئة الافتراضية في أسلوبي **getCurrentUserResource** و **getDelegatedResourcesForCurrentUser** في فئة **TSTimesheetSettingsService**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-287">This default category is set in the **getCurrentUserResource** and **getDelegatedResourcesForCurrentUser** methods in the **TSTimesheetSettingsService** class.</span></span>
2. <span data-ttu-id="9e3bb-288">إذا لم يتم توفير الفئة الافتراضية على مستوى موارد المشروع ، فسيحاول التطبيق سحبها من نشاط المشروع.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-288">If the default category isn't provided at the project resource level, the app tries to pull it from the project activity.</span></span> <span data-ttu-id="9e3bb-289">تم تعيين هذه الفئة الافتراضية في أسلوب **getActivitiesForProject** في فئة **TSTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-289">This default category is set in the **getActivitiesForProject** method in the **TSTimesheetProjectService** class.</span></span>
3. <span data-ttu-id="9e3bb-290">إذا لم يتم توفير الفئة الافتراضية على مستوى نشاط المشروع ، فإن الفئة الافتراضية المأخوذة من معلمات المشروع.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-290">If the default category isn't provided at the project activity level, the default category it taken from the project parameters.</span></span> <span data-ttu-id="9e3bb-291">تم تعيين هذه الفئة الافتراضية في أسلوب **getProjectDetailsbyRule** في فئة **TSTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-291">This default category is set in the **getProjectDetailsbyRule** method in the **TSTimesheetProjectService** class.</span></span>
