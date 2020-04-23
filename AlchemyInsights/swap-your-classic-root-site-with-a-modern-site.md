---
title: Byt din Klassiske rod site med en moderne site
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741538"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byt din Klassiske rod site med en moderne site

Hvis dit miljø blev konfigureret før april 2019, kan du ændre rodwebstedet til et moderne websted ved hjælp af Microsoft PowerShell:

- Hvis du har et andet websted, som du vil bruge som rodwebsted, kan du erstatte [(bytte) rodwebstedet](https://docs.microsoft.com/sharepoint/modern-root-site) med det. 
    - Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted. Tilgængelig for både teamwebsted (ikke forbundet til en gruppe) og kommunikationswebsted. 

- Yderligere funktioner vil blive indført snart, som vil give dig mulighed for at fortsætte med at bruge indholdet på webstedet, men konvertere det eksisterende websted til en kommunikation site. 
>[!Important]
>Disse funktioner vil blive udrullet gradvist. Fortsæt med at kontrollere opdateringerne i Meddelelsescenter. 

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer med byttewebsteder

- Destinationswebstedet kan returnere en "ikke fundet" (HTTP 404) fejl i en kort periode.
- Indholdet skal crawles igen for at opdatere søgeindekset. Der er ingen manuel trin påkrævet - dette vil ske automatisk.
- Alt, hvad der er afhængigt af "statiske" links (f.eks. filsynkronisering og OneNote-filer), skal rettes manuelt.
- Hvis kildewebstedet var et organisationsnyhedswebsted, skal du opdatere URL-adressen.Få en liste over alle organisatoriske nyhedssites.
- Project Server-websteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt.
