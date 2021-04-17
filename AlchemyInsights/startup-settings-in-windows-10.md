---
title: Startindstillinger i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828146"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="e5a09-102">Startindstillinger i Windows 10</span><span class="sxs-lookup"><span data-stu-id="e5a09-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="e5a09-103">**Ændre, hvilke apps der køres automatisk ved start**</span><span class="sxs-lookup"><span data-stu-id="e5a09-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="e5a09-104">Gå til [Indstillinger > Apps > Start.](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="e5a09-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="e5a09-105">Kontrollér, at alle apps, du vil køre ved start, er slået **Til.**</span><span class="sxs-lookup"><span data-stu-id="e5a09-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="e5a09-106">**Tilføj en app, der skal køre automatisk ved start**</span><span class="sxs-lookup"><span data-stu-id="e5a09-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="e5a09-107">Klik eller tryk **på Start,** og find den app, du vil køre ved start.</span><span class="sxs-lookup"><span data-stu-id="e5a09-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="e5a09-108">Højreklik på appen, klik på **Mere**, og klik derefter på **Åbn filplacering**.</span><span class="sxs-lookup"><span data-stu-id="e5a09-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="e5a09-109">Dette åbner den placering, hvor genvejen til appen er gemt.</span><span class="sxs-lookup"><span data-stu-id="e5a09-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="e5a09-110">Hvis der ikke er nogen indstilling for Åbn filplacering, betyder det, at appen ikke kan køre ved start.</span><span class="sxs-lookup"><span data-stu-id="e5a09-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="e5a09-111">Åbn filplaceringen, tryk på **Windows-tasten + R**, skriv **shell:startup**, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="e5a09-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="e5a09-112">Derved åbnes mappen Start.</span><span class="sxs-lookup"><span data-stu-id="e5a09-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="e5a09-113">Kopiér og indsæt genvejen til appen fra filplaceringen til mappen Start.</span><span class="sxs-lookup"><span data-stu-id="e5a09-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="e5a09-114">**Avancerede startindstillinger (herunder Fejlsikret tilstand, UEFI-indstillinger og start fra en anden enhed)**</span><span class="sxs-lookup"><span data-stu-id="e5a09-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="e5a09-115">Gem dit arbejde, og luk alle åbne dokumenter, da disse trin genstarter din pc.</span><span class="sxs-lookup"><span data-stu-id="e5a09-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="e5a09-116">Gå til [Indstillinger > opdatering & > genoprettelse.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="e5a09-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="e5a09-117">Klik **på Genstart** nu under **Avanceret start.**</span><span class="sxs-lookup"><span data-stu-id="e5a09-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="e5a09-118">Når pc'en genstarter, skal du gå til skærmbilledet Vælg en indstilling:</span><span class="sxs-lookup"><span data-stu-id="e5a09-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="e5a09-119">Hvis du vil starte fra en enhed som f.eks. et USB-drev, skal **du klikke på Brug en enhed**.</span><span class="sxs-lookup"><span data-stu-id="e5a09-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="e5a09-120">Hvis du vil angive UEFI-indstillingerne (nogle gange kaldetFUNKTIONER), skal du klikke på **Fejlfinding > avancerede indstillinger > UEFI-firmwareindstillinger.**</span><span class="sxs-lookup"><span data-stu-id="e5a09-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="e5a09-121">Hvis du vil skifte fejlsikret tilstand eller ændre de avancerede startindstillinger, skal du klikke **på Fejlfinding >** avancerede > Indstillinger for start og derefter klikke på **Genstart.**</span><span class="sxs-lookup"><span data-stu-id="e5a09-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="e5a09-122">Du bliver muligvis bedt om at angive [bitLocker-genoprettelsesnøglen](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="e5a09-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="e5a09-123">Når pc'en genstarter igen, skal du klikke på den startindstilling, du vil bruge.</span><span class="sxs-lookup"><span data-stu-id="e5a09-123">After your PC restarts again, click the startup setting you want to use.</span></span>