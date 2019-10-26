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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Hændelsen OnChange indtræffer ikke, hvis feltet ændres programmatisk

Hændelsen *onChange* indtræffer ikke, hvis feltet ændres programmatisk ved hjælp af *attributten.* metoden [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Hvis du vil have hændelseshandlere for hændelsen *onChange* til at køre, når du har angivet værdien, skal du bruge *attributten formcontext. data. Entity.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -metoden i din kode.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
