---
title: Vilkår, der mangler i SharePoint Online-ordlagring
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766847"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="06b23-102">Aktivering af Bitlocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="06b23-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="06b23-103">Intune Endpoint Protection Policy kan bruges til at konfigurere Boitlocker-krypteringsindstillinger for Windows-enheder som beskrevet i : Windows10-indstillinger (og nyere) for at beskytte enheder, der bruger Intune</span><span class="sxs-lookup"><span data-stu-id="06b23-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="06b23-104">Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10 understøtter automatisk bitlocker kryptering, som udløses uden anvendelse af MDM politik.</span><span class="sxs-lookup"><span data-stu-id="06b23-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="06b23-105">Dette kan påvirke anvendelsen af politikken, hvis der ikke er konfigureret standardindstillinger.</span><span class="sxs-lookup"><span data-stu-id="06b23-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="06b23-106">Se ofte stillede spørgsmål for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="06b23-106">See FAQ for more detail.</span></span>


<span data-ttu-id="06b23-107">Ofte  stillede spørgsmål Q: Hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af slutpunktsbeskyttelsespolitikken?</span><span class="sxs-lookup"><span data-stu-id="06b23-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="06b23-108"> Sv.: Intune-slutpunktsbeskyttelsespolitikken implementeres ved hjælp af Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="06b23-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="06b23-109">Ikke alle udgaver eller builds af Windows understøtter Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="06b23-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="06b23-110">På dette tidspunkt Windows Editions: Enterprise; Uddannelse, mobil, mobil virksomhed og professionel (fra build 1809 og fremefter) understøttes.</span><span class="sxs-lookup"><span data-stu-id="06b23-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="06b23-111">Sp: Hvis en enhed allerede er krypteret med Bitlocker ved hjælp af OS-standardindstillingerne for krypteringsmetode og krypteringsstyrke (XTS-AES-128) vil anvende en politik med forskellige indstillinger automatisk udløse re-kryptering af drevet med de nye indstillinger?</span><span class="sxs-lookup"><span data-stu-id="06b23-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="06b23-112">A: Nej.</span><span class="sxs-lookup"><span data-stu-id="06b23-112">A: No.</span></span> <span data-ttu-id="06b23-113">For at anvende de nye cipher indstillinger drevet skal først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="06b23-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="06b23-114">Bemærk For enheder, der er tilmeldt Autopilot, udløses den automatiske kryptering, der ville opstå under OOBE, ikke, før Intune-politikken er evalueret, hvilket gør det muligt at bruge de politikbaserede indstillinger i stedet for os-standardindstillingerne</span><span class="sxs-lookup"><span data-stu-id="06b23-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="06b23-115">Q Hvis en enhed er krypteret som følge af anvendelsen af Intune politik vil det blive dekrypteret, når denne politik er fjernet?</span><span class="sxs-lookup"><span data-stu-id="06b23-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="06b23-116">A: Fjernelse af kryptering relateret politik ikke resulterer i dekryptering af de drev, der blev konfigureret.</span><span class="sxs-lookup"><span data-stu-id="06b23-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="06b23-117">Sp: Hvorfor viser intune Compliance-politikken, at min enhed ikke har "Bitlocker aktiveret", men det er den?</span><span class="sxs-lookup"><span data-stu-id="06b23-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="06b23-118">Sv. Indstillingen "Bitlocker enabled" i intune compliance policy anvender DHA-klienten (Windows Device Health Attestation).</span><span class="sxs-lookup"><span data-stu-id="06b23-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="06b23-119">Denne klient måler kun enhedens tilstand på starttidspunktet.</span><span class="sxs-lookup"><span data-stu-id="06b23-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="06b23-120">Så hvis en enhed ikke er blevet genstartet, da bitlocker kryptering blev afsluttet DHA klienttjeneste vil ikke rapportere bitlocker som værende aktiv.</span><span class="sxs-lookup"><span data-stu-id="06b23-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>