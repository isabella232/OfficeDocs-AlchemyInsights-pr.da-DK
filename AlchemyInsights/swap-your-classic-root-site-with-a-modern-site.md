---
title: Ombyt dit klassiske rod-websted med et moderne websted
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691173"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Ombyt dit klassiske rod-websted med et moderne websted

Hvis dit miljø er konfigureret før april 2019, kan du ændre rodwebstedet til et moderne websted ved hjælp af Microsoft PowerShell:

- Hvis du har et andet websted, som du vil bruge som dit rodwebsted, kan du erstatte [(bytte) om på rodwebstedet](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) for at udskifte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted. Tilgængelig for begge team websteder (ikke forbundet til en gruppe) og kommunikationswebsted. 

- Der vil blive introduceret flere muligheder, der giver dig mulighed for at fortsætte med at bruge indholdet på webstedet, men konvertere det eksisterende websted til et kommunikationswebsted. 
>[!Important]
>Disse egenskaber bliver udrullet gradvist. Fortsæt med at kontrollere meddelelses Center for opdateringer. 

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer med swap websteder

- Destinationswebstedet kan returnere fejlen "ikke fundet" (HTTP 404) for en kort periode.
- Indhold skal gennemsøges for at opdatere søgeindekset. Der kræves intet manuelt trin. dette sker automatisk.
- Alt afhængigt af "statiske" links (f. eks. filsynkronisering og OneNote-filer) skal rettes manuelt.
- Hvis kildewebstedet var et organisations nyhedswebsted, skal du opdatere URL-adressen.Få en liste over alle organisationens nyheds websteder.
- Project Server-websteder skal muligvis valideres for at sikre, at de stadig er knyttet korrekt.
