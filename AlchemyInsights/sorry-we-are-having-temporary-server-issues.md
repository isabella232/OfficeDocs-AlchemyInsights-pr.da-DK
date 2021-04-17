---
title: Vi beklager, men vi har midlertidige serverproblemer i forbindelse med Microsoft 365-apps
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835265"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="62ae2-102">Vi rettelse af meddelelsen "Vi beklager, men vi har midlertidige serverproblemer" i Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="62ae2-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="62ae2-103">Hvis du modtager denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="62ae2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="62ae2-104">Kontrollér din firewall, din antivirussoftware og dine proxyindstillinger for at bekræfte, at de ikke blokerer internetadgang til Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="62ae2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="62ae2-105">Se [URL-adresser og IP-adresseintervaller](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="62ae2-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="62ae2-106">Gå til **Start**  >  **Kør**, og skriv **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="62ae2-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="62ae2-107">Sørg for, at følgende tjenester kører alle:</span><span class="sxs-lookup"><span data-stu-id="62ae2-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="62ae2-108">Automatisk konfiguration af netværksforbundne enheder</span><span class="sxs-lookup"><span data-stu-id="62ae2-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="62ae2-109">Netværklistetjeneste</span><span class="sxs-lookup"><span data-stu-id="62ae2-109">Network List Service</span></span>
    - <span data-ttu-id="62ae2-110">Kendskab til netværksplacering</span><span class="sxs-lookup"><span data-stu-id="62ae2-110">Network Location Awareness</span></span>
    - <span data-ttu-id="62ae2-111">Windows-hændelseslog</span><span class="sxs-lookup"><span data-stu-id="62ae2-111">Windows Event Log</span></span>

<span data-ttu-id="62ae2-112">Hvis en af disse tjenester ikke kører, kan du prøve at starte den.</span><span class="sxs-lookup"><span data-stu-id="62ae2-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="62ae2-113">Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:</span><span class="sxs-lookup"><span data-stu-id="62ae2-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="62ae2-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="62ae2-114">**sfc /scannow**</span></span>

<span data-ttu-id="62ae2-115">Når denne kommando er fuldført, skal du genstarte computeren.</span><span class="sxs-lookup"><span data-stu-id="62ae2-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="62ae2-116">Du kan finde flere oplysninger [i "Vi beklager, men vi kan ikke oprette forbindelse til din konto. Prøv igen senere"-fejlen, når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="62ae2-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>