---
title: Moderne site som roden site
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713785"
---
# <a name="modern-site-as-root-site"></a>Moderne websted som rodwebsted

Vi er begyndt at udrulle en ny funktion, der vil give dig mulighed for at [bytte din klassiske site root site med en moderne hjemmeside.](https://docs.microsoft.com/sharepoint/modern-root-site) Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted. Tilgængelig for både teamwebsted (ikke forbundet til en gruppe) og kommunikationswebsted.

>[!Important]
> Slet ikke dit klassiske rodwebsted for at oprette et moderne kommunikationswebsted. Dette understøttes ikke af Microsoft. Hvis du sletter rodwebstedet, bliver alle SharePoint-websteder i organisationen utilgængelige for alle brugere, indtil du gendanner webstedet eller opretter et nyt websted på den samme URL-adresse. Vi kommunikerer denne funktion via meddelelsescentret. Du bør forvente, at funktionen snart er slået til i din lejer.

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer med byttewebsteder
- Destinationswebstedet kan returnere en "ikke fundet" (HTTP 404) fejl i en kort periode.
- Indholdet skal crawles igen for at opdatere søgeindekset. Der er ingen manuel trin kræves her, vil dette ske automatisk.
- Alt, hvad der er afhængigt af "statiske" links (f.eks. filsynkronisering og OneNote-filer), skal rettes manuelt.
- Project Server-websteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt. 
