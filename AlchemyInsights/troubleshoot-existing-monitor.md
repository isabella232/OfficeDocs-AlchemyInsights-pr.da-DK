---
title: Fejlfinding af eksisterende skærm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738563"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="301a6-102">Fejlfinding af en eksisterende skærm</span><span class="sxs-lookup"><span data-stu-id="301a6-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="301a6-103">Prøv disse løsninger for at foretage fejlfinding af en skærm.</span><span class="sxs-lookup"><span data-stu-id="301a6-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="301a6-104">**Opdater skærmens skærm:**</span><span class="sxs-lookup"><span data-stu-id="301a6-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="301a6-105">Tryk på følgende taster på samme tid: Windows-tasten + Ctrl + Shift + B. Dette vil opdatere kommunikationen med din grafikdriver.</span><span class="sxs-lookup"><span data-stu-id="301a6-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="301a6-106">Dine skærme vil blinke momentant og komme tilbage efter et par sekunder.</span><span class="sxs-lookup"><span data-stu-id="301a6-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="301a6-107">**Fejlfinding af skærmhardware:**</span><span class="sxs-lookup"><span data-stu-id="301a6-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="301a6-108">Fjern kablet, der forbinder pc'en med skærmen, og sæt den i igen.</span><span class="sxs-lookup"><span data-stu-id="301a6-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="301a6-109">Afbryd alle ikke-væsentlige enheder fra din PC (f. eks. adaptere eller dokker).</span><span class="sxs-lookup"><span data-stu-id="301a6-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="301a6-110">**Hvis du for nylig har installeret en opdatering på din PC, kan du rulle din skærmdriver tilbage:**</span><span class="sxs-lookup"><span data-stu-id="301a6-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="301a6-111">Vælg **Start**, Skriv **Enhedshåndtering**, og vælg **Enhedshåndtering** i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="301a6-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="301a6-112">Udvid sektionen **skærmkort** , Højreklik på skærmkortet, og vælg **Egenskaber**.</span><span class="sxs-lookup"><span data-stu-id="301a6-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="301a6-113">Naviger til fanen **driver** og vælg **roll back driver**.</span><span class="sxs-lookup"><span data-stu-id="301a6-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="301a6-114">Bemærk: Hvis dette ikke er tilgængeligt eller er nedtonet, skal du vælge **Nej** fra indstillingerne nedenfor for at gå til næste trin.</span><span class="sxs-lookup"><span data-stu-id="301a6-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="301a6-115">Det kan være nødvendigt at genstarte pc'en, før ændringerne træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="301a6-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="301a6-116">**Afinstaller og geninstaller din skærmdriver:**</span><span class="sxs-lookup"><span data-stu-id="301a6-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="301a6-117">Vælg **Start**, Skriv **Enhedshåndtering**, og vælg **Enhedshåndtering** i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="301a6-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="301a6-118">Udvid sektionen **skærmkort** , Højreklik på skærmkortet, og vælg **Fjern enhed**.</span><span class="sxs-lookup"><span data-stu-id="301a6-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="301a6-119">Markér afkrydsningsfeltet ud for **Slet driversoftwaren til denne enhed** , og vælg **Afinstaller**.</span><span class="sxs-lookup"><span data-stu-id="301a6-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="301a6-120">Bemærk: du kan blive bedt om at genstarte computeren på dette tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="301a6-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="301a6-121">Sørg for at skrive de resterende instruktioner ned, før du genstarter.</span><span class="sxs-lookup"><span data-stu-id="301a6-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="301a6-122">Åbn Enhedshåndtering igen.</span><span class="sxs-lookup"><span data-stu-id="301a6-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="301a6-123">Udvid sektionen **skærmkort** , Højreklik på skærmkortet, og vælg **Opdater driver**.</span><span class="sxs-lookup"><span data-stu-id="301a6-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="301a6-124">Vælg **Søg automatisk efter opdaterings driver software** , og følg installationsvejledningen.</span><span class="sxs-lookup"><span data-stu-id="301a6-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>