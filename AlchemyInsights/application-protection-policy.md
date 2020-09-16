---
title: Politik for beskyttelse af programmer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716887"
---
# <a name="application-protection-policy"></a><span data-ttu-id="e2289-102">Politik for beskyttelse af programmer</span><span class="sxs-lookup"><span data-stu-id="e2289-102">Application protection policy</span></span>

<span data-ttu-id="e2289-103">Hvis du er ny for program beskyttelsespolitik (APP), skal du se [Oversigt over politikker for app-beskyttelse](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="e2289-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="e2289-104">Hvis du vil begynde at bruge APPEN, skal du se [Sådan oprettes og tildeles politikker for app-beskyttelse](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="e2289-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="e2289-105">Krav til politik for beskyttelse af programmer:</span><span class="sxs-lookup"><span data-stu-id="e2289-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="e2289-106">Brugeren har en Intune-eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="e2289-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="e2289-107">Brugeren tilhører en gruppe, der er målrettet mod politikker for beskyttelse af programmer.</span><span class="sxs-lookup"><span data-stu-id="e2289-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="e2289-108">Kun én erhvervsbruger er logget på beskyttede apps på en enhed.</span><span class="sxs-lookup"><span data-stu-id="e2289-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="e2289-109">Programmet har implementeret [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="e2289-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="e2289-110">Du kan finde en liste over apps, der understøtter SDK, under [Microsoft Intune-beskyttede apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="e2289-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="e2289-111">Politikker gælder, når en bruger, der opfylder ovenstående krav, logger på en Intune SDK-aktiveret app.</span><span class="sxs-lookup"><span data-stu-id="e2289-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="e2289-112">Den nemmeste måde at finde ud af, om en politik anvendes, er ved at kræve, at brugeren angiver en pinkode i politikken.</span><span class="sxs-lookup"><span data-stu-id="e2289-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="e2289-113">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="e2289-113">For more information, see:</span></span>

[<span data-ttu-id="e2289-114">Ofte stillede spørgsmål om fejlfinding af apps/MAM</span><span class="sxs-lookup"><span data-stu-id="e2289-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="e2289-115">Sådan validerer du konfigurationen af politik for app-beskyttelse</span><span class="sxs-lookup"><span data-stu-id="e2289-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="e2289-116">Forstå timing for levering af politik for app-beskyttelse</span><span class="sxs-lookup"><span data-stu-id="e2289-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="e2289-117">Sådan overvåges politikker for app-beskyttelse</span><span class="sxs-lookup"><span data-stu-id="e2289-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)