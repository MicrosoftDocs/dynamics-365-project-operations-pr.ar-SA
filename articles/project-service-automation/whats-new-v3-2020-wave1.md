---
title: الجديد أو المتغير في الإصدار 3.x من Project Service Automation، الموجة 1 لعام 2020
description: يقدم هذا الموضوع معلومات حول الجديد والمتغير في الإصدار رقم 3 من Project Service Automation، الموجة 1 لعام 2020.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 01/24/2020
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x wave 1 2020
author: stsporen
ms.assetid: 48b408c1-11e7-4005-abac-8fd7c0b064b1
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 478080c0570b71188c9f1e12b18b5aadc13903e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748650"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="d8664-103">الجديد أو المتغير في الإصدار 3 من Project Service Automation، الموجة 1 لعام 2020</span><span class="sxs-lookup"><span data-stu-id="d8664-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>
<span data-ttu-id="d8664-104">هذا الموضوع يلقي الضوء على اعتبارات الترقية عند الانتقال إلى الإصدار الأخير 3.x من Project Service Automation (PSA)، الموجة 1 لعام 2020.</span><span class="sxs-lookup"><span data-stu-id="d8664-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="d8664-105">إدخال الوقت</span><span class="sxs-lookup"><span data-stu-id="d8664-105">Time entry</span></span>
<span data-ttu-id="d8664-106">تم توسيع تجربة إدخال الوقت لتوفير إمكانيات لتوسيع إدخال الوقت في المزيد من سيناريوهات العملاء.</span><span class="sxs-lookup"><span data-stu-id="d8664-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="d8664-107">وهذا يشمل إمكانية إضافة أنواع إدخالات، التي تعزز الآن سلوكيات معنية بالاستناد إلى اسم مخطط الحقل **إعدادات إدخال الوقت** الذي يظهر على أنه **مصدر الوقت**.</span><span class="sxs-lookup"><span data-stu-id="d8664-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings**, displayed as **Time Source**.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="d8664-108">اعتبارات الترقية</span><span class="sxs-lookup"><span data-stu-id="d8664-108">Upgrade consideration</span></span>
<span data-ttu-id="d8664-109">لدعم هذه الوظيفة، تم تحديث الأدوار الموجودة في PSA لتشمل امتيازات جديدة.</span><span class="sxs-lookup"><span data-stu-id="d8664-109">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="d8664-110">تمنح هذه الامتيازات حق الوصول للقراءة للكيان الجديد، **إعدادات إدخال الوقت**.</span><span class="sxs-lookup"><span data-stu-id="d8664-110">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="d8664-111">ينبغي منح المستخدمين الذين يحتاجون إلى تسجيل الوقت دور المستخدم **مستخدم إدخال الوقت** بالإضافة إلى الأدوار الموجودة.</span><span class="sxs-lookup"><span data-stu-id="d8664-111">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="d8664-112">يتضمن هذا الدور الوظائف الجديدة ويضمن استمرارية عمل إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="d8664-112">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="d8664-113">تغييرات إدخال الوقت الممدد حاليًا</span><span class="sxs-lookup"><span data-stu-id="d8664-113">Currently extended time entry changes</span></span>
<span data-ttu-id="d8664-114">لتقليل التأثير على مستخدمي إدخال الوقت الحاليين، يعتبر تغيير الدور هذا الشرط الأساسي الوحيد المطلوب لمتابعة استخدام إدخال الوقت.</span><span class="sxs-lookup"><span data-stu-id="d8664-114">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="d8664-115">إذا كنت قد قمت بإنشاء طرق عرض مخصصة أو تجارب إدخال وقت منفصلة، فيجب تعيين حقول **إعداد إدخال الوقت** إلى قيمه PSA الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="d8664-115">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>
