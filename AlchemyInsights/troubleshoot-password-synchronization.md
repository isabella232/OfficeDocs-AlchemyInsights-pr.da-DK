---
title: Fejlfinding af synkronisering af adgangskoder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664920"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="24134-102">Fejlfinding af synkronisering af adgangskoder</span><span class="sxs-lookup"><span data-stu-id="24134-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="24134-103">Hvis du vil udføre fejlfinding af problemer med synkronisering af adgangskoder, skal du starte med at bruge denne AAD-forbindelses fejlfindings opgave for at finde ud af, hvorfor adgangskoder ikke</span><span class="sxs-lookup"><span data-stu-id="24134-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="24134-104">Gå til [Administrer direkte synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)for at starte.</span><span class="sxs-lookup"><span data-stu-id="24134-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="24134-105">Åbn en ny Windows PowerShell-session på Azure AD Connect-serveren, og vælg indstillingen **Kør som administrator** .</span><span class="sxs-lookup"><span data-stu-id="24134-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="24134-106">Kør set-ExecutionPolicy RemoteSigned eller set-ExecutionPolicy ubegrænset.</span><span class="sxs-lookup"><span data-stu-id="24134-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="24134-107">Start guiden Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="24134-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="24134-108">Gå til siden flere opgaver > **Foretag fejlfinding af**  >  **næste**.</span><span class="sxs-lookup"><span data-stu-id="24134-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="24134-109">Vælg **Start** for at åbne PowerShell-fejlfindings menuen.</span><span class="sxs-lookup"><span data-stu-id="24134-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="24134-110">Vælg **fejlfinding af adgangskode synkronisering**.</span><span class="sxs-lookup"><span data-stu-id="24134-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="24134-111">Problemet er normalt, at en adgangskode ikke er synkroniseret for en bestemt brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="24134-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="24134-112">**Noter** Synkronisering af adgangskoder mislykkes, hvis den seneste vellykkede adgangskode synkronisering var et stykke tid siden.</span><span class="sxs-lookup"><span data-stu-id="24134-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="24134-113">Hvis du vil have mere hjælp til fejlfinding af adgangskode synkronisering, skal du se [fejlfinding af synkronisering af adgangskoder med Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="24134-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>