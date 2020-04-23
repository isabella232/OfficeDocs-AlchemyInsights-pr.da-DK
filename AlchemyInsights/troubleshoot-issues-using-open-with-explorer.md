---
title: Fejlfinding i forbindelse med problemer ved hjælp af Åbn med Stifinder
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759686"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løs problemer med Åbn med Stifinder

Løs almindelige problemer med at åbne et dokumentbibliotek i SharePoint eller OneDrive ved hjælp af kommandoen **Åbn med Stifinder:** 
  
- Brug Internet Explorer 10 eller Internet Explorer 11. **Åbn med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åbn med Stifinder** er deaktiveret i alle browsere undtagen Internet Explorer. 
    
- **Åbn med Stifinder** er ikke tilgængelig i den moderne oplevelse for SharePoint-biblioteker. Brug i stedet **Vis i Stifinder.** Vælg **Vis indstillinger** \> **Vis i Stifinder**. Visningen i Stifinder er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox m.fl. **Få vist i Stifinder** i Kun tilgængelig i Internet Explorer. 
    
- Kontroller, at webclient-tjenesten kører. Skriv kør i søgefeltet i Windows, vælg appen Kør skrivebord, skriv services.msc, og tryk derefter på Enter. Rul ned til tjenesten WebClient, og sørg for, at kolonnen **Status** viser "Kørsel". Hvis det ikke er tilfældet, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**. (Du skal muligvis først aktivere tjenesten ved at vælge enten **Manuel** eller **Automatisk** i feltet **Starttype).** 
    
> [!NOTE]
> Det er praktisk at åbne et bibliotek i Stifinder, hvis du har brug for at kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbejde regelmæssigt i biblioteket, anbefaler vi, at du synkroniserer det. Hvis du vil foretage fejlfinding af problemer med at åbne i Stifinder, skal du se [Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665). Du kan finde oplysninger om konfiguration af synkronisering under [Synkronisere SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artiklen [Sådan bruges kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for at få flere oplysninger. 
  

