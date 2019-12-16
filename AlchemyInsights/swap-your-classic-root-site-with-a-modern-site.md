---
title: Byt dit klassiske rodwebsted med et moderne websted
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042921"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byt dit klassiske rodwebsted med et moderne websted

Hvis dit miljø blev oprettet før april 2019, kan du ændre rodwebstedet til et moderne websted ved hjælp af Microsoft PowerShell:

- Hvis du har et andet websted, som du vil bruge som rodwebsted, kan du erstatte [(bytte) rodwebstedet](https://docs.microsoft.com/sharepoint/modern-root-site) med det. 
    - Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted. Tilgængelig for både team websted (ikke forbundet til en gruppe) og kommunikationswebsted. 

- Yderligere funktioner vil blive indført snart, der vil give dig mulighed for at fortsætte med at bruge indholdet på webstedet, men konvertere det eksisterende websted til en kommunikation site. 
>[!Important]
>Disse funktioner vil blive rullet ud gradvist. Fortsæt med at kontrollere Office 365 Message Center for opdateringer. 

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer med swapping sites

- Destinationswebstedet kan returnere fejlen "ikke fundet" (HTTP 404) i en kort periode.
- Indholdet skal sættes i igen for at opdatere søgeindekset. Der er ingen manuelle trin påkrævet-dette vil ske automatisk.
- Alt, hvad der er afhængigt af "statiske" links (f. eks. filsynkronisering og OneNote-filer), skal korrigeres manuelt.
- Hvis kildewebstedet var et organisations nyhedswebsted, bør du opdatere URL-adressen.Få en liste over alle organisatoriske nyhedssites.
- Project Server-websteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt.





