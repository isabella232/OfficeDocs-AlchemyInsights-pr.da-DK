---
title: Fejlfinding af eksisterende skærm
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690705"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="4e546-102">Fejlfinding af en eksisterende skærm</span><span class="sxs-lookup"><span data-stu-id="4e546-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="4e546-103">Prøv disse løsninger for at foretage fejlfinding af en skærm.</span><span class="sxs-lookup"><span data-stu-id="4e546-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="4e546-104">**Opdater skærmvisningen:**</span><span class="sxs-lookup"><span data-stu-id="4e546-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="4e546-105">Tryk på følgende taster på samme tid: Windows-tast + Ctrl + Skift + B. Dette vil opdatere kommunikationen med din grafikdriver.</span><span class="sxs-lookup"><span data-stu-id="4e546-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="4e546-106">Dine skærme blinker kort øjeblik og vender tilbage efter et par sekunder.</span><span class="sxs-lookup"><span data-stu-id="4e546-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="4e546-107">**Fejlfinding på skærmhardware:**</span><span class="sxs-lookup"><span data-stu-id="4e546-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="4e546-108">Fjern kablet fra din PC til skærmen, og sæt den ind igen.</span><span class="sxs-lookup"><span data-stu-id="4e546-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="4e546-109">Fjern eventuelle ikke-vigtige enheder fra din PC (f. eks kort eller docker).</span><span class="sxs-lookup"><span data-stu-id="4e546-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="4e546-110">**Hvis du for nylig har installeret en opdatering på din PC, kan du vende tilbage til din skærmdriver:**</span><span class="sxs-lookup"><span data-stu-id="4e546-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="4e546-111">Vælg **Start**, Skriv **Enhedshåndtering**, og vælg **Enhedshåndtering** fra resultaterne.</span><span class="sxs-lookup"><span data-stu-id="4e546-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="4e546-112">Udvid sektionen **skærmkort** , Højreklik på dit skærmkort, ands Vælg **Egenskaber**.</span><span class="sxs-lookup"><span data-stu-id="4e546-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="4e546-113">Gå til fanen **driver** , og vælg **Annuller tilbage-driver**.</span><span class="sxs-lookup"><span data-stu-id="4e546-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="4e546-114">Bemærk! Hvis den ikke er tilgængelig eller er nedtonet, skal du vælge **Nej** under nedenstående indstillinger for at gå til næste trin.</span><span class="sxs-lookup"><span data-stu-id="4e546-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="4e546-115">Du skal muligvis genstarte din PC, før ændringerne træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="4e546-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="4e546-116">**Fjerne og geninstallere din skærmdriver:**</span><span class="sxs-lookup"><span data-stu-id="4e546-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="4e546-117">Vælg **Start**, Skriv **Enhedshåndtering**, og vælg **Enhedshåndtering** fra resultaterne.</span><span class="sxs-lookup"><span data-stu-id="4e546-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="4e546-118">Udvid sektionen **skærmkort** , Højreklik på dit skærmkort, ands Vælg **Fjern enhed**.</span><span class="sxs-lookup"><span data-stu-id="4e546-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="4e546-119">Markér afkrydsningsfeltet ud for **Slet driversoftwaren til denne enhed** , og vælg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="4e546-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="4e546-120">Bemærk! du bliver muligvis bedt om at genstarte computeren på dette tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="4e546-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="4e546-121">Husk at skrive de resterende instruktioner ned, før du genstarter.</span><span class="sxs-lookup"><span data-stu-id="4e546-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="4e546-122">Åbn Enhedshåndtering igen.</span><span class="sxs-lookup"><span data-stu-id="4e546-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="4e546-123">Udvid sektionen **skærmkort** , Højreklik på dit skærmkort, og vælg **Opdater driver**.</span><span class="sxs-lookup"><span data-stu-id="4e546-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="4e546-124">Vælg **Søg automatisk efter Opdater driversoftware** , og følg installationsvejledningen.</span><span class="sxs-lookup"><span data-stu-id="4e546-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>