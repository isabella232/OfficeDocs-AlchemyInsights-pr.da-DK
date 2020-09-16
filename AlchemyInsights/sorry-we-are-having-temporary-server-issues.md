---
title: Rettelse af Microsoft 365-apps vi beklager, men vi har midlertidige serverproblemer-meddelelse
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758239"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="fbf23-102">Hvis du retter Microsoft 365-apps, kan vi desværre ikke få besked om midlertidige serverproblemer</span><span class="sxs-lookup"><span data-stu-id="fbf23-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="fbf23-103">Hvis du får vist denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="fbf23-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fbf23-104">Kontrollér din firewall, antivirussoftware og proxyindstillinger for at bekræfte, at de ikke blokerer Internet adgang til Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="fbf23-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="fbf23-105">Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="fbf23-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="fbf23-106">Gå til **Start**  >  **Run**, og Skriv **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="fbf23-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="fbf23-107">Sørg for, at følgende tjenester alle kører:</span><span class="sxs-lookup"><span data-stu-id="fbf23-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="fbf23-108">Automatisk konfiguration af netværksforbundne enheder</span><span class="sxs-lookup"><span data-stu-id="fbf23-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="fbf23-109">Netværksliste tjeneste</span><span class="sxs-lookup"><span data-stu-id="fbf23-109">Network List Service</span></span>
    - <span data-ttu-id="fbf23-110">Netværks placerings bevidsthed</span><span class="sxs-lookup"><span data-stu-id="fbf23-110">Network Location Awareness</span></span>
    - <span data-ttu-id="fbf23-111">Logbog i Windows</span><span class="sxs-lookup"><span data-stu-id="fbf23-111">Windows Event Log</span></span>

<span data-ttu-id="fbf23-112">Hvis en af disse tjenester ikke kører, skal du prøve at starte det.</span><span class="sxs-lookup"><span data-stu-id="fbf23-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="fbf23-113">Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:</span><span class="sxs-lookup"><span data-stu-id="fbf23-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="fbf23-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="fbf23-114">**sfc /scannow**</span></span>

<span data-ttu-id="fbf23-115">Genstart computeren, når denne kommando er færdig.</span><span class="sxs-lookup"><span data-stu-id="fbf23-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="fbf23-116">Hvis du vil have mere at vide, skal du se ["beklager, vi kan ikke oprette forbindelse til din konto. Prøv igen senere "-fejl, når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="fbf23-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>