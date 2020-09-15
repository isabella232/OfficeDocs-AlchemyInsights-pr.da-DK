---
title: Problemer med at logge på Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695281"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="a0e46-102">Tomt logonskærmbillede i Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="a0e46-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="a0e46-103">Prøv følgende for at løse dette problem:</span><span class="sxs-lookup"><span data-stu-id="a0e46-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="a0e46-104">Installer de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="a0e46-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="a0e46-105">Nulstil indstillinger for Internet Explorer: gå til **funktioner**  >  **Internetindstillinger**  >  **Avanceret**  >  **Nulstil indstillinger for Internet Explorer** (Bemærk, at du mister brugerdefinerede indstillinger), og prøv derefter at logge på Office igen.</span><span class="sxs-lookup"><span data-stu-id="a0e46-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="a0e46-106">Deaktiver Windows Defender Application Guard (WDAG) eller lignende firewall-eller antivirusprogram:</span><span class="sxs-lookup"><span data-stu-id="a0e46-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="a0e46-107">I kontrol panel skal du gå til **programmer**og derefter vælge **slå Windows-funktioner til eller fra**.</span><span class="sxs-lookup"><span data-stu-id="a0e46-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="a0e46-108">Hvis Windows Defender Application Guard er aktiveret, kan du prøve at deaktivere det.</span><span class="sxs-lookup"><span data-stu-id="a0e46-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="a0e46-109">**Bemærk:** Du skal muligvis genstarte computeren.</span><span class="sxs-lookup"><span data-stu-id="a0e46-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="a0e46-110">Kontrollér, at [WAM-plug-in'en](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) for Microsoft. Aad. BrokerPlugin Aad ikke blokeres af programmer eller firewall/antivirusprogrammer.</span><span class="sxs-lookup"><span data-stu-id="a0e46-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="a0e46-111">[Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows credential Manager.</span><span class="sxs-lookup"><span data-stu-id="a0e46-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a0e46-112">**Bemærk:** Registreringsdatabase stierne til Office 2016 er blevet ændret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="a0e46-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a0e46-113">(F. eks.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a0e46-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="a0e46-114">Hvis du vil have mere at vide, skal du se [forbindelsesproblemer i logon efter opdatering til Office 2016 Build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="a0e46-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>