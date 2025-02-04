---
title: Byt om på dit klassiske rodwebsted med et moderne websted
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
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316134"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byt om på dit klassiske rodwebsted med et moderne websted

Hvis dit miljø blev konfigureret før april 2019, kan du ændre rodwebstedet til et moderne websted ved hjælp af Microsoft PowerShell:

- Hvis du har et andet websted, du vil bruge som rodwebsted, kan du erstatte [(bytte) rodwebstedet](https://docs.microsoft.com/sharepoint/modern-root-site) med det. 
    - Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted under arkivering af det oprindelige websted. Tilgængelig for både Teamwebsted (ikke forbundet med en gruppe) og Kommunikationswebsted. 

- Der introduceres snart yderligere funktioner, der giver dig mulighed for at fortsætte med at bruge indholdet på webstedet, men konvertere det eksisterende websted til et kommunikationswebsted. 

**Vigtigt:** Disse funktioner udrulles gradvist. Fortsæt med at kontrollere, om der er opdateringer i Meddelelsescenter. 

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer med udskiftning af websteder

- Destinationswebstedet returnerer muligvis fejlen "blev ikke fundet" (HTTP 404) i en kort periode.
- Indhold skal slås sammen igen for at opdatere søgeindekset. Der kræves ingen manuelle trin – dette udføres automatisk.
- Alt afhængigt af "statiske" links (f.eks filsynkronisering og OneNote filer) skal rettes manuelt.
- Hvis kildewebstedet var et virksomhedsnyhederswebsted, skal du opdatere URL-adressen. Få en liste over alle organisationens nyhedswebsteder.
- Project Serverwebsteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt.
