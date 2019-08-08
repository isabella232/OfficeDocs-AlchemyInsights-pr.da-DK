---
title: Byt dine Classic-rodwebstedet med et moderne websted
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245951"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byt dine Classic-rodwebstedet med et moderne websted

Hvis dit miljø blev oprettet før April 2019, kan du ændre rod-websted til et moderne websted ved hjælp af Microsoft PowerShell:

- Hvis du har et andet websted, som du vil bruge som rod-websted, kan du erstatte (swapfilen) rod-websted med den. 
    - Brug [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at skifte placeringen af et websted med et andet websted under arkivering af det oprindelige websted. Tilgængelig for både Team (ikke har forbindelse til en gruppe) og kommunikation. 

- Ekstra funktioner introduceres snarest, der giver dig mulighed at holde med indhold på webstedet, men konvertere det eksisterende websted til et kommunikationswebsted. 
>[!Important]
>Disse funktioner vil blive gennemført gradvist. Fortsætte med at kontrollere Office 365 Message Center for opdateringer. 

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer i forbindelse med udskiftning af websteder

- Målwebstedet kan returnere fejlen "ikke fundet" (HTTP 404) for en kort periode.
- Indholdet skal være recrawled for at opdatere søgeindekset. Der er ingen manuelle trin, der kræves - dette gøres automatisk.
- Alt afhængig af "statiske" links (f.eks filsynkronisering og OneNote-filer) skal rettes manuelt.
- Hvis kildewebstedet var en organisatorisk nyhedswebsted, kan du opdatere URL-adressen.Få en liste over websteder med alle Nyheder i virksomheden.
- Project Server-websteder skal valideres for at sikre, at de er stadig knyttet korrekt.





