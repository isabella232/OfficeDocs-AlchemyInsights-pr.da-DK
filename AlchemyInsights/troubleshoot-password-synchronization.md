---
title: Fejlfinding i forbindelse med synkronisering af adgangskoder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387871"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="f4e23-102">Fejlfinding i forbindelse med synkronisering af adgangskoder</span><span class="sxs-lookup"><span data-stu-id="f4e23-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="f4e23-103">Hvis du vil foretage fejlfinding af problemer med synkronisering af adgangskoder, skal du starte med at bruge denne fejlfindingsopgave til AAD Connect for at finde ud af, hvorfor adgangskoder ikke synkroniseres.</span><span class="sxs-lookup"><span data-stu-id="f4e23-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="f4e23-104">Gå til Administrer direkte [synkronisering for at begynde.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)</span><span class="sxs-lookup"><span data-stu-id="f4e23-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="f4e23-105">Åbn en ny Windows PowerShell-session på din Azure AD Connect-server, og vælg **indstillingen Kør som** administrator.</span><span class="sxs-lookup"><span data-stu-id="f4e23-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="f4e23-106">Kør Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="f4e23-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="f4e23-107">Start guiden Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f4e23-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="f4e23-108">Gå til siden Yderligere opgaver > **Fejlfinding af**  >  **næste**.</span><span class="sxs-lookup"><span data-stu-id="f4e23-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="f4e23-109">Vælg **Start** for at åbne fejlfindingsmenuen i PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f4e23-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="f4e23-110">Vælg **Fejlfinding af synkronisering af adgangskode**.</span><span class="sxs-lookup"><span data-stu-id="f4e23-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="f4e23-111">Problemet er normalt, at en adgangskode ikke synkroniseres for en bestemt brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="f4e23-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="f4e23-112">**Bemærkninger** Synkronisering af adgangskoder mislykkes, hvis den seneste vellykkede synkronisering af adgangskoder var for nogen tid siden.</span><span class="sxs-lookup"><span data-stu-id="f4e23-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="f4e23-113">Du kan finde flere hjælp til fejlfinding af synkronisering af adgangskoder under [Fejlfinding af synkronisering af hash for adgangskoder med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="f4e23-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>