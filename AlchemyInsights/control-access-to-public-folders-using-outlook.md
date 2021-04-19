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
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="3ec6c-102">Kontrollere adgang til offentlige mapper ved hjælp af Outlook</span><span class="sxs-lookup"><span data-stu-id="3ec6c-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="3ec6c-103">Sådan styrer du, hvilke brugere der kan få adgang til offentlige mapper ved hjælp af Outlook:</span><span class="sxs-lookup"><span data-stu-id="3ec6c-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="3ec6c-104">Brug `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="3ec6c-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="3ec6c-105">$true: Giv brugere adgang til offentlige mapper i Outlook</span><span class="sxs-lookup"><span data-stu-id="3ec6c-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="3ec6c-106">$false: Forebyd brugeradgang til offentlige mapper i Outlook.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="3ec6c-107">Dette er standardværdien.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="3ec6c-108">Bemærk! Denne fremgangsmåde kan kun styre forbindelser med Outlook-skrivebord til Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="3ec6c-109">Brugere kan fortsætte med at få adgang til offentlige mapper ved hjælp af OWA eller Outlook til Mac.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="3ec6c-110">Du kan finde flere oplysninger [i Kontrollerede forbindelser til offentlige mapper i Outlook](https://aka.ms/controlpf) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
