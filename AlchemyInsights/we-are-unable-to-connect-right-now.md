---
title: Aktiveringsproblem - Vi kan ikke oprette forbindelse lige nu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581869"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="731a3-102">Rettelse af Microsoft 365-apps "Vi kan ikke oprette forbindelse lige nu"</span><span class="sxs-lookup"><span data-stu-id="731a3-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="731a3-103">Hvis du modtager denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="731a3-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="731a3-104">Kontroller din firewall, dit antivirusprogram og dine proxyindstillinger for at bekræfte, at de ikke blokerer for internetadgang til Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="731a3-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="731a3-105">Se [Microsoft URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="731a3-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="731a3-106">Gå til **Start**  >  **kørsel**, og skriv derefter **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="731a3-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="731a3-107">Sørg for, at følgende tjenester alle kører:</span><span class="sxs-lookup"><span data-stu-id="731a3-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="731a3-108">Automatisk installation af netværksforbundne enheder</span><span class="sxs-lookup"><span data-stu-id="731a3-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="731a3-109">Tjenesten Netværksliste</span><span class="sxs-lookup"><span data-stu-id="731a3-109">Network List Service</span></span>
    - <span data-ttu-id="731a3-110">Kendskab til netværksplacering</span><span class="sxs-lookup"><span data-stu-id="731a3-110">Network Location Awareness</span></span>
    - <span data-ttu-id="731a3-111">Windows-hændelseslog</span><span class="sxs-lookup"><span data-stu-id="731a3-111">Windows Event Log</span></span>

<span data-ttu-id="731a3-112">Hvis en af disse tjenester ikke kører, kan du prøve at starte den.</span><span class="sxs-lookup"><span data-stu-id="731a3-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="731a3-113">Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med udvidede tilladelser:</span><span class="sxs-lookup"><span data-stu-id="731a3-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="731a3-114">**sfc /scannow delte et**</span><span class="sxs-lookup"><span data-stu-id="731a3-114">**sfc /scannow**</span></span>

<span data-ttu-id="731a3-115">Genstart computeren, når denne kommando er færdig.</span><span class="sxs-lookup"><span data-stu-id="731a3-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="731a3-116">Du kan finde detaljerede oplysninger under ["Vi kan desværre ikke oprette forbindelse til din konto. Prøv igen senere", når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="731a3-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>