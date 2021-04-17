---
title: Kan ikke få adgang til offentlige mapper
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819506"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke oprette forbindelse til offentlige mapper

Hvis adgang til offentlige mapper ikke fungerer for nogle brugere, kan du prøve følgende:

Opret forbindelse til EXO PowerShell, og konfigurer DefaultPublicFolderMailbox-parameteren på problembrugerkontoen, så den matcher parameteren på en arbejdsbrugerkonto.

Eksempel:

Get-Mailbox WorkingUser-| ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Vent mindst en time, indtil ændringen træder i kraft.

Hvis problemet fortsætter, skal du følge denne [fremgangsmåde for at foretage fejlfinding](https://aka.ms/pfcte) af problemer med adgang til offentlige mapper ved hjælp af Outlook.
 
**Sådan styrer du, hvilke brugere der kan få adgang til offentlige mapper ved hjælp af Outlook:**

1.  Brug Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $false  
      
    $true: Giv brugere adgang til offentlige mapper i Outlook  
      
    $false: Forebyd brugeradgang til offentlige mapper i Outlook. Dette er standardværdien.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Bemærk!** Denne fremgangsmåde kan kun styre forbindelser med Outlook-skrivebord til Windows-klienter. En bruger kan fortsætte med at få adgang til offentlige mapper ved hjælp af OWA eller Outlook til Mac.
 
Du kan få mere [at vide under Meddelelse om understøttelse af kontrollerede forbindelser til offentlige mapper i Outlook.](https://aka.ms/controlpf)