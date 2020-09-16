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
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771895"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive, langsom, utilgængelig eller ikke tilgængelig for flere brugere

SharePoint eller OneDrive kan være langsom, utilgængeligt eller utilgængeligt eller kan vise tjeneste ikke-tilgængelig eller 503-fejl, for flere årsager:
  
- Hvis dit SharePoint-eller OneDrive-websted er langsomt eller forsinket for flere brugere, kan der være et midlertidigt tjeneste problem, hvor brugerne oplever uregelmæssige forsinkelser eller navigerings fejl ved adgang til SharePoint-websteder eller OneDrive-indhold. Se [dashboardet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation er påvirket.
  
- Brugere kan modtage en *503-server, der er optaget* -fejl, når de forsøger at navigere til SharePoint-eller OneDrive-websteder. Denne fejl kan skyldes begrænsning i SharePoint-tjenesten. SharePoint Online anvender begrænsning til at opretholde optimal ydeevne og pålidelighed for SharePoint Online-tjenesten. Begrænsning begrænser antallet af brugerhandlinger eller samtidige kald (via script eller kode) for at forhindre overbelastning af ressourcer. Du kan finde flere oplysninger om begrænsning under [undgå at blive begrænset eller blokeret i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Hvis du oplever langsom ydeevne med et **klassisk** eller **moderne** SharePoint-websted eller-side, skal du bruge [værktøjet til side diagnosticering](https://aka.ms/perftool) til at analysere siderne.
  
- Hvis du stadig oplever generel langsom ydeevne, skal du gennemgå ressourcerne nederst i denne artikel: [Introduktion til justering af ydeevnen for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  