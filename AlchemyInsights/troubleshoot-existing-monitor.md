---
title: Fejlfinding af eksisterende skærm
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824573"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="ff60a-102">Fejlfinding af en eksisterende skærm</span><span class="sxs-lookup"><span data-stu-id="ff60a-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="ff60a-103">Prøv disse løsninger for at foretage fejlfinding af en skærm.</span><span class="sxs-lookup"><span data-stu-id="ff60a-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="ff60a-104">**Opdater skærmens skærm:**</span><span class="sxs-lookup"><span data-stu-id="ff60a-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="ff60a-105">Tryk på følgende taster på samme tid: Windows-tast+Ctrl+Skift+B. Dette opdaterer kommunikationen med grafikdriveren.</span><span class="sxs-lookup"><span data-stu-id="ff60a-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="ff60a-106">Dine skærme blinker kortvarigt og vender tilbage efter et par sekunder.</span><span class="sxs-lookup"><span data-stu-id="ff60a-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="ff60a-107">**Fejlfinding af skærmhardware:**</span><span class="sxs-lookup"><span data-stu-id="ff60a-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="ff60a-108">Træk kablet ud, som forbinder pc'en med din skærm, og sæt det i igen.</span><span class="sxs-lookup"><span data-stu-id="ff60a-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="ff60a-109">Afbryd forbindelsen til alle ikke-vigtige enheder fra din pc (f.eks. adaptere eller docks).</span><span class="sxs-lookup"><span data-stu-id="ff60a-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="ff60a-110">**Hvis du for nylig har installeret en opdatering på din pc, kan du tilbagerulle skærmdriveren:**</span><span class="sxs-lookup"><span data-stu-id="ff60a-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="ff60a-111">Vælg **Start**, skriv **enhedshåndtering**, og **vælg Enhedshåndtering** fra resultaterne.</span><span class="sxs-lookup"><span data-stu-id="ff60a-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="ff60a-112">Udvid **sektionen Skærmkort,** højreklik på dit skærmkort, og vælg **Egenskaber**.</span><span class="sxs-lookup"><span data-stu-id="ff60a-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="ff60a-113">Gå til fanen **Driver,** og vælg **Flyt driver tilbage.**</span><span class="sxs-lookup"><span data-stu-id="ff60a-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="ff60a-114">Bemærk! Hvis dette ikke er tilgængeligt eller er nedtonet, skal du **vælge** Nej i indstillingerne nedenfor for at gå til næste trin.</span><span class="sxs-lookup"><span data-stu-id="ff60a-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="ff60a-115">Du skal muligvis genstarte computeren, før disse ændringer træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="ff60a-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="ff60a-116">**Fjern og geninstaller skærmdriveren:**</span><span class="sxs-lookup"><span data-stu-id="ff60a-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="ff60a-117">Vælg **Start**, skriv **enhedshåndtering**, og **vælg Enhedshåndtering** fra resultaterne.</span><span class="sxs-lookup"><span data-stu-id="ff60a-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="ff60a-118">Udvid **sektionen Skærmkort,** højreklik på dit skærmkort, og vælg **Fjern enhed**.</span><span class="sxs-lookup"><span data-stu-id="ff60a-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="ff60a-119">Markér afkrydsningsfeltet ud for **Slet driversoftwaren til denne enhed, og** vælg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="ff60a-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="ff60a-120">Bemærk! Du bliver muligvis bedt om at genstarte computeren på dette tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="ff60a-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="ff60a-121">Sørg for at skrive de resterende instruktioner ned, før du genstarter.</span><span class="sxs-lookup"><span data-stu-id="ff60a-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="ff60a-122">Åbn Enhedshåndtering igen.</span><span class="sxs-lookup"><span data-stu-id="ff60a-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="ff60a-123">Udvid **sektionen Skærmkort,** højreklik på dit skærmkort, og vælg **Opdater driver.**</span><span class="sxs-lookup"><span data-stu-id="ff60a-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="ff60a-124">Vælg **Søg automatisk efter opdateringsdriversoftware,** og følg installationsvejledningen.</span><span class="sxs-lookup"><span data-stu-id="ff60a-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>