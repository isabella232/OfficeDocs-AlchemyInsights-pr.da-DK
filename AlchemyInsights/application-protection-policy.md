---
title: Politik for beskyttelse af programmer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423431"
---
# <a name="application-protection-policy"></a><span data-ttu-id="d31ba-102">Politik for beskyttelse af programmer</span><span class="sxs-lookup"><span data-stu-id="d31ba-102">Application protection policy</span></span>

<span data-ttu-id="d31ba-103">Hvis du er ny bruger af App(Application Protection Policy), kan du se [oversigten over politikker for appbeskyttelse](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="d31ba-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="d31ba-104">Hvis du vil begynde at bruge APP, [skal du se Sådan oprettes og tildeles politikker for appbeskyttelse](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="d31ba-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="d31ba-105">Krav til politikken for beskyttelse af programmer:</span><span class="sxs-lookup"><span data-stu-id="d31ba-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="d31ba-106">Brugeren har en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="d31ba-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="d31ba-107">Brugeren tilhører en gruppe, der er målrettet mod programbeskyttelsespolitikker.</span><span class="sxs-lookup"><span data-stu-id="d31ba-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="d31ba-108">Kun én virksomhedsbruger er logget på beskyttede apps på en enhed.</span><span class="sxs-lookup"><span data-stu-id="d31ba-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="d31ba-109">Ansøgningen har implementeret [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="d31ba-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="d31ba-110">Du kan finde en liste over apps, der understøtter SDK, i [Microsoft Intune-beskyttede apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="d31ba-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="d31ba-111">Politikker gælder, når en bruger, der opfylder ovenstående krav, logger på en Intune SDK-aktiveret app.</span><span class="sxs-lookup"><span data-stu-id="d31ba-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="d31ba-112">Den nemmeste måde at afgøre, om en politik anvendes, er ved at kræve, at brugeren angiver en nål i politikken.</span><span class="sxs-lookup"><span data-stu-id="d31ba-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="d31ba-113">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="d31ba-113">For more information, see:</span></span>

[<span data-ttu-id="d31ba-114">Ofte stillede spørgsmål om fejlfinding af APP/MAM</span><span class="sxs-lookup"><span data-stu-id="d31ba-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="d31ba-115">Sådan validerer du konfigurationen af din politik for appbeskyttelse</span><span class="sxs-lookup"><span data-stu-id="d31ba-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="d31ba-116">Forstå leveringstidstidspunktet for appbeskyttelsespolitik</span><span class="sxs-lookup"><span data-stu-id="d31ba-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="d31ba-117">Sådan overvåges politikker for appbeskyttelse</span><span class="sxs-lookup"><span data-stu-id="d31ba-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)