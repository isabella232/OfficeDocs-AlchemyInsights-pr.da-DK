---
title: Søg i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044037"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Indholds gennemsøgning og indeksering i SharePoint Online

Indholdet skal crawlede og føjes til søgeindekset, for at brugerne kan finde det, de søger efter, i SharePoint Online. Indhold gennemsøges automatisk ud fra en foruddefineret tidsplan (gennemsøgnings planen kan ikke ændres). Crawleren henter indhold, der er ændret siden sidste gennemsøgning, og opdaterer indekset. Bemærk følgende for at sikre, at indholdet gennemsøges, og indekset opdateres:

- Sørg for, at indhold kan findes ved [at gøre webstedsindhold søgbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Når du har ændret en administreret egenskab, eller når du har ændret tilknytningen af gennemsøgte og administrerede egenskaber, skal webstedet crawles igen, før ændringerne afspejles i søgeindekset. 

    Da dine ændringer foretages i søgeskemaet og ikke på det faktiske websted, indekseres webcrawleren ikke automatisk webstedet igen. 

    Du kan finde flere oplysninger under [Manuel anmodning om gennemsøgning og genindekse ring af et websted, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Vent mindst 24 timer efter, at du manuelt har anmodet om en gennemsøgning og et fuldstændigt genindeks for at se, om du stadig oplever et problem. 

    Hvis der er gået mere end 24 timer, siden du indledte gennemsøgningen og fuld re-index, skal du logge en support sag. I mange tilfælde arbejder vi allerede på en løsning. Giv os mindst 24 timer til at gennemføre en løsning.

> [!IMPORTANT]
> Hvis et websted, dokument (bibliotek) eller en liste er blevet slettet og stadig vises i søgeresultaterne, skal brugerne modtage en **fejl 404-fil, der ikke blev fundet** , da de forsøgte at få adgang til den. Dette spørgsmål skal registreres som en støtte sag for yderligere undersøgelse. 



