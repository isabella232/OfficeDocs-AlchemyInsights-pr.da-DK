---
title: EndPoint Manager – grundlinjer for sikkerhed
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420774"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="fda26-102">EndPoint Manager – grundlinjer for sikkerhed</span><span class="sxs-lookup"><span data-stu-id="fda26-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="fda26-103">Sikkerheds baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span><span class="sxs-lookup"><span data-stu-id="fda26-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="fda26-104">Disse oprindelige planer kan tilpasses, så de kun leverer de ønskede indstillinger og værdier.</span><span class="sxs-lookup"><span data-stu-id="fda26-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="fda26-105">Du kan finde flere oplysninger om grundlinjer for sikkerhed under Brug af sikkerheds oprindelige planer til konfiguration af [Windows 10-enheder i Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="fda26-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="fda26-106">Der er i øjeblikket grundlinjer for disse produkter:</span><span class="sxs-lookup"><span data-stu-id="fda26-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="fda26-107">Sikkerhedsindstillinger for Windows MDM</span><span class="sxs-lookup"><span data-stu-id="fda26-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="fda26-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="fda26-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="fda26-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="fda26-109">Microsoft Edge</span></span>

<span data-ttu-id="fda26-110">Hver af de oprindelige planer opdateres med jævne mellemrum og udgives i trinvise versioner.</span><span class="sxs-lookup"><span data-stu-id="fda26-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="fda26-111">Hver version tilføjer og fjerner indstillinger fra den forrige version for at sikre, at den oprindelige plan opfylder den aktuelle vejledning.</span><span class="sxs-lookup"><span data-stu-id="fda26-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="fda26-112">Konsollen sikkerhedsmæssige grundlinjer i Slutpunktssikkerhed gør det muligt at sammenligne forskellige versioner ved at gøre ændringerne fra version til version synlige.</span><span class="sxs-lookup"><span data-stu-id="fda26-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="fda26-113">Du kan finde en vejledning til, hvordan du mest effektivt kan ændre, hvilken version af den oprindelige plan der installeres, under Administrere profiler for oprindelige [sikkerhed i Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="fda26-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="fda26-114">Når du har implementeret en grundlinje for sikkerhed, kan du overvåge installationstilstanden og gennemse indstillingerne på enhed for enhed.</span><span class="sxs-lookup"><span data-stu-id="fda26-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="fda26-115">**Bemærk!** Det kan tage op til 24 timer, før data for oprindelige planer vises fra installationsstart til en enhed og op til 6 timer for yderligere opdateringer.</span><span class="sxs-lookup"><span data-stu-id="fda26-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="fda26-116">Den mest almindelige årsag til, at en oprindelig plan ikke anvendes, er, at den samme indstilling bruges i en anden profil.</span><span class="sxs-lookup"><span data-stu-id="fda26-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="fda26-117">Dette scenarie kan undersøges for en bestemt enhed ved at vælge enheden i knudepunktet Enhedsstatus i profilen Grundlinje for sikkerhed.</span><span class="sxs-lookup"><span data-stu-id="fda26-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="fda26-118">Du kan finde flere oplysninger [i Løse konflikter for sikkerheds oprindelige planer.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="fda26-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>