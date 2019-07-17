---
title: Dynamics 365 danner forretningsregler - forretningsregel udløser ikke i en formular
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747293"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="a2dfb-102">OnChange-hændelsen opstår ikke, hvis feltet ændres via programmering</span><span class="sxs-lookup"><span data-stu-id="a2dfb-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="a2dfb-103">*OnChange* -hændelsen opstår ikke, hvis feltet ændres via programmering ved hjælp af den *attribut.* [AngivVærdi](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metode.</span><span class="sxs-lookup"><span data-stu-id="a2dfb-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="a2dfb-104">Hvis du vil hændelseshandlere for hændelsen *OnChange* til at køre, når du angiver den værdi, du skal bruge den *attribut for formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metode i din kode.</span><span class="sxs-lookup"><span data-stu-id="a2dfb-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
