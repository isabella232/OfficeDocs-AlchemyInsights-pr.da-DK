---
title: Kontrollere adgang til offentlige mapper ved hjælp af Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032552"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrollere adgang til offentlige mapper ved hjælp af Outlook

Sådan styrer du, hvilke brugere der kan få adgang til offentlige mapper Outlook:

1. Brug `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Giv brugere adgang til offentlige mapper i Outlook  
$false: Forebyd brugeradgang til offentlige mapper i Outlook. Dette er standardværdien.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Bemærk! Denne fremgangsmåde kan kun styre forbindelser med Outlook til Windows klienter. Brugere kan fortsætte med at få adgang til offentlige mapper ved hjælp af OWA eller Outlook til Mac.

Du kan finde flere oplysninger [under Kontrollerede forbindelser til offentlige mapper i Outlook](https://aka.ms/controlpf) for at få flere oplysninger.
