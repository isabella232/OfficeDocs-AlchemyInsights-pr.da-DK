---
title: Ret Bluetooth-problemer i Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730153"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="55b77-102">Ret Bluetooth-problemer i Windows 10</span><span class="sxs-lookup"><span data-stu-id="55b77-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="55b77-103">Hvis Bluetooth-ikonet mangler, eller Bluetooth ikke kan slås til eller fra, kan det være en god ide at køre Bluetooth-fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="55b77-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="55b77-104">[Åbn fejlfindingsindstillinger](ms-settings:troubleshoot), klik på **Bluetooth** under **Søg og løs andre problemer**, og klik på **Kør fejlfindingsværktøjet**.</span><span class="sxs-lookup"><span data-stu-id="55b77-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="55b77-105">Hvis du ikke kan se Bluetooth-ikonet, men Bluetooth vises i Enhedshåndtering:</span><span class="sxs-lookup"><span data-stu-id="55b77-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="55b77-106">Klik på **Bluetooth**i Enhedshåndtering.</span><span class="sxs-lookup"><span data-stu-id="55b77-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="55b77-107">Tryk på og hold (eller højreklik) på Bluetooth-kortets navn, og klik på **Fjern enhed**.</span><span class="sxs-lookup"><span data-stu-id="55b77-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="55b77-108">Luk din Windows-enhed, vent et øjeblik, og tænd for det igen.</span><span class="sxs-lookup"><span data-stu-id="55b77-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="55b77-109">Windows vil forsøge at geninstallere driveren.</span><span class="sxs-lookup"><span data-stu-id="55b77-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="55b77-110">Hvis du for nylig har installeret Windows 10-opdateringer eller opgraderet til Windows 10, kan du kontrollere, om der er driveropdateringer:</span><span class="sxs-lookup"><span data-stu-id="55b77-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="55b77-111">I Enhedshåndtering skal du klikke på **Bluetooth**og derefter klikke på navnet på Bluetooth-kortet (som muligvis indeholder ordet "radio").</span><span class="sxs-lookup"><span data-stu-id="55b77-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="55b77-112">Tryk på og hold (eller højreklik) på Bluetooth-adapteren, og klik derefter på **Opdater driver**  >  **søgning automatisk for at få opdateret driversoftware**.</span><span class="sxs-lookup"><span data-stu-id="55b77-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="55b77-113">Følg trinnene, og klik derefter på **Luk**.</span><span class="sxs-lookup"><span data-stu-id="55b77-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="55b77-114">Hvis Windows ikke kan finde en ny Bluetooth-driver, skal du gå til PC-producentens websted og hente den nyeste Bluetooth-driver derfra.</span><span class="sxs-lookup"><span data-stu-id="55b77-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="55b77-115">Når du har hentet det, skal du klikke på **Opdater driver**  >  **Gennemse min computer for driversoftware**  >  **Find** den placering, hvor driverfilerne er gemt > **OK**  >  **næste**, og følg trinnene for at installere.</span><span class="sxs-lookup"><span data-stu-id="55b77-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="55b77-116">Når du har installeret den opdaterede driver, skal du genstarte computeren og derefter kontrollere, om det løser forbindelsesproblemet.</span><span class="sxs-lookup"><span data-stu-id="55b77-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="55b77-117">Du kan finde flere oplysninger om, hvordan du foretager fejlfinding af Bluetooth-problemer, i hele artiklen, [rette Bluetooth-problemer i Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="55b77-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
