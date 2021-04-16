---
title: Brug indstillingen til fingeraftrykslåsning i Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796671"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="cd2b8-102">Brug indstillingen til fingeraftrykslåsning i Windows 10</span><span class="sxs-lookup"><span data-stu-id="cd2b8-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="cd2b8-103">**Aktivér Windows Hello-fingeraftryk**</span><span class="sxs-lookup"><span data-stu-id="cd2b8-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="cd2b8-104">Hvis du vil låse Windows 10 op ved hjælp af dit fingeraftryk, skal du konfigurere Windows Hello-fingeraftryk ved at tilføje (så Windows lærer at genkende) mindst én finger.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="cd2b8-105">Gå til **Indstillinger > konti > Logonindstillinger** (eller klik [her).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="cd2b8-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="cd2b8-106">De tilgængelige indstillinger for logon vises.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="cd2b8-107">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="cd2b8-107">For example:</span></span>

    ![Logonindstillinger.](media/sign-in-options.png)

2. <span data-ttu-id="cd2b8-109">Klik eller tryk på **Windows Hello-fingeraftryk,** og klik **derefter på Konfigurer**.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="cd2b8-110">Klik på Introduktion i vinduet til konfiguration **af** Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="cd2b8-111">Fingeraftrykssensoren aktiveres, og du vil blive bedt om at placere din finger på sensoren:</span><span class="sxs-lookup"><span data-stu-id="cd2b8-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Fingeraftrykssensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="cd2b8-113">Følg vejledningen, som beder dig om at scanne din finger gentagne gange.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="cd2b8-114">Når dette er afsluttet, har du mulighed for at tilføje andre fingre, som du kan bruge til at logge på med.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="cd2b8-115">Næste gang du logger på Windows 10, har du mulighed for at bruge dit fingeraftryk til at gøre det.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="cd2b8-116">**Windows Hello-fingeraftryk er ikke tilgængeligt som logonindstilling**</span><span class="sxs-lookup"><span data-stu-id="cd2b8-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="cd2b8-117">Hvis Windows **Hello-fingeraftryk** ikke vises som en indstilling i Logonindstillinger, betyder det, at Windows ikke er opmærksom på nogen fingeraftrykslæser/scanner, der er tilsluttet din pc, eller at en systempolitik forhindrer brugen af den (hvis f.eks. din pc administreres af arbejdspladsen).</span><span class="sxs-lookup"><span data-stu-id="cd2b8-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="cd2b8-118">Sådan foretager du fejlfinding:</span><span class="sxs-lookup"><span data-stu-id="cd2b8-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="cd2b8-119">Vælg knappen **Start** på proceslinjen, og søg efter **Enhedshåndtering**.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="cd2b8-120">Klik eller tryk for at **åbne Enhedshåndtering**.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="cd2b8-121">I Enhedshåndtering skal du udvide biometriske enheder ved at klikke på dens vinkel.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriske enheder.](media/biometric-devices.png)

4. <span data-ttu-id="cd2b8-123">Din fingeraftryksscanner skal angives som en biometrisk enhed, f.eks. Synaptics WBDI-scanneren:</span><span class="sxs-lookup"><span data-stu-id="cd2b8-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriske enheder.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="cd2b8-125">Hvis din fingeraftryksscanner ikke vises, og scanneren er integreret i din pc, skal du gå til pc-producentens websted.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="cd2b8-126">I afsnittet teknisk support til din pc-model skal du søge efter en Windows 10-driver til en scanner, du kan installere.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="cd2b8-127">Hvis scanneren er adskilt fra pc'en (tilsluttet via USB), skal du gå til scannerproducentens websted for at finde og installere Windows 10-enhedsdriversoftware til den scannermodel, du har.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
