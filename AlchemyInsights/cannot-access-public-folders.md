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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819506"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="35082-102">Outlook kan ikke oprette forbindelse til offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="35082-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="35082-103">Hvis adgang til offentlige mapper ikke fungerer for nogle brugere, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="35082-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="35082-104">Opret forbindelse til EXO PowerShell, og konfigurer DefaultPublicFolderMailbox-parameteren på problembrugerkontoen, så den matcher parameteren på en arbejdsbrugerkonto.</span><span class="sxs-lookup"><span data-stu-id="35082-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="35082-105">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="35082-105">Example:</span></span>

<span data-ttu-id="35082-106">Get-Mailbox WorkingUser-| ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="35082-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="35082-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="35082-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="35082-108">Vent mindst en time, indtil ændringen træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="35082-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="35082-109">Hvis problemet fortsætter, skal du følge denne [fremgangsmåde for at foretage fejlfinding](https://aka.ms/pfcte) af problemer med adgang til offentlige mapper ved hjælp af Outlook.</span><span class="sxs-lookup"><span data-stu-id="35082-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="35082-110">**Sådan styrer du, hvilke brugere der kan få adgang til offentlige mapper ved hjælp af Outlook:**</span><span class="sxs-lookup"><span data-stu-id="35082-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="35082-111">Brug Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $false</span><span class="sxs-lookup"><span data-stu-id="35082-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="35082-112">$true: Giv brugere adgang til offentlige mapper i Outlook</span><span class="sxs-lookup"><span data-stu-id="35082-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="35082-113">$false: Forebyd brugeradgang til offentlige mapper i Outlook.</span><span class="sxs-lookup"><span data-stu-id="35082-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="35082-114">Dette er standardværdien.</span><span class="sxs-lookup"><span data-stu-id="35082-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="35082-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="35082-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="35082-116">**Bemærk!** Denne fremgangsmåde kan kun styre forbindelser med Outlook-skrivebord til Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="35082-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="35082-117">En bruger kan fortsætte med at få adgang til offentlige mapper ved hjælp af OWA eller Outlook til Mac.</span><span class="sxs-lookup"><span data-stu-id="35082-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="35082-118">Du kan få mere [at vide under Meddelelse om understøttelse af kontrollerede forbindelser til offentlige mapper i Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="35082-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>