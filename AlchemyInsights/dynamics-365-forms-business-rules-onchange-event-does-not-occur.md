---
title: Dynamics 365-formular forretningsregler – forretningsregel, der udløser ikke for en formular
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711485"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="7c2e0-102">Hændelsen OnChange opstår ikke, hvis feltet ændres automatisk</span><span class="sxs-lookup"><span data-stu-id="7c2e0-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="7c2e0-103">Hændelsen *onChange* indtræffer ikke, hvis feltet er blevet ændret ved hjælp af et program ved hjælp af en *attribut.* metoden [AngivVærdi](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="7c2e0-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="7c2e0-104">Hvis du ønsker, at hændelseshandlerne *onChange* -hændelsen skal køre, når du har angivet værdien, skal du bruge *formContext. data. Entity-attributten* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -metoden i din kode.</span><span class="sxs-lookup"><span data-stu-id="7c2e0-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
