---
title: Problemer med at logge på Microsoft 365-apps
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833025"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="6ebd5-102">Tom logonskærm i Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="6ebd5-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="6ebd5-103">Du kan løse dette problem ved at prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="6ebd5-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="6ebd5-104">Installér de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="6ebd5-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="6ebd5-105">Nulstil indstillinger i Internet Explorer: Gå til Værktøjer Internetindstillinger Avanceret Nulstil  >    >    >  **indstillinger i Internet Explorer** (bemærk, at du mister brugerdefinerede indstillinger), og prøv derefter at logge på Office igen.</span><span class="sxs-lookup"><span data-stu-id="6ebd5-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="6ebd5-106">Deaktiver Windows Defender Application Guard (WDAG) eller en lignende firewall eller et antivirusprogram:</span><span class="sxs-lookup"><span data-stu-id="6ebd5-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="6ebd5-107">I Kontrolpanel skal du gå **til Programmer** og derefter vælge **Slå Windows-funktioner til eller fra**.</span><span class="sxs-lookup"><span data-stu-id="6ebd5-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="6ebd5-108">Hvis Windows Defender Application Guard er aktiveret, kan du prøve at deaktivere den.</span><span class="sxs-lookup"><span data-stu-id="6ebd5-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="6ebd5-109">**Bemærk!** Du skal muligvis genstarte computeren.</span><span class="sxs-lookup"><span data-stu-id="6ebd5-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="6ebd5-110">Sørg for, at plug-in'en Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokeres af nogen applikation eller firewall/antivirusprogram.</span><span class="sxs-lookup"><span data-stu-id="6ebd5-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="6ebd5-111">[Ryd Office-legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) hjælp af Windows Legitimationsstyring.</span><span class="sxs-lookup"><span data-stu-id="6ebd5-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6ebd5-112">**Bemærk!** Stierne i registreringsdatabasen til Office 2016 er ændret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="6ebd5-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6ebd5-113">(Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6ebd5-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="6ebd5-114">Du kan få mere at vide under Forbindelsesproblemer ved logon efter opdatering til [Office 2016 build 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="6ebd5-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>