---
title: Konfiguration af udeladelse af Microsoft Defender ATP scanning
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543679"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="b494a-102">Konfiguration af udeladelse af Microsoft Defender ATP scanning</span><span class="sxs-lookup"><span data-stu-id="b494a-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="b494a-103">Generelt kan du udelade bestemte filtypenavne og mappeplaceringer fra Microsoft Defender ATP scanninger.</span><span class="sxs-lookup"><span data-stu-id="b494a-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="b494a-104">Du kan også konfigurere udeladelse af filer, der åbnes af visse processer.</span><span class="sxs-lookup"><span data-stu-id="b494a-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="b494a-105">Du kan finde flere oplysninger i [Konfigurere](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) og validere udeladelse baseret på filtypenavn og mappeplacering og Konfigurere udeladelse [for filer, der er åbnet af processer.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="b494a-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="b494a-106">Hvis du vil konfigurere udeladelse **af Windows Server 2016 og 2019,** skal du se Konfigurere [Microsoft Defender Antivirus udeladelse Windows Server.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="b494a-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="b494a-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="b494a-107">**Mac**</span></span>

<span data-ttu-id="b494a-108">Hvis du vil have mere at vide om understøttede [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) udeladelsestyper og konfiguration af en liste over udeladelsestyper til Mac, skal du se Understøttede udeladelsestyper og Sådan [konfigureres listen over udeladelsestyper.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="b494a-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="b494a-109">**Bemærk!** Du kan også validere udeladelseslister ved hjælp af EICAR-testfilen.</span><span class="sxs-lookup"><span data-stu-id="b494a-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="b494a-110">Du kan finde flere oplysninger [under Valider udeladelseslister med EICAR-testfilen](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="b494a-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="b494a-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="b494a-111">**Linux**</span></span>

<span data-ttu-id="b494a-112">Hvis du vil have mere at vide om understøttede [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) udeladelsestyper og konfiguration af en liste over udeladelsestyper til Linux, skal du se Understøttede udeladelsestyper og Konfigurere og validere [udeladelsestyper for Microsoft Defender ATP til Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="b494a-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="b494a-113">**Bemærk!** Du kan også validere udeladelseslister ved hjælp af EICAR-testfilen.</span><span class="sxs-lookup"><span data-stu-id="b494a-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="b494a-114">Du kan finde flere oplysninger [under Valider udeladelseslister med EICAR-testfilen](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="b494a-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 