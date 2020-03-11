---
title: Brug mulighed for oplåsning af fingeraftryk i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588310"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="dcfd1-102">Brug mulighed for oplåsning af fingeraftryk i Windows 10</span><span class="sxs-lookup"><span data-stu-id="dcfd1-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="dcfd1-103">**Aktiver Windows Hello-fingeraftryk**</span><span class="sxs-lookup"><span data-stu-id="dcfd1-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="dcfd1-104">Hvis du vil låse Windows 10 op ved hjælp af dit fingeraftryk, skal du konfigurere Windows Hello Fingerprint ved at tilføje (lade Windows lære at genkende) mindst én finger.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="dcfd1-105">Gå til **Indstillinger > konti > logonindstillinger** (eller klik [her](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="dcfd1-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="dcfd1-106">Tilgængelige logonindstillinger vises.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="dcfd1-107">Det kan f.eks. være:</span><span class="sxs-lookup"><span data-stu-id="dcfd1-107">For example:</span></span>

    ![Indstillinger for logon.](media/sign-in-options.png)

2. <span data-ttu-id="dcfd1-109">Klik eller tryk på **Windows Hello Fingerprint**, og klik derefter på **Konfigurer**.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="dcfd1-110">Klik på Kom i **gang**i vinduet Windows Hello-konfiguration .</span><span class="sxs-lookup"><span data-stu-id="dcfd1-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="dcfd1-111">Fingeraftrykssensoren aktiveres, og du bliver bedt om at placere fingeren på sensoren:</span><span class="sxs-lookup"><span data-stu-id="dcfd1-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Fingeraftrykssensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="dcfd1-113">Følg vejledningen, som vil bede dig om gentagne gange at scanne din finger.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="dcfd1-114">Når dette er færdigt, har du mulighed for at tilføje andre fingre, som du måske vil bruge til logon.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="dcfd1-115">Næste gang du logger på Windows 10, har du mulighed for at bruge dit fingeraftryk til at gøre det.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="dcfd1-116">**Windows Hello Fingerprint er ikke tilgængelig som logonindstilling**</span><span class="sxs-lookup"><span data-stu-id="dcfd1-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="dcfd1-117">Hvis Windows Hello Fingerprint ikke vises som en indstilling i **logonindstillinger**, betyder det, at Windows ikke har kendskab til nogen fingeraftrykslæser/scanner, der er tilsluttet pc'en, eller at en systempolitik forhindrer brugen (hvis din pc f.eks. administreres af din arbejdsplads).</span><span class="sxs-lookup"><span data-stu-id="dcfd1-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="dcfd1-118">Sådan foretages fejlfinding:</span><span class="sxs-lookup"><span data-stu-id="dcfd1-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="dcfd1-119">Vælg knappen **Start** på proceslinjen, og søg efter **Enhedshåndtering**.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="dcfd1-120">Klik eller tryk for at åbne **Enhedshåndtering**.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="dcfd1-121">I Enhedshåndtering skal du udvide biometriske enheder ved at klikke på dens vinkel.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriske enheder.](media/biometric-devices.png)

4. <span data-ttu-id="dcfd1-123">Din fingeraftryksscanner skal være opført som en biometrisk enhed, f.eks.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriske enheder.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="dcfd1-125">Hvis fingeraftryksscanneren ikke vises, og scanneren er integreret i pc'en, skal du gå til pc-producentens websted.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="dcfd1-126">I afsnittet teknisk support til pc-modellen skal du søge efter en Windows 10-driver til en scanner, du kan installere.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="dcfd1-127">Hvis scanneren er adskilt fra pc'en (vedhæftet via USB), skal du gå til scannerproducentens websted for at finde og installere Windows 10-enhedsdriversoftware til den scannermodel, du har.</span><span class="sxs-lookup"><span data-stu-id="dcfd1-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
