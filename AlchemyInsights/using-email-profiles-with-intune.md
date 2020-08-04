---
title: Brug af mailprofiler med Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554842"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="b3adc-102">Brug af mailprofiler med Intune</span><span class="sxs-lookup"><span data-stu-id="b3adc-102">Using email profiles with Intune</span></span>

<span data-ttu-id="b3adc-103">Intune kan bruges til at oprette og installere e-mail-profiler for den oprindelige (indbyggede) e-mail-klient på flere enhedsplatforme.</span><span class="sxs-lookup"><span data-stu-id="b3adc-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="b3adc-104">Du kan finde oplysninger om nogle af de begrænsninger, der er knyttet til mailprofiler, herunder hvordan tilstedeværelsen af eksisterende profiler håndteres, og hvordan du fjerner mailprofiler, under [Føje mailindstillinger til enheder, der bruger Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="b3adc-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="b3adc-105">Du kan finde flere oplysninger om, hvordan du opretter mailprofiler for hver enhedsplatform, under:</span><span class="sxs-lookup"><span data-stu-id="b3adc-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="b3adc-106">Indstillinger for Android-enhed til konfiguration af mail, godkendelse og synkronisering i Intune</span><span class="sxs-lookup"><span data-stu-id="b3adc-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="b3adc-107">Tilføje e-mail-indstillinger for iOS- og iPadOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b3adc-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="b3adc-108">Indstillinger for mailprofil i Microsoft Intune for enheder, der kører Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="b3adc-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="b3adc-109">Indstillinger for mailprofil for enheder, der kører Windows 10 i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b3adc-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="b3adc-110">**Almindeligt synkroniseringsproblem**</span><span class="sxs-lookup"><span data-stu-id="b3adc-110">**Common syncing issue**</span></span>

<span data-ttu-id="b3adc-111">**En KNOX på Android-mailprofil forhindrer brugerkontakter, kalender og opgaver i at blive synkroniseret med brugerenheder.**</span><span class="sxs-lookup"><span data-stu-id="b3adc-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="b3adc-112">KNOX på Android KNOX e-mail profil giver admin mulighed for at beslutte, hvilke indholdstyper er sync'd til enheden ved at indstille hver til aktiveret.</span><span class="sxs-lookup"><span data-stu-id="b3adc-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="b3adc-113">Hvis indstillingen for en af indholdstyperne er angivet til **Ikke konfigureret** (standard), synkroniseres denne indholdstype ikke automatisk.</span><span class="sxs-lookup"><span data-stu-id="b3adc-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="b3adc-114">En bruger kan aktivere den ønskede indholdstype direkte på enheden manuelt, men denne konfiguration overskrives af politikindstillingen Intune, og synkroniseringsstoppet for den pågældende indholdstype.</span><span class="sxs-lookup"><span data-stu-id="b3adc-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

