---
title: Fejlfinding i forbindelse med lydproblemer i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265010"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="af9e6-102">Fejlfinding i forbindelse med lydproblemer i Windows 10</span><span class="sxs-lookup"><span data-stu-id="af9e6-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="af9e6-103">**Kør fejlfindingsværktøjet til lyd**</span><span class="sxs-lookup"><span data-stu-id="af9e6-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="af9e6-104">Åbn [indstillingerne for fejlfinding](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="af9e6-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="af9e6-105">Vælg **Afafspilning af lyd** > **Kør fejlfindingsværktøjet**.</span><span class="sxs-lookup"><span data-stu-id="af9e6-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="af9e6-106">**Angive standardenheden**</span><span class="sxs-lookup"><span data-stu-id="af9e6-106">**Set the default device**</span></span>

<span data-ttu-id="af9e6-107">Hvis du opretter forbindelse til en lydenhed ved hjælp af USB eller HDMI, skal du muligvis indstille enheden som standard:</span><span class="sxs-lookup"><span data-stu-id="af9e6-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="af9e6-108">Åbn **Start** > **lyd**, og vælg derefter **Lyd-** eller **Skift systemlyde** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="af9e6-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="af9e6-109">Vælg en enhed under fanen **Afspilning,** vælg **Angiv standard**, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="af9e6-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="af9e6-110">**Kontrollere kabler, lydstyrke, højttalere og hovedtelefoner**</span><span class="sxs-lookup"><span data-stu-id="af9e6-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="af9e6-111">Kontroller højttaler- og hovedtelefontilslutninger for løse kabler, og sørg for, at de er tilsluttet det korrekte stik.</span><span class="sxs-lookup"><span data-stu-id="af9e6-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="af9e6-112">Kontroller strøm- og lydstyrkeniveauet, og prøv at skrue op for alle lydstyrkekontrolelementerne.</span><span class="sxs-lookup"><span data-stu-id="af9e6-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="af9e6-113">Nogle højttalere og apps har deres egne lydstyrkekontroller. du måske nødt til at tjekke dem alle for at sikre, at de er på de rigtige niveauer.</span><span class="sxs-lookup"><span data-stu-id="af9e6-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="af9e6-114">Prøv at oprette forbindelse ved hjælp af en anden USB-port.</span><span class="sxs-lookup"><span data-stu-id="af9e6-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="af9e6-115">**Bemærk:** Husk, at højttalerne muligvis ikke fungerer, når hovedtelefonerne er tilsluttet.</span><span class="sxs-lookup"><span data-stu-id="af9e6-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="af9e6-116">**Tjek Enhedshåndtering**</span><span class="sxs-lookup"><span data-stu-id="af9e6-116">**Check Device Manager**</span></span>

<span data-ttu-id="af9e6-117">Sådan sikrer du dig, at chaufførerne er opdaterede:</span><span class="sxs-lookup"><span data-stu-id="af9e6-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="af9e6-118">Vælg **Start**, skriv **Enhedshåndtering**, og vælg derefter **Enhedshåndtering** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="af9e6-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="af9e6-119">Vælg lydkortet under **Lyd-, video- og spilcontrollere,** åbn det, vælg fanen **Driver,** og vælg **Opdater driver**.</span><span class="sxs-lookup"><span data-stu-id="af9e6-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="af9e6-120">**Bemærk:** Hvis Windows ikke finder en ny driver, skal du kigge efter en på enhedsproducentens websted og følge deres instruktioner.</span><span class="sxs-lookup"><span data-stu-id="af9e6-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="af9e6-121">**Geninstallere driveren**</span><span class="sxs-lookup"><span data-stu-id="af9e6-121">**Reinstall the driver**</span></span>

<span data-ttu-id="af9e6-122">Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, kan du prøve disse trin:</span><span class="sxs-lookup"><span data-stu-id="af9e6-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="af9e6-123">Højreklik (eller tryk og hold) lyddriveren i Enhedshåndtering, og vælg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="af9e6-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="af9e6-124">Genstart enheden, og Windows forsøger at geninstallere driveren.</span><span class="sxs-lookup"><span data-stu-id="af9e6-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="af9e6-125">Hvis geninstallation af driveren ikke virker, kan du prøve at bruge den generiske lyddriver, der følger med Windows.</span><span class="sxs-lookup"><span data-stu-id="af9e6-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="af9e6-126">Højreklik (eller tryk og hold) din lyddriver > **Opdater driversoftware** > **Gennemse min computer for driversoftware** > **Lad mig vælge fra en liste over enhedsdrivere på computeren,** vælge **High Definition Audio Device**, vælge **Næste**og følge vejledningen for at installere den.</span><span class="sxs-lookup"><span data-stu-id="af9e6-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
