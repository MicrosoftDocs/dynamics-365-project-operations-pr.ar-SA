---
title: إنشاء نماذج تنبؤ لموازنات المشروع
description: يصف هذا الموضوع كيفية إنشاء نموذج تنبؤ للموازنات المتبقية.
author: Yowelle
manager: AnnBe
ms.date: 04/24/2020
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
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 5a3b9d3c154a85b50536a67ae0eb45d9b4f25f15
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271022"
---
# <a name="create-forecast-models-for-project-budgets"></a><span data-ttu-id="8df1f-103">إنشاء نماذج تنبؤ لموازنات المشروع</span><span class="sxs-lookup"><span data-stu-id="8df1f-103">Create forecast models for project budgets</span></span> 

[!include [banner](../includes/banner.md)]

<span data-ttu-id="8df1f-104">يصف هذا الموضوع كيفية إنشاء نموذج تنبؤ للموازنات المتبقية.</span><span class="sxs-lookup"><span data-stu-id="8df1f-104">This topic describes how to create a forecast model for remaining budgets.</span></span> <span data-ttu-id="8df1f-105">يستخدم المشروع الذي يخضع لمراقبة الموازنة نوعين من الميزانيات: الأصلية والمتبقية.</span><span class="sxs-lookup"><span data-stu-id="8df1f-105">A project that is subject to budget control uses two types of budgets: original and remaining.</span></span> <span data-ttu-id="8df1f-106">عندما تنشئ موازنة المشروع، يجب عليك تحديد نماذج التنبؤ بالموازنة الأصلية والمتبقية التي تم إنشاؤها في صفحة **نماذج التنبؤ**.</span><span class="sxs-lookup"><span data-stu-id="8df1f-106">When you create a project budget, you must specify the original and remaining budget forecast models that were created in the **Forecast models** page.</span></span> <span data-ttu-id="8df1f-107">يتم إنشاء موازنات المشروع المستندة إلى النماذج المحددة عند الالتزام بموازنة المشروع.</span><span class="sxs-lookup"><span data-stu-id="8df1f-107">Project budgets based on the specified models are created when you commit the project budget.</span></span>

> [!NOTE]
> <span data-ttu-id="8df1f-108">لا يمكن أن يحتوي نموذج التنبؤ الذي يتم استخدامه لمراقبة الموازنة على نموذج فرعي أو لا يمكن استخدامه كنموذج فرعي.</span><span class="sxs-lookup"><span data-stu-id="8df1f-108">A forecast model that is used for budget control can’t have a submodel or be used as a submodel.</span></span>

