---
title: Problemer med onboardingmaskiner
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141365"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="c91e0-102">Problemer med onboardingmaskiner</span><span class="sxs-lookup"><span data-stu-id="c91e0-102">Issues with onboarding machines</span></span>

<span data-ttu-id="c91e0-103">Du har muligvis problemer med onboardingmaskiner til MDATP-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="c91e0-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="c91e0-104">Hvis du har adgang til slutbrugermaskinen, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="c91e0-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="c91e0-105">Hent [diagnosticeringsværktøjet Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="c91e0-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="c91e0-106">Udtræk og kør MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="c91e0-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="c91e0-107">Find diagnosticeringsloggen i mappen MDATPClientAnalyzerResult, den samme mappe, hvor værktøjet Analysator hentes.</span><span class="sxs-lookup"><span data-stu-id="c91e0-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="c91e0-108">Gennemse logfilen, MDATPClientAnalyzer.txt, for at finde problemer med forbindelses- eller internetproxyindstillinger.</span><span class="sxs-lookup"><span data-stu-id="c91e0-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>