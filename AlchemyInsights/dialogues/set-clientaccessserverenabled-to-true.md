---
title: Indstil ClientAccessServerEnabled til Sand
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523832"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Indstil ClientAccessServerEnabled til Sand

Hvis du ikke kan åbne en krypteret mail og i stedet får vist en vedhæftet **fil i rpmsg,** skal du udføre følgende trin:

1. Opret forbindelse til Exchange Online PowerShell.

> [!NOTE]
> Hvis du vil oprette forbindelse til Exchange Online PowerShell, skal du logge på med en global administrator- eller Exchange-administratorkonto.

   a. Åbn Windows PowerShell, og kør derefter følgende kommando: `$UserCredential = Get-Credential`
b. I dialogboksen **med anmodning om legitimationsoplysninger** til Windows PowerShell skal du angive din arbejds- eller skolekonto og adgangskode, c. Klik på **OK**. 

2. Kør følgende kommando for at oprette en ny session:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Kør følgende kommando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Kommandoen `Get-IRMConfiguration` Kør.

4. Kontrollér **indstillingen ClientAccessServerEnabled.** 

    a. Hvis **indstillingen ClientAccessServerEnabled** er indstillet til **Falsk,** skal du køre følgende cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Luk altid din PowerShell-session med følgende kommando: `Remove-PSSession $Session`

Du kan finde flere oplysninger i [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

