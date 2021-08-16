---
title: Moderne websted som rodwebsted
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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000380"
---
# <a name="modern-site-as-root-site"></a>Moderne websted som rodwebsted

Vi er begyndt at udrulle en ny funktion, der giver dig mulighed for at [bytte dit klassiske rodwebsted med et moderne websted.](https://docs.microsoft.com/sharepoint/modern-root-site) Brug [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at bytte placeringen af et websted med et andet websted under arkivering af det oprindelige websted. Tilgængelig for både Teamwebsted (ikke forbundet med en gruppe) og Kommunikationswebsted.

>[!Important]
> Slet ikke dit klassiske rodwebsted for at oprette et moderne kommunikationswebsted. Dette understøttes ikke af Microsoft. Hvis du sletter rodwebstedet, vil SharePoint alle websteder i organisationen være utilgængelige for alle brugere, indtil du gendanner webstedet eller opretter et nyt websted på den samme URL-adresse. Vi kommunikerer denne funktion via meddelelsescenteret. Du kan forvente, at funktionen snart bliver aktiveret i din lejer.

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer med udskiftning af websteder
- Destinationswebstedet returnerer muligvis fejlen "blev ikke fundet" (HTTP 404) i en kort periode.
- Indhold skal slås sammen igen for at opdatere søgeindekset. Der kræves ingen manuelle trin her. Dette udføres automatisk.
- Alt afhængigt af "statiske" links (f.eks filsynkronisering og OneNote filer) skal rettes manuelt.
- Project Serverwebsteder skal muligvis valideres for at sikre, at de stadig er tilknyttet korrekt. 
