---
title: Løs Bluetooth-problemer i Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812926"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="74db0-102">Løs Bluetooth-problemer i Windows 10</span><span class="sxs-lookup"><span data-stu-id="74db0-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="74db0-103">Hvis ikonet Bluetooth mangler, eller Bluetooth ikke kan slås til eller fra, kan du køre Bluetooth-fejlfindingsværktøjet.</span><span class="sxs-lookup"><span data-stu-id="74db0-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="74db0-104">[Åbn indstillingerne for fejlfinding](ms-settings:troubleshoot), klik på **Bluetooth** under Find og løs **andre problemer**, og klik på **Kør fejlfindingsværktøjet**.</span><span class="sxs-lookup"><span data-stu-id="74db0-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="74db0-105">Hvis du ikke kan se Bluetooth-ikonet, men Bluetooth vises i Enhedshåndtering:</span><span class="sxs-lookup"><span data-stu-id="74db0-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="74db0-106">Klik på Bluetooth i **Enhedshåndtering.**</span><span class="sxs-lookup"><span data-stu-id="74db0-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="74db0-107">Tryk og hold (eller højreklik) på navnet på Bluetooth-adapteren, og klik på **Fjern enhed**.</span><span class="sxs-lookup"><span data-stu-id="74db0-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="74db0-108">Luk Windows-enheden, vent et par sekunder, og tænd den derefter igen.</span><span class="sxs-lookup"><span data-stu-id="74db0-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="74db0-109">Windows forsøger at geninstallere driveren.</span><span class="sxs-lookup"><span data-stu-id="74db0-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="74db0-110">Hvis du for nylig har installeret Windows 10-opdateringer eller opgraderet til Windows 10, kan det være en ide at søge efter driveropdateringer:</span><span class="sxs-lookup"><span data-stu-id="74db0-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="74db0-111">I Enhedshåndtering skal du klikke **på Bluetooth** og derefter klikke på navnet på Bluetooth-adapteren (som kan indeholde ordet "radio").</span><span class="sxs-lookup"><span data-stu-id="74db0-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="74db0-112">Tryk og hold (eller højreklik) på Bluetooth-adapteren, og klik derefter på **Opdater**  >  **driversøgning automatisk efter opdateret driversoftware**.</span><span class="sxs-lookup"><span data-stu-id="74db0-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="74db0-113">Følg trinnene, og klik derefter på **Luk**.</span><span class="sxs-lookup"><span data-stu-id="74db0-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="74db0-114">Hvis Windows ikke kan finde en ny Bluetooth-driver, skal du gå til pc-producentens websted og downloade den nyeste Bluetooth-driver derfra.</span><span class="sxs-lookup"><span data-stu-id="74db0-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="74db0-115">Når du har downloadet den, skal du klikke på Opdater **driver** Gennemse computeren efter driversoftware Søg efter den placering, hvor driverfilerne er gemt >  >    >   **OK**  >  **Næste,** og følg trinnene for at installere.</span><span class="sxs-lookup"><span data-stu-id="74db0-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="74db0-116">Når du har installeret den opdaterede driver, skal du genstarte computeren og derefter kontrollere, om det løser forbindelsesproblemet.</span><span class="sxs-lookup"><span data-stu-id="74db0-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="74db0-117">Hvis du vil have mere at vide om fejlfinding af Bluetooth-problemer, skal du se hele artiklen [Løs Bluetooth-problemer i Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="74db0-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
