---
title: Løsning af Office-apps Beklager, vi har midlertidige serverproblemer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764111"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="bfec8-102">Rettelse af Office-apps "Beklager, vi har midlertidige serverproblemer"</span><span class="sxs-lookup"><span data-stu-id="bfec8-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="bfec8-103">Hvis du modtager denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="bfec8-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bfec8-104">Kontroller dine firewall-, antivirusprogrammer s- og proxyindstillinger for at bekræfte, at de ikke blokerer for internetadgang til Office-apps.</span><span class="sxs-lookup"><span data-stu-id="bfec8-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="bfec8-105">Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bfec8-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="bfec8-106">Gå til **Start** > **kørsel**, og skriv derefter **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="bfec8-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="bfec8-107">Sørg for, at følgende tjenester kører:</span><span class="sxs-lookup"><span data-stu-id="bfec8-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="bfec8-108">Automatisk installation af netværksforbundne enheder</span><span class="sxs-lookup"><span data-stu-id="bfec8-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="bfec8-109">Tjenesten Netværksliste</span><span class="sxs-lookup"><span data-stu-id="bfec8-109">Network List Service</span></span>
    - <span data-ttu-id="bfec8-110">Kendskab til netværksplacering</span><span class="sxs-lookup"><span data-stu-id="bfec8-110">Network Location Awareness</span></span>
    - <span data-ttu-id="bfec8-111">Windows-hændelseslog</span><span class="sxs-lookup"><span data-stu-id="bfec8-111">Windows Event Log</span></span>

<span data-ttu-id="bfec8-112">Hvis en af disse tjenester ikke kører, kan du prøve at starte den.</span><span class="sxs-lookup"><span data-stu-id="bfec8-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="bfec8-113">Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med udvidede tilladelser:</span><span class="sxs-lookup"><span data-stu-id="bfec8-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="bfec8-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="bfec8-114">**sfc /scannow**</span></span>

<span data-ttu-id="bfec8-115">Når kommandoen er færdig, skal du genstarte computeren.</span><span class="sxs-lookup"><span data-stu-id="bfec8-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="bfec8-116">Du kan finde detaljerede oplysninger under ["Vi kan desværre ikke oprette forbindelse til din konto. Prøv igen senere",, når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="bfec8-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>