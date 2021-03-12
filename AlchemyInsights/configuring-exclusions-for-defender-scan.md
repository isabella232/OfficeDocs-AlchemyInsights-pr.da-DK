---
title: Konfiguration af udeladelse for Microsoft Defender ATP-scanning
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713401"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="0da60-102">Konfiguration af udeladelse for Microsoft Defender ATP-scanning</span><span class="sxs-lookup"><span data-stu-id="0da60-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="0da60-103">Generelt kan du udelade bestemte filtypenavne og mappeplaceringer fra Microsoft Defender ATP-scanninger.</span><span class="sxs-lookup"><span data-stu-id="0da60-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="0da60-104">Du kan også konfigurere udeladelse for filer, der åbnes af visse processer.</span><span class="sxs-lookup"><span data-stu-id="0da60-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="0da60-105">Du kan få mere at vide under [Konfigurere](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) og validere udeladelser baseret på filtypenavn og mappeplacering og konfigurere udeladelse for filer, [der er åbnet af processer.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="0da60-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="0da60-106">Hvis du vil konfigurere udeladelser for **Windows Server 2016 og 2019,** skal du se [Konfigurere Udeladelse af Microsoft Defender Antivirus på Windows Server.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="0da60-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="0da60-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="0da60-107">**Mac**</span></span>

<span data-ttu-id="0da60-108">Hvis du vil have mere at vide om understøttede [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) udeladelsestyper og konfiguration af en liste over udeladelser til Mac, skal du se Understøttede udeladelsestyper, og hvordan du konfigurerer listen [over udeladelser.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="0da60-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="0da60-109">**Bemærk!** Du kan også validere udeladelseslister ved hjælp af EICAR-testfilen.</span><span class="sxs-lookup"><span data-stu-id="0da60-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="0da60-110">Du kan få mere at vide [under Valider udeladelseslister med EICAR-testfilen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="0da60-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="0da60-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="0da60-111">**Linux**</span></span>

<span data-ttu-id="0da60-112">Hvis du vil have mere at vide om understøttede [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) udeladelsestyper og konfigurere en liste over udeladelser til Linux, skal du se Understøttede udeladelsestyper og konfigurere og validere udeladelser [for Microsoft Defender ATP til Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="0da60-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="0da60-113">**Bemærk!** Du kan også validere udeladelseslister ved hjælp af EICAR-testfilen.</span><span class="sxs-lookup"><span data-stu-id="0da60-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="0da60-114">Du kan få mere at vide [under Valider udeladelseslister med EICAR-testfilen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="0da60-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 