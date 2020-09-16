---
title: Wi-Fi-profiler i Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696255"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="7d372-102">Wi-Fi-profiler i Intune</span><span class="sxs-lookup"><span data-stu-id="7d372-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="7d372-103">Vellykket implementering af Wi-Fi-forbindelse til MDM-klienter afhænger af en korrekt installeret profil, der afspejler kravene til virksomhedens Wi-Fi-infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="7d372-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="7d372-104">Hvis du vil gennemgå de relevante indstillinger for de klientplatforme, du undersøger, skal du se:</span><span class="sxs-lookup"><span data-stu-id="7d372-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="7d372-105">Tilføj Wi-Fi-indstillinger for enheder, der kører Android i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7d372-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="7d372-106">Tilføj Wi-Fi-indstillinger for Android Enterprise-dedikerede og fuldt administrerede enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7d372-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="7d372-107">Tilføj Wi-Fi-indstillinger for iOS-og iPadOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7d372-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="7d372-108">Tilføje Wi-Fi-indstillinger for Windows 10 og nyere enheder i Intune</span><span class="sxs-lookup"><span data-stu-id="7d372-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="7d372-109">Importere Wi-Fi-indstillinger for Windows-enheder i Intune</span><span class="sxs-lookup"><span data-stu-id="7d372-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="7d372-110">**Almindelige problemer**</span><span class="sxs-lookup"><span data-stu-id="7d372-110">**Common Issues**</span></span>

<span data-ttu-id="7d372-111">**Jeg installerer en Wi-Fi-profil, der er afhængig af et installeret certifikat, der er angivet i Wi-Fi-profilen. Men konfigurationsprofilerne viser en fejlstatus.**</span><span class="sxs-lookup"><span data-stu-id="7d372-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="7d372-112">Kontrollér, at din enhed har modtaget certifikatet.</span><span class="sxs-lookup"><span data-stu-id="7d372-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="7d372-113">Gå til **alle enheder** i Intune, og vælg enheds > **enhedskonfiguration**.</span><span class="sxs-lookup"><span data-stu-id="7d372-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="7d372-114">Kontrollér, at alle de forventede profiler er angivet og i en vellykket tilstand.</span><span class="sxs-lookup"><span data-stu-id="7d372-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="7d372-115">Hvis du har en Android-profil, skal du sørge for, at de er installeret på Android-enheder, hvis du har mellemliggende certifikater i certifikatkæden.</span><span class="sxs-lookup"><span data-stu-id="7d372-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="7d372-116">Hvis du vil kontrollere certifikatstatus, skal du gå til **enheds konfigurations**  >  **profiler**  >  **Android**-  >  **Egenskaber for**  >  **certifikater, der er tillid til**.</span><span class="sxs-lookup"><span data-stu-id="7d372-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="7d372-117">Hvis du fortsat får vist fejlene, skal du gennemgå procedurerne og afsnittet om fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="7d372-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="7d372-118">Du kan finde flere oplysninger under [Oversigt over fejlfinding af SCEP-certifikat profiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="7d372-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="7d372-119">**Jeg har installeret en Wi-Fi-profil til en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="7d372-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="7d372-120">En status for succes betyder, at Intune har installeret profilen som konfigureret.</span><span class="sxs-lookup"><span data-stu-id="7d372-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="7d372-121">Disse konfigurationer stemmer dog muligvis ikke overens med dit netværks-og/eller godkendelseskrav.</span><span class="sxs-lookup"><span data-stu-id="7d372-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="7d372-122">Hvis du vil have mere at vide om den forsøgte forbindelse, skal du gennemgå loggene i infrastrukturen og godkendelsestjenesten (på Wi-Fi Access Point-controlleren og NPS/RADIUS-serveren).</span><span class="sxs-lookup"><span data-stu-id="7d372-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="7d372-123">Det kan være nødvendigt at arbejde med dit netværksinfrastruktur team eller en Wi-Fi-tredjepartsleverandør for at indsamle og gennemse loggene.</span><span class="sxs-lookup"><span data-stu-id="7d372-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>