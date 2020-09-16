---
title: Aktiverings problem-vi kan ikke oprette forbindelse lige nu
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725977"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="8b5f2-102">Retter Microsoft 365-apps "vi kan ikke oprette forbindelse lige nu"</span><span class="sxs-lookup"><span data-stu-id="8b5f2-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="8b5f2-103">Hvis du får vist denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="8b5f2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="8b5f2-104">Kontrollér din firewall, antivirussoftware og proxyindstillinger for at bekræfte, at de ikke blokerer Internet adgang til Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="8b5f2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="8b5f2-105">Se [Microsoft URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="8b5f2-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="8b5f2-106">Gå til **Start**  >  **Run**, og Skriv **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="8b5f2-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="8b5f2-107">Sørg for, at følgende tjenester alle kører:</span><span class="sxs-lookup"><span data-stu-id="8b5f2-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="8b5f2-108">Automatisk konfiguration af netværksforbundne enheder</span><span class="sxs-lookup"><span data-stu-id="8b5f2-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="8b5f2-109">Netværksliste tjeneste</span><span class="sxs-lookup"><span data-stu-id="8b5f2-109">Network List Service</span></span>
    - <span data-ttu-id="8b5f2-110">Netværks placerings bevidsthed</span><span class="sxs-lookup"><span data-stu-id="8b5f2-110">Network Location Awareness</span></span>
    - <span data-ttu-id="8b5f2-111">Logbog i Windows</span><span class="sxs-lookup"><span data-stu-id="8b5f2-111">Windows Event Log</span></span>

<span data-ttu-id="8b5f2-112">Hvis en af disse tjenester ikke kører, skal du prøve at starte det.</span><span class="sxs-lookup"><span data-stu-id="8b5f2-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="8b5f2-113">Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:</span><span class="sxs-lookup"><span data-stu-id="8b5f2-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="8b5f2-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="8b5f2-114">**sfc /scannow**</span></span>

<span data-ttu-id="8b5f2-115">Genstart computeren, når denne kommando er færdig.</span><span class="sxs-lookup"><span data-stu-id="8b5f2-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="8b5f2-116">Hvis du vil have mere at vide, skal du se ["beklager, vi kan ikke oprette forbindelse til din konto. Prøv igen senere "-fejl, når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="8b5f2-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>