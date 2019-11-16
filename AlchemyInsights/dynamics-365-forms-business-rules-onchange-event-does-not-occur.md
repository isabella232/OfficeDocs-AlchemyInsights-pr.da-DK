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
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769333"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Hændelsen OnChange indtræffer ikke, hvis feltet ændres programmatisk

Hændelsen *onChange* indtræffer ikke, hvis feltet ændres programmatisk ved hjælp af *attributten.* metoden [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Hvis du vil have hændelseshandlere for hændelsen *onChange* til at køre, når du har angivet værdien, skal du bruge metoden *formcontext. data. Entity-attribut* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) i din kode.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
