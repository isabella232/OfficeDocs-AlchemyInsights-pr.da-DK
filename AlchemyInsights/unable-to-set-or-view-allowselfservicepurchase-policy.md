---
title: Det er ikke muligt at angive eller få vist AllowSelfServicePurchase-politikken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735193"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Det er ikke muligt at angive eller få vist AllowSelfServicePurchase-politikken

Når du forsøger at angive eller få vist AllowSelfServicePurchase-politikken, får du vist følgende fejlmeddelelse:

*HandleError: det lykkedes ikke at hente produktpolitik med PolicyId ' AllowSelfServicePurchase ', ErrorMessage-den underliggende forbindelse blev lukket: der opstod en uventet fejl i en Send.*

Dette kan skyldes en ældre version af TLS (Transport Layer Security). Hvis du vil oprette forbindelse til MSCommerce-tjenesten, skal du bruge TLS 1,2 eller nyere.  

Benyt følgende fremgangsmåde for at aktivere/konfigurere TLS-protokollen til 1,2, bekræfte og prøve igen.
 1. Ved kommandoprompten i PowerShell (PS C: \) Skriv følgende kommando for at indstille TLS-protokollen til version 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Bekræft de TLS-protokoller, der er i brug, med følgende kommando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Prøv kommandoerne Hent eller Opdater efter behov.

