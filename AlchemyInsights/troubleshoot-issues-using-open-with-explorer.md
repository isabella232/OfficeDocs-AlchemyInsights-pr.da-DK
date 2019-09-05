---
title: Fejlfinding af problemer ved hjælp af Åbn med Stifinder
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742727"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løs problemer med Åbn med Stifinder

Løs almindeligt forekommende problemer med at åbne et dokumentbibliotek i SharePoint eller OneDrive ved hjælp af kommandoen **Åbn med Stifinder** : 
  
- Brug Internet Explorer 10 eller Internet Explorer 11. **Åbn med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åbn med Stifinder** er deaktiveret i alle browsere undtagen Internet Explorer. 
    
- **Åbn med Stifinder** er ikke tilgængelig i den moderne oplevelse for SharePoint-biblioteker. Brug **i stedet Vis i Stifinder** . Vælg Vis **visningsindstillinger** \> **i Stifinder**. View in File Explorer er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis i Stifinder** i kun tilgængelig i Internet Explorer. 
    
- Kontroller, at tjenesten WebClient kører. Skriv Kør i søgefeltet i Windows, vælg Kør skrivebordsappen, skriv Services. msc, og tryk derefter på ENTER. Rul ned til tjenesten WebClient, og sørg for, at kolonnen **status** viser "kører". Hvis den ikke gør det, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**. (Du skal muligvis først aktivere tjenesten ved at vælge enten **Manuel** eller **automatisk** i feltet **starttype** ). 
    
> [!NOTE]
> Det er praktisk at åbne et bibliotek i Stifinder, hvis du har brug for at kopiere eller flytte flere filer og mapper én gang, men hvis du regelmæssigt vil arbejde i biblioteket, anbefaler vi, at du synkroniserer det. Hvis du vil foretage fejlfinding af problemer, som åbnes i Stifinder, skal du se [åbne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Du kan finde oplysninger om konfiguration af synkronisering under [Synkroniser SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artiklen [Sådan bruger du kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online for at](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) få flere oplysninger. 
  

