---
title: Symboler fungerer ikke ved hjælp af Microsoft Edge-browseren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676132"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="ea36b-102">Symboler fungerer ikke ved hjælp af Microsoft Edge-browseren</span><span class="sxs-lookup"><span data-stu-id="ea36b-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="ea36b-103">Når du har oprettet en indikator, bliver den ikke imødekommet af Edge (SmartScreen).</span><span class="sxs-lookup"><span data-stu-id="ea36b-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="ea36b-104">Få mere at vide under [Opret indikatorer for IP'er og URL-adresser/domæner.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="ea36b-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="ea36b-105">Trin 1: Sørg for følgende</span><span class="sxs-lookup"><span data-stu-id="ea36b-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="ea36b-106">Kontrollér, at indikatoren er korrekt (ingen slåfejl i IP/URL, korrekt handling, de korrekte RBAC-grupper).</span><span class="sxs-lookup"><span data-stu-id="ea36b-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="ea36b-107">Vent mindst 2 timer efter oprettelse af indikatoren for at tage højde for enhver mulig ventetid.</span><span class="sxs-lookup"><span data-stu-id="ea36b-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="ea36b-108">Kontrollér, at systemet/systemerne er onboardet til Microsoft Defender til slutpunkt.</span><span class="sxs-lookup"><span data-stu-id="ea36b-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="ea36b-109">Kontrollér, at systemer kan kommunikere med skyen.</span><span class="sxs-lookup"><span data-stu-id="ea36b-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="ea36b-110">Kontrollér, at Smartscreen er aktiveret og tilgængelig ved at gå til [testwebstedet.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="ea36b-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="ea36b-111">Trin 2: Fejlfinding af det potentielle problem</span><span class="sxs-lookup"><span data-stu-id="ea36b-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="ea36b-112">Kontrollér, at klienten opfylder kravene.</span><span class="sxs-lookup"><span data-stu-id="ea36b-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="ea36b-113">Du kan få mere at [vide under Oprette indikatorer for IP'er og URL-adresser/domæner.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="ea36b-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="ea36b-114">Sørg for, at du kører den nyeste version af Edge-browseren.</span><span class="sxs-lookup"><span data-stu-id="ea36b-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="ea36b-115">Hvis du vil finde ud af den nyeste version, [skal du se Find ud af, hvilken version Microsoft Edge du har.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="ea36b-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="ea36b-116">Genstart Edge-browseren.</span><span class="sxs-lookup"><span data-stu-id="ea36b-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="ea36b-117">Gå til det websted, hvor du har konfigureret en indikator.</span><span class="sxs-lookup"><span data-stu-id="ea36b-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="ea36b-118">Hvis webstedet ikke vises som forventet, skal du fortsætte til trin 3.</span><span class="sxs-lookup"><span data-stu-id="ea36b-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="ea36b-119">Trin 3: Indsaml data</span><span class="sxs-lookup"><span data-stu-id="ea36b-119">Step 3: Collect data</span></span>

- <span data-ttu-id="ea36b-120">**Indsaml diagnostiske MDEClientAnalyzer-data.**</span><span class="sxs-lookup"><span data-stu-id="ea36b-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="ea36b-121">Du kan finde en vejledning [under Problemer med onboardingmaskine til Microsoft Defender til slutpunkt.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="ea36b-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="ea36b-122">Hvis du er tryg ved at installere og indsamle en Fiddler-sporing, skal du [se Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="ea36b-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="ea36b-123">Hvis du foretrækker vejledning fra Microsoft Support, kan du vælge ikonet Support nedenfor for at åbne en supportsag.</span><span class="sxs-lookup"><span data-stu-id="ea36b-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
