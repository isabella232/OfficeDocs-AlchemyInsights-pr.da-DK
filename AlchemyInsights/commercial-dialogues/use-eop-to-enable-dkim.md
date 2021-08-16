---
title: Brug Exchange Online PowerShell til at aktivere DKIM for et bestemt domæne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070288"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Brug Exchange Online PowerShell til at aktivere DKIM for et bestemt domæne

Hvis du ikke kan oprette DKIM DNS-poster i Administration, kan du prøve at bruge Exchange Online PowerShell. 

Hvis du vil oprette en DKIM DNS-post Exchange Online PowerShell, skal du udføre følgende trin:

1. Åbn Windows PowerShell administrator, og kør følgende kommandoer i den beskrevne rækkefølge:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Hvis du har problemer med at oprette forbindelse til Exchange Online PowerShell, [skal du Forbind til Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Når du har forbindelse til Exchange Online PowerShell, skal du køre følgende kommando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Når kommandoen ovenfor er blevet udført, skal du køre følgende kommando for at afslutte Exchange Online PowerShell-session:

    `Remove-PSSession $Session` 



