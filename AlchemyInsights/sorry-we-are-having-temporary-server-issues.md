---
title: Rettelse af Microsoft 365-apps Beklager, vi har midlertidig meddelelse om serverproblemer
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582697"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="8e309-102">Rettelse af Microsoft 365-apps "Beklager, vi har midlertidige serverproblemer"</span><span class="sxs-lookup"><span data-stu-id="8e309-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="8e309-103">Hvis du modtager denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="8e309-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="8e309-104">Kontroller din firewall, dit antivirusprogram og dine proxyindstillinger for at bekræfte, at de ikke blokerer for internetadgang til Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="8e309-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="8e309-105">Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="8e309-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="8e309-106">Gå til **Start**  >  **kørsel**, og skriv derefter **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="8e309-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="8e309-107">Sørg for, at følgende tjenester alle kører:</span><span class="sxs-lookup"><span data-stu-id="8e309-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="8e309-108">Automatisk installation af netværksforbundne enheder</span><span class="sxs-lookup"><span data-stu-id="8e309-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="8e309-109">Tjenesten Netværksliste</span><span class="sxs-lookup"><span data-stu-id="8e309-109">Network List Service</span></span>
    - <span data-ttu-id="8e309-110">Kendskab til netværksplacering</span><span class="sxs-lookup"><span data-stu-id="8e309-110">Network Location Awareness</span></span>
    - <span data-ttu-id="8e309-111">Windows-hændelseslog</span><span class="sxs-lookup"><span data-stu-id="8e309-111">Windows Event Log</span></span>

<span data-ttu-id="8e309-112">Hvis en af disse tjenester ikke kører, kan du prøve at starte den.</span><span class="sxs-lookup"><span data-stu-id="8e309-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="8e309-113">Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med udvidede tilladelser:</span><span class="sxs-lookup"><span data-stu-id="8e309-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="8e309-114">**sfc /scannow delte et**</span><span class="sxs-lookup"><span data-stu-id="8e309-114">**sfc /scannow**</span></span>

<span data-ttu-id="8e309-115">Genstart computeren, når denne kommando er færdig.</span><span class="sxs-lookup"><span data-stu-id="8e309-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="8e309-116">Du kan finde detaljerede oplysninger under ["Vi kan desværre ikke oprette forbindelse til din konto. Prøv igen senere", når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="8e309-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>