---
title: Problemer med ydeevnen – SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911836"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive langsom, utilgængelig eller utilgængelig for flere brugere

SharePoint eller OneDrive er langsomme, utilgængelige eller utilgængelige, eller der kan blive vist fejl om, at tjenesten ikke er tilgængelig eller 503, af forskellige årsager:
  
- Hvis dit SharePoint- eller OneDrive-websted er langsomt eller forsinket for flere brugere, kan der være et midlertidigt tjenesteproblem, hvor brugerne oplever forbigående forsinkelser eller navigationsfejl, når de får adgang til SharePoint websteder eller OneDrive indhold. Kontrollér [dashboardet Tjenestetilstand for](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) at se, om din organisation påvirkes.
  
- Brugere modtager muligvis en *fejl på 503-serveren* er optaget, når de forsøger at navigere til SharePoint eller OneDrive websteder. Denne fejl kan skyldes begrænsning i SharePoint tjeneste. SharePoint Online anvender begrænsning til at opretholde optimal ydeevne og pålidelighed for SharePoint Online-tjenesten. Begrænsning begrænser antallet af brugerhandlinger eller samtidige kald (via script eller kode) for at forhindre overbelastning af ressourcer. Du kan finde flere oplysninger om begrænsning i Undgå at [blive begrænsning eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Hvis du oplever langsom ydeevne med en **klassisk** eller moderne **SharePoint** på et websted eller en side, skal du bruge værktøjet [Sidediagnosticering](https://aka.ms/perftool) til at analysere siderne.
  
- Hvis du stadig oplever generel langsom ydeevne, skal du gennemse ressourcerne nederst i denne artikel: Introduktion til justering af [ydeevnen for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  