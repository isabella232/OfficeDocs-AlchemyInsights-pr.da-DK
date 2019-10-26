---
title: Dynamics 365 forms forretningsregler – forretningsregel, der ikke udløses for en formular
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529013"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="e56b5-102">Hændelsen OnChange indtræffer ikke, hvis feltet ændres programmatisk</span><span class="sxs-lookup"><span data-stu-id="e56b5-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="e56b5-103">Hændelsen *onChange* indtræffer ikke, hvis feltet ændres programmatisk ved hjælp af *attributten.* metoden [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="e56b5-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="e56b5-104">Hvis du vil have hændelseshandlere for hændelsen *onChange* til at køre, når du har angivet værdien, skal du bruge *attributten formcontext. data. Entity.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -metoden i din kode.</span><span class="sxs-lookup"><span data-stu-id="e56b5-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
