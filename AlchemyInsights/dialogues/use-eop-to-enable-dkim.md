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
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523637"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="d1e75-102">Brug Exchange Online PowerShell til at aktivere DKIM for et bestemt domæne</span><span class="sxs-lookup"><span data-stu-id="d1e75-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="d1e75-103">Hvis du ikke kan oprette DKIM DNS-posterne i Administration, kan du prøve at bruge Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d1e75-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="d1e75-104">Hvis du vil oprette en DKIM DNS-post ved hjælp af Exchange Online PowerShell, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="d1e75-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="d1e75-105">Åbn Windows PowerShell som administrator, og kør følgende kommandoer i den beskrevne rækkefølge:</span><span class="sxs-lookup"><span data-stu-id="d1e75-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="d1e75-106">a.</span><span class="sxs-lookup"><span data-stu-id="d1e75-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="d1e75-107">b.</span><span class="sxs-lookup"><span data-stu-id="d1e75-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="d1e75-108">c.</span><span class="sxs-lookup"><span data-stu-id="d1e75-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="d1e75-109">Hvis du har problemer med at oprette forbindelse til Exchange Online PowerShell, skal du se [Opret forbindelse til Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="d1e75-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="d1e75-110">Når du har forbindelse til Exchange Online PowerShell, skal du køre følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="d1e75-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="d1e75-111">Når ovenstående kommando er blevet udført, skal du køre følgende kommando for at afslutte Exchange Online PowerShell-sessionen:</span><span class="sxs-lookup"><span data-stu-id="d1e75-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



