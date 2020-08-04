---
title: Intune Wi-Fi-profiler
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554858"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="4f38c-102">Intune Wi-Fi-profiler</span><span class="sxs-lookup"><span data-stu-id="4f38c-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="4f38c-103">En vellykket implementering af Wi-Fi-forbindelse til MDM-klienter afhænger af en korrekt installeret profil, der afspejler kravene i virksomhedens Wi-Fi-infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="4f38c-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="4f38c-104">Hvis du vil gennemse de relevante indstillinger for de klientplatforme, du undersøger, skal du se:</span><span class="sxs-lookup"><span data-stu-id="4f38c-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="4f38c-105">Tilføje Wi-Fi-indstillinger for enheder, der kører Android i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4f38c-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="4f38c-106">Tilføj Wi-Fi-indstillinger til Android Enterprise-dedikerede og fuldt administrerede enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4f38c-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="4f38c-107">Tilføje Wi-Fi-indstillinger til iOS- og iPadOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4f38c-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="4f38c-108">Tilføje Wi-Fi-indstillinger for Windows 10 og nyere enheder i Intune</span><span class="sxs-lookup"><span data-stu-id="4f38c-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="4f38c-109">Importere Wi-Fi-indstillinger for Windows-enheder i Intune</span><span class="sxs-lookup"><span data-stu-id="4f38c-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="4f38c-110">**Almindelige problemer**</span><span class="sxs-lookup"><span data-stu-id="4f38c-110">**Common Issues**</span></span>

<span data-ttu-id="4f38c-111">**Jeg installerer en Wi-Fi-profil, der er afhængig af et installeret certifikat, der er angivet i Wi-Fi-profilen. Konfigurationsprofilerne viser dog en fejlstatus.**</span><span class="sxs-lookup"><span data-stu-id="4f38c-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="4f38c-112">Kontroller, at enheden har modtaget certifikatet.</span><span class="sxs-lookup"><span data-stu-id="4f38c-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="4f38c-113">Gå til Alle enheder i **Intune, og** vælg > **enhedskonfiguration .**</span><span class="sxs-lookup"><span data-stu-id="4f38c-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="4f38c-114">Kontroller, at alle forventede profiler er angivet og i en vellykket tilstand.</span><span class="sxs-lookup"><span data-stu-id="4f38c-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="4f38c-115">Hvis du har mellemliggende certifikater i din certifikatkæde for en Android-profil, skal du sørge for, at de er installeret på Android-enheder.</span><span class="sxs-lookup"><span data-stu-id="4f38c-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="4f38c-116">Hvis du vil kontrollere certifikatstatus, skal du gå til **Android**Intermediate CA Properties Trusted Certificate for  >  **enhedskonfigurationsprofiler.**  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**</span><span class="sxs-lookup"><span data-stu-id="4f38c-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="4f38c-117">Hvis du bliver ved med at se fejl, skal du gennemgå procedurerne og afsnittet fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="4f38c-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="4f38c-118">Du kan finde flere oplysninger [under Oversigt over fejlfinding af SCEP-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="4f38c-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="4f38c-119">**Jeg har installeret en Wi-Fi-profil på en enhed. Intune viser, at det lykkedes, men enheden opretter ikke forbindelse til Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="4f38c-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="4f38c-120">En vellykket status betyder, at Intune har installeret profilen som konfigureret.</span><span class="sxs-lookup"><span data-stu-id="4f38c-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="4f38c-121">Disse konfigurationer svarer dog muligvis ikke til dine netværks- og/eller godkendelseskrav.</span><span class="sxs-lookup"><span data-stu-id="4f38c-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="4f38c-122">Du kan få flere oplysninger om den forsøgte forbindelse ved at gennemse logfiler i infrastrukturen og godkendelsestjenesten (på Wi-Fi-adgangspunktcontrolleren og NPS/Radius-serveren).</span><span class="sxs-lookup"><span data-stu-id="4f38c-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="4f38c-123">Du skal muligvis samarbejde med dit netværksinfrastrukturteam eller tredjeparts-Wi-Fi-leverandøren for at indsamle og gennemse logfiler.</span><span class="sxs-lookup"><span data-stu-id="4f38c-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>