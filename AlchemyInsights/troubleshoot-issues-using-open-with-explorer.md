---
title: Fejlfinding af problemer ved hjælp af Åbn med Stifinder
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659052"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løs problemer med Åbn med Stifinder

Løse almindelige problemer med at åbne et dokumentbibliotek i SharePoint eller OneDrive ved hjælp af kommandoen **Åbn med Stifinder** : 
  
- Brug Internet Explorer 10 eller Internet Explorer 11. **Åbn med Stifinder** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åbn med Stifinder** er deaktiveret i alle browsere undtagen Internet Explorer. 
    
- **Åbn med Stifinder** er ikke tilgængelig i den moderne oplevelse for SharePoint-biblioteker. Brug **visningen i Stifinder i** stedet. Vælg visningen **Indstillinger for visning** \> **i Stifinder**. Visning i Stifinder er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis i Stifinder** i kun tilgængelig i Internet Explorer. 
    
- Sørg for, at WebClient-tjenesten kører. Skriv Kør i feltet Windows Search, Vælg appen Kør skrivebord, skriv Services. msc, og tryk derefter på ENTER. Rul ned til WebClient-tjenesten, og sørg for, at **status** kolonnen viser "kører". Hvis det ikke er det, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**. (Du skal muligvis først aktivere tjenesten ved enten at vælge **Manuel** eller **automatisk** i feltet **starttype** .) 
    
> [!NOTE]
> Det anbefales at åbne et bibliotek i Stifinder, hvis du har brug for at kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbejde regelmæssigt i biblioteket, anbefaler vi at synkronisere det. Hvis du vil foretage fejlfinding af problemer, der åbnes i Stifinder, skal du se [Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665). Du kan finde oplysninger om, hvordan du konfigurerer synkronisering, under [synkronisere SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666).
  
Læs artiklen [Sådan bruger du kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online for at](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) få flere oplysninger. 
  

