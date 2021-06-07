---
title: Problemer med ydeevnen for Microsoft Defender til slutpunkt på Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793756"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="e4f93-102">Problemer med ydeevnen for Microsoft Defender til slutpunkt på Linux</span><span class="sxs-lookup"><span data-stu-id="e4f93-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="e4f93-103">Denne artikel vejleder dig gennem trinnene til at identificere problemer med ydeevnen for Microsoft Defender til slutpunkt på Linux.</span><span class="sxs-lookup"><span data-stu-id="e4f93-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="e4f93-104">Det er vigtigt først at kontrollere, at det problem, du oplever, er løst med den [nyeste version.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="e4f93-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="e4f93-105">Hvis du vil starte undersøgelsen, skal [du se Fejlfinding af problemer med ydeevnen for Microsoft Defender til Slutpunkt på Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="e4f93-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="e4f93-106">Udeladelse</span><span class="sxs-lookup"><span data-stu-id="e4f93-106">Exclusions</span></span>

<span data-ttu-id="e4f93-107">Udeladelse kan være med til at reducere problemer med ydeevnen.</span><span class="sxs-lookup"><span data-stu-id="e4f93-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="e4f93-108">Gennemse dine undtagelser, før du begynder, så yderligere risici kendes og dokumenteres.</span><span class="sxs-lookup"><span data-stu-id="e4f93-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="e4f93-109">Få mere at vide under [Konfigurer og valider udeladelse af Microsoft Defender til Slutpunkt på Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="e4f93-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="e4f93-110">Når du har flere filer & mapper, der skal udelades, og de alle er på det samme mountpoint, kan det være nemmere at udelukke mountpointen.</span><span class="sxs-lookup"><span data-stu-id="e4f93-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="e4f93-111">Fra og med udgivelsen fra februar 101.22.80 kan du udelade et helt mountpoint.</span><span class="sxs-lookup"><span data-stu-id="e4f93-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="e4f93-112">Hvis /mnt/backup f.eks. er et mountpoint, kan du tilføje /mnt/backup til listen exclude ved at køre denne kommando:</span><span class="sxs-lookup"><span data-stu-id="e4f93-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="e4f93-113">**Bemærk!** Hvis du tilføjer udeladelse, øges risikoen for, at malware ikke registreres, og de skal håndteres og implementeres med omhu.</span><span class="sxs-lookup"><span data-stu-id="e4f93-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="e4f93-114">Har du brug for hjælp?</span><span class="sxs-lookup"><span data-stu-id="e4f93-114">Need Help?</span></span>

<span data-ttu-id="e4f93-115">For at hjælpe dig på den mest effektive måde skal du indsamle de diagnostiske data, før du åbner en supportsag.</span><span class="sxs-lookup"><span data-stu-id="e4f93-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
