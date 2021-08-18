---
title: Angiv ClientAccessServerEnabled til True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320350"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Angiv ClientAccessServerEnabled til True

Hvis du ikke kan åbne en krypteret mail og i stedet kan se en vedhæftet fil i **rpmsg,** skal du udføre følgende trin:

1. Forbind til Exchange Online PowerShell.

    **Bemærk!** For at oprette forbindelse Exchange Online PowerShell skal du logge på med en global administrator eller Exchange-administratorkonto.

   a. Åbn Windows PowerShell, og kør derefter følgende kommando:`$UserCredential = Get-Credential`
   b. I dialogboksen **Windows PowerShell legitimationsoplysninger skal** du angive din arbejds- eller skolekonto og adgangskode, c. Klik på **OK**. 

2. Kør følgende kommando for at oprette en ny session:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Kør følgende kommando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Kommandoen `Get-IRMConfiguration` Kør.

4. Kontrollér **indstillingen ClientAccessServerEnabled.** 

    a. Hvis **indstillingen ClientAccessServerEnabled** er indstillet **til Falsk,** skal du køre følgende cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tip:** Luk altid powershell-sessionen med følgende kommando: `Remove-PSSession $Session`

Du kan finde flere oplysninger [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

