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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="241cd-102">Outlook kan ikke oprette forbindelse til offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="241cd-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="241cd-103">Hvis adgang til offentlige mapper ikke fungerer for nogle brugere, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="241cd-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="241cd-104">Opret forbindelse til EXO PowerShell, og Konfigurer parameteren DefaultPublicFolderMailbox på den problem brugerkonto, så den svarer til parameteren på en arbejds brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="241cd-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="241cd-105">:</span><span class="sxs-lookup"><span data-stu-id="241cd-105">Example:</span></span>

<span data-ttu-id="241cd-106">Hent postkasser WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="241cd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="241cd-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="241cd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="241cd-108">Vent mindst én time, før ændringen træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="241cd-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="241cd-109">Hvis problemet fortsætter, skal du følge [denne fremgangsmåde](https://aka.ms/pfcte) for at foretage fejlfinding af offentlige mappe adgangsproblemer ved hjælp af Outlook.</span><span class="sxs-lookup"><span data-stu-id="241cd-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="241cd-110">**Sådan styrer du, hvilke brugere der har adgang til offentlige mapper ved hjælp af Outlook**:</span><span class="sxs-lookup"><span data-stu-id="241cd-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="241cd-111">Brug set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $FALSE</span><span class="sxs-lookup"><span data-stu-id="241cd-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="241cd-112">$true: Tillad brugere at få adgang til offentlige mapper i Outlook</span><span class="sxs-lookup"><span data-stu-id="241cd-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="241cd-113">$false: undgå bruger adgang til offentlige mapper i Outlook.</span><span class="sxs-lookup"><span data-stu-id="241cd-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="241cd-114">Dette er standardværdien.</span><span class="sxs-lookup"><span data-stu-id="241cd-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="241cd-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="241cd-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="241cd-116">**Bemærk!** Denne fremgangsmåde kan kun styre forbindelser med Outlook-klient til Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="241cd-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="241cd-117">En bruger kan fortsat få adgang til offentlige mapper ved hjælp af OWA eller Outlook til Mac.</span><span class="sxs-lookup"><span data-stu-id="241cd-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="241cd-118">Hvis du vil have mere at vide, skal du se Sådan får du [support til kontrollerede forbindelser til offentlige mapper i Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="241cd-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>