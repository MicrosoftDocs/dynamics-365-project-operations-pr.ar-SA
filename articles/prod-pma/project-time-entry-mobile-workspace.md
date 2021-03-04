---
title: مساحة عمل متنقلة لإدخال وقت المشروع
description: يوفر هذا الموضوع معلومات حول مساحة العمل المتنقلة لإدخال وقت المشروع. تتيح مساحة العمل هذه للمستخدمين إدخال الوقت وتوفيره علي أحد المشروعات باستخدام الجهاز المحمول الخاص بهم.
author: Yowelle
manager: AnnBe
ms.date: 12/01/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 272101
ms.assetid: 4505f021-b9bb-4b87-be24-6bf0bd88ee60
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: 23a5a9f25cfdd6df74257b3500c7a035d711b5f6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070625"
---
# <a name="project-time-entry-mobile-workspace"></a>مساحة عمل متنقلة لإدخال وقت المشروع

[!include [banner](../includes/banner.md)]

يوفر هذا الموضوع معلومات حول مساحة العمل المتنقلة **لإدخال وقت المشروع**. تتيح مساحة العمل هذه للمستخدمين إدخال الوقت وتوفيره علي أحد المشروعات باستخدام الجهاز المحمول الخاص بهم.

مساحة العمل المحمولة هذه مخصصة للاستخدام مع تطبيق الأجهزة المحمولة Dynamics 365 Unified Ops. 

## <a name="overview"></a>Overview
وكجزء من عملهم اليومي ، فان موارد المشروع غالبا ما تكون موجودة في الموقع أو السفر. تتيح مساحة عمل الأجهزة الإلكترونية **إدخال الوقت بالمشروع** للمستخدمين إدخال الوقت القابل للفوترة أو غير القابل للفوترة مقابل مشروع على الجهاز المحمول من اختيارهم. لذلك ، يمكن لموارد المشروع تسجيل إدخالات الوقت في أي وقت وفي أي مكان. يمكنهم أيضًا عرض إدخالات الوقت التي تم تسجيلها بالفعل. 

وبشكل خاص، في مساحة عمل الأجهزة الإلكترونية **إدخال الوقت للمشروع** ، يمكن للمستخدمين تنفيذ هذه المهام:

-   بالنسبة لأي تاريخ محدد ، أدخل عدد الساعات التي قضيتها في مهمة معينة.
-   ابحث عن طريق اسم المشروع أو العميل للعثور على المشروع لإدخال وقته.
-   حدد الفئة والنشاط للوقت الذي قمت بقضاءه.
-   يمكنك تسجيل الوقت علي انه قابل للفوترة أو غير المدفوع للمشروع.
-   قم بإدخال تعليقات خارجيه أو داخلية بشكل اختياري.

## <a name="prerequisites"></a>المتطلبات الأساسية
تختلف المتطلبات الاساسيه، استنادا إلى إصدار Microsoft Dynamics365 الذي تم نشره للمؤسسة الخاصة بك.

### <a name="prerequisites-if-you-use-dynamics-365-finance"></a>المتطلبات الاساسيه إذا كنت تستخدم Dynamics 365 Finance
إذا تم نشر Finance لمؤسستك ، فيجب على مسؤول النظام نشر مساحة عمل الأجهزة الإلكترونية **إدخال الوقت للمشروع**. للحصول علي الإرشادات، راجع [نشر مساحة عمل الأجهزة الإلكترونية](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace).

### <a name="prerequisites-if-you-use-version-1611-with-platform-update-3-or-later"></a>المتطلبات الأساسية إذا كنت تستخدم الإصدار 1611 مع تحديث النظام الأساسي 3 أو إصدار أحدث
إذا تم نشر الإصدار 1611 مع تحديث النظام الأساسي 3 أو الأحدث لمؤسستك ، فيجب على مسؤول النظام إكمال المتطلبات الأساسية التالية. 

<table>
<thead>
<tr class="header">
<th>المتطلبات الأساسية</th>
<th>الدور</th>
<th>‏‏الوصف</th>
</tr>
</thead>
<tbody>
<tr class="odd">

