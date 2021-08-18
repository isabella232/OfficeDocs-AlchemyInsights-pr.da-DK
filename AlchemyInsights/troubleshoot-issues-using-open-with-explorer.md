---
title: Fejlfinding af problemer med Åbn med Stifinder
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
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323560"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løs problemer med Åbn med Stifinder

Løs almindelige problemer med at åbne et dokumentbibliotek i SharePoint eller OneDrive ved hjælp af **kommandoen Åbn med Stifinder:** 
  
- Brug Internet Explorer 10 eller Internet Explorer 11. **Åbn med Stifinder** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åbn med Stifinder** er deaktiveret i alle browsere undtagen Internet Explorer. 
    
- **Åbn med Stifinder** er ikke tilgængelig i den moderne oplevelse for SharePoint biblioteker. Brug **Vis i Stifinder i** stedet. Vælg **Visningsindstillinger** \> **Vis i Stifinder**. Vis i Stifinder er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis i Stifinder** i kun tilgængelig i Internet Explorer. 
    
- Sørg for, at WebClient-tjenesten kører. I søgefeltet Windows skal du skrive Kør, vælge Kør skrivebordsapp, skrive services.msc og derefter trykke på Enter. Rul ned til WebClient-tjenesten, og sørg for, at **kolonnen Status** viser "Kører". Hvis den ikke gør det, skal du dobbeltklikke på tjenesten, klikke **på Start** og derefter klikke på **OK.** Du skal muligvis først aktivere tjenesten ved at vælge enten **Manuel** **eller Automatisk** i **feltet Starttype.** 
    
**Bemærk!** Det er praktisk at åbne et bibliotek i Stifinder, hvis du vil kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbejde regelmæssigt i biblioteket, anbefaler vi, at du synkroniserer det. Hvis du vil foretage fejlfinding af problemer med at åbne i Stifinder, [skal du se Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665). Du kan finde oplysninger om konfiguration af synkronisering [under Synkroniser SharePoint filer med den nye OneDrive-synkronisering klient.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Se artiklen Sådan bruger du kommandoen "Åbn med [Stifinder"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) til at foretage fejlfinding af problemer i SharePoint Online for at få flere oplysninger. 
  

