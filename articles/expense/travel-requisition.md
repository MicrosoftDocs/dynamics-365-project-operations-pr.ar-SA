---
title: طلبات السفر
description: يقدم هذا الموضوع معلومات حول طلبات السفر.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 46a678ac4486c99f11d74dbac07dedd08364cb2f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123656"
---
# <a name="travel-requisitions"></a><span data-ttu-id="ac28c-103">طلبات السفر</span><span class="sxs-lookup"><span data-stu-id="ac28c-103">Travel requisitions</span></span>

<span data-ttu-id="ac28c-104">_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_</span><span class="sxs-lookup"><span data-stu-id="ac28c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ac28c-105">يسرد طلب السفر المصروفات التي سيتم تكبدها وفقًا للغرض من السفر.</span><span class="sxs-lookup"><span data-stu-id="ac28c-105">A travel requisition lists the expenses that will be incurred for the purpose of travel.</span></span> <span data-ttu-id="ac28c-106">يتم إرسال طلب السفر للمراجعة ويمكن استخدامه لتخويل المصروفات.</span><span class="sxs-lookup"><span data-stu-id="ac28c-106">A travel requisition is submitted for review and can be used to authorize expenses.</span></span>

<span data-ttu-id="ac28c-107">قد تتم مطالبتك بإرسال طلب السفر قبل تكبد أي مصروفات يتم سدادها للمؤسسة.</span><span class="sxs-lookup"><span data-stu-id="ac28c-107">You may be required to submit a travel requisition before you incur any expense that is charged to the organization.</span></span> <span data-ttu-id="ac28c-108">ينطبق هذا المطلب، بغض النظر عما إذا كنت تقوم بقيد المصروفات على بطاقة ائتمان شركة، أم تنفق النقدية التي استلمتها من السلفة النقدية، أم تتكبد مصروفات خارج الجيب والتي سيتم تعويضها بواسطة المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="ac28c-108">This requirement applies, regardless of whether you charge expenses to a corporate credit card, spend cash that you received from a cash advance, or incur out-of-pocket expenses that will be reimbursed by the organization.</span></span>

<span data-ttu-id="ac28c-109">يمكن استخدام سياسات وطلبات السفر للمساعدة في إدارة نفقات المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="ac28c-109">Travel requisitions and policies can be used to help manage organization expenditures.</span></span> <span data-ttu-id="ac28c-110">على سبيل المثال، إذا كانت مؤسستك تعمل في مشروع بسعر ثابت يتطلب السفر، فيجب أن يتم احتواء مصروفات السفر الخاصة بأعضاء فريق المشروع داخل موازنة المشروع.</span><span class="sxs-lookup"><span data-stu-id="ac28c-110">For example, if your organization is working on a fixed-price project that requires travel, the travel expenses of the project's team members must fit within the project budget.</span></span> <span data-ttu-id="ac28c-111">من خلال المطالبة بالموافقة على مصروفات السفر قبل تكبدها، يمكن للمؤسسة المساعدة في التأكد من أن المشروع يظل ضمن الميزانية.</span><span class="sxs-lookup"><span data-stu-id="ac28c-111">By requiring that travel expenses be approved before they are incurred, the organization can help make sure that the project remains within budget.</span></span>

## <a name="configuration"></a><span data-ttu-id="ac28c-112">التكوين</span><span class="sxs-lookup"><span data-stu-id="ac28c-112">Configuration</span></span> 

<span data-ttu-id="ac28c-113">يمكن تكوين طلبات السفر على أنها "إلزامية" من خلال تمكين المعلمة "التخويل الأولي للسفر إلزاميا"في معلمات إدارة المصروفات.</span><span class="sxs-lookup"><span data-stu-id="ac28c-113">Travel Requisitions can be configured as "mandatory" by enabling the "Pre-authorization of travel is mandatory" parameter in Expense Management Parameters.</span></span> 

## <a name="create-and-submit-a-travel-requisition"></a><span data-ttu-id="ac28c-114">إنشاء طلب سفر وإرساله</span><span class="sxs-lookup"><span data-stu-id="ac28c-114">Create and submit a travel requisition</span></span>

