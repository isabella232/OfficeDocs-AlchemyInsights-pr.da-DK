---
title: Fejlfinding af lydproblemer i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833285"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="af93e-102">Fejlfinding af lydproblemer i Windows 10</span><span class="sxs-lookup"><span data-stu-id="af93e-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="af93e-103">**Kør lydfejlfinding**</span><span class="sxs-lookup"><span data-stu-id="af93e-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="af93e-104">Åbn indstillingerne [for fejlfinding.](ms-settings:troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="af93e-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="af93e-105">Vælg **Afspilning af lyd** Kør  >  **fejlfindingsværktøjet**.</span><span class="sxs-lookup"><span data-stu-id="af93e-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="af93e-106">**Angiv standardenheden**</span><span class="sxs-lookup"><span data-stu-id="af93e-106">**Set the default device**</span></span>

<span data-ttu-id="af93e-107">Hvis du opretter forbindelse til en lydenhed ved hjælp af USB eller HDMI, skal du muligvis angive den pågældende enhed som standardenhed:</span><span class="sxs-lookup"><span data-stu-id="af93e-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="af93e-108">Åbn **Start**  >  **lyd**, og vælg derefter **Lyd** eller **Skift systemlyde** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="af93e-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="af93e-109">På fanen **Afspilning** skal du vælge en enhed, **vælge Angiv standard** og derefter vælge **OK**.</span><span class="sxs-lookup"><span data-stu-id="af93e-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="af93e-110">**Tjek kabler, lydstyrke, højttalere og hovedtelefoner**</span><span class="sxs-lookup"><span data-stu-id="af93e-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="af93e-111">Kontrollér dine højttaler- og hovedtelefonforbindelser for løse kabler, og sørg for, at de er forbundet til det rigtige stik.</span><span class="sxs-lookup"><span data-stu-id="af93e-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="af93e-112">Kontrollér strøm og lydstyrkeniveauer, og prøv at skrue op for alle lydstyrkeknapper.</span><span class="sxs-lookup"><span data-stu-id="af93e-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="af93e-113">Nogle højttalere og apps har deres egne lydstyrkeknapper. skal du muligvis kontrollere dem alle for at sikre dig, at de er på de rigtige niveauer.</span><span class="sxs-lookup"><span data-stu-id="af93e-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="af93e-114">Prøv at tilslutte ved hjælp af en anden USB-port.</span><span class="sxs-lookup"><span data-stu-id="af93e-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="af93e-115">**Bemærk:** Husk, at dine højttalere muligvis ikke fungerer, når hovedtelefonerne er tilsluttet.</span><span class="sxs-lookup"><span data-stu-id="af93e-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="af93e-116">**Kontrollér Enhedshåndtering**</span><span class="sxs-lookup"><span data-stu-id="af93e-116">**Check Device Manager**</span></span>

<span data-ttu-id="af93e-117">Sådan sikrer du, at driverne er opdaterede:</span><span class="sxs-lookup"><span data-stu-id="af93e-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="af93e-118">Vælg **Start**, skriv **Enhedshåndtering**, og vælg **derefter Enhedshåndtering** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="af93e-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="af93e-119">Under **Lyd, video og spilcontrollere** skal du vælge dit lydkort, åbne det, vælge fanen **Driver** og vælge **Opdater driver**.</span><span class="sxs-lookup"><span data-stu-id="af93e-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="af93e-120">**Bemærk!** Hvis Windows ikke finder en ny driver, skal du søge efter en på webstedet for enhedsproducenten og følge instruktionerne.</span><span class="sxs-lookup"><span data-stu-id="af93e-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="af93e-121">**Geninstaller driveren**</span><span class="sxs-lookup"><span data-stu-id="af93e-121">**Reinstall the driver**</span></span>

<span data-ttu-id="af93e-122">Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, kan du prøve disse trin:</span><span class="sxs-lookup"><span data-stu-id="af93e-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="af93e-123">I Enhedshåndtering skal du højreklikke (eller trykke og holde nede) på lyddriveren og vælge **Fjern.**</span><span class="sxs-lookup"><span data-stu-id="af93e-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="af93e-124">Genstart enheden, så forsøger Windows at geninstallere driveren.</span><span class="sxs-lookup"><span data-stu-id="af93e-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="af93e-125">Hvis det ikke virker at geninstallere driveren, kan du prøve at bruge den generiske lyddriver, der leveres med Windows.</span><span class="sxs-lookup"><span data-stu-id="af93e-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="af93e-126">I Enhedshåndtering skal du højreklikke (eller trykke og holde) på din lyddriver > Opdater **driversoftware** Gennemse computeren efter driversoftware Lad mig vælge på en liste over enhedsdrivere på computeren , vælg Lydenhed med HD , vælg Næste , og følg vejledningen for at installere  >    >  den.  </span><span class="sxs-lookup"><span data-stu-id="af93e-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
