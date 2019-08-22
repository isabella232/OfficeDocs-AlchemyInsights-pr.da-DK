---
title: Søg i SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507625"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Indhold for websøgning eller indeksering i SharePoint Online

Indholdet skal gennemsøges og tilføjet i søgeindekset for brugerne at finde det, de søger efter, i SharePoint Online. Indhold gennemsøges automatisk baseret på en foruddefineret gennemsøgning tidsplan (gennemsøgning tidsplanen ikke kan ændres). Crawleren henter indhold, der er blevet ændret siden den seneste gennemsøgning og opdaterer indekset. For at sikre indhold gennemsøges og indekset bliver opdateret, være opmærksom på følgende:

- Kontroller, at indholdet kan findes ved [at gøre webstedets indhold kan søges](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Når du har ændret en administreret egenskab, eller når du har ændret tilknytning af gennemsøgt og administrerede skal egenskaber for webstedet være gennemsøgt igen, før ændringerne afspejles i søgeindekset. 

    Indeksere webstedet igen, da ændringerne foretages i search-skema, og ikke på webstedet faktiske crawleren ikke automatisk. 

    Flere oplysninger, skal du [manuelt anmode om gennemsøgning og indeksering igen af et websted, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Vent mindst 24 timer efter manuelt anmode om en gennemsøgning og fuld gendanne indekset for at se, hvis du stadig har et problem. 

    Hvis der er gået mere end 24 timer, da du startede gennemsøgning og fuld indekseres, skal du logge en supportsag. I mange tilfælde kan arbejder vi allerede på en løsning. Giv os, mindst 24 timer at gennemføre en løsning.

> [!IMPORTANT]
> Hvis et websted dokument (bibliotek), eller en liste er blevet slettet, og stadig vises i søgeresultaterne, brugere skal modtage en **404 fil ikke fundet fejl** under forsøget på at få adgang til den. Dette problem bør registreres som en supportsag til yderligere undersøgelse. 



