---
title: إزالة تثبيت Dynamics 365 Project Operations
description: يقدم هذا الموضوع معلومات حول كيفية تثبيت Dynamics 365 Project Operations.
author: stsporen
ms.date: 11/09/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b87c9324b1c95c10ef1e18b0fbf4572bdbe76827
ms.sourcegitcommit: b8b7a59eee7d93638446e93726d270316e45ab3d
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/10/2021
ms.locfileid: "7783627"
---
# <a name="uninstall-dynamics-365-project-operations"></a>إزالة تثبيت Dynamics 365 Project Operations 

_**ينطبق على:** Project Operations للسيناريوهات المستندة إلى موارد/منتجات غير مخزنة‬_

لتثبيت Dynamics 365 Project Operations، فإنه يجب تعيين دور المسؤول.

1. انتقل إلى **الإعدادات** > **الحلول**.

    ![صفحة الإعدادات.](./media/uninstall-proj-ops-solutions.png)
  
2. قم بإزالة الحلول بالترتيب الصحيح المدرج في الجدول التالي. 

    | خطوة | اسم الحل                                    | ملاحظة                                                                                         |
    |------|----------------------------------------------------|----------------------------------------------------------------------------------------------|
    | 1  | msdyn_ProjectServiceUpgrade_managed.cab            | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 2  | ProjectOperations_Anchor                           | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 3  | Dynamics365ProjectOperationsDualWriteEntityMaps    | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 4 | Dynamics365ProjectOperationsDualWrite              | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 5 | ProjectService                                     | لا يوجد ملاحظات إضافية.                                                                         |
    |  6 | ProjectServiceCore_Patch                           | لا يوجد ملاحظات إضافية.                                                                         |
    | 7 | ProjectServiceCore                                 | لا يوجد ملاحظات إضافية.                                                                         |
    | 8 | ProjectServiceDeprecatedComponents                 | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 9 | FieldServiceCommon                                 | مطلوب للكتابة المزدوجة باستخدام Dynamics 365 Finance أو Dynamics 365 Supply Chain Management.   |
    | 10 | msdyn_AssetCommon                                  | مطلوب للكتابة المزدوجة باستخدام Dynamics 365 Finance أو Dynamics 365 Supply Chain Management.   |
    | 11 | msdyn_TESA_Anchor                                  | مطلوب لـ Dynamics 365 Field Service.                                                     |
    | 12 | msdyn_TESA_Patch                                   | مطلوب لـ Dynamics 365 Field Service.                                                     |
    | 13 | msdyn_TESA                                         | مطلوب لـ Dynamics 365 Field Service.                                                     |
    | 14 | ResourceSchedulingControls                         | مطلوب لـ Dynamics 365 Field Service.                                                     |
    | 15 | MicrosoftDynamicsScheduling3_CumulativePatch       | مطلوب لـ Dynamics 365 Field Service.                                                     |
    | 16 | MicrosoftDynamicsScheduling_Patch_xx               | مطلوب لـ Dynamics 365 Field Service.                                                     |
    | 17 | MicrosoftDynamicsScheduling                        | مطلوب لـ Dynamics 365 Field Service.                                                     |
    | 18 | Dynamics365FinanceAndOperationsAnchor              | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 19 | Dynamics365Notes                                   | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 20 | Dynamics365FinanceAndOperationsDualWriteEntityMaps | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 21 | DualWriteCore                                      | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 22 | Dynamics365AssetManagementApp                      | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 23 | Dynamics365AssetManagement                         | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 24 | Dynamics365SupplyChainExtended                     | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 25 | Dynamics365FinanceExtended                         | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 26 | HCMCommon                                          | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 27 | Dynamics365FinanceAndOperationsCommon              | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 28 | المجموعة                                              | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 29 | Dynamics365Company                                 | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 30 | CurrencyExchangeRates                              | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
    | 31 | AssetCommon                                        | إذا لم يتم العثور عليه، فتجاوز هذا الحل.                                                            |
