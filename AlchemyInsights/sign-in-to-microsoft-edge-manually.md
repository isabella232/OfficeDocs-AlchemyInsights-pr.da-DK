---
title: Log på Microsoft Edge manuelt
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f9aa27a585d805360e1fadecfd0db3b11d15a3594ed5bd5dc6c68cec37a4d6a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050760"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Log på Microsoft Edge manuelt

Hvis en bruger ikke logges på automatisk under første kørsel, kan brugeren manuelt logge på via browserens indstillinger eller pop op-menuen identitet. Brug følgende politikker til at administrere logon:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – For at sikre, at en bruger altid har en arbejdsprofil i Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – For at begrænse logon til et sæt af pålidelige konti.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – For at deaktivere logon eller tvinge brugere til at logge på.

