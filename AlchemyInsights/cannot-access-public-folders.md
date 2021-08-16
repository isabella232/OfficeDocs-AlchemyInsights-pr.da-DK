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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996624"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke oprette forbindelse til offentlige mapper

Hvis adgang til offentlige mapper ikke fungerer for nogle brugere, kan du prøve følgende:

Forbind EXO PowerShell og konfigurere DefaultPublicFolderMailbox-parameteren på problembrugerkontoen til at matche parameteren på en arbejdsbrugerkonto.

Eksempel:

Get-Mailbox WorkingUser-| ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Vent mindst en time, indtil ændringen træder i kraft.

Hvis problemet fortsætter, skal du følge denne [fremgangsmåde for at](https://aka.ms/pfcte) foretage fejlfinding af problemer med adgang til offentlige mapper ved hjælp Outlook.
 
**Sådan styrer du, hvilke brugere der kan få adgang til offentlige mapper ved hjælp Outlook:**

1.  Brug Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $false  
      
    $true: Giv brugere adgang til offentlige mapper i Outlook  
      
    $false: Forebyd brugeradgang til offentlige mapper i Outlook. Dette er standardværdien.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Bemærk!** Denne fremgangsmåde kan kun styre forbindelser med Outlook til Windows klienter. En bruger kan fortsætte med at få adgang til offentlige mapper ved hjælp af OWA eller Outlook til Mac.
 
Du kan få mere [at vide under Understøttelse af kontrollerede forbindelser til offentlige mapper i Outlook](https://aka.ms/controlpf).