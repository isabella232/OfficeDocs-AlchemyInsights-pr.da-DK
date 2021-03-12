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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744648"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Brug Exchange Online PowerShell til at aktivere DKIM for et bestemt domæne

Hvis du ikke kan oprette DKIM DNS-posterne i Administration, kan du prøve at bruge Exchange Online PowerShell. 

Hvis du vil oprette en DKIM DNS-post ved hjælp af Exchange Online PowerShell, skal du udføre følgende trin:

1. Åbn Windows PowerShell som administrator, og kør følgende kommandoer i den beskrevne rækkefølge:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Hvis du har problemer med at oprette forbindelse til Exchange Online PowerShell, skal du se [Opret forbindelse til Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Når du har forbindelse til Exchange Online PowerShell, skal du køre følgende kommando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Når ovenstående kommando er blevet udført, skal du køre følgende kommando for at afslutte Exchange Online PowerShell-sessionen:

    `Remove-PSSession $Session` 



