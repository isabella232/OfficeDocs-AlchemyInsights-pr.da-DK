---
title: Moderne sted som rodwebstedet
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
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543847"
---
# <a name="modern-site-as-root-site"></a>Moderne sted som rodwebstedet

Vi er begyndt til distribuering af en ny funktion, der gør det muligt at skifte din klassiske websted-rodwebstedet med et moderne websted. Brug [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til at skifte placeringen af et websted med et andet websted under arkivering af det oprindelige websted. Tilgængelig for både Team (ikke har forbindelse til en gruppe) og kommunikation. 

>[!Important]
> Slet ikke klassiske rod-webstedet for at oprette et websted til et moderne kommunikation. Dette understøttes ikke af Microsoft. Slette rodwebstedet, bliver alle SharePoint-websteder i din organisation utilgængelige for alle brugere, før du gendanne webstedet eller oprette et nyt websted med samme URL-adresse. Vi kommunikere denne funktion via Beskedcentret. Du kan forvente, at funktionen være aktiveret i din lejer kort.

## <a name="known-issues-with-swapping-sites"></a>Kendte problemer i forbindelse med udskiftning af websteder
- Målwebstedet kan returnere fejlen "ikke fundet" (HTTP 404) for en kort periode.
- Indholdet skal være recrawled for at opdatere søgeindekset. Der er ingen manuelle trin, der kræves her, dette gøres automatisk.
- Alt afhængig af "statiske" links (f.eks filsynkronisering og OneNote-filer) skal rettes manuelt.
- Project Server-websteder skal valideres for at sikre, at de er stadig knyttet korrekt. 
