---
title: Problemer med ydeevnen-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068390"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive langsom, utilgængelig eller utilgængelig for flere brugere

SharePoint eller OneDrive kan være langsomme, utilgængelige eller utilgængelige eller kan vise tjenesten utilgængelig eller 503 fejl af flere årsager:
  
- Hvis dit SharePoint-eller OneDrive-websted er langsomt eller forsinket for flere brugere, kan der være et midlertidigt serviceproblem, hvor brugere oplever periodiske forsinkelser eller navigationsfejl, når de får adgang til SharePoint-websteder eller OneDrive-indhold. Kontroller [dashboardet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation påvirkes.
  
- Brugere kan modtage en *503 server er optaget* fejl, når de forsøger at navigere til SharePoint eller OneDrive sites. Denne fejl kan forårsages af begrænsning i SharePoint-tjenesten. SharePoint Online brugerbegrænsning til at opretholde den optimale ydeevne og pålidelighed af SharePoint Online-tjenesten. Throttling begrænser antallet af brugerhandlinger eller samtidige kald (efter script eller kode) for at forhindre overforbrug af ressourcer. Du finder flere oplysninger om begrænsning under Se ved at [undgå at blive begrænset eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Hvis du oplever langsom ydeevne med et **klassisk** eller **moderne** SharePoint-websted eller-side, skal du bruge [værktøjet til side diagnosticering](https://aka.ms/perftool) til at analysere siderne.
  
- Hvis du stadig oplever generel langsom ydeevne, skal du gennemse ressourcerne nederst i denne artikel: [Introduktion til justering af ydeevnen for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  