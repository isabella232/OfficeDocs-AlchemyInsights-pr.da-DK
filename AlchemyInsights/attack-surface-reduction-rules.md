---
title: Regler for reduktion af angrebsoverfladen
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676126"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="edb84-102">Regler for reduktion af angrebsoverfladen</span><span class="sxs-lookup"><span data-stu-id="edb84-102">Attack surface reduction rules</span></span>

<span data-ttu-id="edb84-103">Udelukkelse af filer eller mapper kan reducere beskyttelsen, der leveres af regler for reduktion af angrebsoverfladen, alvorligt.</span><span class="sxs-lookup"><span data-stu-id="edb84-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="edb84-104">Filer, der ville være blevet blokeret af en regel, har tilladelse til at køre, og ingen rapport eller hændelse registreres.</span><span class="sxs-lookup"><span data-stu-id="edb84-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="edb84-105">En udeladelse gælder for alle regler, der tillader udeladelse.</span><span class="sxs-lookup"><span data-stu-id="edb84-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="edb84-106">I ASR-udeladelse bruges den samme syntaks som Microsoft Defender Antivirus udeladelser.</span><span class="sxs-lookup"><span data-stu-id="edb84-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="edb84-107">Du kan få mere at [vide under Konfigurere og validere udeladelse for Microsoft Defender Antivirus scanninger.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="edb84-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="edb84-108">Du kan undgå problemer ved at [gennemse Almindelige fejl, der skal undgås, når du definerer udeladelse.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="edb84-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="edb84-109">Ikke alle asr-regler understøtter udeladelse.</span><span class="sxs-lookup"><span data-stu-id="edb84-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="edb84-110">Hvis du vil validere, om din regel understøtter udeladelse, skal du se tabellen [Regler for reduktion af angrebsoverfladen.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="edb84-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="edb84-111">Regler for reduktion af angrebsoverfladen</span><span class="sxs-lookup"><span data-stu-id="edb84-111">Attack surface reduction rules</span></span>

<span data-ttu-id="edb84-112">Din organisations angrebsoverflade indeholder alle de steder, hvor en hacker kan kompromittere organisationens enheder eller netværk.</span><span class="sxs-lookup"><span data-stu-id="edb84-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="edb84-113">At reducere angrebsoverfladen betyder, at du beskytter organisationens enheder og netværket, hvilket efterlader hackere med færre måder at udføre angreb på.</span><span class="sxs-lookup"><span data-stu-id="edb84-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="edb84-114">Konfiguration af regler for reduktion af angrebsoverfladen i Microsoft Defender til slutpunkt kan hjælpe.</span><span class="sxs-lookup"><span data-stu-id="edb84-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="edb84-115">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="edb84-115">For more information, see:</span></span>

- [<span data-ttu-id="edb84-116">Knyt ASR-regel-GUID til navn</span><span class="sxs-lookup"><span data-stu-id="edb84-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="edb84-117">Krav til ASR-regler:</span><span class="sxs-lookup"><span data-stu-id="edb84-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="edb84-118">Windows 10 Pro, version 1709 eller nyere</span><span class="sxs-lookup"><span data-stu-id="edb84-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="edb84-119">Windows 10 Enterprise, version 1709 eller nyere</span><span class="sxs-lookup"><span data-stu-id="edb84-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="edb84-120">Windows Server, version 1803 (halvårlige kanal) eller nyere</span><span class="sxs-lookup"><span data-stu-id="edb84-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="edb84-121">Identificer den korrekte udeladelse, der skal anvendes</span><span class="sxs-lookup"><span data-stu-id="edb84-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="edb84-122">Se efter eventID 1121 eller 1122 i Microsoft-Windows-Windows Defender/Operational Log.</span><span class="sxs-lookup"><span data-stu-id="edb84-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="edb84-123">Vurder blokscenariet og konteksten, og bekræft, at blokeringen af dette scenarie skal være fjernet.</span><span class="sxs-lookup"><span data-stu-id="edb84-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="edb84-124">Læs værdien Sti i oplysninger om begivenheden, som er den værdi, der definerer udeladelse.</span><span class="sxs-lookup"><span data-stu-id="edb84-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="edb84-125">Gør udelukkelsen så streng som mulig.</span><span class="sxs-lookup"><span data-stu-id="edb84-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="edb84-126">Anvend et jokertegn, hvor det er nødvendigt (du kan f.eks. erstatte variablen Bruger).</span><span class="sxs-lookup"><span data-stu-id="edb84-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="edb84-127">Anvend udelukkelsen i henhold til dine installationsbehov.</span><span class="sxs-lookup"><span data-stu-id="edb84-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="edb84-128">Du kan få mere at vide [under Tilpas regler for reduktion af angrebsoverfladen.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="edb84-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="edb84-129">Udeladelse er ikke tilladt</span><span class="sxs-lookup"><span data-stu-id="edb84-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="edb84-130">Afgør, om reglen understøtter udeladelse.</span><span class="sxs-lookup"><span data-stu-id="edb84-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="edb84-131">Du kan få mere at vide [under Regler for reduktion af angrebsoverfladen.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="edb84-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="edb84-132">Gennemse de undtagelser, der er anvendt, og bekræft med hændelsesdataene for slåfejl eller fejlfortolke jokertegn.</span><span class="sxs-lookup"><span data-stu-id="edb84-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="edb84-133">Du kan få mere at vide under [Understøttede udeladelsestyper](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="edb84-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="edb84-134">Hvis effekten af reglen er for stor, skal du overveje at flytte reglen (tilbage) til overvågningstilstand for at udføre yderligere validering.</span><span class="sxs-lookup"><span data-stu-id="edb84-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="edb84-135">Du kan få mere at [vide under Test, hvordan microsoft Defender for Endpoint-funktioner fungerer i overvågningstilstand.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="edb84-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="edb84-136">Indsaml supportdata for at åbne en supportsag ved hjælp af denne kommando:</span><span class="sxs-lookup"><span data-stu-id="edb84-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="edb84-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="edb84-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="edb84-138">Du kan få mere at [vide under Problemer med onboardingmaskine til Microsoft Defender til slutpunkter.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="edb84-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
