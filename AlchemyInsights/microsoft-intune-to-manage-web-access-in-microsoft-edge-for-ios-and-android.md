---
title: Brug Microsoft Intune til at administrere internetadgang i Microsoft Edge til iOS og Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/10/2020
ms.locfileid: "49677445"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="4a073-102">Brug Microsoft Intune til at administrere internetadgang i Microsoft Edge til iOS og Android</span><span class="sxs-lookup"><span data-stu-id="4a073-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="4a073-103">Microsoft Edge til iOS og Android gør det muligt for en bruger at søge på internettet fra flere, helt adskilte profiler.</span><span class="sxs-lookup"><span data-stu-id="4a073-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="4a073-104">De største beskyttelsesfunktioner for Microsoft 365-data bliver tilgængelige, når du abonnerer på Enterprise Mobility +-sikkerhedspakken, der omfatter Microsoft Intune og Azure Active Directory Premium-funktioner, f. eks betinget adgang.</span><span class="sxs-lookup"><span data-stu-id="4a073-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="4a073-105">Du skal som minimum installere en politik for betinget adgang, der (1) gør det muligt for brugere at oprette forbindelse fra mobilenheder til Microsoft Edge til iOS og Android, og at (2) implementerer en Microsoft Intune-politik for app-beskyttelse, der giver en beskyttet browsing-oplevelse.</span><span class="sxs-lookup"><span data-stu-id="4a073-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="4a073-106">Hvis du vil vide, hvordan du kan bruge betinget adgang og politikker, skal du se:</span><span class="sxs-lookup"><span data-stu-id="4a073-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="4a073-107">Anvend politikker for betinget adgang for Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4a073-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="4a073-108">Oprette politikker for Microsoft Intune-app-beskyttelse</span><span class="sxs-lookup"><span data-stu-id="4a073-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="4a073-109">Brug Single Sign-on til Azure Active Directory – forbundne web apps i politik beskyttede browsere</span><span class="sxs-lookup"><span data-stu-id="4a073-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="4a073-110">Brug af appens konfiguration til at administrere søgeoplevelsen</span><span class="sxs-lookup"><span data-stu-id="4a073-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="4a073-111">Tillad kun brug af arbejds-og skole konti</span><span class="sxs-lookup"><span data-stu-id="4a073-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="4a073-112">Installere generelle konfigurations politikker for apps</span><span class="sxs-lookup"><span data-stu-id="4a073-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="4a073-113">Installer konfigurations politikker for appen for databeskyttelse</span><span class="sxs-lookup"><span data-stu-id="4a073-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="4a073-114">Brug Microsoft Endpoint Manager til at installere politikker for konfiguration af apps</span><span class="sxs-lookup"><span data-stu-id="4a073-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="4a073-115">Hvis du vil vide, hvordan du får adgang til administrerede app-logfiler, skal du se [brug af Microsoft Edge til iOS og Android for at få adgang til administrerede app](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="4a073-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
