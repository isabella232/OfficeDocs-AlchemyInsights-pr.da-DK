---
title: Politikken AllowSelfServicePurchase kan ikke angives eller vises
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091682"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Politikken AllowSelfServicePurchase kan ikke angives eller vises

Når du forsøger at angive eller få vist politikken AllowSelfServicePurchase, får du vist følgende fejlmeddelelse:

*HandleError : Produktpolitikken kunne ikke hentes med PolicyId 'AllowSelfServicePurchase', ErrorMessage - Den underliggende forbindelse blev lukket: Der opstod en uventet fejl under en afsendelse.*

Dette kan skyldes en ældre version af Transport Layer Security (TLS). Hvis du vil tilslutte MSCommerce-tjenesten, skal du bruge TLS 1.2 eller derover.  

Prøv følgende trin for at aktivere/indstille TLS-protokollen til 1.2, skal du kontrollere og prøve igen.
 1. Ved Kommandoprompten til PowerShell\) (PS C: Angiv følgende kommando for at indstille TLS-protokollen til version 1.2:

    \[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12

2. Kontroller de TLS-protokoller, der er i brug, med følgende kommando:

    \[Net.ServicePointManager]::SecurityProtocol 

3. Prøv kommandoerne Hent eller Opdater igen efter behov.

