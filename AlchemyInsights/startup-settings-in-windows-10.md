---
title: Startindstillinger i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751129"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="aa81e-102">Startindstillinger i Windows 10</span><span class="sxs-lookup"><span data-stu-id="aa81e-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="aa81e-103">**Ændre, hvilke apps der kører automatisk ved start**</span><span class="sxs-lookup"><span data-stu-id="aa81e-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="aa81e-104">Gå til [indstillinger > Apps > start](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="aa81e-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="aa81e-105">Kontrollér, at alle de apps, du vil køre ved opstart, er slået **til.**</span><span class="sxs-lookup"><span data-stu-id="aa81e-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="aa81e-106">**Tilføj en app til at køre automatisk ved start**</span><span class="sxs-lookup"><span data-stu-id="aa81e-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="aa81e-107">Klik eller tryk på **Start** , og Find den app, du vil køre ved opstart.</span><span class="sxs-lookup"><span data-stu-id="aa81e-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="aa81e-108">Højreklik på appen, klik på **flere**, og klik derefter på **Åbn filplacering**.</span><span class="sxs-lookup"><span data-stu-id="aa81e-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="aa81e-109">Dette åbner den placering, hvor genvejen til appen er gemt.</span><span class="sxs-lookup"><span data-stu-id="aa81e-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="aa81e-110">Hvis der ikke er nogen indstilling for åben filplacering, betyder det, at appen ikke kan køre ved start.</span><span class="sxs-lookup"><span data-stu-id="aa81e-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="aa81e-111">Når filplaceringen er åben, skal du trykke på **Windows-tasten + R**, skrive **Shell: Start**og derefter klikke på **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa81e-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="aa81e-112">Dette åbner mappen Start.</span><span class="sxs-lookup"><span data-stu-id="aa81e-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="aa81e-113">Kopiér og Indsæt genvejen til appen fra filplaceringen til mappen Start.</span><span class="sxs-lookup"><span data-stu-id="aa81e-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="aa81e-114">**Avancerede startindstillinger (herunder fejlsikret tilstand, UEFI-indstillinger og opstart fra en anden enhed)**</span><span class="sxs-lookup"><span data-stu-id="aa81e-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="aa81e-115">Gem dit arbejde, og Luk alle åbne dokumenter, da disse trin vil genstarte din PC.</span><span class="sxs-lookup"><span data-stu-id="aa81e-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="aa81e-116">Gå til [indstillinger > opdater & sikkerhed > genoprettelse](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="aa81e-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="aa81e-117">Under **Avanceret start**skal du klikke på **Genstart nu**.</span><span class="sxs-lookup"><span data-stu-id="aa81e-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="aa81e-118">Når din PC genstarter på skærmbilledet Vælg en indstilling:</span><span class="sxs-lookup"><span data-stu-id="aa81e-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="aa81e-119">Hvis du vil starte fra en enhed som et USB-drev, skal du klikke på **Brug en enhed**.</span><span class="sxs-lookup"><span data-stu-id="aa81e-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="aa81e-120">Hvis du vil angive UEFI-indstillingerne (også kaldet BIOS-konfiguration), skal du klikke på **fejlfinding > avancerede indstillinger > UEFI-firmware indstillinger**.</span><span class="sxs-lookup"><span data-stu-id="aa81e-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="aa81e-121">Hvis du vil angive fejlsikret tilstand eller ændre avancerede startindstillinger, skal du klikke på **fejlfinding > avancerede indstillinger > startindstillinger**og derefter klikke på **Genstart**.</span><span class="sxs-lookup"><span data-stu-id="aa81e-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="aa81e-122">Du bliver muligvis bedt om at angive din [BitLocker-genoprettelsesnøgle](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="aa81e-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="aa81e-123">Når din PC genstartes igen, skal du klikke på den startindstilling, du vil bruge.</span><span class="sxs-lookup"><span data-stu-id="aa81e-123">After your PC restarts again, click the startup setting you want to use.</span></span>