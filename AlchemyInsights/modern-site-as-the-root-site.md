---
title: Moderne websted som rodwebsted
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753898"
---
# <a name="modern-site-as-root-site"></a>Moderne websted som rodwebsted

Vi er begyndt at udrulning en ny funktion, der vil give dig mulighed for at [bytte din klassiske site root site med en moderne hjemmeside](https://docs.microsoft.com/sharepoint/modern-root-site). Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted. Tilgængelig for både team websted (ikke forbundet til en gruppe) og kommunikationswebsted.

>[!Important]
> Du må ikke slette dit klassiske rodwebsted for at oprette et moderne kommunikationswebsted. Dette understøttes ikke af Microsoft. Hvis du sletter rodwebstedet, bliver alle SharePoint-websteder i organisationen utilgængelige for alle brugere, indtil du gendanner webstedet eller opretter et nyt websted på samme webadresse. Vi kommunikerer denne funktion via meddelelsescenteret. Du kan forvente, at funktionen er aktiveret i din lejer inden længe.

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer med swapping sites
- Destinationswebstedet kan returnere fejlen "ikke fundet" (HTTP 404) i en kort periode.
- Indholdet skal sættes i igen for at opdatere søgeindekset. Der er ingen manuelle trin kræves her, dette vil ske automatisk.
- Alt, hvad der er afhængigt af "statiske" links (f. eks. filsynkronisering og OneNote-filer), skal korrigeres manuelt.
- Project Server-websteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt. 