1. <span data-ttu-id="8df1f-109">حدد **إدارة المشاريع والمحاسبة‬** > **الإعداد** > **التنبؤات**  > **نماذج التنبؤ**.</span><span class="sxs-lookup"><span data-stu-id="8df1f-109">Select **Project management and accounting** > **Setup** > **Forecasts**  > **Forecast models**.</span></span>
2. <span data-ttu-id="8df1f-110">حدد **جديد** لإنشاء نموذج تنبؤ جديد، ثم ادخل رقم واسم معرف النموذج للنموذج الجديد.</span><span class="sxs-lookup"><span data-stu-id="8df1f-110">Select **New** to create a new forecast model, and then enter a model ID number and name for the new model.</span></span> 
3. <span data-ttu-id="8df1f-111">قم بتعيين الخيار **إيقاف** إلى **نعم** لمنع حدوث أي تغييرات على بنود التنبؤ الخاصة بنموذج التنبؤ.</span><span class="sxs-lookup"><span data-stu-id="8df1f-111">Set the **Stopped** option to **Yes** to prevent any changes to the forecast lines for the forecast model.</span></span> 
4. <span data-ttu-id="8df1f-112">إذا كان ينبغي على بنود التنبؤ التي يقترن بها النموذج إنشاء تنبؤات التدفقات النقدية في دفتر الأستاذ العام، فعيّن الخيار **تضمين في تنبؤات التدفقات النقدية** إلى **نعم.**</span><span class="sxs-lookup"><span data-stu-id="8df1f-112">If the forecast lines that the model is associated with should generate cash flow forecasts in the general ledger, set **Include in Cash flow forecasts** to **Yes.**</span></span> 
5. <span data-ttu-id="8df1f-113">لاستخدام تاريخ المشروع كتاريخ الفاتورة، عيّن الخيار **التنبؤ بتاريخ الفاتورة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="8df1f-113">To use the project date as the invoice date, set **Forecast Invoice date** to **Yes**.</span></span> 
6. <span data-ttu-id="8df1f-114">في الحقل **نوع الموازنة**، حدد أحد أنواع النماذج التالية:</span><span class="sxs-lookup"><span data-stu-id="8df1f-114">In the **Budget type** field, select one of the following model types:</span></span>

   - <span data-ttu-id="8df1f-115">**الموازنة الأصلية**: استخدام مبالغ الموازنة الأصلية‏‎ التي تم الالتزام بها عند إنشاء الموازنة الأولية والموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="8df1f-115">**Original budget**: Use the original budget amounts that are committed when the initial budget is created and approved.</span></span>
   - <span data-ttu-id="8df1f-116">**الموازنة المتبقية**: استخدام مبالغ الموازنة المتبقية أثناء فترة عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="8df1f-116">**Remaining budget**: Use the remaining budget amounts during the life of the project.</span></span> <span data-ttu-id="8df1f-117">يتم تقليل الأرصدة في نموذج التنبؤ هذا بواسطة الحركات الفعلية ويتم زيادتها أو خفضها بواسطة مراجعات الموازنة.</span><span class="sxs-lookup"><span data-stu-id="8df1f-117">The balances in this forecast model are reduced by actual transactions and increased or decreased by budget revisions.</span></span>
   - <span data-ttu-id="8df1f-118">**التحويل**: استخدام مبالغ الموازنة المحوّلة للمشروع.</span><span class="sxs-lookup"><span data-stu-id="8df1f-118">**Carry-forward**: Use the carry-forward budget amounts for the project.</span></span> <span data-ttu-id="8df1f-119">التحويل هو عملية اختيارية يمكن تشغيلها لتحويل مبالغ الموازنة غير المستخدمة من سنة مالية إلى أخرى.</span><span class="sxs-lookup"><span data-stu-id="8df1f-119">Carry-forward is an optional process that can be run to transfer unused budget amounts from one fiscal year to another.</span></span>

7. <span data-ttu-id="8df1f-120">قم بتعيين الخيارات التالية حسب الاقتضاء:</span><span class="sxs-lookup"><span data-stu-id="8df1f-120">Set the following options as required:</span></span>

   - <span data-ttu-id="8df1f-121">قم بتمكين الخيار **التنبؤ بتاريخ الفاتورة‬‏‫** لاستخدام تاريخ المشروع كتاريخ الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="8df1f-121">Enable **Forecast invoice date** to use the project date as the invoice date.</span></span>
   - <span data-ttu-id="8df1f-122">قم بتمكين الخيار **التنبؤ بواسطة الأعمال قيد التنفيذ** للتنبؤ بالاستناد إلى الأعمال قيد التنفيذ (WIP)، ثم حدد نوع الأعمال قيد التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="8df1f-122">Enable **Forecast with WIP** to forecast based on work in progress (WIP), and then select the type of WIP.</span></span> 
   - <span data-ttu-id="8df1f-123">يمكنك إبقاء **نوع الموازنة** الافتراضي معينًا إلى **بلا** أو يمكنك إدخال نوع جديد.</span><span class="sxs-lookup"><span data-stu-id="8df1f-123">You can keep the default **Budget type** as **None** or enter a new type.</span></span> <span data-ttu-id="8df1f-124">لا يمكن تغيير نوع الموازنة بعد تغيير سجل.</span><span class="sxs-lookup"><span data-stu-id="8df1f-124">The budget type can't be changed after you change a record.</span></span>     
    > [!NOTE]
    > <span data-ttu-id="8df1f-125">إذا قمت بتغيير نوع الموازنة الافتراضية، فلن تكون الخيارات الأخرى متوفرة للتحديثات، ولا يمكنك إعادة استخدام نموذج التنبؤ هذا.</span><span class="sxs-lookup"><span data-stu-id="8df1f-125">If you change the default budget type, all other options will become unavailable for updates, and you can't reuse this forecast model.</span></span> 
   


 



[!INCLUDE[footer-include](../includes/footer-banner.md)]