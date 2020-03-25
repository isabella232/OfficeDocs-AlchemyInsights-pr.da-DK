---
title: Begrænsning af SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931220"
---
# <a name="sharepoint-online-throttling"></a>Begrænsning af SharePoint Online

**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden. Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger. I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.

Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage. Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider. I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.

**503-serveren er optaget**

Brugerne får muligvis vist en 503-server, der er optaget, når de forsøger at navigere til SharePoint- eller OneDrive-websteder. 

Denne fejl kan skyldes begrænsning i SharePoint-tjenesten. SharePoint Online bruger begrænsning til at opretholde optimal ydeevne og pålidelighed i SharePoint Online-tjenesten. Begrænsning begrænser antallet af brugerhandlinger eller samtidige opkald (efter script eller kode) for at forhindre overforbrug af ressourcer. 

Du kan finde flere oplysninger om begrænsning under [Undgå at blive kvalt eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Hvis du mener, at denne fejl ikke er relateret til begrænsning, kan du kontrollere, om der er aktiv vedligeholdelse på din lejer, ved at navigere til [Meddelelsescenter](https://portal.office.com/adminportal/home#/MessageCenter).

 Endelig skal du sørge for at besøge [siden Tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth) for at kontrollere, om der er råd/hændelser, der måtte forekomme.

