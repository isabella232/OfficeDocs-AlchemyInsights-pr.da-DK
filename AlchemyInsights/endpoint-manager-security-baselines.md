---
title: EndPoint Manager – Grundlæggende sikkerhedsindstillinger
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440874"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="37094-102">EndPoint Manager – Grundlæggende sikkerhedsindstillinger</span><span class="sxs-lookup"><span data-stu-id="37094-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="37094-103">Grundlæggende sikkerhedsindstillinger er forudkonfigurerede grupper af Windows-indstillinger, der hjælper dig med at anvende de sikkerhedsindstillinger, der anbefales af de relevante sikkerhedsteams.</span><span class="sxs-lookup"><span data-stu-id="37094-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="37094-104">Disse grundindstillinger kan tilpasses, så de udelukkende leverer de ønskede indstillinger og værdier.</span><span class="sxs-lookup"><span data-stu-id="37094-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="37094-105">Du kan finde flere oplysninger om de grundlæggende sikkerhedsindstillinger under [Brug grundlæggende sikkerhedsindstillinger til at konfigurere Windows 10-enheder i Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="37094-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="37094-106">Der er i øjeblikket grundindstillinger for disse produkter:</span><span class="sxs-lookup"><span data-stu-id="37094-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="37094-107">Sikkerhedsindstillinger for Windows MDM</span><span class="sxs-lookup"><span data-stu-id="37094-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="37094-108">Microsoft Defender for Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="37094-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="37094-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="37094-109">Microsoft Edge</span></span>

<span data-ttu-id="37094-110">Hver grundindstilling opdateres med jævne mellemrum og udgives i trinvise versioner.</span><span class="sxs-lookup"><span data-stu-id="37094-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="37094-111">Hver version tilføjer og eller fjerner indstillinger fra den tidligere version for at sikre, at grundindstillingen opfylder den aktuelle vejledning.</span><span class="sxs-lookup"><span data-stu-id="37094-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="37094-112">De grundlæggende sikkerhedsindstillinger i Endpoint Security gør det muligt at sammenligne forskellige versioner ved at foretage ændringer fra version til version synlig. </span><span class="sxs-lookup"><span data-stu-id="37094-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="37094-113">Du kan få vejledning til, hvordan du mest effektivt ændrer, hvilken version af grundindstilling, der installeres, i [Administrer profiler for grundlæggende sikkerhedsindstillinger i Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="37094-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="37094-114">Når du har udrullet en grundlæggende sikkerhedsindstilling, kan du overvåge dens aktiverede tilstand og gennemse indstillingerne fra enhed til enhed.</span><span class="sxs-lookup"><span data-stu-id="37094-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="37094-115">**Bemærk:** Det kan tage op til 24 timer, før rapporteringsdataene for grundlæggende sikkerhedsindstillinger vises efter den første installation på en enhed og op til 6 timer for yderligere opdateringer.</span><span class="sxs-lookup"><span data-stu-id="37094-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="37094-116">Den mest almindelige årsag til, at en grundindstilling ikke anvendes, er, at den samme indstilling bruges i en anden profil.</span><span class="sxs-lookup"><span data-stu-id="37094-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="37094-117">Dette scenarie kan undersøges for en bestemt enhed ved at vælge den pågældende enhed i enhedens statusnode på profilen Grundlæggende sikkerhedsindstillinger.</span><span class="sxs-lookup"><span data-stu-id="37094-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="37094-118">For flere detaljer, se [Løs konflikter for grundlæggende sikkerhedsindstillinger](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="37094-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>