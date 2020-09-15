---
title: Moderne websted som rodwebstedet
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666864"
---
# <a name="modern-site-as-root-site"></a>Moderne websted som rodwebstedet

Vi er gået i kontakt med en ny funktion, der giver dig mulighed for at [udskifte dit klassiske websted med et moderne websted](https://docs.microsoft.com/sharepoint/modern-root-site). Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) for at udskifte placeringen af et websted med et andet websted, mens du arkiverer det oprindelige websted. Tilgængelig for begge team websteder (ikke forbundet til en gruppe) og kommunikationswebsted.

>[!Important]
> Slet ikke dit klassiske websted for at oprette et moderne kommunikationswebsted. Dette understøttes ikke af Microsoft. Hvis du sletter rodwebstedet, bliver alle SharePoint-websteder i organisationen utilgængelige for alle brugere, indtil du gendanner webstedet eller opretter et nyt websted på den samme URL-adresse. Vi kommunikerer denne funktion via meddelelses Center. Du skal forvente, at funktionen skulle slås til på din lejer i sin tid.

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer med swap websteder
- Destinationswebstedet kan returnere fejlen "ikke fundet" (HTTP 404) for en kort periode.
- Indhold skal gennemsøges for at opdatere søgeindekset. Der kræves intet manuelt trin her, det sker automatisk.
- Alt afhængigt af "statiske" links (f. eks. filsynkronisering og OneNote-filer) skal rettes manuelt.
- Project Server-websteder skal muligvis valideres for at sikre, at de stadig er knyttet korrekt. 
