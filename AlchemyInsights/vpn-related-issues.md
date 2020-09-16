---
title: VPN-relaterede problemer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726085"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="7bb2d-102">VPN-relaterede problemer</span><span class="sxs-lookup"><span data-stu-id="7bb2d-102">VPN related issues</span></span>

<span data-ttu-id="7bb2d-103">Vellykket implementering af VPN-forbindelse for MDM-klienter afhænger af en installeret profil, der afspejler kravene til VPN-infrastrukturen korrekt.</span><span class="sxs-lookup"><span data-stu-id="7bb2d-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="7bb2d-104">Du kan finde relevante indstillinger for de klientplatforme, du undersøger, under:</span><span class="sxs-lookup"><span data-stu-id="7bb2d-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="7bb2d-105">Enhedsindstillinger for Windows 10 og Windows Holographic for at tilføje VPN-forbindelser ved hjælp af Intune</span><span class="sxs-lookup"><span data-stu-id="7bb2d-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="7bb2d-106">Tilføje VPN-indstillinger på iOS-og iPadOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7bb2d-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="7bb2d-107">Indstillinger for Android-enhed til konfiguration af VPN i Intune</span><span class="sxs-lookup"><span data-stu-id="7bb2d-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="7bb2d-108">Tilføje VPN-indstillinger på macOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7bb2d-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="7bb2d-109">Hvis din VPN-profil brugercertifikat baseret godkendelse, skal du kontrollere, at de rodcertifikater for rodcertifikater og klientgodkendelses certifikater, der er knyttet til VPN-profilen, er blevet installeret korrekt.</span><span class="sxs-lookup"><span data-stu-id="7bb2d-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="7bb2d-110">**Almindelige problemer**</span><span class="sxs-lookup"><span data-stu-id="7bb2d-110">**Common Issues**</span></span>

<span data-ttu-id="7bb2d-111">**Jeg har installeret en VPN-profil på en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til VPN.**</span><span class="sxs-lookup"><span data-stu-id="7bb2d-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="7bb2d-112">En status for succes betyder, at Intune har installeret profilen som konfigureret.</span><span class="sxs-lookup"><span data-stu-id="7bb2d-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="7bb2d-113">Disse konfigurationer stemmer dog muligvis ikke overens med dit netværks-og/eller godkendelseskrav.</span><span class="sxs-lookup"><span data-stu-id="7bb2d-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="7bb2d-114">Gennemse loggene i infrastrukturen og godkendelsestjenesten (på VPN-serveren og NPS/RADIUS-serveren) for at få flere oplysninger om den forsøgte forbindelse.</span><span class="sxs-lookup"><span data-stu-id="7bb2d-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="7bb2d-115">Det kan være nødvendigt at arbejde med dit netværksinfrastruktur team eller en VPN-leverandør fra tredjepartsleverandører for at indsamle og gennemse loggene.</span><span class="sxs-lookup"><span data-stu-id="7bb2d-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="7bb2d-116">**Når jeg konfigurerer en brugerdefineret VPN til iOS, bliver VPN-funktionen pr. app ikke tilgængelig.**</span><span class="sxs-lookup"><span data-stu-id="7bb2d-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="7bb2d-117">Per-App VPN til iOS-enheder i Intune er i øjeblikket tilgængelig for en bestemt liste over udbydere og partnere, som også skal opfylde certifikatets forudsætninger, før du konfigurerer en per-appen VPN.</span><span class="sxs-lookup"><span data-stu-id="7bb2d-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="7bb2d-118">Hvis du vil have mere at vide, skal du se [konfigurere per-app virtuelt privat netværk (VPN) til iOS/iPadOS-enheder i Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="7bb2d-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="7bb2d-119">Du kan finde flere oplysninger om alle VPN-forbindelsestyper i Intune under [oprette VPN-profiler for at oprette forbindelse til VPN-servere i Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="7bb2d-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="7bb2d-120">**iOS on-demand VPN udløser ikke, når der opnås adgang til et konfigureret domæne**</span><span class="sxs-lookup"><span data-stu-id="7bb2d-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="7bb2d-121">Hvis du vil teste automatiske VPN-indstillinger, skal du angive følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="7bb2d-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="7bb2d-122">Jeg vil gøre følgende: **Evaluer hvert forbindelsesforsøg**</span><span class="sxs-lookup"><span data-stu-id="7bb2d-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="7bb2d-123">Vælg, om du vil oprette forbindelse: **Opret forbindelse, hvis det er nødvendigt**</span><span class="sxs-lookup"><span data-stu-id="7bb2d-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="7bb2d-124">Når brugere får adgang til disse domæner: **destinations** *domænenavn*</span><span class="sxs-lookup"><span data-stu-id="7bb2d-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="7bb2d-125">Hvis ovenstående konfiguration ikke lykkes, skal du tilføje følgende element:</span><span class="sxs-lookup"><span data-stu-id="7bb2d-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="7bb2d-126">Når denne URL-adresse ikke kan oprettes, skal du oprette forbindelse til VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="7bb2d-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>