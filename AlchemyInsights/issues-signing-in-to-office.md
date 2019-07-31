---
title: Problemer, der logger på Office apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938175"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="01dda-102">Tom-logon-skærmen i Office-programmer</span><span class="sxs-lookup"><span data-stu-id="01dda-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="01dda-103">Du kan løse dette problem, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="01dda-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="01dda-104">Installere de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="01dda-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="01dda-105">Nulstille indstillingerne i Internet Explorer: gå til **Tools** > **Internet-indstillinger** > **Avanceret** > **Reset Internet Explorer Settings** (Bemærk, at du mister brugerdefinerede indstillinger), og prøv derefter at logge på Office igen.</span><span class="sxs-lookup"><span data-stu-id="01dda-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="01dda-106">Deaktiver Windows Defender-programmet Guard (WDAG) eller et tilsvarende firewall eller anti-virus program:</span><span class="sxs-lookup"><span data-stu-id="01dda-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="01dda-107">Gå til **programmer**i Kontrolpanel, og vælg derefter **Slå Windows-funktioner til eller fra**.</span><span class="sxs-lookup"><span data-stu-id="01dda-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="01dda-108">Hvis Windows Defender-programmet Guard er aktiveret, kan du prøve at deaktivere den.</span><span class="sxs-lookup"><span data-stu-id="01dda-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="01dda-109">**Bemærk:** Du skal muligvis genstarte computeren.</span><span class="sxs-lookup"><span data-stu-id="01dda-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="01dda-110">Sørg for, at Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokeres af et program eller en firewall antivirus-/ sikkerhedssoftware program.</span><span class="sxs-lookup"><span data-stu-id="01dda-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="01dda-111">[Fjern Office legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af styring af legitimationsoplysninger i Windows.</span><span class="sxs-lookup"><span data-stu-id="01dda-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="01dda-112">**Bemærk:** Stier i registreringsdatabasen for Office 2016 er ændret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="01dda-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="01dda-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="01dda-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="01dda-114">Yderligere oplysninger finder du under [forbindelsen problemer i logon efter opdatering til Office 2016 build 16.0.7967 på Windows-10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="01dda-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>