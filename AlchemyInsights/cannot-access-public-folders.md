---
title: Kan ikke få adgang til offentlige mapper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341397"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke oprette forbindelse til offentlige mapper

Hvis adgang til offentlige mapper ikke fungerer for nogle brugere, kan du prøve følgende:

Opret forbindelse til EXO PowerShell, og Konfigurer parameteren DefaultPublicFolderMailbox på den problem brugerkonto, så den svarer til parameteren på en arbejds brugerkonto.

:

Hent postkasser WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Vent mindst én time, før ændringen træder i kraft.

Hvis problemet fortsætter, skal du følge [denne fremgangsmåde](https://aka.ms/pfcte) for at foretage fejlfinding af offentlige mappe adgangsproblemer ved hjælp af Outlook.
 
**Sådan styrer du, hvilke brugere der har adgang til offentlige mapper ved hjælp af Outlook**:

1.  Brug set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $FALSE  
      
    $true: Tillad brugere at få adgang til offentlige mapper i Outlook  
      
    $false: undgå bruger adgang til offentlige mapper i Outlook. Dette er standardværdien.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Bemærk!** Denne fremgangsmåde kan kun styre forbindelser med Outlook-klient til Windows-klienter. En bruger kan fortsat få adgang til offentlige mapper ved hjælp af OWA eller Outlook til Mac.
 
Hvis du vil have mere at vide, skal du se Sådan får du [support til kontrollerede forbindelser til offentlige mapper i Outlook](https://aka.ms/controlpf).