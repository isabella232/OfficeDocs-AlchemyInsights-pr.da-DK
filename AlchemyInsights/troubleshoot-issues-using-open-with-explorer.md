---
title: Foretage fejlfinding af problemer ved hjælp af Åbn med Stifinder
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
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759288"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løse problemer med Åbn med Stifinder

Løse almindelige problemer med at åbne et dokumentbibliotek i SharePoint- eller OneDrive ved hjælp af kommandoen **Åbn med Stifinder** : 
  
- Brug Internet Explorer 10 eller Internet Explorer 11. **Åbn med Stifinder** ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åbn med Stifinder** er deaktiveret i alle browsere, med undtagelse af Internet Explorer. 
    
- **Åbn med Stifinder** er ikke tilgængelig i den moderne oplevelse for SharePoint-biblioteker. I stedet for at bruge **Vis i Stifinder** . Vælg **visningsindstillinger** \> **Vis i Stifinder**. Vis i Stifinder er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis i Stifinder** i kun tilgængelig i Internet Explorer. 
    
- Kontroller, at tjenesten WebClient kører. I Windows søgefeltet, Skriv Kør, Vælg Kør stationære programmet, skriv services.msc, og tryk derefter på Enter. Rul ned til tjenesten WebClient, og Sørg for, at kolonnen **Status** viser "Kørsel". Hvis det ikke er tilfældet, skal du dobbeltklikke på tjenesten, klik på **Start**og klik derefter på **OK**. (Du skal muligvis først aktivere tjenesten ved at vælge enten **Manuel** eller **automatisk** i **boksen** ). 
    
> [!NOTE]
> Åbne et bibliotek i Stifinder er praktisk, hvis du vil kopiere eller flytte flere filer og mapper, når, men hvis du vil arbejde regelmæssigt i biblioteket, anbefaler vi synkroniserer den. Hvis du vil foretage fejlfinding af problemer, der er åbne i Filoversigt, se [åbne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Du kan finde oplysninger om konfiguration af synkronisering, [Synkroniser SharePoint-filer med den nye OneDrive sync-klient](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artiklen [Sådan bruges kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for at få yderligere oplysninger. 
  

