---
title: Brug af mail profiler med Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653282"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="79517-102">Brug af mail profiler med Intune</span><span class="sxs-lookup"><span data-stu-id="79517-102">Using email profiles with Intune</span></span>

<span data-ttu-id="79517-103">Intune kan bruges til at oprette og installere mail profiler til den indbyggede mailklient på flere enheder.</span><span class="sxs-lookup"><span data-stu-id="79517-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="79517-104">Hvis du vil have oplysninger om nogle af de begrænsninger, der er knyttet til mail profiler, herunder hvordan tilstedeværelsen af eksisterende profiler håndteres, og hvordan du fjerner mail profiler, skal du se [tilføje mailindstillinger til enheder ved hjælp af Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="79517-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="79517-105">Du kan finde flere oplysninger om, hvordan du opretter mail profiler for hver enhedsplatform, i:</span><span class="sxs-lookup"><span data-stu-id="79517-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="79517-106">Indstillinger for Android-enhed for at konfigurere mail, godkendelse og synkronisering i Intune</span><span class="sxs-lookup"><span data-stu-id="79517-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="79517-107">Tilføje mailindstillinger for iOS-og iPadOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="79517-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="79517-108">Indstillinger for mailprofil i Microsoft Intune til enheder, der kører Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="79517-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="79517-109">Indstillinger for mailprofil for enheder, der kører Windows 10 i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="79517-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="79517-110">**Almindeligt synkroniserings problem**</span><span class="sxs-lookup"><span data-stu-id="79517-110">**Common syncing issue**</span></span>

<span data-ttu-id="79517-111">**En KNOX på Android-mailprofil forhindrer, at brugerkontakter, kalender og opgaver synkroniseres til bruger enheder.**</span><span class="sxs-lookup"><span data-stu-id="79517-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="79517-112">Funktionen KNOX på Android KNOX-mailprofil giver administratoren mulighed for at bestemme, hvilke indholdstyper der skal synkroniseres til enheden, ved at indstille hver til at være aktiveret.</span><span class="sxs-lookup"><span data-stu-id="79517-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="79517-113">Hvis indstillingen for en af indholdstyperne er angivet til **ikke konfigureret** (standard), synkroniseres den pågældende indholdstype ikke automatisk.</span><span class="sxs-lookup"><span data-stu-id="79517-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="79517-114">En bruger kan aktivere den indholdstype, de vil have manuelt, på enheden, men konfigurationen overskrives med Intune-politikindstillingen, og synkroniseringen stopper for den pågældende indholdstype.</span><span class="sxs-lookup"><span data-stu-id="79517-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

