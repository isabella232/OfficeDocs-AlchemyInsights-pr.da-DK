---
title: Fejlfinding af lydproblemer i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750301"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="522cd-102">Fejlfinding af lydproblemer i Windows 10</span><span class="sxs-lookup"><span data-stu-id="522cd-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="522cd-103">**Kør fejlfindingsværktøjet lyd**</span><span class="sxs-lookup"><span data-stu-id="522cd-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="522cd-104">Åbne [fejlfindingsindstillingerne](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="522cd-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="522cd-105">Vælg **afspilning af lyd**  >  **Kør fejlfindingen**.</span><span class="sxs-lookup"><span data-stu-id="522cd-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="522cd-106">**Angive standardenheden**</span><span class="sxs-lookup"><span data-stu-id="522cd-106">**Set the default device**</span></span>

<span data-ttu-id="522cd-107">Hvis du opretter forbindelse til en lydenhed med USB eller HDMI, skal du muligvis angive den pågældende enhed som standard:</span><span class="sxs-lookup"><span data-stu-id="522cd-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="522cd-108">Åbn **Start**  >  **lyd**, og vælg derefter **lyd** eller **Skift systemlyde** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="522cd-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="522cd-109">På fanen **afspilning** skal du vælge en enhed, vælge **Angiv standard**og derefter vælge **OK**.</span><span class="sxs-lookup"><span data-stu-id="522cd-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="522cd-110">**Kontrollér kabler, lydstyrke, højttalere og hovedtelefoner**</span><span class="sxs-lookup"><span data-stu-id="522cd-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="522cd-111">Kontrollér din højttaler og dine hovedtelefon forbindelser for løse kabler, og sørg for, at de er tilsluttet til det rigtige stik.</span><span class="sxs-lookup"><span data-stu-id="522cd-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="522cd-112">Kontrollér dine strøm-og lydstyrkeniveauer, og prøv at tænde for alle lydstyrkeindstillingerne.</span><span class="sxs-lookup"><span data-stu-id="522cd-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="522cd-113">Nogle højttalere og apps har deres egen lydstyrkekontrol. Du skal muligvis kontrollere dem alle for at sikre, at de er på de rigtige niveauer.</span><span class="sxs-lookup"><span data-stu-id="522cd-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="522cd-114">Prøv at oprette forbindelse ved hjælp af en anden USB-port.</span><span class="sxs-lookup"><span data-stu-id="522cd-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="522cd-115">**Bemærk**: Husk, at dine højttalere muligvis ikke fungerer, når hovedtelefoner er tilsluttet.</span><span class="sxs-lookup"><span data-stu-id="522cd-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="522cd-116">**Kontrollér Enhedshåndtering**</span><span class="sxs-lookup"><span data-stu-id="522cd-116">**Check Device Manager**</span></span>

<span data-ttu-id="522cd-117">Sådan sikres det, at driverne er opdaterede:</span><span class="sxs-lookup"><span data-stu-id="522cd-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="522cd-118">Vælg **Start**, Skriv **Enhedshåndtering**, og vælg derefter **Enhedshåndtering** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="522cd-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="522cd-119">Under **enheder til lydoptagelse, video og spil**skal du vælge dit lydkort, åbne det, vælge fanen **driver** og vælge **Opdater driver**.</span><span class="sxs-lookup"><span data-stu-id="522cd-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="522cd-120">**Bemærk**! hvis Windows ikke finder en ny driver, kan du søge efter en på enhedsproducentens websted og følge vejledningen.</span><span class="sxs-lookup"><span data-stu-id="522cd-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="522cd-121">**Geninstaller driveren**</span><span class="sxs-lookup"><span data-stu-id="522cd-121">**Reinstall the driver**</span></span>

<span data-ttu-id="522cd-122">Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, kan du prøve disse trin:</span><span class="sxs-lookup"><span data-stu-id="522cd-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="522cd-123">I Enhedshåndtering skal du højreklikke (eller trykke og holde) på lyddriveren og vælge **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="522cd-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="522cd-124">Genstart din enhed, og Windows vil forsøge at geninstallere driveren.</span><span class="sxs-lookup"><span data-stu-id="522cd-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="522cd-125">Hvis geninstallation af driveren ikke virker, kan du prøve at bruge den generiske lyddriver, der følger med Windows.</span><span class="sxs-lookup"><span data-stu-id="522cd-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="522cd-126">I Enhedshåndtering skal du højreklikke (eller trykke og holde) på lyddriveren > **Opdater driversoftware**  >  **Gennemse min computer for driversoftware**  >  **Lad mig vælge fra en liste over enhedsdrivere på min computer**, Vælg **næste**, og følg vejledningen for at installere den. **High Definition Audio Device**</span><span class="sxs-lookup"><span data-stu-id="522cd-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
