---
title: Brug Microsoft Intune til at administrere webadgang i Microsoft Edge til iOS og Android
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
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989657"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="1cfce-102">Brug Microsoft Intune til at administrere webadgang i Microsoft Edge til iOS og Android</span><span class="sxs-lookup"><span data-stu-id="1cfce-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="1cfce-103">Microsoft Edge til iOS og Android giver en bruger mulighed for at søge på internettet fra flere, helt separate profiler.</span><span class="sxs-lookup"><span data-stu-id="1cfce-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="1cfce-104">De bredeste beskyttelsesfunktioner til Microsoft 365-data bliver tilgængelige, når du abonnerer på Enterprise Mobility + Security-pakken, som omfatter Microsoft Intune- og Azure Active Directory Premium-funktioner, f.eks. betinget adgang.</span><span class="sxs-lookup"><span data-stu-id="1cfce-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="1cfce-105">Du skal som minimum implementere en politik for betinget adgang, som (1) giver brugerne mulighed for at oprette forbindelse fra mobilenheder til Microsoft Edge til iOS og Android, og som (2) implementerer en Microsoft Intune-politik til beskyttelse af apps, der giver en beskyttet browseroplevelse.</span><span class="sxs-lookup"><span data-stu-id="1cfce-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="1cfce-106">For at forstå, hvordan du kan bruge betinget adgang og politikker, skal du se:</span><span class="sxs-lookup"><span data-stu-id="1cfce-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="1cfce-107">Anvend politikker for betinget adgang til Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1cfce-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="1cfce-108">Opret Microsoft Intune-beskyttelsespolitikker for apps</span><span class="sxs-lookup"><span data-stu-id="1cfce-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="1cfce-109">Brug enkelt logon til Azure Active Directory-forbundne webapps i politikbeskyttede browsere</span><span class="sxs-lookup"><span data-stu-id="1cfce-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="1cfce-110">Brug appkonfiguration til at administrere browseroplevelsen</span><span class="sxs-lookup"><span data-stu-id="1cfce-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="1cfce-111">Tillad kun brug af arbejds- og skolekonti</span><span class="sxs-lookup"><span data-stu-id="1cfce-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="1cfce-112">Installér generelle politikker for appkonfiguration</span><span class="sxs-lookup"><span data-stu-id="1cfce-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="1cfce-113">Installér politikker for appkonfiguration til databeskyttelse</span><span class="sxs-lookup"><span data-stu-id="1cfce-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="1cfce-114">Brug Microsoft Endpoint Manager til at installere appkonfigurationspolitikker</span><span class="sxs-lookup"><span data-stu-id="1cfce-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="1cfce-115">Du kan få mere at vide om, hvordan du får adgang til administrerede applogfiler under Brug Microsoft Edge til [iOS og Android til at få adgang til administrerede applogfiler.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="1cfce-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