1. <span data-ttu-id="ac28c-115">انتقل إلى **مصروفاتي: طلب السفر**، وحدد **طلب سفر جديد**.</span><span class="sxs-lookup"><span data-stu-id="ac28c-115">Go to **My expenses: Travel Requisition**, and select **New travel Requisition**.</span></span>
2. <span data-ttu-id="ac28c-116">أدخل الغرض والوجهة للطلب.</span><span class="sxs-lookup"><span data-stu-id="ac28c-116">Enter a purpose and destination for the requisition.</span></span>
3. <span data-ttu-id="ac28c-117">في حقل **وصف السفر**، أدخل أية معلومات إضافية.</span><span class="sxs-lookup"><span data-stu-id="ac28c-117">In the  **Travel description** field, enter any additional information.</span></span> 
4. <span data-ttu-id="ac28c-118">بالنسبة لكل من المصروفات المتوقعة، مثل رحلات الطيران أو الوجبات أو إيجار السيارات، قم بإنشاء عنصر بند مصروفات.</span><span class="sxs-lookup"><span data-stu-id="ac28c-118">For each of the expected expenses, such as Flight, meals, or car rental, create an expense line item.</span></span> <span data-ttu-id="ac28c-119">قم بتضمين التاريخ المقدر والمبلغ المقدر والعملة لكل بند مصروفات.</span><span class="sxs-lookup"><span data-stu-id="ac28c-119">Include the estimated date, estimated amount, and the currency for each expense.</span></span> 
5. <span data-ttu-id="ac28c-120">عند الانتهاء من إضافة المصروفات المتوقعة، حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ac28c-120">When you have finished adding the expected expenses, select **Save**.</span></span>
6. <span data-ttu-id="ac28c-121">عندما تكون جاهزًا لإرسال طلب السفر، حدد **سير العمل** > **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="ac28c-121">When you are ready to submit the travel requisition, select **Workflow** > **Submit**.</span></span>

<span data-ttu-id="ac28c-122">يمكنك عرض طلبات السفر المعتمدة تحت **مصروفاتي: طلب السفر**.</span><span class="sxs-lookup"><span data-stu-id="ac28c-122">You can view your approved travel requisitions under **My Expenses: Travel Requisition**.</span></span> 

## <a name="view-available-travel-requisitions"></a><span data-ttu-id="ac28c-123">عرض طلبات السفر المتوفرة</span><span class="sxs-lookup"><span data-stu-id="ac28c-123">View available travel requisitions</span></span>

<span data-ttu-id="ac28c-124">يمكنك عرض جميع طلبات السفر تحت **مصروفاتي: طلبات السفر**.</span><span class="sxs-lookup"><span data-stu-id="ac28c-124">You can view all of your travel requisitions under **My Expenses: Travel Requisitions**.</span></span>

## <a name="approve-travel-requisitions"></a><span data-ttu-id="ac28c-125">اعتماد طلبات السفر</span><span class="sxs-lookup"><span data-stu-id="ac28c-125">Approve travel requisitions</span></span>

<span data-ttu-id="ac28c-126">حدد طلب السفر الذي ترغب في اعتماده، ثم حدد **سير العمل** > **اعتماد**.</span><span class="sxs-lookup"><span data-stu-id="ac28c-126">Select the travel requisition that you want to approve, and then select **Workflow** > **Approve**.</span></span>  

## <a name="submit-an-expense-report-using-your-approved-travel-requisition"></a><span data-ttu-id="ac28c-127">إرسال تقرير مصروفات باستخدام طلب السفر المعتمد</span><span class="sxs-lookup"><span data-stu-id="ac28c-127">Submit an expense report using your approved travel requisition</span></span>

1. <span data-ttu-id="ac28c-128">قم بإنشاء تقرير مصروفات جديد وفي رأس تقرير المصروفات، ومن قائمة طلبات السفر المعتمدة، حدد **التعيين إلى طلب السفر**.</span><span class="sxs-lookup"><span data-stu-id="ac28c-128">Create a new expense report and in the expense report header, and from the list of approved travel requisitions, select **Map to Travel requisition**.</span></span>
2. <span data-ttu-id="ac28c-129">يتم تحديث حقل **مبلغ طلب السفر** تلقائيًا في رأس تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="ac28c-129">The **Travel requisition amount** field is automatically updated in the expense report header.</span></span>
3. <span data-ttu-id="ac28c-130">أضف كل بند مصروفات يتم تكبده في الجولة.</span><span class="sxs-lookup"><span data-stu-id="ac28c-130">Add each expense incurred for the trip.</span></span> <span data-ttu-id="ac28c-131">وفي حالة تمكين حقل **مخول أوليًا**، سيتم تحديث المبلغ المسوى والمبلغ المخول لفئة المصروفات المحددة.</span><span class="sxs-lookup"><span data-stu-id="ac28c-131">If the **Pre-authorized** field is enabled, the reconciled amount and authorized amount for the specific expense category will be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="ac28c-132">عند تعيين تقرير مصروفات إلى طلب سفر معتمد، لا يمكن أن يكون مبلغ الحركة أكبر من المبلغ المخول.</span><span class="sxs-lookup"><span data-stu-id="ac28c-132">When you map an expense report to an approved travel requisition, the transaction amount can't be greater than the authorized amount.</span></span> 
