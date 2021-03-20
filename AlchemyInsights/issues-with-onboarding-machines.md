---
title: Problemer med onboarding-maskiner til Microsoft Defender til slutpunkter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901561"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="868ce-102">Problemer med onboarding-maskiner til Microsoft Defender til slutpunkter</span><span class="sxs-lookup"><span data-stu-id="868ce-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="868ce-103">Der kan være problemer med onboarding-maskiner til MDE-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="868ce-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="868ce-104">Hvis du kan få adgang til slutbrugerens maskine, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="868ce-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="868ce-105">Hent den nyeste prøveversion af diagnosticeringsværktøjet [MDE Client Analyzer.](https://aka.ms/betamdeanalyzer)</span><span class="sxs-lookup"><span data-stu-id="868ce-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="868ce-106">Højreklik på **MDEClientAnalyzer.cmd,** og vælg "Kør som administrator".</span><span class="sxs-lookup"><span data-stu-id="868ce-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="868ce-107">Følg eventuelle retningslinjer, der foreslås **iMDEClientAnalyzer.htm.**</span><span class="sxs-lookup"><span data-stu-id="868ce-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="868ce-108">Du kan finde flere detaljerede logfiler i den oprettede undermappe **MDEClientAnalyzerResult.**</span><span class="sxs-lookup"><span data-stu-id="868ce-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="868ce-109">Hvis yderligere vejledning er nødvendig, skal du [kontakte support til Microsoft Defender for Endpoint](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) og angive den MDEClientAnalyzerResult.zip fil til analyse.</span><span class="sxs-lookup"><span data-stu-id="868ce-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
