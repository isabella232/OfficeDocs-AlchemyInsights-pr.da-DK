---
title: Fejlfinding af lydproblemer i Windows 10
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
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796043"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="72082-102">Fejlfinding af lydproblemer i Windows 10</span><span class="sxs-lookup"><span data-stu-id="72082-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="72082-103">**Kør fejlfindingsværktøjet lyd**</span><span class="sxs-lookup"><span data-stu-id="72082-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="72082-104">Lydfejlfinding kan muligvis løse lydproblemerne automatisk:</span><span class="sxs-lookup"><span data-stu-id="72082-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="72082-105">Vælg **Start**, Skriv **fejlfinding**, og vælg derefter **fejlfinding** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="72082-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="72082-106">Vælg **afspilning af lyd** > **Kør fejlfindingsværktøjet**.</span><span class="sxs-lookup"><span data-stu-id="72082-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="72082-107">**Kontrollér kabler, lydstyrke, højttalere og hovedtelefoner**</span><span class="sxs-lookup"><span data-stu-id="72082-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="72082-108">Kontrollér dine højttaler-og hovedtelefon tilslutninger for løse kabler, og sørg for, at de er sluttet til det rigtige stik.</span><span class="sxs-lookup"><span data-stu-id="72082-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="72082-109">Kontrollér dine strøm-og lydstyrkeniveauer, og prøv at slå alle lydstyrkekontrollerne op.</span><span class="sxs-lookup"><span data-stu-id="72082-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="72082-110">Nogle højttalere og apps har deres egne lydstyrke Kontroller, og du skal muligvis kontrollere dem alle for at sikre, at de er på de rigtige niveauer.</span><span class="sxs-lookup"><span data-stu-id="72082-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="72082-111">Prøv at oprette forbindelse ved hjælp af en anden USB-port.</span><span class="sxs-lookup"><span data-stu-id="72082-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="72082-112">**Bemærk:** Husk, at dine højttalere muligvis ikke fungerer, når hovedtelefonerne er tilsluttet.</span><span class="sxs-lookup"><span data-stu-id="72082-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="72082-113">**Kontroller Enhedshåndtering**</span><span class="sxs-lookup"><span data-stu-id="72082-113">**Check Device Manager**</span></span>

<span data-ttu-id="72082-114">Sådan sikrer du dig, at driverne er opdateret:</span><span class="sxs-lookup"><span data-stu-id="72082-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="72082-115">Vælg **Start**, Skriv **Enhedshåndtering**, og vælg derefter **Enhedshåndtering** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="72082-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="72082-116">Vælg lydkortet under **enheder til lyd, video og spil**, Åbn det, Vælg fanen **driver** , og vælg **Opdater driver**.</span><span class="sxs-lookup"><span data-stu-id="72082-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="72082-117">**Bemærk:** Hvis Windows ikke finder en ny driver, skal du søge efter en på enhedsproducentens websted og følge instruktionerne.</span><span class="sxs-lookup"><span data-stu-id="72082-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="72082-118">**Geninstallere driveren**</span><span class="sxs-lookup"><span data-stu-id="72082-118">**Reinstall the driver**</span></span>

<span data-ttu-id="72082-119">Hvis du ikke kan opdatere via Enhedshåndtering eller finde en ny driver på producentens websted, skal du prøve disse trin:</span><span class="sxs-lookup"><span data-stu-id="72082-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="72082-120">Højreklik (eller tryk og hold) på lyddriveren i Enhedshåndtering, og vælg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="72082-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="72082-121">Genstart enheden, og Windows vil forsøge at geninstallere driveren.</span><span class="sxs-lookup"><span data-stu-id="72082-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="72082-122">Hvis geninstallation af driveren ikke virker, kan du prøve at bruge den generiske lyddriver, der følger med Windows.</span><span class="sxs-lookup"><span data-stu-id="72082-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="72082-123">I Enhedshåndtering skal du højreklikke (eller trykke og holde) på din lyddriver **> opdatere driver software** > **Gennemse min computer for driver software** > **Lad mig vælge fra en liste over enhedsdrivere på min computer**, Vælg **High Definition Audio Device**, Vælg **næste**, og følg instruktionerne for at installere den.</span><span class="sxs-lookup"><span data-stu-id="72082-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="72082-124">**Angive standardenheden**</span><span class="sxs-lookup"><span data-stu-id="72082-124">**Set the default device**</span></span>

<span data-ttu-id="72082-125">Hvis du opretter forbindelse til en lydenhed ved hjælp af USB eller HDMI, skal du muligvis indstille enheden som standard:</span><span class="sxs-lookup"><span data-stu-id="72082-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="72082-126">Vælg **Start**, Skriv **lyd**, og vælg derefter **lyd** eller **Skift systemlyde** på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="72082-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="72082-127">Vælg en enhed under fanen **afspilning** , Vælg **Angiv standard**, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="72082-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