<td>نفذ قاعدة المعارف 4018050.</td>
<td>مسؤول النظام</td>
<td>قاعدة المعارف 4018050 هي تحديث X ++ أو إصلاح بيانات التعريف الذي يحتوي على مساحة عمل الأجهزة الإلكترونية <strong>إدخال الوقت للمشروع</strong>. لتنفيذ قاعدة المعارف 4018050، يجب علي المسؤول النظام اتباع الخطوات التالية.
<ol>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/download-hotfix-lcs">قم بتنزيل إصلاح بيانات التعريف من Microsoft Dynamics Lifecycle Services ‏(LCS‏)‏</a>.</li>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/install-metadata-hotfix-package">قم بتثبيت الإصلاح العاجل لبيانات التعريف</a>.</li>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/create-apply-deployable-package">قم بإنشاء حزمه قابله للنشر</a> تحتوي على نماذج <strong>ApplicationSuite</strong> و<strong>ProjectMobile</strong>، ثم قم بتحميل الحزمة القابلة للنشر إلى LCS.</li>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/apply-deployable-package-system">قم بتطبيق الحزمة القابلة للنشر</a>.</li>

</ol></td>
</tr>
<tr class="even">
<td>انشر مساحة عمل الأجهزة المحمولة <strong>إدخال الوقت للمشروع</strong>.</td>
<td>مسؤول النظام</td>
<td>راجع <a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace">نشر مساحة عمل الأجهزة المحمولة</a>.</td>
</tr>
</tbody>
</table>

## <a name="download-and-install-the-mobile-app"></a>تنزيل تطبيق الأجهزة المحمولة وتثبيته

تنزيل تطبيق الأجهزة المحمولة Finance and Operations وتثبيته:

-   [لهواتف Android](https://go.microsoft.com/fwlink/?linkid=850662)
-   [لأجهزة iPhones](https://go.microsoft.com/fwlink/?linkid=850663)

## <a name="sign-in-to-the-mobile-app"></a>تسجيل الدخول إلى تطبيق الأجهزة المحمولة
1.  ابدأ التطبيق على جهازك المحمول.
2.  أدخل عنوان URL الخاص بـ Dynamics 365.
3.  في المرة الأولى التي تقوم فيها بتسجيل الدخول ، ستتم مطالبتك بإدخال اسم المستخدم وكلمة المرور. أدخل بيانات الاعتماد.
4.  بعد تسجيل الدخول ، يتم عرض مساحات العمل المتوفرة لشركتك. لاحظ أنه إذا نشر مسؤول النظام مساحة عمل جديدة لاحقًا ، فسيتعين عليك تحديث قائمة مساحات عمل الأجهزة المحمولة.

[![السحب للتحديث](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)

## <a name="enter-time-by-using-the-project-time-entry-mobile-workspace"></a>أدخل الوقت باستخدام مساحة عمل الأجهزة المحمولة لإدخال وقت المشروع
1.  على جهازك المحمول ، حدد مساحة عمل **إدخال وقت المشروع**.
2.  حدد **إدخال الوقت**. يتم عرض تواريخ التقويم الخاصة بالأسبوع الحالي.
3.  بالنسبة لتاريخ محدد، حدد **الإجراءات** &gt; **إدخال جديد**.
4.  أدخل عدد الساعات للتسجيل.
5.  حدد المشروع الخاص بإدخال الوقت. تظهر قائمه بالمشاريع التي تم تحميلها إلى التطبيق الخاص بك للاستخدام دون اتصال. افتراضيا ، يتم تحميل العناصر 50 ، ولكن يمكن للمطور تغيير هذا الرقم. لمزيد من المعلومات، راجع [النظام الأساسي للأجهزة المحمولة](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
6.  إذا لم يكن المشروع موجودا في القائمة، فحدد **بحث**. ابحث حسب الاسم ، أو بدل إلى البحث حسب اسم المشروع أو العميل.
7.  حدد فئة‏‎. تظهر قائمه بالفئات التي تم تحميلها إلى التطبيق الخاص بك للاستخدام دون اتصال. افتراضيا ، يتم تحميل العناصر 50 ، ولكن يمكن للمطور تغيير هذا الرقم. لمزيد من المعلومات، راجع [النظام الأساسي للأجهزة المحمولة](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
8.  إذا لم تكن الفئة موجودة في القائمة، فحدد **بحث**. ابحث حسب الفئة، أو قم بالتبديل للبحث حسب اسم الفئة.
9.  حدد نشاطًا. تظهر قائمه بالأنشطة التي تم تحميلها إلى التطبيق الخاص بك للاستخدام دون اتصال. افتراضيا ، يتم تحميل العناصر 50 ، ولكن يمكن للمطور تغيير هذا الرقم. لمزيد من المعلومات، راجع [النظام الأساسي للأجهزة المحمولة](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
10. إذا لم يكن النشاط موجودًا في القائمة، فحدد **بحث**. قم بالبحث حسب رقم النشاط، أو بدل إلى البحث حسب الغرض.

11. حدد خاصية البند.
12. ختياري: أدخل تعليقات خارجيه أو داخلية.
13. حدد **تم**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]