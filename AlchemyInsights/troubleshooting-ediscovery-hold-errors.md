---
title: Fejlfinding af ediscovery indeholder fejl
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676084"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="0e5b4-102">Fejlfinding af ediscovery indeholder fejl</span><span class="sxs-lookup"><span data-stu-id="0e5b4-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="0e5b4-103">Oplever du problemer med eDiscovery-ventende emner?</span><span class="sxs-lookup"><span data-stu-id="0e5b4-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="0e5b4-104">Her er nogle af de bedste fremgangsmåder at overveje:</span><span class="sxs-lookup"><span data-stu-id="0e5b4-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="0e5b4-105">Kontrollér status for ventepositionsfordelingen.</span><span class="sxs-lookup"><span data-stu-id="0e5b4-105">Check the hold distribution status.</span></span>  <span data-ttu-id="0e5b4-106">Hvis status er **Til (Afventer)** eller **Fra (Afventer),** skal du vente på, at ventepositionsfordelingen fuldføres.</span><span class="sxs-lookup"><span data-stu-id="0e5b4-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="0e5b4-107">Flet opdateringer af eDiscovery-venteposition til en enkelt anmodning om flere poster i stedet for at opdatere politikken gentagne gange for hver transaktion.</span><span class="sxs-lookup"><span data-stu-id="0e5b4-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="0e5b4-108">Kør Set-CaseHoldPolicy <policyname> -RetryDistribution i Security and Compliance Center Powershell.</span><span class="sxs-lookup"><span data-stu-id="0e5b4-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="0e5b4-109">Du kan finde flere [oplysninger Forbind Security & Compliance Center PowerShell.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0e5b4-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="0e5b4-110">Du kan finde trin til at kontrollere disse indstillinger og yderligere bedste fremgangsmåder for at mindske og løse problemer med ventepositioner i eDiscovery under Fejlfinding af [eDiscovery-ventepositionsfejl.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="0e5b4-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="0e5b4-111">Du kan finde oplysninger om fejlfinding af andre almindelige eDiscovery-problemer under Undersøge, foretage [fejlfinding og løse almindelige eDiscovery-problemer.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="0e5b4-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
