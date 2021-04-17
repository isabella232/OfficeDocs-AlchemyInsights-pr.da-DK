---
title: Kan ikke indstille eller få vist politikken AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826085"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Kan ikke indstille eller få vist politikken AllowSelfServicePurchase

Når du forsøger at indstille eller få vist politikken AllowSelfServicePurchase, modtager du følgende fejlmeddelelse:

*Håndteringsfejl: Produktpolitikken kunne ikke hentes med PolicyId 'AllowSelfServicePurchase', ErrorMessage – Den underliggende forbindelse blev lukket: Der opstod en uventet fejl ved en afsendelse.*

Dette kan skyldes en ældre version af TLS (Transport Layer Security). Hvis du vil oprette forbindelse til MSCommerce-tjenesten, skal du bruge TLS 1.2 eller derover.  

Prøv følgende trin for at aktivere/indstille TLS-protokollen til 1.2, bekræfte og prøve igen.
 1. Ved PowerShell-kommandoprompten (PS C: skal du angive følgende kommando for at indstille \) TLS-protokollen til version 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Bekræft, at TLS-protokollen/-protokollen(er) er i brug, med følgende kommando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Prøv igen kommandoerne Hent eller Opdater efter behov.

