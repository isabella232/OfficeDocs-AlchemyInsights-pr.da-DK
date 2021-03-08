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
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="3985f-102">Indstil ClientAccessServerEnabled til Sand</span><span class="sxs-lookup"><span data-stu-id="3985f-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="3985f-103">Hvis du ikke kan åbne en krypteret mail og i stedet får vist en vedhæftet **fil i rpmsg,** skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="3985f-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="3985f-104">Opret forbindelse til Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3985f-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="3985f-105">Hvis du vil oprette forbindelse til Exchange Online PowerShell, skal du logge på med en global administrator- eller Exchange-administratorkonto.</span><span class="sxs-lookup"><span data-stu-id="3985f-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="3985f-106">a.</span><span class="sxs-lookup"><span data-stu-id="3985f-106">a.</span></span> <span data-ttu-id="3985f-107">Åbn Windows PowerShell, og kør derefter følgende kommando: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="3985f-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="3985f-108">b.</span><span class="sxs-lookup"><span data-stu-id="3985f-108">b.</span></span> <span data-ttu-id="3985f-109">I dialogboksen **med anmodning om legitimationsoplysninger** til Windows PowerShell skal du angive din arbejds- eller skolekonto og adgangskode, c.</span><span class="sxs-lookup"><span data-stu-id="3985f-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="3985f-110">Klik på **OK**.</span><span class="sxs-lookup"><span data-stu-id="3985f-110">Click **OK**.</span></span> 

2. <span data-ttu-id="3985f-111">Kør følgende kommando for at oprette en ny session:</span><span class="sxs-lookup"><span data-stu-id="3985f-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="3985f-112">a.</span><span class="sxs-lookup"><span data-stu-id="3985f-112">a.</span></span> <span data-ttu-id="3985f-113">Kør følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="3985f-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="3985f-114">Kommandoen `Get-IRMConfiguration` Kør.</span><span class="sxs-lookup"><span data-stu-id="3985f-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="3985f-115">Kontrollér **indstillingen ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="3985f-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="3985f-116">a.</span><span class="sxs-lookup"><span data-stu-id="3985f-116">a.</span></span> <span data-ttu-id="3985f-117">Hvis **indstillingen ClientAccessServerEnabled** er indstillet til **Falsk,** skal du køre følgende cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="3985f-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="3985f-118">Luk altid din PowerShell-session med følgende kommando: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="3985f-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="3985f-119">Du kan finde flere oplysninger i [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="3985f-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

