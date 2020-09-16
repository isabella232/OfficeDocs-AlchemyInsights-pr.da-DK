---
title: Problemer med Onboarding-maskiner
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
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676876"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="da989-102">Problemer med Onboarding-maskiner</span><span class="sxs-lookup"><span data-stu-id="da989-102">Issues with onboarding machines</span></span>

<span data-ttu-id="da989-103">Der kan være problemer med Onboarding af computere til MDATP-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="da989-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="da989-104">Hvis du har adgang til slutbrugerens maskine, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="da989-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="da989-105">Hent diagnosticeringsværktøjet til [klient forbindelses analyse](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="da989-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="da989-106">Udpak og Kør MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="da989-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="da989-107">Find diagnosticeringslogfilen i den mappe, der hedder MDATPClientAnalyzerResult, den samme mappe, hvor Analyseværktøjet er hentet.</span><span class="sxs-lookup"><span data-stu-id="da989-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="da989-108">Gennemse logfilen, MDATPClientAnalyzer.txt, for at finde problemer med forbindelse eller Internet proxyindstillinger.</span><span class="sxs-lookup"><span data-stu-id="da989-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>