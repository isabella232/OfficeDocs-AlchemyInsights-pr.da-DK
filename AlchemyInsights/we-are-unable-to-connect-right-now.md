---
title: Aktiverings problem-vi kan ikke oprette forbindelse lige nu
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628236"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="11654-102">Rettelse af Office-Apps "vi kan ikke oprette forbindelse lige nu"-meddelelse</span><span class="sxs-lookup"><span data-stu-id="11654-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="11654-103">Hvis du modtager denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="11654-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="11654-104">Kontrollér din firewall, dit antivirusprogram og dine proxyindstillinger for at bekræfte, at de ikke blokerer for Internet adgang til Office-Apps.</span><span class="sxs-lookup"><span data-stu-id="11654-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="11654-105">Se [Office 365 URL-adresser og IP-adresse intervaller](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="11654-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="11654-106">Gå til **Start** > **Kør**, og skriv derefter **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="11654-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="11654-107">Sørg for, at følgende tjenester alle kører:</span><span class="sxs-lookup"><span data-stu-id="11654-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="11654-108">Automatisk konfiguration af netværkstilsluttede enheder</span><span class="sxs-lookup"><span data-stu-id="11654-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="11654-109">Tjenesten netværksliste</span><span class="sxs-lookup"><span data-stu-id="11654-109">Network List Service</span></span>
    - <span data-ttu-id="11654-110">Kendskab til netværksplacering</span><span class="sxs-lookup"><span data-stu-id="11654-110">Network Location Awareness</span></span>
    - <span data-ttu-id="11654-111">Windows hændelseslog</span><span class="sxs-lookup"><span data-stu-id="11654-111">Windows Event Log</span></span>

<span data-ttu-id="11654-112">Hvis en af disse tjenester ikke kører, kan du prøve at starte den.</span><span class="sxs-lookup"><span data-stu-id="11654-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="11654-113">Hvis du har problemer med at starte tjenesten, skal du køre følgende kommando ved at åbne en kommandoprompt med administratorrettigheder:</span><span class="sxs-lookup"><span data-stu-id="11654-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="11654-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="11654-114">**sfc /scannow**</span></span>

<span data-ttu-id="11654-115">Når denne kommando er færdig, skal du genstarte computeren.</span><span class="sxs-lookup"><span data-stu-id="11654-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="11654-116">Yderligere oplysninger finder du under ["beklager, vi kan ikke oprette forbindelse til din konto. Prøv igen senere ", når du aktiverer Office fra Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="11654-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>