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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816734"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrollere adgang til offentlige mapper ved hjælp af Outlook

Sådan styrer du, hvilke brugere der kan få adgang til offentlige mapper ved hjælp af Outlook:

1. Brug `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Giv brugere adgang til offentlige mapper i Outlook  
$false: Forebyd brugeradgang til offentlige mapper i Outlook. Dette er standardværdien.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Bemærk! Denne fremgangsmåde kan kun styre forbindelser med Outlook-skrivebord til Windows-klienter. Brugere kan fortsætte med at få adgang til offentlige mapper ved hjælp af OWA eller Outlook til Mac.

Du kan finde flere oplysninger [i Kontrollerede forbindelser til offentlige mapper i Outlook](https://aka.ms/controlpf) for at få flere oplysninger.
