---
title: VPN-relaterede problemer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554838"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="e6f4d-102">VPN-relaterede problemer</span><span class="sxs-lookup"><span data-stu-id="e6f4d-102">VPN related issues</span></span>

<span data-ttu-id="e6f4d-103">En vellykket implementering af VPN-forbindelse til MDM-klienter afhænger af en installeret profil, der korrekt afspejler kravene i VPN-infrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="e6f4d-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="e6f4d-104">Du kan se de relevante indstillinger for de klientplatforme, du undersøger, på:</span><span class="sxs-lookup"><span data-stu-id="e6f4d-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="e6f4d-105">Indstillinger for Windows 10 og Windows Holographic device for at tilføje VPN-forbindelser ved hjælp af Intune</span><span class="sxs-lookup"><span data-stu-id="e6f4d-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="e6f4d-106">Tilføje VPN-indstillinger på iOS- og iPadOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e6f4d-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="e6f4d-107">Indstillinger for Android-enhed til konfiguration af VPN i Intune</span><span class="sxs-lookup"><span data-stu-id="e6f4d-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="e6f4d-108">Tilføje VPN-indstillinger på macOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e6f4d-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="e6f4d-109">Hvis din VPN-profil bruger certifikatbaseret godkendelse, skal du sørge for, at de rodcertifikat- og klientgodkendelsescertifikatprofiler, der er knyttet til VPN-profilen, er installeret korrekt.</span><span class="sxs-lookup"><span data-stu-id="e6f4d-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="e6f4d-110">**Almindelige problemer**</span><span class="sxs-lookup"><span data-stu-id="e6f4d-110">**Common Issues**</span></span>

<span data-ttu-id="e6f4d-111">**Jeg har indsat en VPN-profil på en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til VPN.**</span><span class="sxs-lookup"><span data-stu-id="e6f4d-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="e6f4d-112">En vellykket status betyder, at Intune har installeret profilen som konfigureret.</span><span class="sxs-lookup"><span data-stu-id="e6f4d-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="e6f4d-113">Disse konfigurationer svarer dog muligvis ikke til dine netværks- og/eller godkendelseskrav.</span><span class="sxs-lookup"><span data-stu-id="e6f4d-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="e6f4d-114">Gennemse logfiler i infrastruktur- og godkendelsestjenesten (på VPN-serveren og NPS/Radius-serveren) for at få flere oplysninger om den forsøgte forbindelse.</span><span class="sxs-lookup"><span data-stu-id="e6f4d-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="e6f4d-115">Du skal muligvis samarbejde med dit netværksinfrastrukturteam eller tredjeparts VPN-leverandøren for at indsamle og gennemse logfiler.</span><span class="sxs-lookup"><span data-stu-id="e6f4d-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="e6f4d-116">**Når jeg konfigurerer en brugerdefineret VPN til iOS, bliver VPN-funktionen pr. app ikke gjort tilgængelig.**</span><span class="sxs-lookup"><span data-stu-id="e6f4d-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="e6f4d-117">Vpn per-app til iOS-enheder i Intune er i øjeblikket tilgængelig for en bestemt liste over udbydere og partnere, som også skal opfylde certifikatforudsætningerne, før du konfigurerer en VPN pr. app.</span><span class="sxs-lookup"><span data-stu-id="e6f4d-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="e6f4d-118">Du kan finde flere oplysninger [under Konfigurere VPN (Virtual Private Network) pr. app (VPN) til iOS/iPadOS-enheder i Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="e6f4d-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="e6f4d-119">Du kan finde flere oplysninger om alle VPN-forbindelsestyper i Intune under [Oprette VPN-profiler for at oprette forbindelse til VPN-servere i Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="e6f4d-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="e6f4d-120">**iOS On-Demand VPN udløses ikke, når der opnås adgang til et konfigureret domæne**</span><span class="sxs-lookup"><span data-stu-id="e6f4d-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="e6f4d-121">Hvis du vil teste automatiske VPN-indstillinger, skal du angive følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="e6f4d-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="e6f4d-122">Jeg vil gøre følgende: **Vurder hvert forsøg på at oprette forbindelse**</span><span class="sxs-lookup"><span data-stu-id="e6f4d-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="e6f4d-123">Vælg, om der skal oprettes forbindelse: **Opret forbindelse, hvis det er nødvendigt**</span><span class="sxs-lookup"><span data-stu-id="e6f4d-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="e6f4d-124">Når brugere får adgang til disse domæner: **target** *måldomænenavn*</span><span class="sxs-lookup"><span data-stu-id="e6f4d-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="e6f4d-125">Hvis ovenstående konfiguration ikke lykkes, skal du tilføje følgende element:</span><span class="sxs-lookup"><span data-stu-id="e6f4d-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="e6f4d-126">Når denne URL-adresse ikke kan nås, skal du tvinge VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="e6f4d-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>