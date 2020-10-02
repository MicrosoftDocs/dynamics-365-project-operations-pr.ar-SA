---
title: تكوين عملية إنشاء فاتورة تلقائية
description: يقدم هذا الموضوع معلومات حول التشغيل السريع لتكوين النظام بحيث يتم إنشاء الفواتير تلقائيًا.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898110"
---
# <a name="configure-automated-invoice-creation"></a><span data-ttu-id="af66d-103">تكوين عملية إنشاء فاتورة تلقائية</span><span class="sxs-lookup"><span data-stu-id="af66d-103">Configure automated invoice creation</span></span>

<span data-ttu-id="af66d-104">_**ينطبق علي:** ‏‫Project Operations للسيناريوهات المستندة إلى مورد/غير مخزنة‬، ‏‫النشر الخفيف – التعامل مع الفواتير الأولية‬_</span><span class="sxs-lookup"><span data-stu-id="af66d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="af66d-105">أكمل الخطوات التالية لتكوين تشغيل فاتورة تلقائية في عمليات المشروع.</span><span class="sxs-lookup"><span data-stu-id="af66d-105">Complete the following steps to configure an automated invoice run in Project operations.</span></span>

1. <span data-ttu-id="af66d-106">الانتقال إلى **إعدادات** \> **الوظائف الدفعية**.</span><span class="sxs-lookup"><span data-stu-id="af66d-106">Go to **Settings** \> **Batch jobs**.</span></span>
2. <span data-ttu-id="af66d-107">قم بإنشاء وظيفة دفعية، وقم بتسميتها **إنشاء فواتير عمليات المشروع**.</span><span class="sxs-lookup"><span data-stu-id="af66d-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="af66d-108">يجب أن يتضمن اسم الوظيفة الدفعية مصطلح "إنشاء الفواتير."</span><span class="sxs-lookup"><span data-stu-id="af66d-108">The name of the batch job must include the term "create invoices."</span></span>
3. <span data-ttu-id="af66d-109">في حقل **نوع الوظيفة**، حدد **بلا**.</span><span class="sxs-lookup"><span data-stu-id="af66d-109">In the **Job type** field, select **None**.</span></span> <span data-ttu-id="af66d-110">افتراضيًا، يتم تعيين  خيارات **التكرار اليومي** و**نشط** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="af66d-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="af66d-111">حدد **تشغيل سير العمل**.</span><span class="sxs-lookup"><span data-stu-id="af66d-111">Select **Run Workflow**.</span></span> <span data-ttu-id="af66d-112">في مربع حوار **البحث عن سجل**، ستري ثلاث مهام لسير العمل:</span><span class="sxs-lookup"><span data-stu-id="af66d-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="af66d-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="af66d-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="af66d-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="af66d-114">ProcessRunner</span></span>
    - <span data-ttu-id="af66d-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="af66d-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="af66d-116">حدد **ProcessRunCaller**، ثم حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="af66d-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="af66d-117">في مربع الحوار التالي، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="af66d-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="af66d-118">يكون سير عمل **السكون** متبوعًا بسير عمل **العملية**.</span><span class="sxs-lookup"><span data-stu-id="af66d-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

    <span data-ttu-id="af66d-119">يمكنك أيضا تحديد **ProcessRunner** في الخطوة 5.</span><span class="sxs-lookup"><span data-stu-id="af66d-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="af66d-120">بعد ذلك، عندما تحدد **موافق**، يكون سير عمل **العملية** متبوعًا بسير عمل **السكون**.</span><span class="sxs-lookup"><span data-stu-id="af66d-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="af66d-121">يؤدي سير عمل **ProcessRunCaller** و**ProcessRunner** إلى إنشاء الفواتير.</span><span class="sxs-lookup"><span data-stu-id="af66d-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="af66d-122">**ProcessRunCaller** يستدعي **ProcessRunner**.</span><span class="sxs-lookup"><span data-stu-id="af66d-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="af66d-123">**ProcessRunner** هو سير العمل الذي ينشئ الفواتير فعليًا.</span><span class="sxs-lookup"><span data-stu-id="af66d-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="af66d-124">ويمر بكافة بنود العقد التي يجب إنشاء الفواتير لها، ويقوم بإنشاء الفواتير لهذه البنود.</span><span class="sxs-lookup"><span data-stu-id="af66d-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="af66d-125">لتحديد شروط التعاقد التي يجب إنشاء الفواتير لها، فإن الوظيفة تبحث عن تواريخ تشغيل الفاتورة لشروط التعاقد.</span><span class="sxs-lookup"><span data-stu-id="af66d-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="af66d-126">إذا كانت بنود العقد التي تنتمي لأحد العقود لها نفس تاريخ تشغيل الفاتورة، سيتم تجميع الحركات في فاتورة واحدة بها بندين للفاتورة.</span><span class="sxs-lookup"><span data-stu-id="af66d-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="af66d-127">إذا لم تكن هناك حركات لإنشاء فواتير لها، تتخطى الوظيفة إنشاء الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="af66d-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="af66d-128">بعد انتهاء تشغيل **ProcessRunner**، فإنه يستدعي **ProcessRunCaller**، الذي يوفر وقت النهاية، وويتم إغلاقه.</span><span class="sxs-lookup"><span data-stu-id="af66d-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="af66d-129">بعد ذلك يبدأ **ProcessRunCaller** المؤقت الذي يعمل على مدار 24 ساعة من وقت النهاية المحدد.</span><span class="sxs-lookup"><span data-stu-id="af66d-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="af66d-130">في نهاية المؤقت، يتم إغلاق **ProcessRunCaller**.</span><span class="sxs-lookup"><span data-stu-id="af66d-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="af66d-131">تعتبر وظيفة المعالجة الدفعية لإنشاء الفواتير وظيفة متكررة.</span><span class="sxs-lookup"><span data-stu-id="af66d-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="af66d-132">إذا تم تشغيل هذه المعالجة الدفعية عده مرات، سيتم إنشاء مثيلات متعددة للوظيفة وتتسبب في حدوث أخطاء.</span><span class="sxs-lookup"><span data-stu-id="af66d-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="af66d-133">بالتالي، يجب عليك بدء عملية المعالجة الدفعية مرة واحدة فقط، وينبغي إعادة تشغيلها في حالة توقفها عن العمل فقط.</span><span class="sxs-lookup"><span data-stu-id="af66d-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="af66d-134">لا يتم تشغيل الفوترة الدفعية إلا لبنود عقد المشروع التي تم تكوينها بواسطة جداول الفواتير.</span><span class="sxs-lookup"><span data-stu-id="af66d-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="af66d-135">يجب أن يحتوي بند العقد مع طريقة فوترة بسعر ثابت على مراحل مكوّنة.</span><span class="sxs-lookup"><span data-stu-id="af66d-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="af66d-136">سيحتاج بند عقد المشروع مع طريقة فوترة الوقت والمواد إلى إعداد جدول فاتورة يستند إلى التاريخ.</span><span class="sxs-lookup"><span data-stu-id="af66d-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="af66d-137">ينطبق الأمر نفسه على بند العقد المستند إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="af66d-137">The same applies to a project-based contract line.</span></span>     
